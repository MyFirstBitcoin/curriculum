# 4.1 Bitcoin ve Enerji

> **Callout**
>
> Cambridge Üniversitesi Elektrik Tüketim Endeksi'ne (CBECI) göre, Bitcoin’in yıllık enerji talebi yaklaşık 148 TW civarındadır (3 Ekim 2024 itibarıyla), **bu da dünyanın toplam elektrik tüketiminin yaklaşık %0,6’sına eşittir.**




#### 4.1.0 Bitcoin’in Enerji Tartışması

![In 2020 Bitcoin will consume more power than the world does today](https://cdn.sanity.io/images/vje9ehw2/staging/02833207718ef7dd689839b6da7a4dbc3a222683-671x733.png)

Bitcoin ağının enerjiyle olan ilişkisi, belki de en tartışmalı ve yanlış anlaşılan özelliğidir. Siyasi söylemlerin, artan sanayileşme ve tüketici davranışlarındaki eğilimler nedeniyle insanlığın çevre üzerindeki etkisine karşı giderek daha hassas hale geldiği bir dünyada, faaliyetleri için büyük miktarda enerji kullanan bir teknolojinin ortaya çıkması, önemli bir kamuoyu denetimini beraberinde getirmektedir. Ancak, bu denetimin çoğu pek bilgilendirici değildir ve birçok durumda oldukça yanlıştır; yukarıdaki Dünya Ekonomik Forumu'nun tweet'i de bunu göstermektedir.

Eleştirmenler, Bitcoin madenciliğinin enerji yoğun doğasının — Proof-of-Work (PoW) mutabakat mekanizması tarafından yönlendirilen — karbon emisyonlarına katkıda bulunduğunu, küresel enerji şebekeleri üzerinde ek baskı yarattığını ve bunun da iklim hedeflerini baltaladığını savunuyorlar. Bitcoin’in enerji kullanımını vurgulayan ve zaman zaman Arjantin gibi tüm ülkeleri geride bıraktığını gösteren raporlar, ağın sürdürülebilirlik çabalarını desteklemek yerine çevresel bozulmayı artırdığı yönündeki endişeleri körüklemiştir.

Bununla birlikte, Bitcoin madenciliğinin enerji şebekelerini modernleştirmede ve yenilenebilir enerji kaynaklarına geçişi kolaylaştırmada aslında olumlu bir rol oynayabileceğini öne süren giderek büyüyen bir karşı anlatı da vardır.

Peki, Bitcoin çevre için net bir fayda sağlayabilir mi? Şebeke verimliliği ve istikrarına katkıda bulunabilir ve böylece yenilenebilir enerji üretimine geçişi destekleyebilir mi?



#### 4.1.1 Güvenlik Olarak Enerji Kullanımı

Bitcoin ağının temel işlevi, merkezi olmayan bir işlem defterini korumaktır. Bunu doğrulayacak merkezi bir otorite olmadığında, ağın defterin bütünlüğünü sağlamak ve 'çifte harcama'nın önüne geçmek için bir yol bulması gerekir. Ağdaki tüm katılımcıların, belirli bir anda defterin durumu (kimin neye sahip olduğu) konusunda hemfikir olması gerekir. İşte burada madencilik devreye girer.

Madenciler, dünya çapında yayılmış özel bilgisayar donanımları veya ASIC'ler (Uygulamaya Özel Entegre Devreler) kullanır. ASIC'ler, saniyede katrilyonlarca hesaplama yaparak kriptografik bir bulmacanın çözümünü tekrar tekrar tahmin etmek üzere tasarlanmıştır. Başarılı bir tahmin, madenciye yeni basılmış bitcoin şeklinde ödül kazandırır ve ağ, madencinin başarılı olduğunu gerçek zamanlı olarak kriptografik olarak doğrular. Bu nedenle bu sürece 'iş ispatı' (proof-of-work) adı verilir.

Dünya çapındaki madenciler topluca muazzam bir hesaplama gücü sağlar. Bu, ağın güvenliğini sağlamak için tasarlanmıştır — ağı kendi çıkarı için saldırmak veya manipüle etmek isteyen kötü niyetli birinin, ağın çoğunluğunu kontrol edecek kadar büyük bir hesaplama gücü kullanması gerekir. Bu mümkün olsa bile, çok büyük mali kaynaklar gerektirir ve yine de Bitcoin ağını önemli ölçüde bozacak kadar uzun süre kontrolü elinde tutması pek olası değildir. Bu nedenle, bu tür bir saldırının başarılı olma olasılığı enerji engeli sayesinde neredeyse sıfıra inmiştir.

> Bitcoin elektrik israf etmez, güvenlik için kullanır.  
_Kyle Torpey_



#### 4.1.2 Boşa Giden Enerjinin Peşinde

Bitcoin madencileri, işlemler defterine bir sonraki bloğu ekleyip 'blok ödülünü' almak için 7/24 süren küresel bir yarışta diğer oyunculara karşı son derece rekabetçi bir ortamda faaliyet gösterirler. Madenciler için hem bol bulunan hem de talep açısından az ya da hiç rekabet olmayan en ucuz enerjiyi bulmak ticari açıdan kritik öneme sahiptir. Bu da madencileri boşa giden veya israf edilen enerji kaynaklarına yönlendirir.

Bunun temel nedeni maliyet etkinliğidir. Elektrik, madenciler için ana işletme maliyetidir çünkü süreç oldukça enerji yoğundur. Boşa giden enerji — yani aksi takdirde kullanılmayacak olan, örneğin yenilenebilir kaynaklardan elde edilen fazla enerji veya doğal gazın yakılması gibi — kullanılarak madenciler enerji maliyetlerini önemli ölçüde azaltabilirler. Boşa giden enerji genellikle daha ucuzdur çünkü kolayca erişilemez veya yüksek talep görmez. Örneğin, fazla hidroelektrik veya rüzgar enerjisi olan bölgelerde, enerjiyi dağıtacak altyapı eksikliği nedeniyle fiyatlar düşebilir. Bu da madencilere düşük maliyetli elektrik anlaşmaları yapma fırsatı sunar ve kâr marjlarını artırır.

Elektrik anlaşmaları, madencilerin boşa giden veya atık enerji kaynaklarına erişimini güvence altına alabilir ve onları geleneksel enerji piyasalarının dalgalanmalarından koruyabilir. Elektrik fiyatları, mevsimsel talep, fosil yakıt fiyatları ve jeopolitik olaylar nedeniyle dalgalanır. Boşa giden enerji, madencilere daha istikrarlı ve öngörülebilir bir enerji arzı sunar, bu da uzun vadeli planlama ve kârlılığı daha mümkün kılar. Ayrıca, boşa giden enerjinin kullanılması, madencinin karbon ayak izini azaltarak çevresel eleştirileri hafifletir ve itibar açısından da fayda sağlar.

Madenciye fayda sağlamanın yanı sıra, enerji üreticisi de fazla enerjisi için güvenilir bir müşteri kazanır. Özellikle uzak veya kaynak açısından zengin bölgelerdeki enerji üreticilerinin fazla enerjiyi satmak için sınırlı seçenekleri olabilir. Bitcoin madencileri, aksi takdirde israf edilecek bu enerji için cazip bir 'son çare alıcısı' sunar. Bu nedenle, enerji üreticileri ile madencilik şirketleri arasındaki ortaklıklar karşılıklı fayda sağlayabilir; üreticiler boşa giden enerjiyi paraya dönüştürürken, madenciler ucuz enerjiye erişim sağlar.

Ayrıca, güneş ve rüzgar gibi yenilenebilir enerji kaynakları, genellikle düşük talep zamanlarında veya büyük enerji tüketicilerinden uzak yerlerde fazla enerji üretir. Bitcoin madencileri, bu kaynakların yakınında operasyon kurarak aksi takdirde sınırlandırılacak (yani israf edilecek) enerjiyi ticari olarak kullanabilirler. Bu, özellikle üretimi düzensiz olan rüzgar çiftlikleri veya güneş tarlaları için önemlidir. Bu durum, kullanılmayan yakıtın ticari talebin olduğu yerlere kolayca taşınabildiği fosil yakıtlı elektrik şebekelerinden farklıdır. Bu nedenle, fosil yakıtlı elektrik genellikle kârlı madenciliği destekleyecek kadar ucuz değildir.



#### 4.1.3 Şebeke Dengeleme Zorluğu



Bir elektrik üreticisinin bakış açısından, şebeke dengelemesi, güneş ve rüzgar gibi birçok yenilenebilir kaynağın aralıklı doğası nedeniyle yenilenebilir enerji şebekeleri için önemli bir zorluktur. Geleneksel enerji kaynaklarının (ör. kömür, gaz veya nükleer) aksine, sürekli elektrik üretebilen yenilenebilirler çevresel koşullara bağlıdır. Bu da enerji üretiminde dalgalanmalara yol açar ve arz ile talebin gerçek zamanlı olarak dengelenmesini zorlaştırır.



Örneğin, güneş ve rüzgar enerjisi üretimi hava durumuna ve günün saatine bağlıdır. Güneş enerjisi yalnızca güneş parladığında çalışır ve rüzgar türbinleri yalnızca rüzgar estiğinde elektrik üretir. Bu da enerji arzının değişkenliğine yol açar ve elektrik arzının her zaman taleple eşleşmesini zorlaştırır. Yenilenebilir enerji üretiminde ani bir düşüş (örneğin, rüzgarın durması veya bulutlu havalarda) elektrik mevcudiyetinde keskin azalmalar yaratabilir, bu da elektrik kesintilerine yol açabilir veya fosil yakıtlı santrallerden yedek güç gerektirebilir.



Ayrıca, yüksek yenilenebilir enerji üretimi (ör. güneşli veya rüzgarlı günler) ve düşük talep dönemlerinde (örneğin her sabah 1-4 arası), şebekenin aşırı yüklenmesini önlemek için bazı yenilenebilir enerji üretimi sınırlandırılmak zorunda kalır. Bu, yenilenebilir enerji projelerinin ekonomik uygulanabilirliğini azaltır ve verimsizlik yaratır.



Bazen pillerin veya diğer enerji depolama teknolojilerinin enerji üretimindeki değişkenliği yumuşatıp yumuşatamayacağı sorulur. Bu teknolojiler, yenilenebilirlerden üretilen fazla enerjiyi depolamaya yardımcı olabilse de, genellikle pahalıdır ve sınırlı kapasiteye sahiptir. Bu da enerji üretimi ve tüketimindeki dalgalanmaları uzun vadede dengelemeyi zorlaştırır.







#### 4.1.4 Bitcoin Dengeleyici Olarak



Bitcoin madenciliği, esnek enerji talebi sayesinde, yenilenebilir enerji şebekelerini dengelemek için etkili bir talep tarafı yönetim aracı olabilir. Bitcoin madencileri, şebekenin ihtiyaçlarına göre enerji tüketimlerini hızla ayarlayabilirler. Yenilenebilir enerji üretiminin fazla olduğu dönemlerde, madenciler operasyonlarını artırarak fazla enerjiyi emebilirler. Tersine, yüksek talep veya düşük yenilenebilir enerji üretimi dönemlerinde, madenciler operasyonlarını hızla durdurabilir veya azaltabilir, böylece temel hizmetler için enerji açığa çıkarırlar. Bu esneklik, şebekenin dengelenmesine yardımcı olur ve aralıklı yenilenebilir kaynakların entegrasyonunu, pahalı depolama çözümlerine veya fazla enerjiyi ısıya dönüştüren dirençli yük bankalarının kullanılmasına gerek kalmadan kolaylaştırır.



Ayrıca, birçok Bitcoin madencisi, şebekenin zorlandığı zamanlarda (ör. sıcak hava dalgaları veya soğuk hava patlamaları sırasında) gönüllü olarak enerji tüketimini azaltmayı içeren talep yanıt programlarına katılır. Kontrol edilebilir bir yük olarak hareket ederek, madenciler elektrik kesintilerini önlemeye ve özellikle yüksek talep dönemlerinde şebekenin istikrarlı kalmasına yardımcı olabilirler.



Fazla yenilenebilir enerjiyi sınırlandırmak yerine, Bitcoin madenciliği bu fazla enerjiyi tüketebilir ve etkin bir şekilde paraya dönüştürebilir. Bu, aksi takdirde israf edilecek enerji için ekonomik bir kullanım alanı yaratır ve yenilenebilir enerji projelerinin genel verimliliğini artırır. Yenilenebilirlerin yaygın olduğu bölgelerde, örneğin Teksas veya İzlanda’da, Bitcoin madencileri yenilenebilir enerji santrallerinin yakınında operasyonlar kurarak fazla enerjiyi emerken şebekenin de dengelenmesine yardımcı olmuştur.



Teksas’ta, Bitcoin madencileri Texas Elektrik Güvenilirliği Konseyi (ERCOT) 2 ile şebeke dengeleme çalışmalarına katılmıştır. Bu madenciler, gerçek zamanlı şebeke koşullarına göre operasyonlarını ayarlayarak elektrik arz ve talebinin dengelenmesine yardımcı olur ve yenilenebilir enerjinin şebeke güvenilirliğinden ödün vermeden etkin bir şekilde entegre edilmesini sağlar. Örneğin, 2021 Teksas kış fırtınası sırasında Bitcoin madencileri enerji tüketimini azaltarak kritik altyapı ve konut kullanımı için enerji açığa çıkarmıştır.





#### 4.1.5 Temiz Enerjiyi Teşvik Etmek



Fazla yenilenebilir enerjiyi paraya dönüştürmenin ve son çare alıcısı olarak hareket etmenin yanı sıra, Bitcoin madencileri enerji sağlayıcılarıyla uzun vadeli ortaklıklar kurarak yeni yenilenebilir enerji altyapısına yatırım yapılmasını da teşvik ediyor. Bu, enerji tedarikçisine istikrarlı ve güvenilir bir gelir akışı sağlar ve ek rüzgar çiftlikleri, güneş santralleri ve hidroelektrik projelerinin geliştirilmesini teşvik eder. Bitcoin madencilerinin varlığı, sürekli bir müşteri tabanı sağlayarak bu tür projeleri finansal olarak daha uygulanabilir hale getirebilir. Ayrıca, madenciler enerjinin bedelini hemen ödeyebilir, yani elektrik kaynağı henüz şebekeye bağlanmadan önce. Bu, geri ödeme süresini önemli ölçüde kısaltır ve yeni bir yenilenebilir enerji projesinin sermaye maliyetini düşürür. Bir Bitcoin madencisi garantili tüketici olarak hareket ettiğinde, enerji sağlayıcı madenci olmadan mümkün olandan daha büyük bir proje inşa etmeyi tercih edebilir.



Yenilenebilir enerji için sürekli bir alıcıya duyulan ihtiyaç, yakın zamanda Birleşik Krallık’ta açıkça ortaya çıktı - rüzgar çiftliklerinin kapatılması için ödeme yapıldığı ve yerlerine gaz santrallerinin kullanıldığı yaygın olarak bildirildi.[Boşa Giden Rüzgar](https://wastedwind.energy/), Birleşik Krallık'taki kullanılmayan rüzgar enerjisi miktarını takip eden bir web sitesi, 2025'in ilk iki ayında bu kısıtlamanın tüketicilere maliyetinin 253 milyon £ olduğunu, bir önceki yılın aynı dönemine göre 158 milyon £ artış olduğunu tahmin etti.



Business Matters, sorunun nedeninin “Britanya'nın iletim altyapısının yükseltilebileceğinden daha hızlı inşa edilen açık deniz rüzgar çiftliklerinin hızlı genişlemesi” olduğunu iddia ediyor. Rüzgarlı ve talebin düşük olduğu günlerde, elektrik ağı fazla enerjiyi iletemez ve ağ operatörü, rüzgar çiftliklerine kapanmaları için fiilen tazminat öder. Ayrıca, talep merkezine daha yakın olan gazla çalışan elektrik santrallerine de farkı karşılamaları için ödeme yapar.

Buna karşılık, jeotermal ve hidroelektrik enerjinin hakim olduğu İzlanda'da, Bitcoin madencileri yenilenebilir enerji altyapısının genişlemesinde itici güç olmuştur. Bölgede mevcut olan düşük maliyetli yenilenebilir enerji, çok sayıda madencilik operasyonunu cezbetmiş ve iki sektör arasında sinerjik bir ilişki yaratmıştır.



> İzlanda hükümeti, Bitcoin madenciliğinin ekonomiyi canlandırma, istihdam yaratma ve yabancı yatırımı çekme potansiyelini tanımıştır. Sonuç olarak, sektörü desteklemiş ve büyümesini aktif olarak teşvik etmiştir.  
_Industry Leaders Magazine_





Bitcoin madenciliğinin coğrafi esnekliği de önemlidir. Bitcoin madenciliği operasyonları, geleneksel endüstrilerde olduğu gibi coğrafi olarak kısıtlanmaz. Bol miktarda yenilenebilir enerji kaynağına sahip, ancak nüfus merkezlerine veya iletim altyapısına sınırlı erişimi olan uzak bölgelerde kurulabilirler. Bu, onları geleneksel endüstrilerin mümkün olmayacağı yerlerde enerji tüketimi için ideal adaylar yapar ve kullanılmayan alanlarda temiz enerji gelişimini teşvik eder. Bu şekilde, Bitcoin madencileri enerji kaynağına gelen bir pazar oluşturur, enerjinin onlara getirilmesini gerektirmez; böylece tüm ilgili altyapı maliyetlerinden kaçınılır.



Bitcoin madenciliği, temiz enerjiye sürekli talep yaratarak, şebekeleri dengelemeye yardımcı olarak ve yenilenebilir kaynaklar açısından zengin bölgelerde altyapı gelişimini destekleyerek yenilenebilir enerji gelişimi için güçlü bir ekonomik teşvik sunar. Madencilik operasyonları giderek daha fazla yenilenebilir enerjiye yöneldikçe, küresel olarak daha sürdürülebilir bir enerji geleceğine geçişte kilit oyuncular haline gelmektedirler.




> **Info – Flaring'in Ortadan Kaldırılması?**
>
> Atık enerjinin, örneğin alevlenen doğal gazın kullanılması sadece para tasarrufu sağlamakla kalmaz, aynı zamanda çevresel eleştirileri de hafifletir. Flaring, fazla doğal gazın (metan) yakıt olarak satılamadığı için petrol sondaj sahalarında yakılmasıdır. Bazı çalışmalara göre5, metan CO2'ye göre yaklaşık 120 kat daha fazla ısı tutar, bu nedenle yakılması gerekir ve bu şekilde CO2'ye dönüştürülür. Ancak, flaring %100 etkili değildir ve yine de metanın atmosfere karışmasına izin verir. Bitcoin madencileri bu enerjiyi operasyonlarını çalıştırmak için kullanabilir, bu da flaring kaynaklı sera gazı emisyonlarını azaltır. Doğal gaz, jeneratörlerde yakılarak elektrik üretilir ve bu elektrik, doğrudan kuyu sahasında bulunan taşınabilir madencilik cihazlarını çalıştırır.
>
> Petrol şirketleri için bu uygulama, bir atık ürünü gelir kaynağına dönüştürür. Doğal gazı Bitcoin madencilerine satarak veya kendi madencilik operasyonlarını kurarak, şirketler aksi halde boşa gidecek gazı paraya çevirebilirler. Bu, petrol çıkarma sürecini daha verimli ve kârlı hale getirir.
>
> Ayrıca, hükümetler daha sıkı çevre düzenlemeleri uyguladıkça, petrol üreticileri emisyonları azaltmak için artan bir baskı ile karşı karşıya kalıyor. Alevlenen gazı yakalayıp kullanmak, şirketlerin çevre yasalarına uymasına ve karbon kredisi kazanmasına yardımcı olabilir; bu da bu çözümü sadece ekonomik faydaları için değil, aynı zamanda düzenleyici nedenlerle de cazip kılar.
>
> Crusoe Energy Systems, alevlenen doğal gazla çalışan taşınabilir madencilik sistemleri kurmak için petrol üreticileriyle ortaklık yapan ABD merkezli bir şirkettir. 2022 yılına gelindiğinde Crusoe, Kuzey Dakota ve Montana'daki petrol kuyularında 98'den fazla konteyner tabanlı veri merkezi kurmuştu.
>
> Aksi halde alevlenecek olan kullanılmayan doğal gazı kullanarak, Bitcoin madenciliği küresel olarak zararlı metan emisyonlarını azaltabilir, petrol üreticileri için ek gelir yaratabilir ve daha sürdürülebilir enerji uygulamalarını teşvik edebilir. Bu yöntem, çevresel bir sorunu fırsata dönüştürerek, Bitcoin madenciliği etrafında gelişen yeniliklerin enerji sektörüyle nasıl kesişebileceğini ve hem ekonomik hem de çevresel faydalar sağlayabileceğini gösteriyor.






#### 4.1.6 Gelişen Olumlu Bir Hikaye



Bitcoin'in enerjiyle olan ilişkisi çok yönlü ve gelişmektedir. Bitcoin madenciliği, yüksek enerji tüketimi nedeniyle eleştirilmiştir; bazı yorumcular ve çevreciler, ağın enerji kullanımının tüm ülkelerle eşdeğer olduğunu gösteren çalışmalara atıfta bulunurken, diğerleri sektörün enerji talebinin iklim değişikliğini daha da kötüleştirebileceğinden endişe ediyor. Ancak bu anlatı, Bitcoin madenciliğinin yenilenebilir enerjiye geçişte ve şebeke verimliliğinde yapıcı bir rol oynama potansiyelini tamamen göz ardı ediyor.



Bitcoin madenciliği, ucuz ve bol elektriğe olan benzersiz ihtiyacıyla giderek daha fazla yenilenebilir enerji kaynaklarıyla uyumlu hale gelmiştir. Rüzgar, güneş veya hidroelektrik açısından zengin bölgelerde, madenciler aksi halde boşa gidecek fazla veya kullanılmayan enerjiden yararlanabilirler. Bu dinamik, özellikle düşük talep zamanlarında fazla elektrik için sürekli bir talep sağlayarak yenilenebilir enerji projelerinin ekonomik uygulanabilirliğini artırmaya yardımcı olur.



Kullanılmayan enerji kaynaklarını aramak, Bitcoin madencileri için ticari açıdan gereklidir çünkü maliyetleri düşürür, çevresel sürdürülebilirliği artırır ve dalgalı bir enerji piyasasında operasyonel istikrar sağlar. Bu strateji, madenciliği sadece daha kârlı hale getirmekle kalmaz, aynı zamanda sektörü şebeke yönetimi ve yenilenebilir enerji gelişiminde kilit bir oyuncu konumuna getirir.



Bitcoin madenciliği, yenilenebilir enerji şebekelerinin karşılaştığı temel zorluklardan bazılarına çözümler sunar. Güneş ve rüzgar enerjisinin kesintili doğası, enerji üretiminin hava koşullarına bağlı olarak dalgalanması nedeniyle istikrarsızlık yaratır. Esnek ve ölçeklenebilir operasyonlara sahip Bitcoin madencileri, fazla üretim zamanlarında fazla enerjiyi tüketerek ve yüksek talep dönemlerinde faaliyetlerini azaltarak şebekeyi dengelemeye yardımcı olabilir. Bu talep-yanıt yeteneği, madencilerin şebeke operatörleriyle iş birliği yaptığı Teksas gibi pazarlarda şimdiden kullanılmaktadır.



![Bitcoin doesn't waste energy. It uses wasted energy.](https://cdn.sanity.io/images/vje9ehw2/staging/83fdab61e09fec09da7448f396e100c3aca342b4-455x587.png)

Bitcoin'in petrol sahalarında metan alevlenmesini ortadan kaldırma potansiyeli, gözden kaçan bir başka faydadır. Aksi halde yakılacak olan kullanılmayan doğal gazı yakalayıp kullanarak, Bitcoin madencileri zararlı metan emisyonlarını azaltmaya yardımcı olabilir ve çevreye zarar veren bir atık ürünü değerli bir kaynağa dönüştürebilir.



Bitcoin madenciliğinin çevresel açıdan incelenmesi beklenen ve memnuniyetle karşılanan bir durumdur. Ancak teknoloji, yenilenebilir enerji benimsenmesini ilerletmek ve şebeke verimliliğini artırmak için benzersiz fırsatlar sunduğunu giderek daha fazla göstermektedir.

Sektör olgunlaştıkça, yenilenebilir enerji sağlayıcıları ve şebeke operatörleriyle daha fazla iş birliği, Bitcoin madenciliğinin küresel olarak daha sürdürülebilir bir enerji geleceğine geçişte kilit bir oyuncu olmasına yardımcı oluyor.




> **Info**
>
> **Bitcoin enerjiyi boşa harcamaz. Boşa harcanan enerjiyi kullanır.**
>
> Bizi dünya genelinde kullanılmayan veya atıl enerji kaynaklarını aramaya ve kullanmaya aktif olarak teşvik ediyor. Ve, bu kaynakların etrafında daha fazla elektrik altyapısı inşa ederek, insanlık ve çevre uzun vadede fayda görecektir.




###### Notlar

1. Bitcoin Elektriği Boşa Harcamaz, Güvenlik İçin Kullanılır, elektriğin Bitcoin’in güvenlik modeli için temel olduğunu açıklayan bir makale, Bitcoin Magazine, Kasım 2015 [https://bitcoinmagazine.com/business/bitcoin-doesn-t-waste-electricity-it-s-used-for-security-1446482572](https://bitcoinmagazine.com/business/bitcoin-doesn-t-waste-electricity-it-s-used-for-security-1446482572)
1. Bitcoin madencileri, Teksas'taki Büyük Esnek Yüklerin %95'ini oluşturuyor, The Miner Mag, Şubat 2024.[https://theminermag.com/news/2024-02-29/bitcoin-mining-map-north-america-texas/](https://theminermag.com/news/2024-02-29/bitcoin-mining-map-north-america-texas/)
1. Şebeke kapasitesi eksikliği ‘boşa giden rüzgar’ maliyetlerini 250 milyon £’a çıkarıyor, Business Matters, Mart 2025[https://bmmagazine.co.uk/news/lack-of-grid-capacity-pushes-wasted-wind-costs-to-250m/](https://bmmagazine.co.uk/news/lack-of-grid-capacity-pushes-wasted-wind-costs-to-250m/)
1. İzlanda: Beklenmedik Bir Bitcoin Madenciliği Merkezi, Industry Leader Magazine, Eylül 2023[https://www.industryleadersmagazine.com/iceland-the-unlikely-bitcoin-mining-hub/](https://www.industryleadersmagazine.com/iceland-the-unlikely-bitcoin-mining-hub/)
1. Metanı karbondioksitten daha güçlü bir sera gazı yapan nedir? Climate Portal, Aralık 2023.[https://climate.mit.edu/ask-mit/what-makes-methane-more-potent-greenhouse-gas-carbon-dioxide](https://climate.mit.edu/ask-mit/what-makes-methane-more-potent-greenhouse-gas-carbon-dioxide)
1. Bitcoin flare firması Crusoe, rakibi Great American Mining'i satın aldı, Data Center Dynamics, Ekim 2022[https://www.datacenterdynamics.com/en/news/bitcoin-flare-firm-crusoe-buys-rival-great-american-mining/](https://www.datacenterdynamics.com/en/news/bitcoin-flare-firm-crusoe-buys-rival-great-american-mining/)
