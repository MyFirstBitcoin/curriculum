# 8 - Bitcoin Nasıl Çalışır

Süre: 90 dakika

Temel Fikir: Bitcoin'in güvenliği, anahtarlar, imzalar, hashleme ve UTXO'lar gibi basit ama güçlü teknik fikirlere dayanır. Bu kavramlar, merkezi bir otorite olmadan sahiplik ve doğrulama sağlar.

#### Öğrenme Hedefleri

Bu dersin sonunda öğrenciler şunları yapabilmelidir:

* Açık ve özel anahtarların, Bitcoin sahipliğini ve işlemlerini nasıl güvence altına aldığını açıklayın.
* Dijital imzanın ne olduğunu ve bir işlemin gerçekten sahibi tarafından yetkilendirildiğini nasıl kanıtladığını açıklayın.
* Bitcoin bağlamında kriptografi, şifreleme ve şifre çözmenin ne anlama geldiğini basit terimlerle açıklayın.
* Hashlemenin tanımını yapın ve hash fonksiyonlarının Bitcoin'in güvenliği ve veri bütünlüğü için neden önemli olduğunu açıklayın.
* Bir hash fonksiyonunun sabit uzunlukta çıktı, tek yönlü davranış ve küçük giriş değişikliklerine duyarlılık gibi temel özelliklerini tanımlayın.
* UTXO modelini ve bitcoin'in işlem çıktıları yoluyla nasıl harcandığını, alındığını ve para üstü olarak geri döndüğünü açıklayın.
* Düğümlerin, bir çıktının daha önce harcanıp harcanmadığını kontrol ederek çift harcamayı nasıl önlediğini açıklayın.

#### Araçlar & Kaynaklar

##### Görsel Materyaller

* Bölüm 8 - Bitcoin Nasıl Çalışır

##### Destek Kütüphanesi

* Kelime Kartı — Bölüm 8 — Terimler: kriptografi, hash, UTXO, dijital imza, özel/açık anahtar, merkle ağacı, blokzincir
* Yanlış Anlamalar Kütüphanesi — Bölüm 8 — Konular: "kayıp tohum ifadesi kurtarılabilir", "özel anahtar = şifre", "blokzincir anonimdir"
* Teknik Açıklamalar & Derinlemesine İncelemeler — Hash fonksiyonları, açık/özel anahtarlar, UTXO modeli, İş Kanıtı güvenliği

#### Etkinlikler

* İşlemler Uygulamada
* Mempool'u Keşfetmek

#### Çevrim İçi Öğretim

* Dijital bir beyaz tahta kullanın ve her kavramı canlı olarak çizin; yalnızca sözlü açıklamaya güvenmeyin.
* Her seferinde bir teknik fikri öğretin ve sık sık kontrol soruları için duraklayın.
* Anahtarlar, imzalar, hashler ve UTXO'lar için görseller kullanın ki öğrenciler yapıyı takip edebilsin.
* Hedefi kavramsal tutun ve matematik ya da teknik terimlere çok fazla girmeyin.

#### Hazırlık

* Diyagramları hazırlayın ve lamine edin: açık/özel anahtar çiftleri, dijital imzalar, UTXO modeli, hashleme (tek yönlü fonksiyon).
* Blokzincir gezgini ve SHA-256 hash hesaplayıcıyı yer imlerine ekleyin; adım adım incelemek için 2-3 gerçek Bitcoin işlemi seçin.
* Girdiler, çıktılar ve işlemlerin blokzincirde nasıl onaylandığını açıklamak için beyaz tahta notları hazırlayın.

#### Yöntem

Bu ders, öğrencilerin Bitcoin'in teknik tarafına ilk bakışını sağlar ve önceden teknik bilgi gerektirmez. Rehber artık Diploma ile aynı sıkıştırılmış yapıyı takip ediyor; kriptografi tek başlık altında, UTXO'lar ise diğer başlık altında toplanmıştır.

##### 8.0 Giriş, 8 dakika

Beklentileri belirleyerek başlayın:

* Merkezi bir banka kontrolü yoksa Bitcoin'i güvenli yapan nedir?
* Ağ, bir kişinin göndermeye çalıştığı bitcoin'in gerçekten ona ait olup olmadığını nasıl bilebilir?
* Birisi bir Bitcoin işlemi yaptığında perde arkasında gerçekte ne olur?

Bu bölüm, öğrencilerin Bitcoin'in temel teknik temellerine, özellikle anahtarlar, imzalar, hashleme ve UTXO'lara odaklandığını netleştirir. Ayrıca öğrencilere, temel mantığı anlamak için mühendis olmalarına gerek olmadığını da belirtin. Bölümün kendisi de bu noktayı, Bitcoin'i internete benzeterek açıkça ortaya koyar; birçok insan her gün interneti kullanır ama altındaki her katmanı tam olarak anlamaz.

##### 8.1 Kriptografi ile Güvenlik, 57 dakika

**Birçok Bilgisayarda Saklanan Bir Defter Olarak Bitcoin**

Bölümün Bitcoin ağına dair basit çerçevesiyle başlayın:

* Bitcoin, işlemlerin bir kaydıdır
* bu kayıt, düğüm adı verilen birçok bilgisayarda saklanır
* defter herkese açıktır ve takma adlarla çalışır
* kişisel kimlik bilgileri değil, adresler ve işlem geçmişi gösterilir

Bu bölüm, öğrencilerin önceki bölümlerden zaten bildiklerine geri dönmelerine yardımcı olur. Bitcoin, bir bankanın gizli hesaplarına dayanmaz. Birçok katılımcının doğrulayabildiği ortak bir deftere dayanır. burada özellikle faydalıdır çünkü kullanıcıları, cüzdanları ve daha geniş Bitcoin ağını ortak deftere bağlı olarak gösterir.

**Açık ve Özel Anahtarlar**

Şimdi kriptografiye geçin.

Her Bitcoin kullanıcısının şunlara sahip olduğunu açıklayın:

* gizli kalması gereken bir özel anahtar
* paylaşılabilen bir açık anahtar

Amaçlarını basit terimlerle açıklayın:

* özel anahtar kontrolü kanıtlar ve harcamayı yetkilendirir
* açık anahtar, başkalarının işlemin doğru şekilde yetkilendirildiğini doğrulamasına yardımcı olur

Bu bölümdeki güçlü bir öğretim noktası, Bitcoin'in ortak/özel anahtar kriptografisi kullandığıdır; bu, iki kişinin önce aynı gizli anahtarı paylaşmasını gerektiren eski modelden farklıdır. Bu önemlidir çünkü kullanıcıların fonlarını koruyan sırrı ifşa etmek zorunda kalmadan güvenli doğrulama sağlar.

Bunu şöyle açıklayabilirsiniz:

* özel anahtar, bitcoin'in size ait olduğunun gizli kanıtı gibidir
* açık anahtar, ağın yetkilendirmenizi doğrulamasını sağlayan şeyin bir parçasıdır
* özel anahtarı kim kontrol ediyorsa, bitcoin'i harcama yetkisine de o sahiptir

Burada şifreleme dilini fazla karmaşıklaştırmamaya dikkat edin. Öğrenciler için en önemli nokta sahiplik ve yetkilendirmedir.

**Dijital İmzalar ve İşlem Yetkilendirmesi**

Şimdi birisi bitcoin gönderdiğinde ne olduğunu açıklayın.

Bölümdeki sıralamayı kullanın:

* bir kullanıcı bir işlem oluşturur
* gönderen, özel anahtarını kullanarak dijital bir imza üretir
* işlem ağa yayınlanır
* düğümler imzanın geçerli olup olmadığını doğrular
* doğrulandıktan ve onaylandıktan sonra, sahiplik defterde aktarılır

Dijital imzanın isim yazmakla aynı şey olmadığını açıkça belirtin. Bu, gerçek sahibin işlemi yetkilendirdiğine dair kriptografik bir kanıttır. Bu, Bitcoin'in işlemleri merkezi bir otoriteye manuel olarak onaylatmadan çalışmasını sağlayan temel mekanizmalardan biridir. Diyagram faydalıdır çünkü hem imzalama ve doğrulamayı görsel olarak hem de işlemin göndericiden ağ doğrulamasına giden yolunu gösterir.

Sınıfta kullanılabilecek iyi bir cümle:

Bitcoin işlemleri bir banka onayladığı için değil, ağ geçerli kriptografik kanıtı doğrulayabildiği için kabul edilir.

**Hashleme ve Tek Yönlü Fonksiyonlar**

Şimdi hashlemeyi açıklayın.

Basit başlayın:

* bir fonksiyon bir girdi alır ve bir çıktı üretir
* tek yönlü bir fonksiyon bir yönde çalıştırmak kolaydır, ancak tersine çevirmek pratikte imkansızdır
* bir hash fonksiyonu, herhangi bir boyuttaki veriyi sabit uzunlukta bir çıktı olan hash'e dönüştürür

Bölümdeki benzetmelerden hangisi kitleniz için daha açıksa onu kullanın:

* tek yönlü fonksiyonlar için smoothie benzetmesi
* hash'ler için parmak izi benzetmesi
* bir şeyin değişip değişmediğini kontrol etmek için müzik notası benzetmesi

Parmak izi benzetmesi çoğu sınıf için muhtemelen en anlaşılır olanıdır:

* bir hash, veriler için dijital bir parmak izi gibidir
* girdi biraz bile değişirse, hash tamamen değişir
* bu, bilgisayarların bütünlüğü kontrol etmesine ve kurcalamayı tespit etmesine yardımcı olur

Sonra hashlemenin Bitcoin'de neden önemli olduğunu açıklayın:

* işlemler hash'lenir
* ağ, bütünlüğü doğrulamak için hash'leri kullanır
* bir işlem değiştirilirse, hash değişir
* bu, defterin fark edilmeden manipüle edilmesini önlemeye yardımcı olur

7 ila 10. sayfalardaki görseller burada çok faydalıdır. Bölüm hem sabit uzunlukta çıktı fikrini hem de "küçük değişiklik, tamamen farklı sonuç" ilkesini gösteriyor; bu, öğrencilerin anlaması gereken en önemli kavramlardan biridir.

**Hash Fonksiyonlarının Temel Özellikleri**

Bölümde vurgulanan özellikleri çok akademik olmadan kısaca gözden geçirin:

* Deterministik: aynı girdi her seferinde aynı çıktıyı verir
* Tek yönlü / ön-görüntü direnci: işlemi tersine çevirmek pratikte mümkün değildir
* Değişime duyarlı: küçük bir girdi değişikliği bile çok farklı bir çıktı oluşturur
* Çakışma direnci: aynı çıktıya sahip iki farklı girdi bulmak son derece zordur
* Doğrulaması hızlı: fonksiyon çalıştırmak ve kontrol etmek için verimlidir

Öğrencilerin her terimi ezberlemesine gerek yok, ancak genel noktayı anlamalılar: hashleme, Bitcoin'e verileri tanımlamak ve değişikliği tespit etmek için güvenilir bir yol sağlar.

##### 8.2 UTXO Modeli, 25 dakika

**UTXO Modeli**

Şimdi bölümün ikinci ana kısmına geçiyoruz: UTXO'lar, yani Harcanmamış İşlem Çıktıları.

Bölümdeki nakit benzetmesini kullanarak bunu basit terimlerle açıklayın:

* bitcoin bir banka hesabı bakiyesi gibi izlenmez sadece
* bunun yerine, harcanabilir parçalardan oluşur ve bunlara UTXO denir
* bitcoin harcadığınızda, mevcut bir veya birden fazla UTXO'yu girdi olarak kullanırsınız
* ardından yeni UTXO'lar çıktı olarak oluşturulur

Bölümdeki örneği kullanın:

* eğer 10 BTC'lik bir UTXO'nuz varsa
* ve 6 BTC gönderirseniz
* yeni bir 6 BTC'lik UTXO alıcıya gider
* yeni bir para üstü UTXO'su size geri gelir
* küçük bir kısmı madenci ücreti olarak ödenir

Bu, öğrencilerin Bitcoin'in basit bir hesap bakiyesinden sayı çıkarmaktan ziyade nakit harcamak ve para üstü almak gibi çalıştığını görmelerine yardımcı olur. Diyagramlar burada özellikle güçlüdür çünkü bir UTXO'nun alıcı çıktısına, para üstü çıktısına ve ücrete nasıl bölündüğünü görsel olarak gösterir.

İki temel noktayı açıkça belirtin:

* cüzdan bakiyeniz UTXO'larınızın toplamıdır
* harcadığınızda, eski UTXO'lar tüketilir ve yenileri oluşturulur

**Çifte Harcamayı Önleme**

İçeriği, UTXO modelinin en önemli sonuçlarından birini açıklayarak kapatın.

Birisi aynı çıktıyı iki kez harcamaya çalışırsa, düğümler ikinci girişimi reddeder çünkü defteri tutar ve o UTXO'nun zaten harcanıp harcanmadığını doğrulayabilirler. Bitcoin, kayıtları yönetecek merkezi bir ödeme şirketine ihtiyaç duymadan çifte harcamayı bu şekilde önler. Buradaki örnek çok faydalıdır çünkü Alice'in UTXO'ları birleştirip Bob'a para göndermesini, para üstü almasını ve onaylanan işlemin defteri düğümler arasında güncellemesini adım adım gösterir.

Sınıfta bunu açıkça söylemenin bir yolu:

Bitcoin çifte harcamayı önler çünkü ağ hangi çıktının harcanmamış, hangisinin zaten kullanılmış olduğunu takip eder.

###### Kapanış ve Anlama Kontrolü

Kapatırken birkaç hızlı soru sorun:

* Açık anahtar ile özel anahtar arasındaki fark nedir?
* Dijital imza neyi kanıtlar?
* Hashleme Bitcoin'de neden faydalıdır?
* Bir işlem hash edildikten sonra değiştirilirse ne olur?
* Basit terimlerle bir UTXO nedir?
* Ağ birinin aynı bitcoini iki kez harcamasını nasıl engeller?

#### Eğitmen Notları

Bu bölüm önceki bölümlere göre daha teknik bir dil içeriyor, bu yüzden açıklık, benzetme ve tekrar öncelikli olmalı.

Amaç, öğrencileri geliştirici yapmak değil. Amaç, Bitcoin güvenliğinin neden işe yaradığını anlamalarını sağlamak.

Zaman kısıtlıysa öncelik verilmesi gereken en güçlü noktalar şunlardır:

* özel anahtar vs açık anahtar
* dijital imzalar
* hashlemenin ne yaptığı
* bitcoin'in harcanabilir parçaları olarak UTXO'lar
* çifte harcamanın nasıl önlendiği

Bu bölümdeki en faydalı görseller şunlardır:

* kullanıcı-cüzdan-ağ diyagramı
* dijital imza görseli
* sayfa 7-10'daki hashleme örnekleri ve sabit uzunluklu çıktı diyagramları
* sayfa 10-12'deki UTXO diyagramları

##### Başarılı Sonuç Nasıl Olur

* Kriptografiyi bir gizem değil temel olarak ele almak, bolca görsel kullanmak, derin matematikten kaçınmak, önceki bölümlere bağlantı kurmak ve "Birisi bir işlemi değiştirirse ne bozulur?" gibi uygulamalarla anlamayı test etmek önemlidir.
* Öğretmenler, zorlanan öğrencilere karşı sabırlı olmalı, görsel düşünmeli ve her şeyi çizmeli, öğrencilerin anlaması gerekmeyen konularda dürüst olmalı, "Bilmiyorum ama nasıl öğrenebileceğimizi göstereyim" demeye istekli olmalı ve süreç boyunca teşvik edici kalmalıdır.
* Öğrenciler, Bitcoin'in matematikle korunduğu için hacklenemeyeceğini anlar, sistemin zarif tasarımına saygı duyar, her detayı bilmeden karmaşıklıkla rahat hisseder, yargılanmadan soru sorma konusunda özgüven kazanır ve çoğu insanın anlamadığı bir şeyi anladıklarını fark ederek kendilerini geliştirmiş hissederler.
* Öğrenciler, tek yönlü fonksiyonlar ve dijital imzalar gibi kriptografi temellerini derin matematik olmadan açıklayabiliyor, UTXO modelini yani hesap değil coin sahibi olunduğunu anlıyor, hashlemenin Bitcoin güvenliğinin temeli olduğunu biliyor, imza ve onayları içeren işlem anatomisini kavrıyor, Bitcoin'in neden değiştirilemez olduğunu açıklayabiliyor ve olası saldırılar veya zayıflıklar hakkında eleştirel sorular sorabiliyorsa Öğrenme Hedefleri karşılanmış olur.

##### Zaman Yönetimi

Zaman kısıtlıysa, öncelik verin:

* Özel anahtar vs açık anahtar
* Dijital imzalar
* Hashlemenin yaptığı şey
* UTXO'lar harcanabilir bitcoin parçaları olarak
* Çifte harcamanın nasıl önlendiği

Öndeyseniz, şu konulara zaman ayırın:

* Kullanıcı-cüzdan-ağ diyagramı ve görsel güvenlik modeli
* Dijital imza görseli: ayrıntılı kriptografik süreç
* Merkle ağaçları ve zincir güvenliği
* Gelişmiş saldırı vektörleri ve neden başarısız oldukları

##### Öğrenciler Zorlanırsa

* Kriptografi tehdit edici geliyor → "Her gün kullanıyorsun; My First Bitcoin de aynı şekilde kullanıyor."
* Hashleme kavramı → Parmak izi benzetmesi; benzersizdir, hash değişmeden değiştirilemez.
* Dijital imzalar → "Şifreyi ifşa etmeden yetkilendirmeyi kanıtlar."
