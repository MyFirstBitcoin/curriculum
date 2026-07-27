# 2.3 Bitcoin, küresel para olmak için çok yavaş.

> Vizyonerler, uzaktan çalışanların, etkileşimli kütüphanelerin ve multimedya sınıflarının olduğu bir gelecek görüyorlar. Elektronik mahalle toplantılarından ve sanal topluluklardan bahsediyorlar... Gerçek şu ki, hiçbir çevrimiçi veritabanı günlük gazetenizin yerini alamaz, hiçbir CD-ROM yetkin bir öğretmenin yerini tutamaz ve hiçbir bilgisayar ağı hükümetin işleyişini değiştiremez.  
_Clifford Stroll_

17 yıl sonra, Newsweek basılı yayını durdurdu ve yalnızca çevrimiçi olarak erişilebilir hale geldi. 1974 yılında İletim Kontrol Protokolü (TCP) ilk oluşturulduğunda hayatta olduğunuzu hayal edin.

Kimse elinizdeki tüm uygulamalarıyla akıllı telefonu öngöremedi. Kimse arabanızdaki navigasyon sistemini göremedi.

İnternet bir anda ortaya çıkmadı, aksine protokollerin ve katmanların evrimiyle yavaş yavaş gelişti. Bu evrimler TCP üzerine inşa edildi, ancak çoğunlukla TCP'yi değiştirmedi.

> Geleceğin iletişim platformlarına geçişe bakarken, internet protokollerinin güzelliğinin hizmet ve teknoloji arasındaki katmanların ayrılmasını sağlamak olduğunu görüyorum.  
_Michael K Powell_



##### Bitcoin’in evrimini internetin evrimiyle karşılaştırın

TCP, internetteki diğer her şeyin ortaya çıkması için gerekliydi ama yeterli değildi. Bitcoin’in evrimi de benzer bir yolu izliyor gibi görünüyor. Açık sistemler, katmanlar halinde geliştirildiğinde daha dayanıklı ve başarılı olma eğiliminde, ancak ilk yapı taşlarının döşenmesiyle yaygın benimsenme arasında çok zaman geçebilir. Tümleşik çözümler, açık sistemlerde protokoller üzerine katmanlar halinde inşa edilenler kadar etkili görünmüyor. Filmler TCP kullanılarak yayınlanamıyor diye kimse interneti baştan inşa etmek zorunda kalmadıysa, Bitcoin’de de muhtemelen durum böyle olacak.

Bitcoin üzerinde halihazırda bir dizi ikinci katman protokolü bulunuyor ve bu ikinci katman protokollerinin üzerinde çalışan birçok uygulama var (bunlar hakkında daha fazla bilgi için bölüm 201.4’e bakınız).

Bitcoin’in ve Bitcoin ağının bugün yapamadıklarına odaklanmak yerine, bugün nelerin yapılabildiğini düşünün ve bunu 10 yıl önce neler yapılabildiğiyle karşılaştırın. Bu egzersizi internet için 1985’ten 1995’e kadar yapın, ardından sonraki 30 yılda internetin ne kadar hızlandığına ve hangi uygulamaların mümkün olduğuna bakın. Bu içgörüyle Bitcoin’in geleceğini hayal edin ve sadece 10 yıl sonra ya da hayal gücünüz yetiyorsa 30 yıl sonra nasıl görünebileceğini düşünün.



##### Bitcoin’i mevcut küresel para sistemiyle karşılaştırın

Bitcoin’in küresel para olmak için çok yavaş olduğu yönündeki temel iddia, yalnızca Bitcoin’in temel katmanıyla sınırlı kalırsak tartışmasız doğrudur. Mevcut para sistemlerimizin temel katmanı da benzer şekilde, özel bankalar ve Visa ile Mastercard gibi ödeme hizmetleri tarafından üzerine bir ödeme altyapısı inşa edilmemiş olsaydı, küresel para olmak için çok yavaştır. Mevcut sistemimiz katmanlar halinde inşa edilmiştir, bu yüzden geleceğin de benzer olmasını bekleyebiliriz. Güven, hız ve maliyet gibi bazı tasarım ödünleşimleri, farklı değer birimlerini taşımak için inşa edilmiş olsalar da, aynı çözümleri sunan sistemler arasında benzer şekilde aktarılabilir.

Bitcoin üzerindeki mevcut ikinci katmanlardan bazıları doğrudan hız sorununu ele alıyor, örneğin Liquid ve Lightning Network (daha fazla bilgi için bölüm 201.4’e bakınız). Liquid, Bitcoin blokzincirinden daha hızlı ve daha ucuzdur, Lightning Network ise Liquid’den bile daha hızlı ve daha ucuzdur. Farklı ödünleşimlere sahip çok sayıda ikinci katmanın ortaya çıkması beklenir ve bu sağlıklıdır.

Muhtemelen daha fazla ikinci ve üçüncü katman olacak ve bunları kullanan uygulamalarda bir patlama yaşanacak, tıpkı internetin evriminde olduğu gibi.



##### Motivasyon

Bu eleştiri dile getirildiğinde, eleştirmenin başka motivasyonları olup olmadığını düşünmekte fayda var. Örneğin, yeni veya farklı bir blokzincir projesi mi var? Bu, daha iyi bir İletim Kontrol Protokolü satmaya çalışmaya benzetilebilir.

Ölçeklenebilirlik ya da Blokzincir Üçlemi, ilk olarak Vitalik Buterin tarafından 2017’de ortaya atıldı. Buna göre, blokzincir tasarımında Merkeziyetsizlik, Güvenlik ve Ölçeklenebilirlik özellikleri arasında her zaman bir ödünleşim vardır. Bitcoin’in çok yavaş olduğunu ve birinci katman blokzincirinde daha hızlı bir çözüme sahip olduklarını iddia eden herkes, bunu başarmak için güvenlikten veya merkeziyetsizlikten bir miktar ödün verecektir. Diğer amaçlar için tasarlanmış bir blokzincirde böyle bir ödünleşim mantıklı olabilirken, küresel bir para için öncelik sırası şöyle olmalıdır:


> **Light**
>
> * **Merkeziyetsizlik**
>   * Güvenilir tarafların kaldırılmasını mümkün kılar
> * **Güvenlik**
>   * Kötü niyetli kişilerin işlemleri veya defteri kurcalamasını engeller
> * **Ölçeklenebilirlik**
>   * Sistemin kullanıcı ve hız açısından ekonomik olarak ölçeklenmesini sağlar


İlk iki özellik, üreticiler olmadan ihraç, aracı olmadan ödeme ve yönetici olmadan saklama ortamını oluşturur.

Bitcoin, hedeflenen kullanım alanı küresel para olduğundan, üç blokzincir tasarım özelliği arasında doğru ödünleşimi yapar ve ölçeklenebilirlik ile hız ödünleşimlerini katmanlar kullanarak hafifletir.

> Satoshi, dijital paranın bütünlüğünü güvenilir taraflara ihtiyaç duymadan nasıl koruyacağını keşfetti – üreticiye, aracıya veya yöneticiye gerek yok.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
