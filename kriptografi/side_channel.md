## Side Channel

Yan Kanal (Side Channel) saldırıları protokollerin çalıştığı sırada fiziksel olarak gerçekleşen olayların gözlenmesi sonucu elde edilen bilgiler sayesinde bir kriptosistemde zaafiyet aradığımız bir alan. Örneğin bir işlemci'nin anlık olarak harcadığı gücü ölçerek o sırada hangi operasyonu çalıştırdığını takip etmek mümkün olabiliyor. Bu durumda işlemciye fiziksel erişim olduğunu varsayıyoruz. Ancak yan kanal saldırılarının fiziksel erişim gerektirmeyen varyantları da var. Örneğin bir sunucu ile mesaj alışverişinde bulunurken sunucunun yolladığı mesajların geliş süresi üzerinden bazı çıkarımlar yapmak mümkün. Bu alanda özet olarak, bir kriptosistem çalıştığı esnada çeşitli fiziksel veriler toplayıp. Bu veriler üzerinde istatistiksel analizler yaparak belirli tahminlerde bulunuyoruz.


### Nasıl Başlarım?

<strong>Önkoşul:</strong> Temel kriptografi

- [ChipWhisperer - Introduction to Side Channel Analysis](https://learn.chipwhisperer.io/courses/introduction-to-side-channel-analysis): Chipwhisperer yan kanal saldırılarında kullanılan bir çok ölçüm cihazını üreten bir firma. Eski olsa da genel bir fikir edinmek için çok iyi bir kaynak.
- [SideChannelSecurity Youtube Kanalı](https://www.youtube.com/@SideChannelSecurity/about): TU Graz yan kanal saldırıları konusunda dünyada çok önemli çalışmalara sahip ve aktif olarak bu alanda çalışan bir araştırma grubuna sahip. Bu youtube kanalı araştırma grubundaki insanlar tarafından çeşitli mizahsenler ile bazı yan kanal saldırıları konseptlerini anlatıyor. Normalde bu tarz içerikler gereğinden fazla basitleştirilmiş olabiliyor ve bu duruma fazlasıyla karşıyım. Bu ekibin videoları bazı şeyleri olduğundan daha basit göstermeden nasıl erişilebilir kılınacağının çok güzel bir örneği.


### Nasıl İlerlerim?:

Yan kanal saldırılarının bir çok çeşidi var, ben bunlardan sadece bir tanesi ile kısa bir süre ilgilendiğim için bu alanda ilerleme konusunda bir öneride bulunmayacağım. Fault attack adını verdiğimiz hesaplama sırasında gerçekleşen fiziksel hataları (buna fault diyoruz) kullanarak yapılan saldırılar ilginizi çekerse, bu kaynağı [The Sorcerer’s Apprentice Guide to Fault Attacks](https://eprint.iacr.org/2004/100.pdf) okuyarak ilerleyebilirsiniz. Bunun dışında timing (hesaplama süresine bağlı), power (harcanan güce bağlı), EM (yayılan elektromanyetik yayılmalara bağlı) şeklinde diğer popüler alt dalları inceleyebilirisiniz fakat nasıl ilerlenebileceği hakkında bir fikrim yok.
