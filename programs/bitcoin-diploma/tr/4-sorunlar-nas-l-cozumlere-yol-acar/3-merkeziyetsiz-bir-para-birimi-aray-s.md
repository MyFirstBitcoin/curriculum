# 4.3 Merkeziyetsiz Bir Para Birimi Arayışı

Tarih boyunca paranın bankalar ve hükümetler tarafından giderek ele geçirilmesine tanık olduk; bu da bugün bildiğimiz itibari para sistemine ve toplum için yıkıcı sonuçlara yol açtı. Ancak şifreleme ve internet gibi yeni teknolojilerin yükselişi, hükümet müdahalesinden bağımsız, herkese açık ve erişilebilir dijital para gibi yeni fikirlerin ortaya çıkmasına olanak tanıdı. Şimdi bu devrimci hareketin öncülerinin yolculuğuna bakalım: Cypherpunklar.

#### Cypherpunklar

> Bilgisayar, insanları kontrol etmek yerine onları özgürleştirmek ve korumak için bir araç olarak kullanılabilir.  
_Hal Finney_

20. yüzyılın ikinci yarısında kişisel bilgisayarlar ve internet gibi güçlü yeni teknolojiler ortaya çıktı. Bu yenilikler, insanların iletişim kurma, bilgi paylaşma ve toplumu organize etme biçimlerini değiştirmeye başladı.

Bazı düşünürler ve programcılar, bu teknolojilerin ya bireysel özgürlüğü artırabileceğini ya da hükümetlerin ve şirketlerin insanları daha kolay izleyip kontrol etmesine olanak tanıyabileceğini fark etti.

Bu grup Cypherpunklar olarak tanındı. Onlar, bilgiyi güvence altına almak için matematiksel kodların kullanıldığı şifrelemenin, dijital çağda bireysel özgürlüğü koruyabileceğine inanıyordu.

Cypherpunklar, çevrimiçi gizliliği koruyacak, iletişimi güvenli hale getirecek ve insanların internette merkezi otoritelere ihtiyaç duymadan etkileşimde bulunmasını sağlayacak araçlar üzerinde çalıştılar.

Onların temel hedeflerinden biri, insanların bankalar veya hükümetler tarafından kontrol edilmeden kullanabileceği bir dijital para biçimi yaratmaktı. Bitcoin daha sonra bu soruna bir çözüm olarak ortaya çıktı.


> **Definition – Orwellvari bir geleceğin tanımı**
>
> **Orwellvari gelecek**, güçlü bir otoritenin, genellikle hükümetin, insanların hayatlarını yakından kontrol ettiği bir distopik toplumu ifade eder. Böyle bir dünyada vatandaşlar sürekli izlenir, bilgiler manipüle edilir ve iktidardakilere karşı konuşmak cezalandırılabilir. Kişisel özgürlükler kısıtlanır ve gerçeğin çarpıtılması, nüfus üzerinde kontrolü sürdürmek için sıkça kullanılır.


Cypherpunk hareketinin önde gelen isimleri arasında Eric Hughes, Timothy C. May ve John Gilmore vardı. 1992 yılında Eric Hughes _Bir Cypherpunk Manifestosu_ yazdı ve insanların dijital yaşamları üzerinde gizlilik ve kontrol hakkına sahip olması gerektiğini savundu.

Cypherpunklar, şifrelemenin bireyleri çevrimiçi ortamda koruyabileceğine inanıyordu. 1991 yılında Phil Zimmermann, yalnızca alıcının okuyabileceği şekilde şifreli e-posta göndermeyi sağlayan PGP (Pretty Good Privacy) adlı aracı geliştirdi.

Onlar, şifrelemenin internet ve bilgisayarlarla birleştiğinde, insanların merkezi otoritelere ihtiyaç duymadan çevrimiçi iletişim kurup etkileşimde bulunmasını sağlayabileceğine inanıyordu.

Ancak büyük bir sorun hâlâ çözülmemişti: Dünya hâlâ insanların internette özgürce kullanabileceği merkeziyetsiz bir dijital para biriminden yoksundu.

#### Merkezi ve Merkeziyetsiz Sistemler

##### Merkezi Sistemler

Merkezi bir sistemde her şey, bir şehirdeki yüksek bir bina gibi tek bir ana otorite etrafında döner. Bu otorite, tüm sistemin nasıl çalıştığını kontrol eder. Geleneksel bankaları örnek olarak düşünebilirsiniz; burada küçük bir grup tüm kararları alır.

###### Merkezi Sistemlerin Sorunları

* **Tek bir arıza noktası**: Merkezi otoritede bir sorun olursa, tüm sistem çöker.
* **Kontrol**: Zirvedeki küçük bir grup tüm kontrol ve güce sahiptir; bu da genellikle herkesin değil, onların yararına kararlar alınmasına yol açar.
* **Verimsizlik ve aracı kurumlar**: Bir şehirdeki trafik sıkışıklığı gibi, merkezi sistemler gereksiz aracı kurumlar nedeniyle yavaş ve pahalı hale gelebilir.
* **Özerklik eksikliği**: İnsanlar kendi finansal kararlarını veremeyebilir; her şey üst otorite tarafından belirlenir.
* **Sansür ve kısıtlama**: Bir şehirde bazı bölgelerin kapatılması gibi, merkezi sistemler de bazı finansal kaynaklara erişimi engelleyebilir veya kısıtlayabilir.
* **Büyüme zorlukları**: Daha fazla insan finansal hizmetlere ihtiyaç duyduğunda, merkezi sistemler buna ayak uydurmakta zorlanabilir.
* **Güvenlik riskleri**: Merkezi otoritedeki sorunlar, tüm sistemi siber saldırılara karşı savunmasız bırakabilir.
* **Şeffaflık ve güven eksikliği**: Merkezi sistemlerin iç işleyişi anlaşılması zor olabilir; bu da insanların onlara güvenmesini güçleştirir.


> **Light**
>
> 2022 yılında Kanada'daki barışçıl protestolar sırasında, bankalar protestocuların hesaplarını dondurdu ve merkezi bir otoritenin finansal erişimi nasıl kontrol edebileceğini gösterdi.


##### Merkeziyetsiz Sistemler

Merkeziyetsiz bir sistemi bir orman gibi düşünün. Her ağaç ayrı bir parça, tüm orman ise sistemin kendisidir. Bir şehirdeki tek bir merkezden farklı olarak, merkeziyetsiz bir sistem daha dayanıklıdır ve bir parça bozulsa bile çalışmaya devam edebilir.

###### Merkeziyetsiz Sistemlerin Faydaları

* **Artırılmış dayanıklılık ve güvenilirlik**: Tek bir arıza noktası yoktur; bu da sistemin, sorunlar ortaya çıktığında bile güçlü kalmasını sağlar.
* **Artan güvenlik**: Doğru şifreleme/koruma ile merkeziyetsiz bir sistem, tek bir otoritenin kontrolüne karşı daha dirençlidir.
* **Daha fazla egemenlik**: İnsanlar paraları, verileri ve seçimleri üzerinde daha fazla kontrole sahiptir.
* **Gelişmiş şeffaflık**: Herkes aynı bilgiyi görür; bu da sistemi daha güvenilir kılar.
* **İzinsiz ve sınırsız**: Herkes katılabilir veya dahil olabilir.
* **Eşit fırsatlar**: Herkes katkıda bulunmak ve söz sahibi olmak için adil bir şansa sahiptir.
* **Gelişmiş Gizlilik**: Veriler birden fazla katılımcı arasında dağıtılır ve çoğunlukla takma adlarla kullanılır, bu da merkeziyetsiz sistemleri daha gizli kılar.

Merkeziyetsiz sistemlerin birçok avantajı olsa da, birlikte karar almak biraz zor olabilir. Herkesin birlikte çalışmasını gerektirir.

Merkezi ve merkeziyetsiz sistemlerin olduğu bir dünyada, her şey gücün kimde olduğuyla ilgilidir. Merkezi sistemler gücü küçük bir gruba verirken, merkeziyetsiz sistemler gücü dağıtarak herkesin söz sahibi olmasını sağlar. Bu güç değişimi, hayatlarını şekillendiren sistem üzerinde birçok insanın etkili olduğu daha adil bir gelecek anlamına gelir.


> **Light**
>
> Tor Ağı, insanların çevrimiçi olarak anonim kalabildiği ve ağın durdurulmasının veya sansürlenmesinin zor olduğu merkeziyetsiz bir sistem oluşturur.


#### Dijital Paraların Kısa Tarihi

Cypherpunklar tarafından tartışılan ana fikirlerden biri **dijital para** idi. Onlar, paranın devlet kontrolünden ayrılması gerektiğine ve insanların ödemeleri çevrimiçi olarak özgürce ve gizli bir şekilde gönderebilmesi ve alabilmesi gerektiğine inanıyordu.

Erken dönem kriptograf **David Chaum**, işlemleri güvenli ve gizli hale getirmek için kriptografi kullanan ilk dijital para sistemlerinden birini oluşturdu. Ancak, onun sistemi hâlâ bir **merkezi otoriteye** dayanıyordu, bu da sistemin başarısız olabileceği veya işlemleri sansürleyebileceği anlamına geliyordu.

Sonraki on yıllarda, birçok Cypherpunk merkezi bir otoriteye bağlı olmayan bir dijital para tasarlamaya çalıştı. Önemli yenilikler getirmiş olsalar da, hiçbir sistemleri güvenli, merkeziyetsiz ve yaygın olarak kullanılabilir bir dijital para için gereken tüm zorlukları çözemedi.

Bu girişimler eksik olanı ortaya çıkardı. Daha sonra birisi bu fikirlerin üzerine inşa ederek nihayet merkeziyetsiz dijital para için çalışan bir sistem yarattı.

###### Kaynaklar


[▶ Bu videoyu izle ve Cypherpunkların hikayesini keşfet!](https://www.youtube.com/watch?v=9vM0oIEhMag)
