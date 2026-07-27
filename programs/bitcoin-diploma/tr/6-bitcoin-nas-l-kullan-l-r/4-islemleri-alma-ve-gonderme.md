# 6.4 İşlemleri Alma ve Gönderme

Bir Bitcoin işlemi, bitcoin'in mülkiyetinin yeni bir sahibine devredilmesidir. Burada aktarılan şeyin gerçek madeni paralar değil, onların mülkiyeti olduğunu unutmayın: başka bir deyişle, onları harcama hakkı. Bir işlem bir bloğa kabul edildiğinde, ağdaki tüm düğümler, kamu defterinin yerel kopyalarını mülkiyet değişikliğini yansıtacak şekilde günceller. Bu açıdan, bir Bitcoin işlemi nakit işlemden ziyade bir gayrimenkul (veya başka bir mülk) işlemine daha çok benzer.

Bitcoin "göndermek" için, gönderen kişi özel anahtarıyla bir mesaj imzalar ve ağdaki herkese bitcoin'in gerçek sahibinin mülkiyeti alıcıya devrettiğini bildirir.

Bitcoin artık alıcının adresine bağlı olacak ve ona bitcoin'in mülkiyetini verecek, böylece yalnızca yeni sahibi, kendi özel anahtarını kullanarak bu bitcoinleri harcayabilecektir.

Yeni Bitcoin işlemleri dünyanın dört bir yanındaki cüzdanlardan başlatılır, ancak merkezi bir ödeme işlemcisi yoktur. Bunun yerine, madenciler işlemleri deftere kaydetmek için rekabet eder.

Diyelim ki Cem, Elif'e 0,5 BTC borçlu ve borcunu ödemeye hazır. İkisinin de dijital cüzdanı var.

1. Elif, adresini Cem ile paylaşır.
1. Cem, cüzdan yazılımını kullanarak işlemi oluşturur. Bu işlem Elif’in adresini, aktarılacak miktarı (0,5 BTC) ve madenciye ödenecek bir ücreti içerir. Daha yüksek ücretler, bir madencinin işlemi bir sonraki bloğa dahil etme olasılığını artırır.
1. İşlem imzalandıktan sonra ağa yayınlanır ve düğümler tarafından doğrulanır. Cem’in yeterli bakiyesi olup olmadığı ve harcamak istediği coinlerin gerçek sahibi olup olmadığı kontrol edilir. Eğer değilse, işlem hemen reddedilir.
1. İşlem doğrulandıktan sonra, madenciler genellikle seçilen ücrete göre işlemi bir sonraki bloğa ekleyip eklememeye karar verir. İşlem bir bloğa dahil edildiğinde, blockchain'e eklenir ve fonlar Elif’in adresine aktarılır.
1. Mülkiyet Elif’e devredildi. Artık fonları harcamak için kendi özel anahtarını kullanabilir.

_İşlem tamamlandıktan sonra geri alınamayacağını unutmamak önemlidir._


> **Light – Bir Bitcoin İşlemi Nasıl Çalışır?**
>
> 1. Birisi bir işlem talep eder
> 1. İşlem, P2P bilgisayarlara (düğümlere) yayınlanır
> 1. Madenciler işlemi doğrular
> 1. İşlemler bir veri bloğu oluşturacak şekilde birleştirilir
> 1. Yeni blok mevcut blockchain'e eklenir
> 1. İşlem tamamlanır



> **Light – Bitcoin İşlemlerini Alma**
>
> Bitcoin almak için, gönderen kişiye bir Bitcoin genel adresi sağlamanız gerekir. Bu, cüzdanınızı temsil eden ve Bitcoin ağında tanımlanmasını sağlayan benzersiz bir harf ve rakam dizisidir.
>
> Genel adresinizi, Bitcoin cüzdanınızı açıp “Al” veya “Yatır” bitcoin seçeneğini arayarak bulabilirsiniz.
>
> Bitcoin adresinizi birkaç farklı şekilde paylaşabilirsiniz:
>
> 1. **Adresi kopyala ve yapıştır**: Adresi seçip "Kopyala"ya basarak kopyalayabilir, ardından bir e-posta veya mesaj içine yapıştırabilirsiniz.
> 1. **Bitcoin cüzdanınıza bir bağlantı paylaşın**: Bazı Bitcoin cüzdanları, gönderenle paylaşabileceğiniz bir cüzdan bağlantısı oluşturmanıza izin verir. Gönderen bu bağlantıya tıklayarak cüzdanınıza erişebilir ve bitcoin gönderebilir.
> 1. **Bir QR kodu paylaşın**: Gönderenin akıllı telefonunda bir Bitcoin cüzdan uygulaması varsa, QR kodunu tarayarak Bitcoin adresinizi alabilir.


Gönderen adresinizi aldıktan sonra, göndermek istediği miktarı ve adresinizi girerek size bitcoin gönderebilir. Bitcoin, gönderenin cüzdanından sizin cüzdanınıza aktarılır.

İşlem, Bitcoin Ağı tarafından onaylanır ve genellikle yaklaşık 10 dakika sürer. Daha fazla güvenlik için iki onay beklemeniz önerilir; bu da yaklaşık 20 dakika sürer.


> **Light – Bitcoin İşlemleri Gönderme**
>
> Bitcoin göndermek için birkaç şeye ihtiyacınız olacak: bir Bitcoin cüzdanı, alıcının genel adresi ve göndermek istediğiniz bitcoin miktarı.
>
> 1. Bitcoin cüzdanınızı açın.
> 1. “Gönder” butonuna gidin ve alıcının adresini "Alıcı" alanına yapıştırın. Alternatif olarak, alıcı bir QR kodu sağlarsa onu da tarayabilirsiniz.
> 1. “Miktar” alanına göndermek istediğiniz bitcoin miktarını girin.
> 1. Alıcının adresini ve gönderilecek miktarı iki kez kontrol edin. Unutmayın, işlemler geri alınamaz!
> 1. “Onayla ve Gönder”e tıklamadan önce, doğru miktarda bitcoin'i doğru adrese gönderdiğinizden emin olmak için işlem detaylarını bir kez daha kontrol etmenizi öneririz.
> 1. İşlemi yayınlayın ve ağın işlemi onaylamasını bekleyin.
>
> Artık kendi kendine saklama yapan bir Bitcoin cüzdanını nasıl değerlendireceğinizi, seçeceğinizi ve kuracağınızı biliyorsunuz. Bitcoin ağında bitcoin gönderme ve alma işlemlerine “on-chain” işlemler denir. Bunun nedeni, işlemlerin ana Bitcoin ağında gerçekleşmesi ve blockchain'e kaydedilmesidir.
>
> On-chain işlemler, ağın sağladığı merkeziyetsiz doğrulama sayesinde bitcoin ile işlem yapmanın en güvenli yoludur.
>
> Ancak, on-chain işlemler daha yavaş ve madenci ücreti nedeniyle diğer seçeneklere göre (Bölüm 7'de tartışacağız) çok daha pahalı olabilir.


#### Etkinlik: İşlemler Uygulamada


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Bu, bir Bitcoin işlemine dahil olan kişilerin temel rollerini basitleştiren işbirlikçi bir egzersizdir.**

###### Temel Noktalar

1. Her bitcoin işleminde dört tür katılımcı vardır: gönderen, alıcı, madenciler ve düğüm operatörleri.
1. Gönderen, göndermek istediği **bitcoin miktarını** VE **belirli adresi** onaylamak (kriptografik olarak imzalamak) zorundadır.
1. Alıcı, gönderen kişiye **geçerli bir adres** vermeli VE işlemin blokzincirinde başarıyla onaylandığını doğrulamalıdır.
1. Madenciler, işlemleri gelecekteki bloklara eklemeden önce tüm kriterlerin geçerli olduğundan emin olur.
1. Node (düğüm) operatörleri, blokzincirlerinin (defterlerinin) sürümünü güncellemeden önce kazılmış blokların geçerli olduğunu doğrular.

###### Öğrenci İpucu

Her bir katılımcının ne yaptığını deneyimlemek için dört rolün hepsini sırayla oynayın.
