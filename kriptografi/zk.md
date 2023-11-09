## Zero-Knowledge Proofs


**Nasıl Başlarım?**

<strong>Önkoşul:</strong> Temel Kriptografi, Teorik Bilgisayar Bilimine Giriş

Öncelikle ben hatırladığım kadarıyla bu konuyu ilk 2018 yılında öğrenmeye çalıştım, o sırada Boneh Shoup kitabının 2017 versiyonunun 19 ve 20. bölümlerini okuyarak başlamıştım. Sonradan bu konuda kaynaklar çoğaldıktan sonra tekrar öğrendim, Boneh Shoup her ne kadar gayet iyi olsa da birincil önerim farklı olacak:

- [Foundations of Probabilistic Proofs Part I](https://www.youtube.com/watch?v=yWD_1WK3DNU&list=PLGkwtcB-DfpzST-medFVvrKhinZisfluC): Linkteki playlist'in ilk 8 videosu (önkoşulları takip ettiğinizi varsayarak) bu konuda sağlam bir temel oluşturmak için eşi bulunmaz bir kaynak. Alessandro Chiesa ders aldığım kişiler arasında anlatma stili olarak örnek teşkil eden birisi. Oldukça ağır konuları bile konunun detaylarını halının altına süpürmeden anlaşılır bir şekilde anlatıyor. Bazı kısımları bir kaç kez tekrar etmek veya öğrenen başka insanlara sormak faydalı olabilir.

- [On Sigma Protocols - Damgard](https://www.cs.au.dk/~ivan/Sigma.pdf): Sıfır bilgi ispatlarında en yaygın protokol stillerinden biri olan sigma protokolleri hakkında biraz daha detaylı bilgi sahibi olmak ve birden fazla örnek görmek açısından çok iyi bir döküman. Damgard'ın makalelerinin konvansiyonel makalelere göre daha anlaşılır olmasının da bu öneride etkisi var.


**Nasıl İlerlerim?**

- [Foundations of Probabilistic Proofs Part II](https://www.youtube.com/watch?v=yWD_1WK3DNU&list=PLGkwtcB-DfpzST-medFVvrKhinZisfluC): Nasıl başlarım kısmında önerdiğim ilk 8 videonun sonrası. 9. videodan itibaren materyal biraz ağırlaşacak ve eğer teorik bilgisayar bilimi konularından karmaşıklık teorisi (complexity theory) konusunda eksiğiniz varsa bu derste ilerlemenizi yavaşlatabilir TODO(TCS) yazısından bu konuda önerilere bakabilirsiniz. Burada aynı zamanda 18. videodan itibaren (Lecture 17) Reed-Solomon error correcting code kullanılmaya başlanacak. Buradan önce Mary Wootters tarafından anlatılan [Alebraic Coding Theory](https://www.youtube.com/watch?v=vfjN7MmSB6g&list=PLkvhuSoxwjI_UudECvFYArvG0cLbFlzSr) serisinin 1-4., 8. ve 15-17. videolarını izleyebilirsiniz.

- [Proofs Arguments and Zero-Knowledge](https://people.cs.georgetown.edu/jthaler/ProofsArgsAndZK.html): Bu kitap aslında Foundations of Probabilistic Proofs dersi ile paralel konulara sahip ancak ilk kaynakta anlatılan teorik modellerin gerçek hayatta kriptografik olarak nasıl gerçeklendiği de anlatılıyor. Dolayısıyla bunu ya ilk kaynağa paralel, ya da sonrasında çalışmayı öneriyorum.

- Pratikte bir çok protokol "pairing" dediğimiz eliptik eğriler üzerinde tanımlı bir operasyonu kullanıyor. Bu operasyonun nasıl çalıştığı veya hangi eğriler üzerinde çalıştığının matematiği kriptografiye giriş tarzı derslerde genelde bulunmuyor ve nasıl çalıştığını bilmediğimiz bir şeyi bir kriptosistemde kullanmak büyük bir hata olur. Bu açığı Pairings for beginners (https://static1.squarespace.com/static/5fdbb09f31d71c1227082339/t/5ff394720493bd28278889c6/1609798774687/PairingsForBeginners.pdf) kitabını kullanarak çok doğru ve sağlam bir şekilde kapatabilirsiniz. Bu kitap konusundaki tek eleştirim implementasyon örneklerinin Sage yerine oldukça pahalı bir araç olan Magma ile yazılmış olması. Ancak bu durum aynı örnekleri Sage ile yazma egzersizi olarak güzel bir fırsat.


Bazılarınız burada [zk-learning.org](https://zk-learning.org)'u direkt görmediği için şaşırmış olabilir. Bunun iki sebebi var

1. Birden fazla kişi tarafından tasarlanmış dersler ne olursa olsun tek kişi tarafından tasarlanmış materyallerin sağladığı tutarlılığı sağlamıyor. O yüzden ana materyal olarak önermek istemedim. Zaten ikinci kaynağın yazarı Justin Thaler'da bu derslerde yer aldığı için ortak olan bir çok nokta da var.
2. Yukarıdaki materyalleri tüketirken bazen direkt olarak anlaşılmayan veya yeterince spesifik olmayan şeyler olacak, bu durumlarda başka bir kişiden dinlemek/okumak iyi olabiliyor. Zk-learning üniteleri birbirinden yeterince ayrı olduğu için o kaynağı aradan bazı konuları seçerek dinlemek/okumak için kullanabilirsiniz.



