# 6 - Bitcoin Nasıl Kullanılır

Süre: 90 dakika

Temel Fikir: Bitcoin'i zincir üzerinde kullanmak, öğrencilere sahiplik, kendi kendine saklama ve doğrulamanın pratikte nasıl işlediğini öğretir; teoriyi doğrudan finansal eyleme dönüştürür.

#### Öğrenme Hedefleri

Bu dersin sonunda öğrenciler şunları yapabilmelidir:

* Bitcoin edinmenin ve takas etmenin yaygın yollarını, eşler arası ve merkezi borsa yöntemleri dahil olmak üzere tanımlayın.
* Kendi kendine saklamalı ve saklamalı cüzdanlar arasındaki farkı açıklayın ve Bitcoin'de neden kendi kendine saklamanın önemli olduğunu anlatın.
* Özel anahtarların, açık adreslerin, yedek anahtar kelimelerinin ve cüzdan arayüzlerinin amacını açıklayın.
* Farklı cüzdan türlerini karşılaştırın ve güvenlik, kullanım kolaylığı, gizlilik ve kontrol açısından avantaj ve dezavantajlarını değerlendirin.
* Bir mobil Bitcoin cüzdanı kurun ve temel kurtarma sürecini açıklayın.
* Zincir üzerinde bir bitcoin işlemini almayı ve göndermeyi gösterin.

"Güvenme, Doğrula" ilkesini cüzdan seçimine, işlemlere ve genel Bitcoin kullanımına uygulayın.

#### Araçlar & Kaynaklar

##### Görsel Yardımlar

* Bölüm 6 - Bitcoin Nasıl Kullanılır

##### Destek Kütüphanesi

* Kelime Kartı — Bölüm 6 — Terimler: cüzdan, özel anahtar, açık adres, yedek anahtar kelimesi, saklamalı, kendi kendine saklamalı, UTXO, işlem ücreti
* Karşılaştırma Tabloları & Referans Sayfaları — Cüzdan türleri karşılaştırması (saklamalı, mobil, donanım, kağıt)
* Teknik Açıklamalar & Derinlemesine İncelemeler — Açık/özel anahtarlar, UTXO modeli, işlem onayı
* Özel Anahtar Güvenliği Derinlemesine — Yedek anahtar kelimeleri, anahtar türetme, yedekleme yöntemleri, saldırı vektörleri
* İşlem Anatomisi Rehberi — Bir Bitcoin işleminin nasıl çalıştığına dair adım adım örnek
* Güvenlik En İyi Uygulamalar Kontrol Listesi — Başlamadan önce, cüzdan oluşturma, alma, gönderme, oltalama önleme

#### Etkinlikler

* İşlemler Uygulamada
* Lightning Bayrak Yarışı
* Mempool'u Keşfetmek

#### Çevrimiçi Öğretim

* Öğrencilerin bir demo izleyip izlemediğini veya kendi cüzdanlarını kurup kurmadıklarını baştan netleştirin.
* Her cüzdan kurulum adımı için büyük, okunabilir ekran görüntüleri kullanın.
* Her adımda duraklayın ve devam etmeden önce öğrencilerden sohbetten anladıklarını onaylamalarını isteyin.
* Yedek anahtar kelimesi bölümünden önce doğrudan uyarı verin ve öğrencileri hassas bilgileri asla çevrimiçi paylaşmamaları konusunda tekrar hatırlatın.

#### Hazırlık

* Bir mobil cüzdan uygulaması indirin ve test edin (Blue Wallet veya Muun); ana kurulum adımlarının ekran görüntülerini hazırlayın.
* Referans için cüzdan kurulum rehberi hazırlayın (indir → oluştur → yedek anahtar kelimesi → al).
* Ağ/WiFi'nin çalıştığından emin olun; göstermek için bir demo adresi ve QR kodu hazır bulundurun.

#### Yöntem

Bu ders, teoriden doğrudan uygulamaya geçer. Artık Diploma yapısıyla doğrudan eşleşir; edinim, cüzdanlar, kurulum, işlemler ve doğrulama, öğrenci rehberindeki ana başlıklarla aynı başlıklar altında yer alır. Ek öğretim desteği ise bu bölümlerin içinde yer almaya devam eder.

##### 6.0 Giriş, 8 dakika

Bu bölümü bir öncekiyle ilişkilendirerek başlayın:

* Eğer Bitcoin bir para ise, insanlar onu gerçekten nasıl elde eder ve kullanır?
* Bitcoin'inizi gerçekten kontrol etmek ne anlama gelir?
* Bitcoin kullanmak neden bir banka uygulaması kullanmaktan farklıdır?

Bu bölümün pratik kullanım hakkında olduğunu netleştirin. Öğrenciler artık sadece Bitcoin'in ne olduğunu öğrenmiyor, onunla doğrudan nasıl etkileşime geçileceğini öğreniyorlar.

##### 6.1 Bitcoin Edinme ve Takas Etme, 12 dakika

İnsanların bitcoin'i farklı şekillerde edinebileceğini açıklayın, örneğin:

* bitcoin ile ödeme almak
* bitcoin madenciliği yapmak
* nakit para ile yüz yüze bitcoin takası yapmak
* nakit para ile çevrimiçi bitcoin takası yapmak

Daha sonra bölümde ele alınan iki ana edinim yoluna odaklanın:

* eşler arası, yüz yüze
* eşler arası, çevrimiçi
* merkezi borsalar

Avantaj ve dezavantajları net bir şekilde belirtin.

Yüz yüze P2P için, banka veya aracı olmadan doğrudan takas yapıldığını vurgulayın, ancak nakit işlemler için biriyle buluşmanın pratik risklerinden de bahsedin.

Çevrimiçi P2P için, emanet sistemini basit terimlerle açıklayın; bu, eşler arasında doğrudan takasa izin verirken karşı taraf riskini azaltmanın bir yoludur.

Merkezi borsalar için, bunların kullanışlı olduğunu ancak kullanıcıların bir şirkete güvenmek, genellikle kişisel bilgilerini paylaşmak ve fonlarını çekene kadar üçüncü bir tarafın kontrolünde bırakmak zorunda olduklarını açıkça belirtin. Bu, kolaylığın genellikle mahremiyet ve egemenlikten ödün vermek anlamına geldiğini vurgulamak için iyi bir yerdir.

##### 6.2 Bitcoin Cüzdanlarına Giriş, 35 dakika

**Bir Bitcoin Cüzdanı Aslında Nedir**

Yaygın bir yanlış anlamayı hemen açıklığa kavuşturun: bitcoin, fiziksel nakit gibi cüzdan uygulamasının içinde saklanmaz.  
Bitcoin, ağ tarafından tutulan defterde bulunur. Kullanıcının kontrol ettiği şey, özel anahtarlar aracılığıyla onu harcama yetkisidir.

Daha sonra insanların "cüzdan" derken genellikle iki şeyi kastettiğini açıklayın:

* adreslerin üretildiği özel anahtar sistemi
* ağ ile etkileşim kurmak için kullanılan uygulama veya arayüz

Gerekirse bölümdeki e-posta benzetmesini kullanın:

* açık adres = paylaşabileceğiniz bir e-posta adresi gibi
* özel anahtar = korumanız gereken bir şifre gibi

Burada çok net olun: özel anahtarları kim kontrol ediyorsa bitcoin'i de o kontrol eder. Öğrencilerin anlaması gereken temel kavram budur.

**Kendi Saklamalı ve Saklamalı Cüzdanlar**

Bu bölümün en önemli kısımlarından biridir.

Ayrımı net bir şekilde açıklayın:

* Kendi saklamalı cüzdan: kullanıcı özel anahtarları kontrol eder
* Saklamalı cüzdan: üçüncü bir taraf, kullanıcı adına özel anahtarları kontrol eder

Daha sonra avantaj ve dezavantajları açıklayın:

Kendi saklamalı

* fonlar üzerinde tam kontrol
* onay süreci yok
* keyfi el koymaya karşı koruma
* daha fazla sorumluluk
* tohum ifadesi kaybolursa kolay kurtarma yok

Saklamalı

* daha kolay kurtarma ve destek
* yeni başlayanlar için daha basit
* hesap dondurma, saldırı ve üçüncü taraf kontrolüne daha açık
* kullanıcı bitcoin'i gerçekten elinde tutmaz

Burada şu ifadeyi vurgulamak için doğru bir an:

"Anahtar senin değilse, coin de senin değildir."

Öğrenciler bu bölümden sadece sloganı değil, bunun pratikte ne anlama geldiğini de anlayarak ayrılmalıdır.

**Farklı Cüzdan Türleri ve Birini Seçmek**

Bölümde ele alınan cüzdan türlerini tanıtın:

* çevrimiçi cüzdan
* mobil cüzdan
* masaüstü cüzdan
* donanım cüzdanı
* kağıt cüzdan

Hiçbirini kusursuz olarak göstermeyin. Bunun yerine, her birinin şu konularda farklı avantaj ve dezavantajlar içerdiğini açıklayın:

* güvenlik
* mahremiyet
* kolaylık
* uyumluluk
* ücretler
* kontrol
* itibar

Ayrıca, cüzdan yazılımının açık kaynak olup olmadığına dikkat edilmesini önerdiğimizi açıkça belirtin; çünkü açık kaynaklı araçlar topluluk tarafından incelenebilir, denetlenebilir ve sürdürülebilir. Bu, Bitcoin'deki doğrulama ilkesine doğrudan bağlanır.

##### 6.3 Mobil Bitcoin Cüzdanı Kurulumu, 10 dakika

Öğrencilere bölümde gösterilen temel süreci adım adım anlatın:

* cüzdanı indir
* yeni bir cüzdan oluştur
* kurtarma ifadesini oluştur ve bir yere yaz
* kurtarma ifadesini onayla
* varsa ek güvenlik ekle
* cüzdanı aç ve alım (receive) fonksiyonunu bul

Tohum ifadesi (seed phrase) uyarısını çok açık yapın:

* tohum ifadesi kaybolursa, fonlara erişim kaybedilebilir
* başka biri tohum ifadesini ele geçirirse, fonları alabilir

Öğrenciler bu işlemleri uygulamalı olarak yapıyorsa, eğitmen her adımda durmalı ve herkesin ne yaptığını anladığından emin olmalıdır. Ders daha kavramsal ise, bu bölüm canlı olarak yapılmak yerine bir anlatımla açıklanabilir. Bölümde gösterilen kurtarma seçeneği, cüzdanların tohum ifadesi doğru şekilde yedeklenmişse geri yüklenebileceğini açıklamak için de faydalıdır.

##### 6.4 Alım ve Gönderim İşlemleri, 17 dakika

**Zincir Üzerinde (On-chain) Alım ve Gönderim İşlemleri**

Şimdi zincir üzerindeki işlemlerin nasıl çalıştığını açıklayın.

Bitcoin almak için:

* cüzdanı aç
* al veya yatır (receive/deposit) seçeneğine dokun
* adresi kopyala, bağlantıyı paylaş veya QR kodunu göster

Bitcoin göndermek için:

* cüzdanı aç
* alıcı adresini yapıştır veya tara
* miktarı gir
* tüm detayları iki kez kontrol et
* işlemi yayınla (broadcast)
* onay için bekle

Şu önemli noktaları açıkça belirtin:

* işlem sahipliği devreder, fiziksel coinleri değil
* işlemler geri alınamaz
* düğümler (nodes) geçerliliği doğrular
* madenciler işlemleri bloklara dahil eder
* ücretler (fees) onay önceliğini etkiler
* zincir üzerindeki işlemler genellikle güvenlidir, ancak Lightning işlemlerine göre daha yavaş ve çoğu zaman daha pahalıdır

Bölümdeki işlem akış diyagramı burada özellikle faydalıdır, çünkü öğrencilerin cüzdan isteğinden ağ onayına kadar olan yolu görselleştirmesine yardımcı olur.

**İşlemler Uygulamada ve Rol Tabanlı Pratik**

Anlayışı pekiştirmek için bölümdeki işbirlikçi egzersiz yapısını kullanın. Dahil olan dört rolü açıklayın:

* gönderici
* alıcı
* madenci
* düğüm operatörü

Sınıfta basit bir yaklaşım, rolleri atamak ve bir işlemi adım adım yürütmektir. Bu, öğrencilerin bir Bitcoin işleminin sihir olmadığını, onay, doğrulama, bloğa dahil edilme ve defter güncellemelerini içeren koordineli bir süreç olduğunu görmelerine yardımcı olur.

Buradaki amaç teknik derinlik değildir. Amaç, öğrencilerin bir işlemde kimin ne yaptığını ve neden doğrulamanın önemli olduğunu anlamalarına yardımcı olmaktır.

##### 6.5 Güvenme, Doğrula, 8 dakika

Bunun şunlar için geçerli olduğunu açıklayın:

* cüzdanlar
* borsalar
* uygulamalar
* işlem detayları
* "kolay kazanç" iddiaları
* Bitcoin gibiymiş gibi davranan projeler

Bitcoin'in kullanıcıların eleştirel düşünmesini, kullandıklarını doğrulamasını ve körü körüne güvenmekten kaçınmasını gerektirdiğini açıkça belirtin. Ayrıca, bu bağlamda açık kaynaklı araçların neden önemli olduğunu açıklayın: Bağımsız doğrulamayı mümkün kılarlar.

###### Kapanış ve Anlama Kontrolü

Kapatırken birkaç hızlı soru sorun:

* Vekil cüzdan ile kendi kendine saklama cüzdanı arasındaki fark nedir?
* Tohum ifadesi neden bu kadar önemli?
* Zincir üstü bir işlem gönderdiğinizde ne olur?
* Neden zincir üstü işlemler bazı diğer Bitcoin ödemelerine göre daha yavaştır?
* "Güvenme, Doğrula" uygulamada ne anlama gelir?

#### Eğitmen Notları

Bu bölüm oldukça pratiktir, bu yüzden açıklık, güvenlik ve tekrar öncelikli olmalıdır.

Öğrencilerin her cüzdan türünü tek bir derste ustalıkla öğrenmeleri gerekmez. Ana hedefler şunlardır:

* cüzdanın temellerini anlamak
* kendi kendine saklamayı anlamak
* temel işlem akışını öğrenmek
* sorumlu bir doğrulama bakış açısı benimsemek

Tohum ifadeleri ve cüzdan kurulumu konularında özellikle dikkatli olun. Öğrenciler, bunların küçük detaylar olmadığını, Bitcoin sahipliğinin temeli olduğunu anlayarak ayrılmalıdır.

Bu bölümdeki en faydalı görseller ve etkinlikler şunlardır:

* kendi kendine saklama ile vekil cüzdan karşılaştırması
* cüzdan türü karşılaştırma tablosu
* adım adım cüzdan kurulum egzersizi
* işlem akış diyagramı
* rol tabanlı işlem etkinliği

##### Başarılı Uygulama Örneği

* Öğrencilerin gerçekten bir cüzdan kurması veya dikkatli bir demoyu izlemesi, tohum ifadesinin "Bu 12 kelime SİZİN Bitcoin'inizdir" vurgusuyla merkeze alınması, "Telefonunuzu kaybederseniz ne olur?" gibi senaryoların test edilmesi ve oltalama tanıma pratiği yapılması önemlidir.
* Eğitmenler, daha önce bunu yapmış, güvenlik bilinci yüksek ama paranoyak olmayan, zorluk eğrisini ve öğrenme gerekliliğini dürüstçe anlatan rehberler olmalıdır.
* Öğrenciler, gerçekten kullanabilecekleri bir beceri öğrendiklerini hisseder, tohum ifadesinin soyut değil gerçek ve önemli olduğunu anlar, kendi Bitcoin'lerini tutabileceklerini hisseder ve merkeziyetsizliğin kişisel sorumluluk gerektirdiğini kavrar.
* Öğrenciler bir cüzdan kurabiliyor ve açık anahtar ile özel anahtar arasındaki farkı anlayabiliyorsa, vekil cüzdan ile kendi kendine saklama cüzdanları arasındaki saklama farklarını kavrayabiliyor, bir işlemin nasıl çalıştığını (girdi, çıktı ve ücretler dahil) açıklayabiliyor, tohum ifadesi koruması dahil güvenlik farkındalığı gösterebiliyor ve sahiplik ile kontrol hakkında eleştirel sorular sorabiliyorsa, Öğrenme Hedefleri karşılanmış olur.

##### Zaman Yönetimi

Zaman kısıtlıysa öncelik verin:

* Cüzdanın temellerini anlamak
* Kendi kendine saklamayı anlamak
* Temel işlem akışını öğrenmek
* Sorumlu bir doğrulama bakış açısı benimsemek

Zamanınız varsa şunlara vakit ayırın:

* Kendi kendine saklama ile vekil cüzdan karşılaştırma tablosu
* Cüzdan türü karşılaştırma tablosu
* Canlı demo ile adım adım cüzdan kurulum egzersizi
* Ücret hesaplamalarıyla işlem akış diyagramı
* İleri düzey güvenlik uygulamaları ve donanım cüzdanı değerlendirmeleri

##### Öğrenciler Zorlanırsa

* Tohum ifadeleri "gerçek" olarak → "Bu ifade sizin bitcoin'inizdir; müşteri hizmeti yok."
* Açık anahtar vs. özel anahtar → E-posta benzetmesi (adres vs. şifre).
* Neden zor? → "Siz kontrol ediyorsunuz; siz sorumlusunuz." Takası kabul edin.
