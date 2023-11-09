------------------------------------------------------------------
title      : Kriptografi Üzerine
subtitle   : Abdullah Talayhan
nav-group  : featured
nav-width  : 300px
css-header : background:linear-gradient(to bottom right, #06c, #fc0); color:white
menu       : 
   Ana Sayfa    : ?
   Konular : ?post=topics.md
   Karanlık Modu    : javascript:darkmode()
   İletişim   : https://abdullahtalayhan.com
------------------------------------------------------------------
<style comment="additional style">
span.post-tags{
    display: none;
    visibility: hidden;
}

a {
    font-weight: bold;
}

</style>

<div id="md-post">

## Kriptografi Öğrenmek Üzerine

<span class="post-date">2023-10-07</span>

Bu sayfada 2015 yılından beri kriptografi alanında çalışmaya başlama ve sonrasında çalıştığım alanı daraltma sürecinde kullandığım materyalleri organize bir şekilde toplamayı amaçlıyorum. Türkiye'deki üniversite müfredatlarına daha hakim olduğum için yazılardaki perspektif ve önerilerin Türk öğrencilere daha faydalı olmasını umuyorum. Kriptografi'nin farklı alanları için oluşturduğum her sayfada; alanın genel olarak ne tarz problemler üzerine çalıştığı hakkında ufak bir özet, sonrasında **nasıl başlarım** ve **nasıl ilerlerim** başlıkları altında materyal önerileri var. Soldaki menüden veya mobil bir cihazdan okuyorsanız üstteki "Konular" sekmesinden yazılara ulaşabilirsiniz.

Önerilen kaynaklar hususunda takip ettiğim bir kaç prensip var:

1. Önerilen kaynakların tamamı benim bireysel olarak tercih ettiğim veya birlikte çalıştığım öğrenciler tarafından kullanım sürecine şahitlik ettiğim kaynaklardan oluşuyor. Kaynak üzerinde yeterli vakit harcamadıysam önerilerde yer almıyor.
2. Bazı konular için önerilebilecek birden fazla kaynak var, kendi öğrenim sürecimde aynı konu için farklı kaynaklar arasında çok fazla vakit kaybettim. Sonrasında bir konuyu öğrenmek için "yeterince iyi" bir kaynak belirleyip geri kalan her şeyi ikincil olarak görme gibi bir düstur edindim. Bu sebeple hem nasıl başlarım hem de nasıl ilerlerim alt başlıklarında bulunan kaynaklar, birbirlerinin alternatifi olarak değil, öğrenmek istediğiniz şeye göre ard arda tüketilebilecek şekilde düzenlendi.  
3. 2. prensipin geçerli olmadığı tek durum ücretsiz olarak erişilemeyen bir kaynağa ücretsiz bir alternatif sunmak istediğim durumlar.

**Not: Bir konuyu öğrenmenin birden fazla ve kişiden kişiye göre efektifliği değişen yolları var. Bu yazıların amacı insanları farklı farklı bir sürü kaynağa boğmak yerine tecrübelere dayanarak daha spesifik bir yol çizmek. Bu sebeple yeterince iyi olup bu yazılarda belirtilmeyen kaynaklar ve yaklaşımlar olacaktır.**

**Altyapı problemleri:** 
Kriptografi, Bilgisayar Bilimi ve Matematiğin tam ortasında duran bir alan olduğu için iki taraftan da kalburüstü bilgi gerektiriyor. Bu da kişinin kendi öğrendiği konu ne olursa olsun iki alanda da ortak bir hakimiyet yoksa belli noktalarda durup başka bir konuyu çalışmasını gerektiriyor. Bu sebeple Teorik Bilgisayar Bilimi ve Matematik adları altında bulunan iki sayfada bu alanlardan kriptografi öğrenirken gerekecek konulardan ve bu konularla ilgili materyallerden bahsettim.

**Crypto Boom ve ZK Üzerine:** 
Blockchain ve Zero-Knowledge alanında son yıllarda gerçekleşen ilerlemeler ve endüstriyel motivasyonlar sebebi ile kriptografi öğrenmek isteyen insan sayısında ciddi bir artış var. Bu inanılmaz mutlu edici bir gelişme. Ancak burada bir problem var. Öğrenilmek istenen en popüler konu sıfır bilgi ispatları (zero-knowledge proofs) veya bu konuya yakın diğer konular. İnsanların temel kriptografi bilgisi edinmeden direkt olarak bu konuyu öğrenme gibi bir çabası var. Bu çabayı gören akademik ve endüstriyel oluşumlar buna karşılık direkt olarak bu konulara merakı olan insanlara odaklı pedagojik materyaller üretmeye çalışıyor. Bunlardan bazıları pedagojik olarak başarılı, bazıları başarısız. Ben genel olarak bu yaklaşımı doğru bulmuyorum. Temel kriptografi bilgisi derken; şifreleme, dijital imzalar, özet fonksiyonları gibi temel kriptografik yapıların nasıl çalıştığı konusunda bilgi sahibi olmak ve çok daha önemlisi bu yapıların hangi durumlarda veya hangi saldırı modellerinde güvenli olduğunu bilmekten bahsediyorum. Bu konular sıfır bilgi ispatları gibi başka bir çok kriptografik protokolün de temelini oluşturmakla beraber, alakasız olsalar bile "kriptografik saldırgan" mentalitesi kazanmak için çok önemli konular. Mahremiyet, güven, para gibi yüksek riskli şeylerin çeşitli protokoller ile korunduğu bu alanda bazı şeyleri öğrenmek için acele etmek yapılabilecek en yanlış şeylerden biri. Bu söylediklerim gatekeeping gibi anlaşılmasın. Bir kapı tutmanın aksine bir kapı açmaya çalışıyorum, bunun ilk aşamasını da yanlış kapıda bekleyenleri uyarmak olarak görüyorum. Burada bir şeyler öğrenmeye çalışan insanların bir hatası yok. Endüstriyel bir yarış içerisinde yeterli olgunluğa erişmeyen protokolleri canlıya alanların, **gereğinden fazla** basitleştirilmiş blog yazılarıyla insanlara yanlış bilgi verenlerin hatası var. "Kriptografi pahalı bir zevktir, hata kaldırmaz" diyerek bu kısmı da bitirmiş olalım.

Herkese iyi çalışmalar diliyorum.

Abdullah Talayhan


Bu site <a href="https://github.com/casualwriter/casual-markdown">casual-markdown</a> kullanılarak oluşturuldu.

## Yazılar

* 2023/10/08: [Temel Kriptografi](temel_kriptografi.md) {#starter}
* 2023/10/08: [Simetrik Kriptografi](simetrik.md) {#featured}
* 2023/10/08: [Multiparty Computation](mpc.md) {#featured}
* 2023/10/08: [Zero-Knowledge Proofs](zk.md) {#featured}
* 2023/10/08: [Post-Quantum Cryptography](post_quantum.md) {#featured}
* 2023/10/08: [Side Channel Attacks](side_channel.md) {#featured}
* 2023/10/08: [Matematik](matematik.md) {#alt}
* 2023/10/08: [Teorik Bilgisayar Bilimi](tcs.md) {#alt}




</div>