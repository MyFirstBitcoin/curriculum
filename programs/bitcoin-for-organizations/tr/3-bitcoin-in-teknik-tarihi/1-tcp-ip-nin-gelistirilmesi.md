# 3.1 TCP/IP'nin geliştirilmesi

Çoğumuz bugün internetin temeli olarak kullanılan TCP/IP protokollerine aşinayız. Bu protokollerin kökeni, 70’lerin sonlarına kadar uzanır; o dönemde bilim insanları, Arpanet’e alternatif tasarımlar araştırıyorlardı – Arpanet ise, ABD Savunma Bakanlığı tarafından uzak bilgisayarlar arasında kaynak paylaşımını sağlamak amacıyla tasarlanmış daha da eski bir ağdı. TCP/IP, 1983 yılında Arpanet’in protokol standardı haline geldi ve 1990’ların sonunda baskın ağ modeli olarak internetin temeli oldu. Bugün My First Bitcoin ve Bitcoin’in çalıştığı internetin altyapısını oluşturur.


| OSI Modeli | TCP/IP |
| --- | --- |
| Uygulama | Uygulama |
| Sunum | Uygulama |
| Oturum | Uygulama |
| Taşıma | Taşıma |
| Ağ | Ağ |
| Veri Bağlantı | Veri Bağlantı |
| Fiziksel | Fiziksel |


TCP/IP modeli geliştirilirken, Uluslararası Standartlar Organizasyonu (ISO) ve Telekomünikasyon endüstrisi (CCITT) tarafından benzer ama daha kapsamlı bir çerçeve geliştiriliyordu. Yeni protokoller geliştirme veya değişiklik önerme süreci, TCP/IP'nin geliştirilmesinde kullanılan daha merkeziyetsiz yaklaşıma kıyasla yavaş ve hantaldı; bu da bugün bu yaklaşımın baskın olmasına yol açtı.

##### Değişiklik Talebi

Mevcut protokollerde önerilen herhangi bir gelişme veya yeni fikirler, TCP/IP modelinde bir **Değişiklik Talebi** süreciyle önerilebilir. Bunlar, İnternet Mühendisliği Görev Gücü (IETF) tarafından yönetilen bir onay sürecinden geçer ve onaylandıktan sonra herkesin uygulayabilmesi ve benimseyebilmesi için açık kaynak haline gelir. Dikkate değer bazı örnekler:

* 1969 RFC 1 Arpanet’te paketlerin nasıl gönderileceğini belgeledi
* 1981 RFC791 İnternet protokolü V4’ü tanımladı – bugün hâlâ yaygın olarak kullanılıyor
* 1982 RFC 821 Basit Mail Transfer Protokolü
* 1987 Alan Adı Sistemi – alan adlarının IP adreslerine nasıl çözümlendiği
* 1999 RDC 2616 Hiper Metin Transfer Protokolü – web’de gezinmek için temel


> **Callout**
>
> **Bitcoin İyileştirme Önerisi** (BIP), RFC’ye benzer bir yaklaşımı takip eder, ancak yeni veya alternatif protokollerin geliştirilmesinden ziyade yalnızca Bitcoin’in kendisine yönelik iyileştirmelere odaklanır. Bitcoin ayrıca bu katmanlı modelden de yararlanır ve ek protokoller ikinci veya üçüncü katman olarak tanımlanır.


TCP/IP modelinin temel katmanları son birkaç on yılda nispeten az değiştiği gibi, yenilikler daha çok üst katmanlarda gerçekleşti; Bitcoin’in temel katmanının da bu noktada çok yavaş değişmesi bekleniyor. Ölçeklendirme çözümleri ise Lightning ve Liquid gibi üst katmanlarda gerçekleşiyor.

Temel katman protokollerinin zamanla değiştirilmesinin ne kadar zorlaştığına iyi bir örnek IPv6’dır. IPv4’teki adres alanının tükenmesi beklentisi, yeni bir protokol ihtiyacını doğurdu. İlk taslak standart 1998’de oluşturuldu, ancak 2017’ye kadar internet standardı olarak onaylanmadı. IPv4’teki birçok sorunu çözmesine ve çok daha geleceğe dönük olmasına rağmen, bugün sektörde hâlâ çok yavaş benimsenmiştir. Bu süre zarfında, üst katmanlarda multimedya, e-posta vb. için birçok yeni protokol tanımlandı.

##### Bitcoin’in kullandığı yapı taşları

Bağlantılılık sorunlarının bu şekilde ayrılması, protokollerin üst ve alt katmanlardan bağımsız olarak geliştirilmesine olanak tanır. Her katman için çözümleri yeniden icat etmek yerine, My First Bitcoin ve Bitcoin ağı, fiziksel ve veri bağlantı katmanlarında sunulan temel ağ yeteneklerine güvenebilir.


| Katman | TCP/IP Orijinal |
| --- | --- |
| Uygulama | Komşu düğümleri tanımlamak için Alan Adı Sistemi (DNS) kullanılır. 8333 numaralı port, Bitcoin protokolünü işaret eder. |
| Taşıma | Madenciler arasında düşük gecikmeli FIBRE iletişimi için UDP. Düğümler arası eşler arası iletişim için TCP. |
| Taşıma | TOR Yönlendirme: Anonimlik ve gizlilik sağlar. Yayın Protokolü: Trafiği ağda yönlendirir. |
| Bağlantı | Herhangi bir ortamda çalışır (ör. Ethernet, Wi-Fi, vb.) |
| Fiziksel | Kablosuz, Ethernet veya diğer donanım arayüzleri üzerinden fiziksel iletim. |


##### Bitcoin, HTTPS’in bilgi aktarması gibi, değeri aktaran tarafsız bir protokoldür.

* **HTTPS**: Güvenli Web Siteleri
* **SMTP**: E-posta Gönder
* **FTP**: Dosya transferi
* **DNS**: Alan adlarını yönet
* **BTC**: Değer sakla ve transfer et

Bitcoin, insanlar veya cihazlar arasında, üçüncü bir tarafa ihtiyaç duymadan ve güvenilir bir şekilde değerin internet üzerinden taşınmasını sağlar. Bunun muazzam bir değer yaratması beklenmektedir.
