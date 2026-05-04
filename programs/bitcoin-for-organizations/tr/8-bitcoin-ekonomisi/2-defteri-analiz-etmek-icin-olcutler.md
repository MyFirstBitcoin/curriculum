# 8.2 Defteri Analiz Etmek İçin Ölçütler

Bitcoin’in şeffaflığı, geleneksel finansal sistemlerden farklıdır — burada paranın büyük bir kısmı kapalı kurumsal kapılar ardında hareket eder — bu nedenle zincir üzerindeki analizler için zengin bir alan ortaya çıkar. Ağ düzeyindeki veriler, kullanıcı davranışını, para akışlarını ve uzun vadeli eğilimleri anlamak için bir mercek haline gelir. Bu metrikler, ağın ne kadar aktif kullanıldığını, coinlerin biriktirilip biriktirilmediğini veya satılıp satılmadığını ve ağın daha güvenli hale gelip gelmediğini gibi belirli sorulara yanıt bulmaya yardımcı olabilir.

Bu metrikleri anlamak, yalnızca Bitcoin kullanıcıları için değil, aynı zamanda bu benzersiz şekilde şeffaf finansal sistemi anlamak isteyen araştırmacılar veya politika yapıcılar için de faydalıdır.

Bu bölüm, Bitcoin aktivitesini analiz etmek için yaygın olarak kullanılan bazı metrikleri alt kategoriler halinde gruplandırılmış olarak içerir. Bu kapsamlı bir liste değildir. Daha fazla metrik ve açıklama için [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) adresini ziyaret edebilirsiniz.



#### 8.2.1 Adres Metrikleri

Adres metriklerini zaman içinde izlemek faydalıdır çünkü bunlar Bitcoin ağındaki aktivite seviyesini gösterir. Örneğin, Bitcoin daha fazla benimsendikçe, aktif adres sayısı artar. Bunu daha da detaylandırmak için, belirli bir zaman diliminde (örneğin bir yıl) en az 0.1 BTC tutan adreslerin sayısını inceleyebiliriz. Bu, zaman içinde Bitcoin benimsenmesine dair bir bakış sunar, ancak mükemmel değildir çünkü bir kişi birden fazla Bitcoin adresine sahip olabilir. Öte yandan, borsalar veya ETF’ler, çok sayıda kişi adına fon tuttuklarında tek bir varlık gibi görünebilir.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Yıllara Göre X BTC'den Fazla Bitcoin Tutan Adresler. Kaynak: Bitcoin Magazine Pro._

Adresleri mevcut BTC piyasa fiyatı ile karşılaştırarak, toplam Bitcoin adreslerinin kârda olan yüzdesini görebiliriz. Bu, piyasa hissiyatını izlememizi sağlar çünkü piyasanın ne kadarının BTC’yi kârda veya zararda tuttuğunu görebiliriz.

Örneğin, aşağıdaki **Gerçekleşmemiş Kâr Yüzdesi** grafiği, tüm defter adreslerinin ABD doları cinsinden ölçülen gerçekleşmemiş kâr oranını gösterir. Aşağıdaki grafik Bitcoin’in tüm zamanların en yüksek seviyesine yakın bir zamanda alındığı için, gerçekleşmemiş kâr gösteren adreslerin yüzdesi neredeyse yüzde yüze yakındır. Ayrıca, Gerçekleşmemiş Kâr Yüzdesi'nin ortalamanın bir standart sapmasının altına düştüğü uzun dönemlerin nadir olduğunu görebiliriz. Bu nedenle, bu çizginin altına bir düşüş, alıcılar için iyi bir giriş noktası önerebilir.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Gerçekleşmemiş Kâr Yüzdesi. Kaynak: checkonchain.com_



#### 8.2.2 Zincir Üzeri Göstergeler

Zincir üzeri göstergeler faydalıdır çünkü fiyat ve adres metriklerinin tek başına gösteremeyeceği şekilde ağ davranışına dair içgörüler sunar. Analistler, coinlerin nasıl tutulduğunu, taşındığını veya zaman içinde nasıl değerlendiğini izleyerek uzun vadeli sahipler ile kısa vadeli yatırımcıların eylem ve hissiyatını anlayabilirler. Bu göstergeler, defterin şeffaf doğasından yararlanarak birikim, dağıtım veya yatırımcı inancı gibi gizli piyasa dinamiklerini ortaya çıkarır. Bu da onları yapısal eğilimleri belirlemek, piyasanın aşırı ısınmış mı yoksa değeri düşük mü olduğunu değerlendirmek ve piyasa döngüsündeki dönüş noktalarını öngörmek için özellikle faydalı kılar.

Örneğin, BTC varlıklarının en son ne zaman hareket ettiğinden beri değerini inceleyerek, piyasanın sıkıntı içinde olup olmadığını (örneğin büyük bir döngü dibinde olduğu gibi) çıkarabiliriz. Bu metrik, **Gerçekleşen Fiyat** olarak bilinir ve dolaşımdaki tüm BTC’nin ‘ortalama maliyet tabanını’ verir. Piyasa fiyatı Gerçekleşen Fiyat’ın altına düşerse, bu, toplamda adreslerin çoğunun kâğıt üzerinde zarar ettiğini gösterir.

Defter verilerini yaş bantlarına göre daha da gruplandırarak, BTC miktarının zaman içinde adresler arasında nasıl hareket ettiğini gösterebiliriz; bu da grafikte dalga benzeri desenler oluşturan ve **HODL dalgaları** olarak bilinen bir görünüm sunar.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL Dalgaları. Kaynak: Bitcoin Magazine Pro._

HODL dalgaları, uzun vadeli, orta vadeli ve kısa vadeli sahiplerin BTC’leriyle ne yaptığını gösterir. Örneğin, yukarıdaki grafikte kısa vadeli sahipler kırmızı ve turuncu ile gösterilmiş ve bu grubun piyasa zirvelerine yakın alım yapmak için acele ettiği zamanlarda aktivite artışları görebiliyoruz. Diğer tarafta, çok uzun vadeli sahiplerin (mor ve mavi) ağdaki toplam paylarının istikrarlı bir şekilde arttığını, bu gruplar arasında yüksek bir inanç olduğunu gösteriyor. Grafik mükemmel değildir çünkü bazı coinler aynı kullanıcı kontrolünde eski adreslerden yeni adreslere taşınabilir. Ancak, uzun vadeli sahiplerin inancına dair ilginç bir bakış sunar.

Uzun vadeli sahiplerin ‘akıllı parası’nı incelemenin bir başka yolu da **Coin Günleri Yok Edildi** (CDD) metriğini incelemektir. ‘Coin Günleri’ kavramı, BTC miktarının coinlerin en son hareket ettiği günden bu yana geçen günlerle çarpılmasıdır. Örneğin, 100 gündür hareket etmeyen 5 BTC, 500 coin günü biriktirmiş olur ve 10 gündür hareket etmeyen 10 BTC, 100 coin günü biriktirmiş olur. Bu şekilde, daha uzun süre tutulan coinlere ekstra ağırlık veririz. Bu coinler hareket ettiğinde, bu coin günleri ‘yok edilir’. Bu gösterge, önemli fiyat hareketleri sırasında CDD’de artışlar gösterir ve analistlere rutin piyasa aktivitesi ile uzun vadeli sahiplerin hissiyatındaki anlamlı değişimleri ayırt etme imkanı sunar.

Piyasanın BTC’yi düşük veya yüksek değerli görüp görmediğini belirlemeye yardımcı olabilecek bir diğer metrik ise Piyasa Değeri / Gerçekleşen Değer oranı, yani **MVRV**. Bu oran, Piyasa Değeri’nin (dolaşımdaki BTC sayısı ile piyasa fiyatının çarpımı) Gerçekleşen Değer’e (coinlerin en son hareket ettiği zamandan bu yana tüm BTC’nin toplamı) bölünmesiyle hesaplanır. Yüksek MVRV, daha fazla coinin kârda olduğunu (genellikle piyasa zirvelerinde görülür) ve düşük MVRV, birçok coinin zararda tutulduğunu (piyasa diplerinde görülür) gösterir.



#### 8.2.3 Madencilik Metrikleri

Madencilik metrikleri, Bitcoin ağının güvenliğini, ekonomik teşviklerini ve genel sağlığını anlamak için faydalıdır. Hashrate, madenci geliri, zorluk ve ücret oranları gibi metrikler, blokzincirini ne kadar hesaplama gücünün koruduğunu ve madencilerin faaliyetleri için ne kadar iyi ödüllendirildiğini gösterir.

**Hashrate** Bitcoin ağının belki de en çok atıfta bulunulan sağlık ve güvenlik göstergesidir. Madencilik işlemi ağı güvence altına aldığı ve defterdeki işlemlerin geçerli olduğunu doğruladığı için, ne kadar fazla hesaplama (veya hash) gücü varsa, kötü niyetli bir aktörün ağı ele geçirip saldırması o kadar zor olur.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Kaynak: Bitcoin Magazine Pro._

Yukarıdaki grafik, Mayıs 2025’te ağın toplam hesaplama gücünün yaklaşık 900 TeraHash/s (saniyede 900 trilyon kriptografik ‘hash’ hesaplaması) seviyesinde olduğunu gösteriyor. Hashrate yükseliyorsa, ağın daha güvenli hale geldiğini gösterir ve bu da kullanıcılar için güven vericidir.

Puell Multiple (David Puell tarafından geliştirilmiştir), piyasa döngüsüne madenciler ve onların gelirleri açısından bakar. Metrik, günlük BTC ihraç miktarının (USD cinsinden) 365 günlük hareketli ortalamasına bölünmesiyle hesaplanır. Bu metrik, madenci stresi veya rahatlama dönemlerini belirlemeye yardımcı olur. Tarihsel olarak, 3’ün üzerindeki bir değer, madencilerin çok kârlı olduğunu gösterdiği için BTC piyasa değerinde bir düşüşten önce gelmiştir. 0.5’in altındaki bir değer ise stresi ve BTC değerinde tarihsel olarak piyasa diplerini işaret etmiştir.
