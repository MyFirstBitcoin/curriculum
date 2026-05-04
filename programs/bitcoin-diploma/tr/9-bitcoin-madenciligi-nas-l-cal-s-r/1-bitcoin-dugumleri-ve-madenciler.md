# 9.1 Bitcoin Düğümleri ve Madenciler

Bitcoin düğümleri teknik gibi görünebilir, ancak aslında bir bilgisayarda Bitcoin blok zincirinin bir kopyasını tutan yazılımlardır. Blok zinciri, tüm Bitcoin işlemlerinin paylaşılan bir kaydıdır.

Kendi düğümünüzü çalıştırdığınızda, Bitcoin işlemlerini başkasına güvenmek yerine kendiniz doğrularsınız. Bu size daha fazla bağımsızlık kazandırır ve Bitcoin ağının merkeziyetsiz kalmasına yardımcı olur.

Bir Bitcoin düğümünü, birkaç önemli görevi olan dijital bir trafik polisi gibi düşünebilirsiniz.

1. Blok zincirinin bir kopyasını tutar; bu, tüm Bitcoin işlemlerinin geçmişidir.
1. Düğümler, dünya çapındaki diğer düğümlerle bağlantı kurar ve bilgi paylaşır. Buna bir örnek, onay bekleyen yeni işlemlerin listesi olan mempool’dur.
1. Düğümler, her işlemin Bitcoin’in kurallarına uyup uymadığını kontrol eder. Bir işlem geçersizse, düğüm onu reddeder.

Düğümler ayrıca yeni düğümlerin ağa katılmasına, blok zincirini onlarla paylaşarak yardımcı olur. Ancak, her yeni düğüm yine de tüm kuralları bağımsız olarak kontrol eder.

Herkes Bitcoin Core gibi bir yazılım kurup blok zincirini indirerek bir düğüm çalıştırabilir. Kurulum tamamlandıktan sonra, düğüm yaklaşık her 10 dakikada bir yeni bloklar almaya devam eder ve bunları kendi blok zinciri kopyasına eklemeden önce doğrular.

Bir düğüm çalıştırmak, Bitcoin ağını daha güvenli ve merkeziyetsiz hale getirir; çünkü daha fazla insan sistemi bağımsız olarak doğrulamış olur.

#### Bitcoin Düğümü Nedir?

> Madenciliğin amacı yeni bitcoin üretmek değildir; bu, teşvik sistemidir. Madencilik, Bitcoin’in güvenliğinin merkeziyetsizleştirildiği mekanizmadır.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Madenciler, onaylanmamış işlemleri toplar, bir blok oluşturur ve bloğu ekleyip güvence altına almak için bir anahtar bulmak amacıyla enerji harcar.


Madenciler, işlemlerden oluşan bir sonraki bloğu blok zincirine eklemek için yarışır. Bunu yapmak için, geçerli bir blok hash’i oluşturan özel bir sayı bulmaları gerekir. Bunu, milyarlarca olasılık arasından doğru anahtarı aramak gibi düşünebilirsiniz. Doğru hash’i ilk bulan madenci yarışı kazanır ve bloğunu blok zincirine ekleme hakkı elde eder.

Bir madenci geçerli bir hash bulduğunda, bloğunu ağa paylaşır. Diğer madenciler çözümün doğru olup olmadığını hızla doğrular. Eğer doğruysa, blok blok zincirine eklenir ve Bitcoin’in halka açık defterinin güvenli kalmasına yardımcı olur.

Madenciler iki şekilde bitcoin kazanır:

* **Blok ödülleri:** Yeni bitcoin, bir bloğu başarıyla blok zincirine ekleyen madenciye verilir.
* **İşlem ücretleri:** İnsanlar bitcoin gönderirken küçük bir ücret eklerler. Bloğu ekleyen madenci, o blokta yer alan işlemlerden gelen ücretleri alır.

#### Bitcoin Yarılanmaları


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12.5 BTC | 6.25 BTC | 3.125 BTC |



> **Callout**
>
> Madencilerin bir bloğu tamamladıklarında aldıkları ödül her 210.000 blokta bir, yani yaklaşık her dört yılda bir yarıya iner.


Bitcoin’in maksimum arzı 21.000.000 bitcoin ile sabittir, ancak bunların hepsi Bitcoin başladığında oluşturulmamıştı. Bunun yerine, yeni bitcoin’ler dolaşıma kademeli olarak **madencilik** yoluyla girer.

Madenciler, Bitcoin ağına yeni bir işlem bloğu eklemeyi başardıklarında, **blok ödülü** olarak bitcoin alırlar. Bitcoin’in ilk zamanlarında bu ödül blok başına 50 bitcoin’di. Bu ödül, insanların ağı güvenceye almak için bilgisayar gücü ve elektrik kullanmasını teşvik etti.

Yaklaşık her 210.000 blokta bir (yaklaşık her 4 yılda bir), blok ödülü yarıya düşer. Bu olaya **yarılanma** denir. Yarılanma, yeni bitcoin üretimini yavaşlatır ve toplam arzın asla 21 milyonu geçmemesini sağlar. Zamanla bu, bitcoin’i giderek daha kıt hale getirir.


> **Definition – Dolaşımdaki arz**
>
> **Dolaşımdaki arz** bir para biriminin mevcut toplam miktarını ifade eder. Bitcoin’de, toplam dolaşımdaki arz, herhangi bir anda kazılmış ve dolaşımda olan coin sayısıdır.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/40d7f8b6f4fff4fdc944d66d89ed93eb0f81b682-292x200.svg)


> **Definition – Bitcoin arz takvimi**
>
> **Bitcoin arz takvimi**, yeni bitcoin’lerin dolaşıma girmesi için önceden belirlenmiş ve herkese açık bir plandır; zaman içinde Bitcoin’in kıtlığını korumak için tasarlanmıştır.


Her yarılanma olayından sonra, madencilerin bir blok eklediklerinde aldıkları bitcoin ödülü yarıya iner. Bu, yeni bitcoin’lerin oluşturulma hızını azaltır.

Madenciler, kazdıkları blokta yer alan işlemlerden gelen işlem ücretlerini kazanmaya devam eder. Zamanla, bu ücretlerin madencilerin gelirinde daha büyük bir paya sahip olması beklenmektedir.

Halving'ler Bitcoin protokolüne yerleşiktir ve yaklaşık her dört yılda bir otomatik olarak gerçekleşir. Bu nedenle, Bitcoin’in arz takvimi öngörülebilir ve şeffaftır.

Tablo, yaklaşan halving'leri, yaklaşık tarihlerini, gerçekleşeceği blok numarasını, yeni blok ödülünü ve toplam bitcoin arzının ne kadarının kazılmış olacağını göstermektedir.


| Olay | Tarih | Blok | Ödül | Kazılan |
| --- | --- | --- | --- | --- |
| 5. Halving | 2028 | 1.050.000 | 1,5625 BTC | %98,44 |
| 6. Halving | 2032 | 1.260.000 | 0,78125 BTC | %99,22 |
| 7. Halving | 2036 | 1.470.000 | 0,390625 BTC | %99,61 |


Daha fazla bitcoin kazıldıkça, dolaşımdaki arz artmaya devam eder ve 21.000.000 bitcoinlik maksimum arza ulaşılır; bunun 2140 yılı civarında gerçekleşmesi bekleniyor. Zamanla daha az yeni bitcoin üretildiği için, talep artarsa Bitcoin’in fiyatı yükselebilir. Bu durum ayrıca madencileri, ağın güvenliğini sağlamak için hesaplama güçlerini sunmaya teşvik eder.

#### Bitcoin’de geçerli bir blok hash’i nedir?

Bitcoin’de madenciler, **blok hash’i** adı verilen özel bir kodu bulmak için yarışırlar. Bu kod, bir işlem bloğunu tanımlar ve onun blokzincire eklenmesini sağlar.

Her blok, son işlemler hakkında bilgi içerir ve ayrıca bir önceki bloğun hash’ini de barındırır. Bu, tüm blokları birbirine bağlar ve ilk bloktan (Genesis Bloğu) en son bloğa kadar bir zincir oluşturur.

Bir hash, bloktaki veriler için bir **dijital parmak izi** gibi çalışır. Bloktaki herhangi bir bilgi değişirse, parmak izi de değişir. Bu sayede, blokzincirin işlem geçmişinin değiştirilmediğini herkes kolayca doğrulayabilir ve ağın güvenli kalmasına yardımcı olur.


> **Callout**
>
> Bitcoin’in yaratıcısı Satoshi Nakamoto, Genesis Bloğu’nu kazdı ve toplamda 50 bitcoin açığa çıkardı.


#### Bir Blok Kazma Yarışı

Madenciler, geçerli bir blok hash’i bulmak için yarışırlar. İlk bulan madenci, yeni bloğu blokzincire ekler ve bitcoin ödülünü alır.

Geçerli olabilmesi için, bloğun hash’i ağ tarafından belirlenen zorluk hedefinden daha düşük olmalıdır. Hash’ler rastgele olduğu için, madenciler işe yarayanı bulana kadar farklı girdiler denemek zorundadır.

Çok fazla madenci yarışırsa, bloklar çok hızlı bulunurdu. Çok az madenci katılırsa, blokların bulunması çok uzun sürerdi. Sistemin düzgün çalışmasını sağlamak için, Bitcoin zorluğu her 2.016 blokta bir (yaklaşık iki haftada bir) otomatik olarak ayarlar.

Bu ayarlama, ortalama olarak her 10 dakikada bir yeni bir bloğun blokzincire eklenmesini sağlar.


> **Definition – Zorluk seviyesi tanımı**
>
> **zorluk seviyesi** Bitcoin madenciliğinde, geçerli bir blok hash’i bulmanın ne kadar zor olduğunu ölçer. Ağ, bu zorluğu her 2.016 blokta bir (yaklaşık iki haftada bir) ayarlar, böylece yeni bloklar yaklaşık her 10 dakikada bir blokzincire eklenir. Zorluk ne kadar yüksekse, madencilerin geçerli bir blok bulması o kadar zordur.


Geçerli bir blok hash’i bularak, bir madenci yeni bir bloğu blokzincire eklemek için gereken işi yaptığını kanıtlar. Bu işleme **İş Kanıtı** (Proof of Work - PoW) denir. Bu, Bitcoin’in işlemleri onaylamasını ve yeni blokları blokzincire eklemesini sağlayan güvenlik mekanizmasıdır. Geçerli hash’i ilk bulan madenci, blok ödülü ve o blokta yer alan işlemlerden alınan işlem ücretleriyle birlikte bitcoin kazanır.

İş Kanıtı (PoW), Bitcoin’in güvenliğini sağlar çünkü birinin ağı kandırmaya veya ele geçirmeye çalışmasını son derece maliyetli hale getirir. Bunun yerine kurallara uymak çok daha kârlıdır.

Madenciler dört ana rol oynar:

1. **İşlemleri toplamak**: Madenciler, ağa gönderilmiş işlemleri seçer ve bunları aday bir bloğa yerleştirir.
1. **İş Kanıtı yapmak**: Madenciler, geçerli bir blok hash’i bularak zor bir matematiksel bulmacayı çözmek için yarışırlar.
1. **Bloğu yayınla**: Geçerli bir çözüm bulan ilk madenci, yeni bloğu ağa paylaşır.
1. **Ödül kazan**: Blok geçerliyse, blok zincire eklenir ve madenciye yeni oluşturulan bitcoin ile işlem ücretleri verilir.

Dünyanın dört bir yanındaki birçok madenci aynı anda bir sonraki bloğu oluşturmaya çalışır. Bir madenci geçerli bir çözüm bulduğunda, ağ bloğu kontrol eder. Her şey doğruysa, blok zincire eklenir. Diğer rakip bloklar ise atılır. Bu süreç, ağın uzlaşmasını sağlar ve çift harcamayı önler.

* Madenciler, Bitcoin’in defterini koruyan ve güncelleyen bilgisayarlardır.
* İşlemleri toplar ve bunları bir blokta birleştirirler. Sonra, bloğun verilerini bir karma algoritmasından geçirerek hash adı verilen benzersiz bir kod oluştururlar.
* Madenciler bu işlemi defalarca tekrarlar, Bitcoin’in kurallarına uyan bir hash bulmaya çalışırlar. Geçerli bir hash bulan ilk madenci, ödül olarak yeni oluşturulan bitcoin alır ve bloğu blok zincire eklenir.
* Her bloğun hash’i, onu önceki bloğa da bağlar. Birisi geçmişteki bir işlemi değiştirmeye çalışırsa, hash’ler artık eşleşmez ve ağ değiştirilmiş zinciri reddeder. Bu, Bitcoin’in defterini güvenli tutan şeydir.
