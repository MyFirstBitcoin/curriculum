# 2.4 Bitcoin'da hiçbir yenilik olmuyor.

> Binlerce ormanın yaratılması bir meşe palamudunda gizlidir.  
_Ralph Waldo Emerson_

Eleştirmenler, Bitcoin'in temel katman protokolünü rakip blokzincirler kadar sık değiştirmediği için 'eski' veya 'ölü' bir teknoloji olduğunu iddia etmeye çalışırlar. Bu iddia, Bitcoin'de değişikliklerin neden yavaşça benimsendiğini ve Lightning Network gibi üst katmanlarda ağı ölçeklendirmek için gerçekleşen yenilik miktarını göz ardı eder. Ayrıca, en esnek ve dayanıklı teknolojilerimizin çoğunun da temel katmanda hızlıca ölçeklenmediğini görmezden gelir.

Örneğin, internetin temelini oluşturan İletim Kontrol Protokolü'nde (TCP) de herhangi bir yenilik yapılmıyor. TCP ilk olarak 1974'te oluşturuldu. TCP'nin son güncellemesi 1982'de yapıldı. Yapması gerekeni yapıyor. Mükemmel değil ve gelecekteki internet gelişmelerini desteklemek için IPv4'ün yükseltilmesi gerekip gerekmediği konusunda tartışmalar var. Ancak, 1982'den bu yana internette hiç yenilik olmadığını söylemek dikkate değer bir iddia olurdu. Tüm bu yenilikler TCP'nin 'içinde' değil, 'üzerinde' gerçekleşti.

Gerçekleşen yeniliklerin büyük çoğunluğu Bitcoin'in 'içinde' değil, 'üzerinde' oluyor. Bir gün muhtemelen Bitcoin'in 'içinde' hiç yenilik olmayacak ve bu bir eleştiri değil, ulaşılması gereken bir hedef olmalı; çünkü bu, küresel ekonomiyi desteklemede ne kadar temel bir unsur haline geldiğinin bir yansıması olacak: küresel, tarafsız ve izinsiz sağlam paranın temellerini sağlayarak. Para, hem ekonomik anlamda sabit arzı ve değiştirilemez defteriyle sağlamdır, hem de teknolojik olarak değişmediği ve yıllarca kesintisiz çalıştığı için sağlamdır. Bitcoin son 10 yılda zaten %100 çalışma süresi elde etti.

Ancak, Bitcoin'in 'üzerinde' hiç yenilik olmaması endişe verici olurdu. Son 10 yıla bir göz atalım:



#### 'Bitcoin'in İçinde'

Segregated Witness (SegWit), 2017 yılında işlem değiştirilebilirliğine karşı koruma sağlamak ve blok kapasitesini artırmak için uygulandı. SegWit ayrıca lightning ve bazı yan zincirlerin verimli çalışabilmesi için gerekli bir ön koşuldu.

Taproot, 2021 yılında birden fazla imzanın toplu olarak işlenip doğrulanmasını sağlamak için Schnorr imzalarını entegre ederek uygulandı; daha karmaşık işlevsellik için bir betik dili tanıttı ve işlemlerin gizliliğini ve sansür direncini artırdı.



#### 'Bitcoin'in Üzerinde'

##### Liquid Yan Zinciri

Liquid yan zinciri 2018 yılında uygulandı. Liquid, diğer yan zincirler gibi, ana Bitcoin blokzincirine önceden tanımlanmış bir dizi kurala göre bağlı olan ayrı bir blokzincir defteridir. Bu kurallar, Liquid zincirinin zaman içinde tasarım ve ölçeklenebilirlik iyileştirmeleri geliştirmesine ve entegre etmesine yetecek kadar esnektir. Ancak, Bitcoin blokzincirine olan bağlantı, bitcoin'in toplam 21 milyonluk arz sınırının her iki zincirde de tutarlı olmasını sağlar.

Liquid'deki varlık, L-BTC, ana zincirdeki bitcoin'e iki yönlü sabitlenmiştir. L-BTC'yi bazı uygulamalar için ideal kılan maliyet, hız, gizlilik ve güvenlik arasında bazı ödünleşmeler vardır. L-BTC ile maliyet, hız ve gizlilik artarken, Liquid Federasyonu'nu oluşturan kuruluşlara bir miktar güven duyulması gerekir; bu kuruluşlar, L-BTC'yi bitcoin'e ve tersi yönde çevirmek için 15 imzadan 11'inin gerektiği çoklu imza sürecini kontrol ederler.

##### Lightning Ağı

Lightning ağı 2018 yılında uygulandı. Lightning, kanallar aracılığıyla birbirine bağlı düğümlerden oluşan bir grafik şeklinde eşler arası bir ödeme ağı olarak tasarlanmıştır; bir blokzincir değildir. Bitcoin, Lightning Ağı'nda kullanılabilir hale getirmek için ana blokzincirde bir düğüm çalıştırıcısı tarafından kilitlenir; bu, yalnızca 'gerçek' bitcoin'in kullanıldığını garanti eder. Düğümler daha sonra birbirleriyle çoklu imza akıllı sözleşmeleri aracılığıyla likidite kanalları açabilirler. Ödemeler, ağda kaynaktan hedefe doğru, her düğüm adımında yeterli likidite olması şartıyla maliyet açısından optimize edilerek yönlendirilir. Lightning Ağı, güvenlikte bir kayıp (veya artan güven gereksinimi) ve karmaşıklıkta artış karşılığında maliyet, hız ve gizlilikte büyük iyileşmeler sağlar. Ancak, günlük yüksek hacimli, düşük değerli ödemeler için tasarlanmıştır; bu nedenle milyonlarca günlük işlem için bu ödünleşme oldukça makul kabul edilir (kaynak: River, 2023).

##### Chaumian eCash Mint'leri

Fedimint'ler, toplulukla sınırlı bir lightning ağı olarak düşünülebilir. Belirli topluluklar (ör. aileler, köyler, arkadaş grupları) içinde var olan doğal güveni kullanmak için tasarlanmışlardır; bunun karşılığında kullanıcılar için karmaşıklığı azaltır ve gizliliği artırır. Topluluk bağlamında bitcoin saklamak ve transfer etmek için modüler, açık kaynaklı protokollerdir. Lightning Ağı ile birlikte çalışabilirler.

**Cashu** bir mobil telefon gibi bir cihazda saklanabilen bir hamiline yazılı jetondur; tasarımı, fiziksel nakit paranın avantajlarını dijital ortamda yeniden üretmeyi amaçlar. Cashu, Bitcoin üzerinde inşa edilmiş bir Chaumian eCash örneğidir ve gizliliği ile sansür direncini artırır, karmaşıklığı azaltır; bunun karşılığında kullanılan eCash mint'ine güven duyulması gerekir. Cashu mint'leri, kullanıcıların kimliğini açıklamadan harcayabileceği, bitcoin'i temsil eden eCash jetonları çıkarır. Cashu, Lightning Ağı ile birlikte çalışabilir.

Gelecekte muhtemelen çok daha fazla katman 2 uygulaması inşa edilecek ve bunların her birinin üzerinde de birçok katman 3 uygulaması geliştirilecektir.

Lightning üzerinde inşa edilen inanılmaz sayıdaki uygulamaya bir örnek olarak, işte River tarafından hazırlanan bir Lightning Network Araştırma Raporu'ndan bir alıntı.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
