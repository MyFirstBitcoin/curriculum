# 7.4 Lightning İşlemleri Gönderme ve Alma

Bir Lightning cüzdanı ile Bitcoin kullanmak hızlı, ucuz ve gizlidir; bu da iki kişi arasında işlem yapmayı kolaylaştırır. Günlük şeyler için, örneğin kahve almak gibi, bitcoin göndermek ve almak çok hızlıdır.

Lightning Ağı'nın nasıl çalıştığına dair birkaç örneğe bakalım.

###### Örnek 1

Hem Marcia hem de Ece'nin 5 birim parası var. Marcia, Ece'ye 2 birim göndermek istiyor. Ödeme, Lightning Ağı üzerinden ödemeyi ileten Cem aracılığıyla gidiyor. Ödeme tamamlandıktan sonra, Ece'nin 7 birimi ve Marcia'nın 3 birimi oluyor.

Cem, ödemenin yönlendirilmesine yardımcı olur, ancak fonları çalamaz. Lightning Ağı, yalnızca hedef alıcının ödemeyi alabilmesini sağlamak için kriptografi kullanır. Cem sadece ödemenin ağda ilerlemesine yardımcı olur.

Bu, Lightning Ağı'nın önemli bir avantajını gösterir: insanlar, bankalar gibi aracı kurumlara güvenmeden ödemeleri hızlıca gönderebilir.

Cem gibi düğüm operatörleri, ödemeleri yönlendirmeye yardımcı oldukları için küçük ücretler de kazanabilirler. Bunu yaparak, ağın merkeziyetsiz ve verimli kalmasına katkıda bulunurlar.

Normal Bitcoin işlemleriyle karşılaştırıldığında:

* **Zincir üstü işlemler** doğrudan Bitcoin blokzincirinde gerçekleşir. Çok güvenlidirler, ancak daha yavaş ve daha pahalı olabilirler.
* **Lightning işlemleri** zincir dışında gerçekleşir ve ödemelerin çok daha hızlı ve düşük maliyetle yapılmasını sağlar.

Bu nedenle Lightning, küçük ve günlük ödemeler için kullanışlıdır; zincir üstü işlemler ise genellikle daha büyük transferler veya uzun vadeli saklama için kullanılır.

###### Örnek 2

Mina dışarıda yemek yemeyi çok sever ve sık sık favori yerel kafesine uğrar. Birçok farklı ödeme seçeneği olduğu için hangisinin en iyi olduğundan emin değildir. Neyse ki, Bitcoin ve Lightning Ağı hakkında biraz bilgi edinmiştir. Seçeneklerini gözden geçirdikten sonra, Mina Lightning ödeme yönteminin en iyi seçenek olduğunu fark eder.

Mina bir kahve almak istiyor, ancak normal bir Bitcoin işlemiyle ödeme yapmak bazen zaman alabilir ve daha yüksek ücretler gerektirebilir. Bunun yerine Lightning Ağını kullanmaya karar verir.

Lightning Ağı, insanların bitcoin'i anında ve çok düşük ücretlerle göndermesine olanak tanır. Bu da onu kahve gibi küçük ve günlük alışverişler için ideal kılar.

Lightning kullanmaya başlamak için Mina, telefonuna bir Lightning cüzdanı indirir. Ardından, normal Bitcoin cüzdanından Lightning cüzdanına biraz bitcoin gönderir. Bu adım, blokzincir üzerinde normal bir Bitcoin işlemiyle gerçekleşir. Fonlar Lightning cüzdanına ulaştıktan sonra, Lightning Ağı'nda kullanılabilir.

Artık Mina, kafeye Lightning ile anında ödeme yapabilir. Ödeme, ana Bitcoin blokzinciri dışında gerçekleşir; bu nedenle, normal zincir üstü bir işleme göre çok daha hızlı ve ucuzdur.


| Faydalar | Lightning Ağı | Geleneksel Bankacılık Sistemi |
| --- | --- | --- |
| Hız | Hızlı | Yavaş |
| Şeffaflık | Şeffaf | Kapalı |
| Güvenlik | Güvenli | Savunmasız |
| İşlem ücretleri | Düşük | Yüksek |
| Finansal kapsayıcılık | Yüksek | Sınırlı |
| Ölçeklenebilirlik | Yüksek | Düşük |
| Gizlilik | Yüksek | Orta |
| Birlikte çalışabilirlik | Yüksek | Düşük |
| Yasal uyumluluk | Orta | Yüksek |
| Maliyet etkinliği | Yüksek | Orta |


Zincir üstü işlemler doğrudan Bitcoin blokzincirinde gerçekleşir ve daha fazla zaman ile ücret gerektirebilir. Lightning işlemleri ise zincir dışında gerçekleşir, böylece bitcoin kullanmaya devam ederek hızlı ve düşük maliyetli ödemeler yapılmasını sağlar.


| Visa, Inc. | Bitcoin Zincir Üstü | Lightning Ağı |
| --- | --- | --- |
| Saniyede 65.000 işlem kapasitesi. | Saniyede 7 işlem kapasitesi. | Saniyede milyonlarca işlem kapasitesi. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Bu, tüm Lightning Ağının bir haritasıdır. Binlerce Lightning düğüm operatörüne teşekkürler, dünyanın neresinde olursa olsun bir Bitcoin Lightning cüzdanına sahip herhangi bir kullanıcıya sats gönderebilirsiniz. Ödeme birkaç saniye içinde ulaşır ve sadece birkaç kuruşa mal olur.**Kendiniz deneyin!**

#### Etkinlik: Lightning Bayrak Yarışı

https://qr.myfirstbitcoin.org/lightning.pdf

**Bu, öğrencilerin Lightning Ağı'nı kullanarak gerçek sats gönderip aldığı uygulamalı bir egzersizdir.**

###### Temel Noktalar

1. Bir Lightning cüzdanı kullanmak, gerçek sats alıp göndermek konusunda kendinize güveninizi artıracaktır.
1. Birimlere dikkat edin. Bazı cüzdanlar kullanıcıların bitcoin VEYA sats (bir bitcoinin 1/100.000.000'i) göndermesine izin verir.
1. Lightning ödemeleri bazen, özellikle büyük ödemelerde, yönlendirme sırasında takılabilir. Bu mümkün olsa da, ağ olgunlaştıkça bu tür kullanıcı deneyimi giderek daha az yaygın hale geliyor.

###### Öğrenci İpucu

Kullandığınız Lightning cüzdanında mevcut zincir üstü Bitcoin işlem ücretlerinin nasıl/etkileyip etkilemediğini eğitmeninizle doğrulayın.
