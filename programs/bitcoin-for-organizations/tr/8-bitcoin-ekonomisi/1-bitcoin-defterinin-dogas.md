# 8.1 Bitcoin Defterinin Doğası

Bitcoin’in işlem defteri (alternatif olarak zaman zinciri veya blokzincir olarak da adlandırılır), ağda şimdiye kadar gerçekleşmiş her geçerli işlemin herkese açık, zaman damgalı bir kaydıdır. Geleneksel finansal sistemde, dahili işlemler yalnızca bankalar, düzenleyiciler veya SWIFT, BACS ya da SEPA gibi veri operatörleri gibi yetkili katılımcılar tarafından görülebilir. Geleneksel sistemlerde ödeme verilerine erişim oldukça kısıtlı ve pahalı olabilir.

Buna karşılık, Bitcoin ağında internet bağlantısı olan herkes, en büyük değer transferinden tek bir Satoshi’ye kadar her işlemi görebilir. Katılımcılar, bitcoin’in toplam arzını gerçek zamanlı olarak takip edebilir, adres ve cüzdan hareketlerini izleyebilir, madenci ödüllerini ve ücret davranışlarını görebilir. Defterde görülebilen hareketler, bireysel kimliklere değil, açık anahtar adreslerine bağlı olsa da, harcama davranışları üzerine büyük veri setleri birleştirilebilir; bu da herkesin ekonomik faaliyetleri gerçek zamanlı olarak derlemesine ve araştırmasına olanak tanır. Ağ büyüdükçe ve ekonomik gerçeklerin kaynağı olarak daha fazla kabul gördükçe, harcama davranışlarıyla ilgili istatistiksel analizlerin ve raporların üretilmesinde devlet kurumlarına ve üçüncü taraf sağlayıcılara olan bağımlılığın azaldığını görebiliriz.



#### 8.1.1 Node’lar ve Blok Gezgini

Bitcoin defterini bağımsız olarak doğrulamak ve verilerine erişmek isteyen herkes tam node çalıştırmalıdır. Tam node, Bitcoin ekonomisine katılmanın ve onu doğrulamanın en temel yolu olarak tanımlanır. Ocak 2009’da yayımlanan ‘Genesis Block’tan bugüne kadar tüm Bitcoin defterini indirip doğrulayan açık kaynaklı bir yazılım olarak dünya çapında kullanılabilir. Ayrıca, deftere eklenen yeni işlemleri doğrulamaya yardımcı olarak Bitcoin ağının güvenliğini destekler. Bitcoin defterine bu şekilde erişildiğinde, tam node araştırmacılar ve denetçiler için bir gerçeklik kaynağı görevi görür. Ve Bitcoin kullanıcıları için tam node, Bitcoin ekonomisinin işlem bilgilerine ‘kendi egemenliğinde’ bir kapı işlevi görür; çünkü üçüncü taraf hizmetlere olan bağımlılığı ortadan kaldırarak gizliliği ve güvenliği artırır.

Tam node’lar ham verileri indirirken, mempool.space veya blockstream.info gibi blok gezginleri defter hareketlerini aramak ve yorumlamak için görsel bir arayüz sunar. Blok gezgini, bireysel işlemlerin izlenmesine, cüzdan bakiyelerinin ve geçmişlerinin görüntülenmesine olanak tanır. Ayrıca, blok ödülleri ve işlem ücreti verileri gibi madenci faaliyet metriklerini de gösterir.

Birlikte, tam node’lar ve blok gezginleri, Bitcoin ağının şeffaflığını kullanılabilir kılan araçlardır.



#### 8.1.2 Etkinlik: Bitcoin Defterini Keşfetmek

1. Aç [mempool.space](https://mempool.space) ve ana sayfayı keşfet.
  * En son blok yüksekliği nedir?
  * Mevcut işlem ücreti nedir? (Düşük, Orta ve Yüksek Öncelik)
  * Bir sonraki blok için mempool’da kaç işlem bekliyor?
1. Defterdeki en son bloğa eriş.
  * Kaç işlem dahil edildi?
  * Blokun madencisinin adı nedir?
  * Blok ödülü neydi?
1. Bloktaki bir işleme eriş.
  * İşlemin kaç girdi ve çıktısı var?
  * İşlem değeri BTC ve USD cinsinden nedir?

Paranın geleneksel sistemde nasıl hareket ettiğinden ve bir işletme veya devletin bu tür bir şeffaflığı nasıl kullandığından farkları tartışın.
