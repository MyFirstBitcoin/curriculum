# 9 - Bitcoin Madenciliği Nasıl Çalışır

Süre: 90 dakika

Temel Fikir: Bitcoin madenciliği ve node doğrulaması, ağı güvence altına almak, işlemleri onaylamak ve sistemin kurallarını İş Kanıtı (Proof of Work) yoluyla uygulamak için birlikte çalışır.

#### Öğrenme Hedefleri

Bu dersin sonunda öğrenciler şunları yapabilmelidir:

* Bitcoin node'larının rolü ile Bitcoin madencilerinin rolü arasındaki farkı açıklayın.
* Node'ların işlemleri nasıl doğruladığını, bilgileri nasıl paylaştığını ve Bitcoin'in kurallarının uygulanmasına nasıl yardımcı olduğunu açıklayın.
* Madencilerin ne yaptığını açıklayın; işlemleri seçmek, aday bloklar oluşturmak ve geçerli bir blok hash'i bulmak için yarışmak dahil.
* Mempool'u tanımlayın ve neden onaylanmamış işlemler için bir bekleme odası gibi çalıştığını açıklayın.
* İşlem ücretlerinin madenci seçimini ve onay hızını nasıl etkilediğini açıklayın.
* Bitcoin'i güvence altına alan mekanizma olarak İş Kanıtı'nı (Proof of Work) ve saldırıları neden pahalı hale getirdiğini açıklayın.
* Zorluk ayarlamasının ortalama blok süresini yaklaşık 10 dakika olarak korumaya nasıl yardımcı olduğunu açıklayın.
* Bir Bitcoin işleminin tam yaşam döngüsünü, oluşturulmasından ve imzalanmasından blokta onaylanmasına kadar adım adım anlatın.

#### Araçlar & Kaynaklar

##### Görsel Yardımlar

* Bölüm 9 - Bitcoin Madenciliği Nasıl Çalışır?

##### Destek Kütüphanesi

* Kelime Kartı — Bölüm 9 — Terimler: madencilik, İş Kanıtı, hash bulmacası, zorluk ayarlaması, blok ödülü, mempool, %51 saldırısı
* Yanlış Anlamalar Kütüphanesi — Bölüm 9 — Ele alın: "madenciler Bitcoin'i yoktan yaratır", "madenciler Bitcoin'i kontrol eder", "daha fazla madencilik = daha az güvenlik"
* Karşılaştırma Tabloları & Referans Sayfaları — Madencilik ekonomisi: gelir, maliyetler, teşvik uyumu; zorluk ayarlaması
* Teknik Açıklamalar & Derinlemesine İncelemeler — İş Kanıtı güvenliği; saldırının neden pahalı olduğu; %51 eşiği

#### Etkinlikler

* Mempool'u Keşfetmek
* İşlemler İş Başında

#### Çevrim İçi Öğretim

* Cüzdan imzalamadan onaya kadar net bir işlem akış diyagramı kullanın.
* Ders boyunca node'ları ve madencileri ekranda görsel olarak ayrı tutun.
* Onaylanmamış işlemleri ve ücret baskısını göstermek için mempool.space'i veya bir ekran görüntüsünü kullanın.
* Madencilik sürecinin her aşamasından sonra duraklayın ve kısa bir anlama sorusu sorun.

#### Hazırlık

* Görüntülemek için madencilik süreci diyagramı hazırlayın (mempool → işlem seçimi → blok oluşturma → zorluk ayarlaması).
* mempool.space veya blockchain.com madencilik sayfasını yer imlerine ekleyin; mevcut madencilik istatistikleri ve zorluk ayarlamaları için ekran görüntüleri hazırlayın.
* İş Kanıtı'nın güvenlik mekanizması olarak görsel açıklamasını oluşturun; son 3-6 ayda zorluk ayarlamasını gösterin.

#### Yöntem

Bu ders, Bitcoin işlemlerinin ağda nasıl hareket ettiğine ve blokzincirin bir parçası haline geldiğine daha yakından bakar. Artık Diploma yapısını doğrudan takip ediyor, böylece ana bölümler öğrenci rehberiyle uyumlu olurken her bölümde daha kapsamlı eğitmen açıklaması korunuyor.

##### 9.0 Giriş, 8 dakika

Bu bölümü bir öncekiyle ilişkilendirerek başlayın:

* Bir kullanıcı bir işlemi özel anahtarıyla imzalarsa, sonra ne olur?
* Bu işlemin geçerli olup olmadığını kim kontrol eder?
* Bu işlem blokzincire nasıl eklenir?
* Bitcoin'in hem node'lara hem de madencilere neden ihtiyacı var?

Bu bölümün, ağın işlemleri pratikte nasıl işlediğini ve madenciliğin merkezi bir otorite olmadan sistemi nasıl güvence altına aldığını açıkladığını netleştirin.

##### 9.1 Bitcoin Node'ları ve Madenciler, 47 dakika

**Node'lar ve Madenciler, Farklı Roller**

İki rolü açıkça ayırarak başlayın.

Bitcoin node'ları:

* blokzincirin bir kopyasını tutar
* işlemlerin kurallara uyup uymadığını doğrular
* diğer node'larla bilgi paylaşır
* cüzdanların ve diğer yazılımların blokzincir verilerine erişmesine yardımcı olur
* geçersiz işlemleri veya geçersiz blokları reddedebilir

Bu bölüm, düğümleri doğrulamanın bekçileri olarak tanımlar ve bunu "dijital trafik polisi" benzetmesiyle genişletir. Bu benzetme, düğümlerin denetleyici ve koordine edici olduklarını, yönetici olmadıklarını gösterdiği için faydalıdır. Diyagram ayrıca, dünyanın dört bir yanında birçok düğümün defterin kopyalarını tuttuğunu da pekiştirir.

Bitcoin madencileri:

* geçerli işlemleri toplar
* aday bloklar oluşturur
* geçerli bir blok hash'i bulmak için yarışır
* kazandıklarında geçerli blokları yayınlar
* blok ödülleri ve işlem ücretleri alır

Bölümdeki temel öğretici noktalardan biri, madenciliğin amacının sadece yeni bitcoin üretmek olmadığını, aynı zamanda Bitcoin'in güvenliğini merkeziyetsizleştirmek olduğunu vurgulamaktır. Yeni bitcoin teşvik olarak verilirken, madencilik sürecinin kendisi güvenlik mekanizmasıdır.

**Düğümler Aslında Ne Yapar?**

Düğüm bölümünü, bölümdeki düğüm işlevleri listesiyle genişletin:

* Doğrulamanın bekçileri: işlemlerin ve blokların kurallara uyup uymadığını kontrol ederler
* İletişim merkezi: birbirleriyle bağlantı kurar ve işlem verilerini paylaşırlar
* Kalite denetçisi: geçersiz bilgileri reddederler
* Blokzincir bilgilendiricisi: cüzdanlar gibi diğer yazılımlara veri sağlarlar
* Yeni düğüm karşılayıcısı: yeni düğümlerin blokzinciri edinmesine yardımcı olurlar, ancak her yeni düğüm yine de verileri bağımsız olarak doğrular

Bu, bir düğüm çalıştırmanın kullanıcıya daha fazla bağımsızlık sağladığını vurgulamak için iyi bir andır. Ağın durumunu tamamen dış hizmetlere bağımlı olarak öğrenmek yerine, kendileri doğrulayabilirler. My First Bitcoin bu noktayı açıkça ortaya koyar ve kullanıcıların çalıştırabileceği bir uygulama olarak Bitcoin Core'dan da bahseder.

**Madenciler Aslında Ne Yapar?**

Şimdi madenciliği daha dikkatli açıklayın.

Madenciler:

* doğrulanmış ama henüz onaylanmamış işlemleri toplar
* bunları bir aday blokta bir araya getirir
* geçerli bir blok hash'i bulana kadar blok verilerini tekrar tekrar hash'ler
* kazanan bloğu ağa yayınlar
* blok kabul edilirse ödül kazanır

Bölümdeki "devasa anahtar samanlığı" benzetmesini kullanabilirsiniz. Bu, öğrencilere madencilik yarışını somut bir şekilde anlatır. Ana fikir, madencilerin sıradan anlamda faydalı bir matematik problemi çözmedikleri, bunun yerine sistemi güvence altına almak için gerçek dünyada enerji ve hesaplama harcadıklarını kanıtladıklarıdır.

Burası aynı zamanda madenci ödüllerini açıklamak için doğru yerdir:

* blok ödülü: yeni çıkarılan bitcoin
* işlem ücretleri: kullanıcıların onaylanmasını istediği işlemlere eklenen ücretler

Madencilerin genellikle daha yüksek ücretli işlemleri önceliklendirdiğini açıklayın, çünkü bunlar ödüllerini artırır. Bölüm burada yarılanmaları da açıklar, bu yüzden blok ödülünün her 210.000 blokta, yaklaşık her dört yılda bir, Bitcoin'in halka açık arz takvimine göre azaldığını kısaca belirtebilirsiniz. 5. ve 6. sayfalarda arz takvimi ve yaklaşan yarılanma tablosu yer alır; bu da Bitcoin'in öngörülebilir ihraç sürecini pekiştirmeye yardımcı olabilir.

**Geçerli Blok Hash'i, İş Kanıtı ve Zorluk Ayarı**

Bu bölüm, bölümün özüdür.

Madencilerin geçerli bir blok hash'i aradıklarını, yani ağın hedefini karşılayan bir blok hash'i bulmaya çalıştıklarını açıklayın. Bölüm, bunun ağ tarafından belirlenen hedeften daha küçük bir sayı bulmak olarak açıklar.

Sonra İş Kanıtı'nı net bir şekilde açıklayın:

* madenciler tekrar tekrar hesaplama yapmak zorundadır
* geçerli hash'i ilk bulan, bu işi yaptığını kanıtlar
* bu, defteri yeniden yazmayı veya saldırmayı pahalı hale getirir
* düğümler daha sonra bloğu kabul etmeden önce doğrular

Öğretim için güçlü bir cümle:

İş Kanıtı, Bitcoin'i güvensizliği pahalı, doğrulamayı ise kolay hale getirerek korur.

Zorluk ayarını da açıklayın:

* ağ, madencilik zorluğunu her 2.016 blokta bir ayarlar
* bu yaklaşık her iki haftada bir gerçekleşir
* amaç, ortalama blok süresini 10 dakikaya yakın tutmaktır
* ağa daha fazla hash gücü katılırsa zorluk artar
* daha az hash gücü varsa zorluk azalır

7. ve 8. sayfalar bu süreci açıklar ve daha zor hedeflerin daha fazla iş gerektirdiğini gösterir. Bu, öğrencilerin Bitcoin'in zamanlamasının merkezi bir otorite tarafından değil, ağ koşullarına otomatik olarak yanıt veren protokol kurallarıyla belirlendiğini anlamalarına yardımcı olur.

##### 9.2 Mempool Nedir?, 15 dakika

Şimdi mempool konusuna geçin.

Mempool'un, geçerli ama henüz onaylanmamış işlemler için bir bekleme odası olduğunu açıklayın. Bir kullanıcı bir işlem yayınladığında, düğümler önce onu doğrular. Geçerliyse, kendi mempool'larına ekler ve diğer düğümlerle paylaşırlar. Ardından madenciler, bir blok oluştururken bu bekleyen işlemler arasından seçim yapabilir. 10. ve 11. sayfalar bu süreci doğrudan açıklar.

Vurgulanması gereken önemli noktalar:

* mempool blokzinciri değildir
* oradaki işlemler henüz onaylanmamıştır
* her düğüm kendi mempool'unu tutar
* tek bir evrensel mempool yoktur
* daha yüksek ücretli işlemler daha hızlı seçilme olasılığına sahiptir

Bu bölüm ayrıca bir işlemin neden uzun süre onaylanmadan kalabileceğine dair yaygın nedenleri açıklar:

* düşük ücret
* ağ tıkanıklığı
* çifte harcama girişimi
* yanlış veya eksik veri
* hatalı işlem

Faydalıysa, mempool.space ile yapılan etkinliği, onaylanmamış işlemleri ve ücret oranlarını görselleştirmenin pratik bir yolu olarak belirtin. Ayrıca mempool.space'in sadece bir explorer olduğunu, mempool'un kendisi olmadığını açıkça belirtin.

##### 9.3 Bitcoin İşlemleri Nasıl Çalışır, 20 dakika

Şimdi, bölümün adım adım sıralamasını kullanarak her şeyi bir araya getirin.

Sınıf için net bir versiyon şudur:



1. Gönderen bir UTXO seçer ve bir işlem oluşturur
1. Gönderen, alıcı adresini ve ücreti ekler
1. Gönderen işlemi özel anahtarıyla imzalar
1. İşlem ağa yayınlanır
1. Düğümler işlemi doğrular ve kendi mempool'larına ekler
1. Madenciler işlemi aday blok için seçer
1. Madenciler İş Kanıtı ile yarışır
1. Bir madenci geçerli bir blok hash'i bulur ve bloğu yayınlar
1. Düğümler bloğu doğrular ve blokzincirine ekler
1. İşlem, daha fazla blok eklendikçe onay alır
1. Son noktayı açıkça belirtin:
1. işlem geçerli bir bloğa dahil edildiğinde onaylanır
1. harcanan girdiler artık kullanılamaz
1. alıcı artık bu işlemle oluşturulan yeni UTXO'ları kontrol eder

Özet diyagramı burada özellikle faydalıdır çünkü tüm süreci cüzdan imzalamadan madenciye dahil etmeye, düğüm doğrulamasına ve blok dağıtımına kadar görsel olarak bağlar.

###### Kapanış ve Anlama Kontrolü

Kapatırken birkaç hızlı soru sorun:

* Bir düğüm ile madenci arasındaki fark nedir?
* Mempool nedir?
* Neden bazı işlemler diğerlerinden daha hızlı onaylanır?
* İş Kanıtı neyi kanıtlar?
* Bitcoin neden madencilik zorluğunu ayarlar?
* Bir işlemin gönderilmesi ile onay alınması arasındaki ana adımlar nelerdir?

#### Eğitmen Notları

Ana öğretim hattını net tutun: düğümler doğrular, madenciler yarışır, İş Kanıtı ağı güvenceye alır ve mempool geçerli işlemleri onaylanana kadar tutar.

Bu bölüm teknik gelebilir, bu yüzden sık sık benzetmeler ve diyagramlar kullanın.

Madenciliği "hiç yoktan bitcoin yaratmak" gibi göstermemekten kaçının. Ödülün teşvik olduğunu, madencilik sürecinin ise ağı güvenceye aldığını açıkça belirtin.

Zaman kısıtlıysa öncelik verilmesi gereken en güçlü noktalar şunlardır:



1. Düğüm ve madenci rolleri
1. Mempool bekleme odası olarak
1. İş Kanıtı
1. Zorluk ayarlaması
1. İmzalamadan onaya kadar işlem akışı

##### Başarılı Eğitim İçin İpuçları

* Madenciler ≠ Düğümler olduğunu hemen açıklığa kavuşturmak, madenciliği gerçek donanım maliyetleri ve elektrik giderleri olan ekonomik bir faaliyet olarak göstermek, güvenlik mekanizmasını zorluk ayarlaması ve İş Kanıtı ile açıklamak ve ağ değişiklikleriyle ilgili senaryolarla anlama düzeyini test etmek önemlidir.
* Eğitmenler, tartışmaları somutlaştırmak için gerçek rakamlar kullanmalı, Madenciler ile Düğümler arasındaki farkı kristal netliğinde ve tekrarlı bir şekilde vurgulamalı, madencilik havuzlarıyla ilgili merkezileşme endişelerinde gerçekçi olmalı ve işin içindeki gerçek karmaşıklığa saygı göstermelidir.
* Öğrenciler, madenciliğin karmaşık işler yapan zeki insanlar tarafından yapıldığını çünkü Bitcoin kazandıklarını, teşviklerin dürüst davranışı yönlendirdiğini çünkü madencilerin kârının Bitcoin'in başarısına bağlı olduğunu, sistemin otomatik zorluk ayarıyla kendini düzenlediğini, madenciliğin bir hayır işi değil gerçek bir iş olduğunu ve Bitcoin'in güvenliğinin gerçek elektrik ve para maliyeti olduğunu anlar.
* Öğrenciler, blokları oluşturan madenciler ile onları doğrulayan düğümleri ayırt edebiliyorsa, İş Kanıtı'nı saldırıları üstel olarak pahalı hale getiren bir güvenlik mekanizması olarak anlayabiliyorsa, zorluk ayarının blok süresini yaklaşık 10 dakikada tuttuğunu fark edebiliyorsa, madencilerin blok ödülleri ve ücretler etrafındaki teşviklerini kavrayabiliyorsa, %51 saldırısının neden işe yaramadığını açıklayabiliyorsa ve madenciliği gerçek maliyet ve faydaları olan bir ekonomik faaliyet olarak görebiliyorsa, Öğrenme Çıktıları karşılanmış olur.

##### Zaman Yönetimi

Zaman kısıtlıysa öncelik verin:

* Düğüm ve madenci rolleri (kritik ayrım)
* Mempool bekleme odası olarak
* İş Kanıtı mekanizması
* Zorluk ayarı (kendini düzenleyen sistem)
* İşlemin imzalanmasından onaylanmasına kadar olan akış

Öndeyseniz, şu konulara zaman ayırın:

* Madencilik ekonomisi ve donanım detayları
* Madencilik havuzu dinamikleri ve merkezileşme endişeleri
* %51 saldırı senaryoları ve neden matematiksel olarak başarısız oldukları
* Teşvik uyumu yoluyla uzun vadeli güvenlik

##### Öğrenciler Zorlanırsa

* Madenciler vs. düğümler (karışıklık) → "Düğümler doğrular, madenciler önerir; hakemler vs. oyuncular."
* İş Kanıtı israf → "Pahalı güvenlik saldırıları önler; onları anlamsız kılar."
* Zorluk ayarı → "Daha fazla madenci = daha hızlı bloklar = zorluk artar; sistem nefes alır."
