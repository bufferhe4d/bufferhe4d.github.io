## Multiparty Computation (MPC)

MPC protokolleri birden fazla bilgisayarın birlikte hesap yaptığı protokoller. Bu senaryodaki güvenlik kriteri protokolde yer alan bilgisayarların belirli girdileri saklayabilmeleri. Örneğin sırasıyla x, y ve z girdilerine sahip 3 farklı bilgisayar f(x, y, z) fonksiyonunu hesaplarken, bilgisayarların birbirlerinin girdilerini öğrenmemelerini istiyoruz. Özellikle tek bir kişiye güvenilmesi gereken sistemlerde bu güveni dağıtma amacıyla MPC protokolleri oldukça yaygın kullanılıyor.

### Nasıl Başlarım?

<strong>Önkoşul:</strong> Temel kriptografi ve teorik bilgisayar bilimi (Özellikle boolean circuit'lar) 
konusunda giriş seviyesi bile olsa bilgi sahibi olmanız aşağıda bahsi geçen kaynaklardan daha iyi faydalanmanızı sağlayacaktır.

- [Pragmatic MPC - Evans, Kolesnikov & Rosulek](https://securecomputation.org/docs/pragmaticmpc.pdf): Bu kaynak daha önce MPC alanında çalışmamış ve bu alana ilgi duyup duymadığını merak eden insanlar için oldukça faydalı bir kitap. Günümüzde aktif araştırmaları okurken sıklıkla karşılaşılabilecek temel MPC protokollerinin çoğu anlaşılabilir bir şekilde anlatılıyor.

### Nasıl İlerlerim?

- Pragmatic MPC kitabının her ünitesinin sonunda Further Reading adı altında listelenen kaynaklara bakabilirsiniz. Bunlardan bazıları okuması zor eski makaleler olabilir, yine de kitap içerisinde bahsedilen bazı yapıların hangi makalede ve hangi tarihte ortaya çıktığını bilmek bile faydası olan bir şey.
- [Secure Multiparty Computation and Secret Sharing - Cramer, Damgard, Nielsen](https://www.cambridge.org/dk/universitypress/subjects/computer-science/cryptography-cryptology-and-coding/secure-multiparty-computation-and-secret-sharing?format=HB): Pragmatic MPC üzerine ikincil bir kaynak olarak oldukça uygun. Yazarları da bu alanda önemli ilerlememeler sağlamış isimlerden oluşuyor.

MPC alanında yapılan güvenlik ispatlarının neredeyse tamamı Universally Composable (UC) adını verdiğimiz framework altında yapılıyor. Bu ispat yönetime alışmanın en iyi yollarından biri bol bol UC ispatı okumak ancak başta bu ispatları anlamak oldukça zor olabiliyor, sürece alışmayı kolaylaştıracak iki kaynak önerebiliriz:
- [How To Simulate It - Lindell](https://eprint.iacr.org/2016/046.pdf): UC'nin biraz daha limitli bir varyantını (Sequential Composition) en açık şekilde öğreten kaynaklardan biri.
- [https://eprint.iacr.org/2014/553](https://eprint.iacr.org/2014/553): UC'nin bir çok protokolün ispatı için yeterli olan daha basit bir varyantı.


<strong>İmplementasyon:</strong>
- Öğrenme odaklı basit bir kütüphane: [https://github.com/kennysong/tinysmpc](https://github.com/kennysong/tinysmpc)