## Temel Kriptografi

Aslında "temel kriptografi" diyebileceğimiz bir alt alan yok. Ancak burada ekstra bir alt alan belirtmeye gerek kalmayacak kadar kriptografi şemsiyenin altında yer etmiş yapıları kast ediyorum. Bunlar, şifreleme, dijital imzalar, özet fonksiyonları gibi bir çok başka protokolün parçası ve kendi içlerinde de ayrı araştırma alanları bulunan konular. Dolayısıyla hiç kriptografi bilmeyen kişilerin de başlangıç noktası burası.



### Nasıl Başlarım?

- [Introduction to Cryptography - Paar](https://www.youtube.com/@introductiontocryptography4223/videos): 2015 yılında ilk defa sistematik bir şekilde kriptografi öğrendiğim kaynak. Bu sebeple ekstra bir sempatim olsa da, ilk defa kriptografiyle ilgili bir şey öğrenmek için daha iyi bir kaynak aklıma gelmiyor. Tahtaya yazarak anlatım sebebiyle temposu çok hızlı değil. Anlatım sırasında tarihsel örneklerle kriptografi konusunun genel etkileri ve bazı çalışma alanlarından da bahsediliyor. Haftasonları hariç her gün 1, 1.5 saat çalışma vaktiniz varsa 24 videoyu 1 ay gibi bir süreye yayarak tüketebilirsiniz. Dersin bir kitabı da var ancak önerim bu seriyi bitirene kadar sadece videolara odaklanmak ve başka bir kaynak ile ilgilenmemek.

- [Introduction to Modern Cryptography - Katz & Lindell](https://www.cs.umd.edu/~jkatz/imc.html): Lisans seviyesinde bir çok okulun kriptografiye giriş dersinde kullanılan kitap, hala güncelliğini koruyor (2020 yılında 3. versiyonu yayınlandı). Kriptografi ile ilgili makale okurken veya genel olarak bir şeyler öğrenirken en çok zorlanılan kısım genelde güvenlik ispatları oluyor. Kriptografik protokollerin güvenliği formal olarak tanımlı bir şey olduğu için, bu güvenliğin sağlanıp sağlanmadığını ortaya koyduğumuz protokol için ispatlamak istiyoruz. Bu da ancak ispat okuyup yazarak gelişen bir beceri. Bir sürü kriptografiye giriş kitabı arasından bunu önerme sebebim (ve bir çok okulun da kullanıyor olma sebebi) kitabın bahsettiğim bu sıkıntı çekilen noktalara öğretici bir şekilde yükleniyor olması. Kitapta ilk okuyuşta geçilmesi önerilen yıldızlı üniteler var. Bu genelde ilk defa kriptografi öğrenenler için, siz yukarıdaki video serisini tamamladığınız için o üniteleri de geçmeden okuyabilirsiniz.




### Nasıl İlerlerim?

İlerlemenin bir çok yolu olmakla beraber ilerlerken karşılaşılabilecek bazı problemler var. Farklı alt alanlara başlamaya o alanların kendi yazısında değindiğim için burada daha genel şeylerden bahsedeceğim. Öncelikle üstteki kaynaklarla yeterince vakit geçirip bazı konularda daha fazla bilgiye veya farklı bir perspektife ihtiyaç varsa şu kaynağa geçmek mantıklı olacaktır:

- [A Graduate Course in Applied Cryptography - Boneh & Shoup](http://toc.cryptobook.us): Bu kitap henüz bitmedi ancak teknik içeriğin çoğu yazılmış durumda. Katz & Lindell kitabından bildiğiniz bazı kısımları atlayabilirsiniz ama tam oturmadığını düşündüğünüz veya unuttuğunuz şeylerin tekrar üzerinden geçecekseniz biraz daha detaylı ve daha tecrübeli bir okuyuca hitap ettiği için bu kitabı kullanmakta fayda var. Kriptografinin bir çok alt alanı konusunda da ünitlere sahip olduğu için o alanlar hakkında fikir edinmek için de uygun sayılır.

- **Makale okuma:** Bu noktada yavaş yavaş kriptografi makaleleri okumaya başlamak mümkün. Kriptografi alanı bu konuda çok şanslı çünkü neredeyse bütün makaleler tek bir çatı altında toplanmış durumda. eprint.iacr.org adresinden 1996'dan itibaren yayınlanmış neredeyse her kriptografi makalesini bulabilirsiniz. Tabi çoğu makale maalesef anlaşılabilirlik gayesi ile yazılmadığı için bazen okumak zor olabilir (makalesine göre de değişir). Ancak tam olarak anlamadan da bazı makaleleri yavaş yavaş okumaya başlamak bu alışkanlığı edinmek için iyi bir yol. Takıldığınızda makale hakkında soru sormak için https://askcryp.to platformunu kullanabilirsiniz.
- <strong>İmplementasyon</strong> Bir kriptografik protokolün tasarımı ne kadar zorsa, implementasyonu da bir o kadar zor. Güvenli protokol implementasyonları yapmak kendi içerisinde bambaşka problemler içeriyor. İmplementasyon yapmaktan daha çok keyif alan biri temel kriptografi bilgisi edindikten sonra tamamen bu konuya da kanalize olabilir. Burada Cryptopals gibi implementasyon görevlerinin bulunduğu bir platformda sorular çözmek faydalı olabilir. 

- **Günlük hayatta kriptografi:** Nasıl başlarım kısmında kısa bir mesafe kat ettikten sonra bile günlük hayatta kullandığımız bazı protokollerin nasıl çalıştığını biliyor olacaksınız. Bu sebeple bir noktada bu protokollerin günlük hayattaki örneklerini incelemek, implementasyon veya yasal detaylarına bakmak bu konuyu körü körüne sadece teorik amaçlarla çalışmaya kıyasla daha keyifli hale getirecektir.

- **CTF:** Capture The Flag, genel olarak siber güvenlik alanlarında oldukça popüler olan bir yarışma formatı. Çoğunda kriptografi ile ilgili sorular da oluyor ve çoğunlukla gerçek hayatta da bir noktada gerçekleşmiş zaafiyetleri barındırıyorlar. Yarışmacıların amacı bu zaafiyetleri keşfedip kullanarak bayrak adını verdiğimiz gizli değerlere ulaşıp, bu değerleri sisteme girip puan kazanmak. Bu yarışmalar da hem zevkli hem de öğrenmeyi tetikleyici olabiliyor. Ancak burada ufak bir uyarıda bulunmak lazım, eğer sadece pratik bilginizi geliştirmek amacıyla oynuyorsanız çok fazla rekabete kapılmamak gerekiyor. Aynı zamanda, yarışma ortamında bazı şeyleri hızlı düşünmek gerekiyor, ancak gerçek hayatta durum böyle değil ve aksine bazı şeyleri daha düşük tempoda düşünmek faydalı olabiliyor. Bu açıdan aktif yarışmalar yerine hali hazırda yayınlanmış CTF sorularını kendi zaman çizelgenizde çözebilirsiniz. CTF tarzı sorularla kriptografi problemleri çözmeyi amaçlayan https://cryptohack.org platformu bu iş için oldukça iyi.


