# 7.1 Lightning Ağı

Lightning Network, kullanıcıların bitcoin'i hızlı ve düşük maliyetle göndermesini ve almasını sağlayan bir ödeme sistemidir. İki tarafın bitcoin'lerinin bir kısmını depoladığı ortak bir cüzdan kurarak çalışır. Böylece, ana blokzincirine her işlemi kaydetmeye gerek kalmadan birbirleriyle sınırsız işlem yapabilirler. Bu sayede, her işlemin bir bloğa dahil edilip doğrulanması gerekliliği atlanır ve süreç hem hızlı hem de ekonomik hale gelir. Düşük ücretler sayesinde Lightning Network, zincir üstünde her zaman mümkün olmayan küçük ödemeler için de kullanılabilir. Taraflar işbirliğini sonlandırmaya karar verdiğinde ise yalnızca nihai bakiye blokzincirine kaydedilir.

Bir kafede çalıştığınız bir günü hayal edin. Bir süre kalmayı planladığınız için her sipariş için ayrı ayrı ödeme yapmak yerine bir hesap açıp önceden ödeme yaparsınız. Günün sonunda, siz ve işletme sahibi hesabı gözden geçirip borcunuzu kapatırsınız. Eğer depozitonuz harcadığınızdan fazlaysa, aradaki farkı geri alırsınız; eğer daha fazla harcadıysanız, kalan borcunuzu ödersiniz.

Bu sistem daha fazla katılımcıyı kapsayacak şekilde genişletilebilir. Örneğin, kafeye yaptığınız ziyaretlerden birinde, barmenin tanımadığı ve hesap açamayacak bir arkadaşınızı getiriyorsunuz. Arkadaşınızın harcamalarını karşılamak için mevcut hesabınızı kullanmasına izin veriyorsunuz ve aranızda, size özel olarak geri ödeme yapacağına dair anlaşıyorsunuz. Şimdi binlerce kişinin aynı anda bunu yaptığını ve başkalarının da mevcut hesapları kullanarak daha fazla kişiyle bağlantı kurabildiğini hayal edin — işte Lightning Network böyle çalışır!

Lightning ile, yalnızca doğrudan hesap açtığınız kişiye değil, ağdaki herkese ödeme yapabilirsiniz — iki taraf arasında bir yol bulunabildiği sürece. Ödemeniz, alıcıya ulaşana kadar ağ üzerinden yönlendirilir; doğrudan alıcıyla açık bir kanalınız olmasa bile.

Zincir üstü ve zincir dışı işlemler arasındaki farka bir göz atalım.

##### Zincir Üstü İşlemler

Bunlar, doğrudan Bitcoin blokzincirinde gerçekleşen işlemlerdir. Onaylanmaları yaklaşık 10 dakika sürer ve ücretler, işlemin sanal bayt cinsinden boyutuna bağlıdır. Daha güvenlidirler fakat daha yavaştırlar, çünkü ağın uzlaşmasını gerektirirler.

##### Lightning Network İşlemleri

Bu işlemler, Bitcoin blokzinciri üzerine inşa edilmiş ayrı bir ağda gerçekleşir. Daha hızlı sonuçlanır ve daha düşük ücretlidir. Genellikle, işlemlerin hızı ve maliyeti gibi unsurların daha önemli olduğu durumlarda kullanılır. Zincir üstü işlemlerle karşılaştırıldığında, daha az güvenlidirler.


|  | Bitcoin Ağı | Lightning Network |
| --- | --- | --- |
| Tanım | Finansal işlemleri güvence altına almak için kriptografi kullanan merkeziyetsiz dijital bir ağ. | Bitcoin blokzinciri üzerinde çalışan, daha hızlı ve ucuz işlemler sağlayan ikinci katman bir ödeme protokolü. |
| Avantajlar | Merkeziyetsiz ve güvenli. Ters ibraz veya dolandırıcılık yok. Takma adla kullanılabilir. Küresel kabul. | Daha hızlı ve ucuz işlemler. Artan ölçeklenebilirlik. Zincir dışı işlemler blokzincirini tıkamaz. |
| Dezavantajlar | Yavaş işlem süreleri. Bazı işlem türlerinde yüksek ücretler. Yeni başlayanlar için karmaşık. | Kanal operatörlerine güven gerektirebilir. Kanal açmak ve kapatmak için zincir üstü işlem gerekir. |
