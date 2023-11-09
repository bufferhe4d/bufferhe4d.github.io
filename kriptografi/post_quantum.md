## Post-Quantum Cryptography (PQC)

Kriptografi alanında protokollerin güvenliklerini sağlarken güvenliği, bu protokollere saldıracak kişinin hesaplama gücünün yetmeyeceği problemlerin çözümlerine dayandırıyoruz. Bu problemlerin parametrelerini dünyada bulunan toplam hesaplama gücünün çözemeyeceği şekilde seçmeye çalışıyoruz. Hali hazırda aşina olduğumuz bilgisayarlar (klasik bilgisayarlar) için zor olan bazı problemler, belirli özelliklere sahip kuantum bilgisayarlar için kolay olabiliyor. Bu sebeple her ne kadar bu tarz kuantum bilgisayarlar günümüzde var olmasa da (bildiğimiz kadarıyla) kriptografik protokollerin bir çok alanda yüksek riskli protokoller olduğu için kuantum bilgisayarlar üzerinde gerçekleştirilebilecek saldırıları önlemeye çalışıyoruz. Bu senaryo kuantum sonrası kriptografi (post-quantum) cryptography dediğimiz alt alanı tanımlıyor. Burada dikkat edilmesi gereken nokta geliştirdiğimiz protokollerin hala klasik bilgisayarlarda çalışıyor oluşu. Sadece saldıran bilgisayarların kuantum bilgisayarlar olduğunu varsayıyoruz. 

### Nasıl Başlarım?

<strong>Önkoşul:</strong> Temel kriptografi

Kuantum sonrası protokollerın standardizasyonu yeni yeni bitiyor, bu sebeple kullanılan/kullanılacak protokoller konusunda diğer alt alanlara kıyasla pedagojik açıdan uygun daha az materyal var. Şu an kullanılan problemlerin tipi üzerinden 4 kategoriye ayırabiliriz (ilki hariç Türkçe karşılıklarının yaygın kullanıma eriştiğini düşünmediğim için kullanmadım):

1. Lattice based (Kafes tabanlı)
2. Isogeny based
3. Hash based
4. Code based
5. Multi-variate based

Kafes tabanlı kriptosistemler dışında diğer seçenekler üzerine daha önce çalışmadığım için maalesef diğerleri hakkında kaynak önerisinde bulunmayacağım. Kafes tabanlı kriptosistemler için Şu iki kaynak faydalı olacaktır:

- [Basic Lattice Based Cryptography - Lyubashevsky](https://drive.google.com/file/d/1JTdW5ryznp-dUBBjN12QbvWz9R41NDGU/view): İlk okuma olarak bu kaynak gayet faydalı çünkü temelden başlayıp döküman içerisinde kullanılacak her şey tanımlanıyor. Sonrasında bir şifreleme ve bir dijital imza protokolü basitleştirilmiş şekilde anlatılıyor. Hem kullanılan problemlerin tanımı, hem de bu problemlerin protokollerde kullanılış şeklini en sade şekilde gösteren bir kaynak.

### Nasıl İlerlerim?

- [A Tutorial Introduction to Lattice-based Cryptography and Homomorphic Encryption - Li, Ng & Purcell](https://arxiv.org/abs/2208.08125): Bu kitap kafes tabanlı sistemlerin matematiğini öğrenmek için oldukça uygun ve konu hakkındaki bir çok başka yazıya göre daha anlaşılır. Ancak bu kitabın yazılış sebebi kafes tabanlı problemlerin başka bir alt alan olan Fully Homomorphic Encryption (FHE) alanında kullanımını göstermek. Bu yüzden sadece kuantum sonrası kriptografi ile ilgileniyorsanız. Chapter 10'u atlayabilirsiniz.

- [NIST PQC Standardization](https://csrc.nist.gov/projects/post-quantum-cryptography): Daha önce protokollerin standardizasyonunun yeni yeni bittiğinden bahsetmiştim. Standardizasyon dediğimiz süreç belirli kriptografik protokollerin farklı araştırmacılar tarafından halka açılması, bu protokollere araştırmacılar tarafından saldırıların gerçekleştirilmesi ve bu araştırmaların ışığında aralarından beklenen kriterlere en uygun protokolün seçilmesi süreci. Bu süreçte birden fazla raund oluyor ve her raund'da bazı protokoller eleniyor. Verilen linkten her raund'da bulunan protokolleri ve 2022 yılında standart olarak seçilmiş protokolleri görüp inceleyebilirsiniz. Bu protokollerin makalelerini veya bu protokolleri açıklayan farklı makaleleri incelemek genel olarak faydalı olacaktır. Bir çoğunun belirli açılardan birbirine benzediğini göreceksiniz. Standardizasyonların tartışıldığı bir forum da mevcut: [PQC Forum](https://groups.google.com/a/list.nist.gov/g/pqc-forum).

