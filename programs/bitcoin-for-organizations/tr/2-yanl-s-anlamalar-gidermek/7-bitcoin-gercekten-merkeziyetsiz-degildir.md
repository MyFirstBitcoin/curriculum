# 2.7 Bitcoin gerçekten merkeziyetsiz değildir.

> Kriptonun karmaşıklığı, sistemdeki güç ve yönetimi dağıtarak merkeziyetsizleşme çabalarından kaynaklanır—teorik olarak, finansal kurumlar gibi güvenilir aracıların gerekliliği ortadan kalkar. Bu, ilk Bitcoin teknik dokümanının temeliydi; öyle ki, ödemelerin herhangi bir finansal kurum veya başka bir güvenilir aracı dahil olmadan gönderilmesine olanak tanıyan kriptografik bir çözüm sundu. Ancak, Bitcoin çok hızlı bir şekilde merkezileşti ve şu anda işlevini sürdürebilmek için küçük bir yazılım geliştirici ve madencilik havuzu grubuna bağımlı hale geldi.  
_Uluslararası Para Fonu_

Yukarıdaki alıntıda da görüldüğü gibi, Uluslararası Para Fonu'nun oldukça yakın tarihli bir paylaşımında, ana akım finans sektörü Bitcoin'in merkeziyetsiz olmadığını iddia etmeye devam ediyor ve Bitcoin'i diğer kripto varlıklarla karıştırıyor.

##### Giriş

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/bf49c8e6ee0ffe5f1d13bb296426d0a77039def3-161x167.svg)

Merkeziyetsizlik, Bitcoin'in kritik bir yönüdür. Kıtlık ve dağıtım gibi protokol kurallarının merkezi bir otorite olmadan korunabilmesi, Bitcoin'in küresel toplum için izinsiz bir para olarak işlev görebilmesini sağlar.

Satoshi'nin çevrimiçi yazışmalarında belirttiği gibi, BitTorrent gibi merkeziyetsiz hizmetler, hükümet baskılarına karşı 'kendi başlarına ayakta duruyordu'; bu, sahibi belli olan ve merkezi sunucuları olan hizmetlerle karşılaştırıldığında önemli bir farktı. Satoshi, hükümetlerin veya başka çıkar gruplarının Bitcoin'i kapatması ya da olumsuz etkilemesi riskinden açıkça endişe duyuyordu.

Bu bağlamda, merkeziyetsizliğini şu alanlarda inceliyoruz:

* Protokolü çalıştıran kodun geliştirilmesi ve yönetimi; kuralları kim değiştirebilir?
* Kurallara uygun olarak yeni bloklar oluşturan ve çifte harcamaya karşı doğrulama yapan madencilik işlevi
* İşlemlerin geçerliliğini doğrulayan ve blokzincirin bir kopyasını tutan düğümler

##### Geliştiriciler

Bitcoin, herkesin inceleyebileceği, indirebileceği, kopyalayabileceği veya değişiklik önerebileceği açık kaynaklı bir protokoldür. 2009 yılında Satoshi Nakamoto tarafından başlatılan kaynak kodu, bir GitHub kütüphanesinde mevcuttur. Herkes kodu indirip bir düğüm çalıştırabilir; çoğunluk, zaman içinde güncellenen orijinal Bitcoin Core yazılımını kullanır.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Kaynak: https://river.com/learn/what-is-bitcoin-core/_

Bitcoin Core geliştirme süreci, açık kaynak geliştirme en iyi uygulamalarını takip eder. Her an, kod değişiklikleri yazan veya gözden geçiren birçok geliştirici olabilir. Kritik bir kod değişikliği yapılmadan önce, düğüm operatörlerinin, madencilerin ve kullanıcıların endişelerini dinlemeleri gerekir; bu değişiklikler yukarıdaki akış şemasında gösterildiği gibi gözden geçirilir ve üzerinde anlaşmaya varılır, ardından koda dahil edilir.

Bitcoin'in kuralları, her düğümde çalışan bu Bitcoin Core yazılımında kodlanmıştır. Herkes kurallarda değişiklik önerebilir – kurallar koddur, ancak sadece_sadece_ kod değil, aynı zamanda _üzerinde anlaşılmış_ koddur. Eğer tek taraflı olarak değiştirilirse, yeni kod artık konsensüsün bir parçası olmaz ve Bitcoin'in de bir parçası olmaz. Bitcoin'de bir şeyi değiştirip konsensüste kalmak zordur. Koda önerilen değişiklikler üç kategoriye ayrılır:

* Mevcut kurallar dahilinde: Yazım hataları, daha iyi bir arayüz veya veri yönetimi gibi küçük güncellemeler bu kategoriye girer ve onay almak görece kolaydır.
* Kurallara kısıtlama getiren yeni bir kural eklemek – örneğin blok boyutunu küçültmek. Buna 'yumuşak çatallanma' (soft fork) denir. Kod değişikliğini uygulamayan ve eski sürümde kalan düğümler yine de ağa katılmaya devam edebilir.
* Mevcut kuralları bozan yeni bir kural eklemek, örneğin blok boyutunu artırmak. Yeni koda geçmeyen düğümler, daha büyük boyutta oluşturulan bir bloğu geçersiz olarak reddeder. Buna 'sert çatallanma' (hard fork) denir ve orijinal ve yeni kodu çalıştıran düğümler arasında zincir bölünmesine ve yeni bir coin oluşmasına yol açar. Bu daha önce yaşanmıştır, ancak yeni coin için uzun vadeli bir başarıya yol açmamıştır; çünkü düğümlerin çoğu orijinal kodda kalmaya karar vermiştir.

Bu nedenle, tek bir kişi veya grup, konsensüs anlaşması olmadan Bitcoin kodunu tek taraflı olarak değiştiremez; aksi takdirde bir zincir bölünmesi ve farklı kurallarla yeni bir coin oluşması riskiyle karşı karşıya kalır.

##### Madencilik

Madencilik işlevi, ağdaki diğer düğümler gibi işlemleri doğrular, ancak ardından kodda yer alan konsensüs kurallarına uygun yeni bir blok oluşturmak için gerekli enerjiyi harcar. Başarı, madenciye işlem ücretleri ve Bitcoin ödülleri (yazım sırasında blok başına 3,125 coin) şeklinde ödül kazandırır.

Madencilik genellikle, blok madenciliğinde başarı şansını artırmak ve ödülleri paylaşmak için madencilik gücünün veya hash oranının birleştirildiği 'madencilik havuzları' tarafından yapılır. Bu madencilik havuzlarından birinin veya birkaçının birleşerek madencilikte %51'lik bir hakimiyet elde etmesi ve ağı kendi lehlerine çift harcama yapmak için geçersiz kılması tehlikesi vardır. Bunu başarmak için çok büyük kaynaklar gerekir ve bireysel madenciler istedikleri zaman kolayca başka bir madencilik havuzuna geçebilirler. Böyle bir saldırı, ağ bütünlüğünün bozulduğu açıkça görüleceğinden, bitcoin'in değerinin de muhtemelen çökmesine yol açar. Bu nedenle saldırgan, elde ettiği bitcoin'i değer kaybetmeden önce hızla itibari paraya çevirmek zorunda kalır. Bu da saldırının uzun süre sürdürülmesini daha da zorlaştırır ve bu nedenle bir madenci veya havuz operatörü için kurallara uymak ve geçerli bloklar çıkarmaya çalışmak daha kârlı olur.

Madencilik işlevinin coğrafi olarak dağılmış olması da önemlidir; örneğin, hükümetlerin madencilik kapasitesini ele geçirmesini veya kapatmasını önler. Örneğin, Çin'in yakın zamanda getirdiği madencilik yasağı, Bitcoin'in böyle bir hükümet müdahalesine uyum sağlayıp hayatta kalabildiğini, hash gücündeki kayıptan sonra hızla toparlanabildiğini gösterdi.

##### Düğümler

Yeni blokları madencilik yarışında etkili bir şekilde çıkarmak için önemli bir finansal yatırım gerektiren madenciliğin veya kodlama uzmanlığı gerektiren kod geliştirme sürecinin aksine, bir düğüm çalıştırmak, Bitcoin'in merkeziyetsizliğini korumaya yardımcı olmak isteyen herkesin yapabileceği bir şeydir.

Düğümler, Bitcoin Core yazılımını çalıştırır ve kodda yer alan kuralları uygular; böylece madencilerin, örneğin kendilerine izin verilenden daha fazla blok ödülü vermesini engellerler. Ayrıca, Bitcoin'in kıtlığını korumak için kritik olan 21 milyonluk arz sınırını da uygularlar. Herhangi bir hükümetin veya kötü niyetli aktörün Bitcoin'i durdurabilmesi için, şu anda dünya genelinde binlerce düğümde çalışan blokzincirin her bir kopyasını yok etmesi gerekir ki bu neredeyse imkansızdır.

##### İnsanlar

Potansiyel merkezileşmenin bir diğer yönü de insanlardır. Diğer tüm 'alt-coin'lerde bir lider figür vardır—bu kişi, Bitcoin'in çıkarına olmayan değişiklikleri savunmaya zorlanabilir. Satoshi Nakamoto, Bitcoin'in başarı yolunda olduğundan emin olana kadar ortalıkta kaldı ve ardından tamamen ortadan kaybolarak yazılımı geliştirmek ve uyarlamak için başkalarına bıraktı.

Peki ya büyük miktarda Bitcoin tutanlar? Erken yatırımcılar, coinlerini kaybetmeden tutanlar şu anda son derece zengin olmuşlardır. Ancak, bu durumun böyle olması onların sistem üzerinde başkalarına göre daha fazla etkisi olduğu anlamına gelmez; 'proof of stake' coinlerinde ise, o coinin ilk sahipleri ve hali hazırda zengin olanlar, karar alma ve gelecekteki coinlerin dağıtımında avantaj elde ederler. Bu, zamanla kaçınılmaz olarak merkezileşmeye yol açmıştır veya açacaktır.

##### Sonuç

Merkeziyetsizliğin azaltmaya çalışabileceği potansiyel tehditler nelerdir?

* Hükümetin Bitcoin'i kapatması veya yasaklaması
* Bitcoin'de bir çıkar grubunu kayıran, istenmeyen kod değişiklikleri; örneğin blok ödülünün artırılması
* Protokolün hükümet veya kötü niyetli aktörler tarafından yönlendirilerek protokolün gidişatının etkilenmesi
* Bir madenci havuzunun ağı ele geçirip Bitcoin'i 'çifte harcama' yapabilmesi – %51 saldırısı

Görüldüğü gibi, düğümlerin, kod geliştiricilerinin ve madencilerin birleşimi ile 'iş ispatı' mekanizmasının kullanılması, Bitcoin'i bu potansiyel tehditlerin büyük bir endişe kaynağı olarak görülmeyeceği kadar yeterli düzeyde merkeziyetsizleştirir. Topluluk, bunun böyle kalmasını sağlamak için durumu izlemeye devam etmelidir.
