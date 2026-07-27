# 5.1 Bitcoin Nasıl Çalışır?

#### Nakamoto Konsensüs Mekanizması

Peki, Bitcoin nasıl çalışır? Bitcoin'in birçok özelliği vardır ve tavşan deliği oldukça derindir — hem de çok derin. Neyse ki, Bitcoin dünyasına ilk kez giriyorsanız, kullanmaya başlamak için nasıl çalıştığını mükemmel bir şekilde anlamak zorunda değilsiniz.

İnternet için de aynı şey geçerlidir: Çoğu insan TCP/IP protokolünün nasıl çalıştığını bilmez, yine de her gün e-posta ve mesaj gönderir, sosyal medyada içerik paylaşır. Bu, araba sürmek gibidir — çoğu insan bir arabanın tam olarak nasıl çalıştığını bilmez, ama nasıl sürüleceğini bilir.


> **Callout – Bitcoin henüz yaygın olarak benimsenmedi**
>
> Bitcoin henüz yaygın olarak benimsenmedi. Hâlâ oldukça yeni bir teknoloji, tıpkı 90'lı yıllarda internetin olduğu gibi. Bu nedenle, Bitcoin'in teknik yönlerinden ziyade temel prensiplerine odaklanmak faydalı olabilir.


Bitcoin'in nasıl çalıştığının arkasındaki temel fikir tek bir cümlede özetlenebilir: Bitcoin, tüm ağ katılımcılarının üzerinde anlaştığı ortak bir kurallar bütünüdür. Bunu, arkadaşlarınızla oynadığınız bir masa oyunu gibi düşünebilirsiniz. Monopoly gibi bir oyunda, diğer oyuncularla belirli kurallar üzerinde anlaşmış olursunuz. Monopoly'nin kurallarından biri, yalnızca özel “Monopoly paraları”nın kabul edilmesidir. Eğer Ahmet (oyunculardan biri) kurallara aykırı olarak Monopoly parası yerine tuvalet kağıdıyla ev almaya kalkarsa, diğer oyuncular Ahmet'e hile yaptığını söyler ve onunla oynamayı bırakır. Kısacası, oyunu oynamak için bir kurallar bütününde uzlaşmanız ve bu kurallardan sapmamayı kabul etmeniz gerekir, aksi takdirde reddedilirsiniz.

Bitcoin temelde böyle çalışır. Bitcoin, aynı kurallar bütününde anlaşan insanlardan oluşan bir ağdır. Bu kurallar matematiksel olarak belirlenmiş, bilgisayar koduyla yazılmıştır ve Bitcoin yazılımını çalıştıran herkes tarafından doğrudan kabul edilir. Bitcoin'in kuralları tüm katılımcılara eşit şekilde uygulanır, yani her oyuncu ya oyunun kurallarına uyar ya da ağa katılamaz çünkü ağ onları reddeder.

Örneğin, Bitcoin'in kurallarından biri "Toplamda asla 21 milyon adetten fazla bitcoin olmayacak" şeklindedir. Birisi kendisi için fazladan bir milyon bitcoin üretmeye kalkarsa, bunun ona hiçbir faydası olmaz çünkü otomatik olarak diğer herkes tarafından tespit edilip reddedilir. Bitcoin'i bu kadar sağlam yapan da budur.


> **Dark**
>
> Kim olduğunuzun veya nereden geldiğinizin bir önemi yok: Bitcoin dünyasına giriyorsanız, herkesle aynı kurallar bütününe uymak zorundasınız.


Bu durum, itibari para dünyasında orantısız etkiye sahip tüm kişi ve kuruluşlar için de geçerlidir. Bitcoin dünyasında hileye veya sabotaja yer yoktur — herkes eşit şekilde muamele görür ve bunu kimse değiştiremez.


> **Callout**
>
> Biliyor muydunuz, 2009'dan bu yana Bitcoin'e on binlerce saldırı, müdahale veya değiştirme girişimi oldu? Bitcoin, kimsenin onu durduramayacağını, kontrol edemeyeceğini veya manipüle edemeyeceğini sürekli olarak kanıtladı.


#### Oyunun Oyuncuları

Bitcoin'in merkeziyetsizliğini daha iyi anlamak için ağdaki farklı rollere daha yakından bakmamız gerekiyor. Bitcoin dünyasında, çeşitli katılımcılar farklı ama uyumlu roller üstlenir ve protokolün sorunsuz çalışmasına katkıda bulunur.

##### 1. Madenciler: Güvenliğin Mimarları

Madenciler, Bitcoin'in bel kemiğidir. Proof-of-Work (PoW) adı verilen bir mekanizma ile ağı korur ve sürdürürler.

Bu oyuncular, yüksek hesaplama gücüne sahip özel bilgisayarlarla donatılmıştır. Bu güçlerini Bitcoin ağına sunar, dünyanın dört bir yanında birbirleriyle yarışarak Bitcoin’in merkeziyetsiz defterine (blokzincir) yeni işlem blokları eklemek için rekabet ederler. Bu bağlılıkları, defterin değiştirilemezliğini sağlar ve kötü niyetli saldırılara karşı korur.

Madenciliğin merkeziyetsiz doğası, teoride herkesin katılabileceği anlamına gelir — ancak pratikte rekabet çok yoğundur. Katkılarının karşılığı olarak, bulmacayı ilk çözen madenciye yeni bitcoin şeklinde ödül verilir, buna blok ödülü denir.

Bitcoin madencileri dünyanın dört bir yanına dağılmıştır, bu da ağı merkezileşmeye karşı korur ve Bitcoin'in güvenliğinin güçlü ve dağınık kalmasını sağlar.

##### 2. Düğümler: Doğrulamanın Bekçileri

Bitcoin düğümleri, dünyanın dört bir yanındaki sıradan insanlar tarafından çalıştırılır. Bu katılımcılar, bilgisayarlarında Bitcoin yazılımını çalıştırarak tüm defterin bir kopyasını tutar ve Bitcoin ağının bekçileri olurlar. Düğümler işlemleri doğrular ve tüm katılımcıların konsensüs kurallarına uyduğundan emin olur.

Doğrulama sorumluluğunun düğümler ağına dağıtılması sayesinde, Bitcoin saldırılara karşı dayanıklı kalır ve güvene dayalı olmayan yapısını korur. Düğümler, defterin bütünlüğünü korumada kritik bir rol oynar ve Bitcoin'in merkeziyetsizlik anlayışına katkıda bulunur.

##### 3. Kullanıcılar: Güçlenmiş Katılımcılar

Kullanıcılar — Bitcoin ağının can damarı — işlemlere katılan bireylerdir. Kullanıcıları, hayatlarına Bitcoin'i entegre ederek kendilerini güçlendiren sıradan insanlar olarak düşünebilirsiniz. Örneğin, bazı kullanıcılar birikimlerini bitcoin olarak tutarken, bazıları ise market alışverişi yapmak ve maaş almak için para olarak kullanır.

Bitcoin, aracı kurumlara — bankalar ve hükümetler gibi — ihtiyaç duymadan, kullanıcıların doğrudan birbirleriyle işlem yapmasını sağlar. Bu da kullanıcıların paraları ve işlemleri üzerinde tam kontrol sahibi olmaları anlamına gelir.

##### 4. Geliştiriciler ve Projeler: Yeniliğin Mimarları

Geleceğin para sistemi kendiliğinden inşa edilmeyecek, etik açıdan doğru bir şekilde küresel olarak benimsenmesi de çaba gerektirir. İşte burada Bitcoin geliştiricileri ve projeleri devreye girer. Geliştiriciler, teknik uzmanlıklarını Bitcoin protokolünü geliştirmek ve yenilik yapmak için kullanır. Bu kişiler kod yazar, iyileştirmeler önerir ve güvenlik açıklarını giderir, böylece ağın her türlü zorluğa karşı evrilmesini sağlar. Bitcoin'in açık kaynak yapısı, dünyanın dört bir yanındaki geliştiricilerin katkıda bulunmasına olanak tanır.

Bu merkeziyetsiz geliştirme güzelliği, protokol üzerinde tek bir varlığın kontrolü ele geçirmesini engeller. Bu, konsensüs odaklı bir süreçle gerçekleşir. Geliştiriciler fikir ve değişiklikler önerir, ancak yalnızca en iyi fikirlere ve daha iyi bir dünya vizyonuna uyumlu olanlara topluluk destek verir; böylece Bitcoin, şeffaf ve demokratik bir şekilde 8 milyar insana ölçeklenirken evrilir.

Bitcoin projeleri, misyona odaklı sivil toplum kuruluşlarından şirketlere, değerli içerik üreten gruplardan bireylere kadar çeşitli toplulukları kapsar. Bu insanlar, daha büyük Bitcoin misyonu içinde kolektif özgürlük için belirli bir hedef veya odak üzerinde birlikte çalışır. Bitcoin projeleri, Bitcoin'in benimsenmesini şekillendirme ve teşvik etmede kritik bir rol oynar; insanlığın güçlenmesini ve özgürlüğünü önceliklendiren bir gelecek için çalışırlar.

#### Senfoni

Bitcoin'in merkeziyetsizliği, birlikte en güzel müziği yapan farklı müzisyenlerin uyum içinde olduğu bir orkestra gibi düşünülebilir. Bitcoin ağında bir patron yoktur: madenciler, düğümler, kullanıcılar, geliştiriciler ve projeler rollerini özerklik ve iş birliğiyle yerine getirir.

Düğümler tarafından tutulan merkeziyetsiz defter şeffaflığı garanti ederken, proof-of-work mekanizması madencilikte güvenlik ve merkezileşmeye karşı koruma sağlar; kullanıcılar, itibari para sisteminin kontrolünden bağımsız olarak finansal egemenlik ve güçlenme yaşar; geliştiriciler, konsensüsle yönlendirilerek protokolün insanlığın değişen ihtiyaçlarına uyum sağlamasını temin eder; Bitcoin projeleri ise kendi benzersiz yollarıyla kolektif özgürlük misyonuna katkıda bulunur.

Bu merkeziyetsiz orkestradaki her katılımcı, Bitcoin'in benimsenmesinde ve insanlığın güçlenmesinde hayati bir rol oynar; Bitcoin'in dayanıklılığına ve uzun ömürlülüğüne katkıda bulunur ve güvene dayalı olmayan, sınır tanımayan ve güçlendirici bir ekosistem yaratır.

![Networks](https://cdn.sanity.io/images/vje9ehw2/staging/ed2eea135d64a5245f37feea5a2a6ca3665cc6af-344x235.svg)


> **Callout – Özet**
>
> Bitcoin'deki merkeziyetsizlik senfonisi, Satoshi Nakamoto'nun vizyonunun ve özgürlük ile güçlenme arayışındaki küresel topluluğun büyük tutkusunun bir kanıtı olarak yankılanır.


#### Etkinlik: Konsensüs


https://qr.myfirstbitcoin.org/consensus.pdf

_Activity: Consensus_


Bu, katılımcıların tanımlı bir lider olmadan bir grupta eylemleri senkronize etmenin ne kadar zor olduğunu ilk elden öğrendiği bir sınıf etkinliğidir. Amaç, katılımcıların Bitcoin'de anlaşmanın (konsensüsün) nasıl sağlandığını anlamasıdır.

###### Temel Noktalar

1. **Konsensüs = uzlaşma**
1. Merkezi kontrolü olan bir grup ile olmayan bir grup arasındaki en büyük farklardan biri güven meselesidir. Eşler arası ağlar gibi merkeziyetsiz gruplarda lider yoktur ve katılımcılar birbirine güvenmez. Koordinasyon için farklı bir yol gerekir.
1. Eşler arası ağların geliştiricileri için bu, Bizans Generalleri Problemi olarak bilinir. Bitcoin bu zorluğu matematik ve proof-of-work madenciliğiyle çözer.
1. Bitcoin'in merkeziyetsiz olması, değerinin temelidir. Tarih boyunca, insan liderler uzun vadede parayı değersizleştirme cazibesine her zaman yenik düşmüştür.
1. Nakamoto Konsensüsü, Bitcoin'in yaratıcısı Satoshi Nakamoto'nun adını taşır. Bu konsensüs mekanizması, birbirine güvenmeyen binlerce yabancının 2009'dan beri Bitcoin defterini nasıl koruduğudur.
