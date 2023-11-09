## Simetrik Kriptografi

Şifreleme ve özet fonksiyonları gibi başka kriptografik protokollerin altyapısını oluşturan bir çok yapı
simetrik kriptografi dediğimiz alana ait. Hemen hemen her protokolde en az bir simetrik yapı kullanıldığı ve bu sebeple aklımıza gelebilecek her cihazda var olmaları gerektiği için yazılım ve donanım implementasyonları açısından en performanslı protokoller bu alt alana dahil. Burada performans kelimesi sadece hız değil aynı zamanda hafıza ve kullanılan enerji olarak da anlaşılmalı. Hafif Siklet Kriptografi (Lightweight Cryptography) dediğimiz bir diğer alt alan spesifik olarak düşük kaynaklar tüketen ortamlarda çalışmak üzere geliştirilen protokollerden oluşuyor.


### Nasıl Başlarım?

<strong>Önkoşul:</strong> Temel kriptogafi bilgisi.

- [The Design of Rijndael - Daemen & Rijmen](https://link.springer.com/book/10.1007/978-3-662-04722-4): Bu kitap temel kriptografi bilgisi edindikten sonra oldukça aşina olacağınız ve günümüz şifreleme standardı olarak hala geçerliliğini koruyan (ve yüksek ihtimalle koruyacak olan) AES (bir diğer adıyla Rijndael) şifreleme sisteminin tasarım hikayesini anlatıyor (tasarlayanlar tarafından). Tek bir sisteme odaklanan bir kitap olsa da, diğer simetrik yapılara baktığınızda bir çok alt birimin birbirlerine benzediğini göreceksiniz. Bu sebeple bu kitap bu alanda yapılan çalışmalar hakkında bir fikir edinmek ve temel bazı teknikleri öğrenmek için çok faydalı.

### Nasıl İlerlerim?

- Simetrik protokollerin kriptanalizi (kriptografik açıdan güvenli olup olmamalarının analizi): Simetrik yapıların çoğunda matematiksel bir güvenlik ispatı olmasa da, çeşitli saldırılara karşı güvenliğin analiz edilmesiyle bu protokollerin güvenlikleri hakkında belirli güvencelere sahip olabiliyoruz. Bu konuda iki iyi kaynak:

- [Cihangir Tezcan Hoca'nın Applied Cryptanalysis Dersi](https://www.youtube.com/watch?v=CXcHNkq5mFo&list=PLUoixF7agmIsF8NiiQcCMB9x5mi3l8dEW): Sadece kriptanaliz üzerine derlenmiş bir video ders serisi bulmak diğer kaynaklara kıyasla oldukça zor. Cihangir Hoca'nın bu dersi bu konudaki en iyi videolu kaynaklardan biri.

- [A Tutorial on Linear and Differential Cryptanalysis - Heys](https://ioactive.com/wp-content/uploads/2015/07/ldc_tutorial.pdf): En yaygın kriptanaliz tekniklerinden lineer ve diferansiyel tekniklerin anlatıldığı her derste mutlaka ek materyal olarak kullanılan bir dökuman.

- Simetrik protokollerin tasarımı: Nasıl başlanır kısmında bahsedilen kitabı okuduktan sonra bu konuda biraz daha fikriniz oluşmuş olacak. Bundan sonrasında farklı simetrik yapılar hakkında makaleler okumak ve bazı düşünce egzersizleri yapmak oldukça faydalı. Bu egzersizlere örnekler
- Öğrenilen farklı yapıalr arasında paraleller çekmek (S-Box'ların kullanımlarının benzerliği vb.)
- Protokolleri oluşturan bazı kısımları yoksayıp, bu kısmın yokluğunda güvenliğin nasıl etkileneceğini düşünmek.

