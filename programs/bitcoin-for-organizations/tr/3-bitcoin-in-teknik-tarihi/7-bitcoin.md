# 3.7 Bitcoin

Yıllar süren birçok başarısız denemenin ardından, Cypherpunk'lar büyük ölçüde dijital, izinsiz bir para birimi fikrine olan ilgilerini kaybetmeye başlamışlardı ki, Adam Back, kendisini Satoshi Nakamoto olarak tanıtan anonim bir kişiden 'üçüncü bir taraf olmadan elektronik nakit' başlıklı bir taslak beyaz kağıda bağlantı içeren bir e-posta aldı.

Bu noktada özetlemek gerekirse, elimizde en azından şu fikirler var:

* Gizlilik ve anonimlik düzeyi sağlayabilen kriptografik imzalar
* Teminatsız bir para birimi kavramı (B-Money)
* Yeni para biriminin ihraç edilmesini sınırlamaya yönelik öneriler (ancak bir yöntem yok)
* Sahipliği açık anahtarlarla atanan dijital paralar (B-Money) ve imzalanarak taşınabilen, alıcı adresine göre yeniden atanabilen paralar (RPOW ve Hashcash)
* Tüm düğümlerin tamamen dağıtık bir defterin bir kopyasını tutması (B-Money) (o zamanlar uygulanamaz olarak reddedilmişti)
* Zaman damgalama protokolü – Tüm kullanıcılar aynı kayıtları tuttuğu sürece, olayların matematiksel olarak kanıtlanabilir bir kronolojisini sağlamak için Merkle ağacı karması kullanmak ve bu kayıtların tahrif edilmesini zorlaştırmak
* Gerçek dünyadaki çabayı sisteme bağlamak için iş ispatı (ancak paranın kendisi olarak hash kullanılıyordu)
* Tüm eşlerin eşit olduğu ve ağa girip çıkabildiği tamamen merkeziyetsiz ağlar (BitTorrent)
* Yeni hash'lerin önceki hash'lere bağlanması kavramı (Bit Gold ve zaman damgalama)

O dönemde eksik olanlar şunlardı:

* ‘Bizans generalleri’ problemini çözecek uygulanabilir bir çözüm
* Donanım sürekli gelişirken dolaşımdaki para miktarını sınırlayacak bir yöntem
* Katılımı teşvik edecek bir ödül sistemi (tavuk-yumurta sorunu)

Son dönemdeki denemeler ile Bitcoin arasındaki bir diğer büyük fark ise, Satoshi'nin, Bit Gold ve B-Money'nin daha çok kavramsal olmasına karşın, duyurmadan önce bir süredir kod üzerinde çalışıyor olmasıydı; bu, gerçek 'Cypherpunk'lar kod yazar' ilkesiyle uyumluydu.

Bitcoin’i önceki elektronik nakit denemelerinden ayıran yenilik neydi?

İş ispatı, bir fikir birliği mekanizması ve güvenlik ile değişmezlik sağlama yöntemi olarak kullanılacaktı: Hash'i bir para birimi olarak kullanmak yerine, madencilik adı verilen yeni bir kavramsal süreçte kullanılacaktı; burada bir düğüm bir dizi işlemi bir araya getirir, rastgele bir sayı ekler ve ardından bu 'blok' verisine hash uygular. Hash gereksinimini karşılayan geçerli bir blok daha sonra ağa duyurulurdu. Bu bloklar, her birinde önceki bloğun hash'i kullanılarak birbirine bağlanır ve farklı düğümlerin aynı anda farklı blokları doğrulayıp duyurmasıyla zincir bölünmeleri oluştuğunda, en uzun blok zinciri tiebreaker olarak kullanılırdı. İş ispatı, Bizans generalleri problemini çözmek için dağıtık bir tiebreaker haline geldi.

Bu madencilere, iş ispatını gerçekleştirmek için gereken CPU gücünü sağlamaları karşılığında her blok için yeni bitcoin tahsis edilerek bir teşvik de verildi. Aldıkları Bitcoin miktarı da yaklaşık her 4 yılda bir azalacak şekilde programlanmıştır ve tüm Bitcoin'ler üretildiğinde sıfırlanır; böylece dolaşımdaki toplam Bitcoin miktarı 21 milyon ile sınırlandırılmış olur.

En özgün fikir, donanım geliştikçe ve ağa daha fazla güç uygulanabildikçe ne kadar para üretileceği sorununu çözme şekliydi. Belirli sayıda bloğun (2016) zaman damgaları ortalaması alınacak ve eğer bloklar çok hızlı üretiliyorsa, yeni bir blok oluşturmak için gereken hash daha zor hale getirilecek, çok yavaşsa daha kolaylaştırılacaktı. Bu, tüm düğümlerin çalıştırdığı merkeziyetsiz protokole yerleştirildi ve bu kuralı görmezden gelen herhangi bir madenci, ağı geri kalanının reddedeceği bir bloğu üretmek için enerji harcamış olacaktı. Bu ayarlama, yeni blokların oluşturulmasının planlanan ihraç takvimine uygun kalmasını sağlar ve madencilerin 'kurallara uymasını' teşvik eder.

####   
Özet

Sağlam para ilkelerine dayalı merkeziyetsiz, eşler arası bir elektronik nakit sistemi inşa etmek için gereken bulmacanın birçok parçası, Satoshi beyaz kağıdını yayınlamadan ve kısa süre sonra kodun ilk sürümünü çıkarmadan önce zaten mevcuttu.

> Bitcoin'in doğası gereği, 0.1 sürümü yayınlandıktan sonra çekirdek tasarımı ömrü boyunca değiştirilemez şekilde sabitlenmiş oldu  
_Satoshi Nakamoto_

Birçok iyileştirme fikri (BIP) önerilip kabul edilmiş olsa da, Bitcoin 2009'dan beri arka planda, ilk sürümde tasarlanan protokolü takip ederek ve neredeyse hiç kesintiye uğramadan çalışıyor. Tüm iyileştirmeler, önceki tüm sürümlerle geriye dönük uyumluluk sağlanarak gerçekleştirildi.



##### Notlar

1. Bizans Generalleri problemi açıklaması için bkz.[https://tr.wikipedia.org/wiki/Bizans_hatası](https://en.wikipedia.org/wiki/Byzantine_fault)
