# 2.7 A Bitcoin nem igazán decentralizált.

> A kriptovaluták összetettsége a decentralizációs törekvésekből fakad – azáltal, hogy a rendszerben a hatalmat és az irányítást elosztják, elméletileg nincs szükség megbízható közvetítőkre, például pénzügyi intézményekre. Ez volt az eredeti Bitcoin white paper alapgondolata is, amely egy kriptográfiai megoldást kínált arra, hogy a fizetések pénzügyi intézmény vagy más megbízható közvetítő bevonása nélkül történhessenek. Azonban a Bitcoin nagyon gyorsan centralizálódott, és ma már egy kis csoportnyi szoftverfejlesztőre és bányász poolra támaszkodik a működéshez.  
_Nemzetközi Valutaalap_

Ahogy a fenti idézet is mutatja a Nemzetközi Valutaalap egyik viszonylag friss bejegyzéséből, a hagyományos pénzügyi ipar továbbra is azt állítja, hogy a Bitcoin nem decentralizált, valamint összekeveri a Bitcoint más kriptoeszközökkel.

##### Bevezetés

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/c47ad3f526d9de1ae73647247e966494ae25364a-161x167.svg)

A decentralizáció a Bitcoin egyik kulcsfontosságú jellemzője. Az a képesség, hogy a protokoll szabályait – például a szűkösséget és az elosztást – központi hatóság nélkül fenntartsa, biztosítja, hogy engedélyköteles pénz helyett engedély nélküli pénzként működhessen egy globális társadalomban.

Ahogy Satoshi az online levelezésében megjegyezte, a decentralizált szolgáltatások, mint például a BitTorrent, „megállják a helyüket” a kormányzati fellépésekkel szemben, szemben azokkal a szolgáltatásokkal, amelyeknek azonosítható tulajdonosa(i) és központosított szerverei vannak. Nyilvánvalóan aggódott amiatt, hogy a kormányok vagy más érdekcsoportok leállíthatják vagy más módon hátrányosan befolyásolhatják a Bitcoint.

Ebben az összefüggésben a következők decentralizációja érdekel minket:

* A protokollt futtató kód fejlesztése és kezelése; ki változtathatja meg a szabályokat?
* A bányászati funkció, amely az új blokkokat a szabályoknak megfelelően hozza létre, és ellenőrzi a dupla költés elleni védelmet
* A node-ok, amelyek ellenőrzik a tranzakciók érvényességét, és másolatot tartanak a blokkláncról

##### Fejlesztők

A Bitcoin egy nyílt forráskódú protokoll, amelyet bárki szabadon megtekinthet, letölthet, lemásolhat vagy javaslatot tehet a módosítására. Elérhető egy GitHub könyvtárban, a forráskódot eredetileg 2009-ben Satoshi Nakamoto tette közzé. Bárki letöltheti a kódot és futtathat egy node-ot, amelyek többsége az eredeti Bitcoin Core szoftvert futtatja, amelyet az idők során frissítettek.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Forrás: https://river.com/learn/what-is-bitcoin-core/_

A Bitcoin Core fejlesztése a nyílt forráskódú fejlesztés legjobb gyakorlatait követi. Bármikor bármennyi fejlesztő írhat vagy ellenőrizhet kódmódosításokat. Nekik figyelembe kell venniük a node üzemeltetők, bányászok és a felhasználói bázis véleményét, mielőtt bármilyen kritikus változtatást hajtanának végre a kódban, amelyet a fenti folyamatábra szerint felülvizsgálnak és hagynak jóvá, mielőtt bekerülne a kódba.

A Bitcoin szabályai ebben a Bitcoin Core szoftverben vannak kódolva, amely minden node-on fut. Bárki javasolhat változtatást a szabályokon – a szabályok kódok, de nem_csak_kódok, hanem_közösen elfogadott_kódok. Ha egyoldalúan változtatják meg őket, az új kód már nem része a konszenzusnak, és nem része a Bitcoinnak. Valamit megváltoztatni a Bitcoinban és a konszenzusban maradni nehéz feladat. A kódra javasolt változtatások három kategóriába sorolhatók:

* A meglévő szabályokon belül: kisebb frissítések, mint például helyesírási hibák javítása, szebb felhasználói felület vagy adatkezelés, ebbe a kategóriába tartozhatnak, és viszonylag egyszerűen jóváhagyhatók.
* Új szabály hozzáadása, amely korlátozásokat vezet be – például a blokkméret csökkentése. Ezt „soft fork”-nak nevezik. Azok a node-ok, amelyek nem vezetik be a kódváltozást, és a régi verzión maradnak, továbbra is részt vehetnek a hálózatban.
* Új szabály hozzáadása, amely megsérti a jelenlegi szabályokat, például a blokkméret növelése. Azok a node-ok, amelyek nem frissítenek az új kódra, érvénytelennek tekintik a nagyobb méretű blokkokat. Ezt „hard fork”-nak nevezik, és lánchasadást eredményez a régi és az új kódot futtató node-ok között, valamint új érmét hoz létre. Ez már megtörtént korábban, de hosszú távon az új érme nem járt sikerrel, mivel a node-ok többsége az eredeti kód mellett döntött.

Ezért egyetlen fél vagy csoport sem tudja egyoldalúan megváltoztatni a Bitcoin kódját konszenzusos megállapodás nélkül, különben lánchasadást és egy új, más szabályokat követő érme létrejöttét kockáztatják.

##### Bányászat

A bányászati funkció ugyanúgy ellenőrzi a tranzakciókat, mint bármely más node a hálózaton, de ezután energiát fordít arra, hogy új blokkot hozzon létre, amely megfelel a kódban rögzített konszenzusos szabályoknak. A sikeres bányász jutalma a tranzakciós díjakból és Bitcoin jutalomból áll (a cikk írásakor 3,125 érme blokkonként).

A bányászatot általában bányász poolok végzik, ahol az emberek egyesítik a bányászati teljesítményüket vagy hash rate-jüket, hogy növeljék az esélyüket egy blokk sikeres kibányászására és a jutalom megosztására. Fennáll a veszélye annak, hogy egy vagy több ilyen bányász pool összefog, és eléri az 51%-os dominanciát a bányászatban, így lényegében a saját javukra írhatják felül a hálózati érvényesítési protokollt, hogy kétszer költsenek érméket. Ehhez azonban hatalmas erőforrásokra lenne szükség, óriási költséggel, és az egyes bányászok bármikor könnyen átléphetnek másik poolba. Egy ilyen támadás valószínűleg a bitcoin értékének összeomlásához vezetne, mivel nyilvánvalóvá válna, hogy a hálózat integritása sérült. A támadónak ezért gyorsan fiat pénzre kellene váltania a megszerzett bitcoint, mielőtt az értéke csökken. Ez még nehezebbé tenné a támadás hosszú távú fenntartását, ezért egy bányász vagy pool üzemeltető számára jövedelmezőbb a szabályok betartása és érvényes blokkok bányászata.

A bányászati funkció földrajzi eloszlása is fontos, hogy például a kormányok ne vehessék át a bányászati kapacitást, vagy ne állíthassák le azt. Például Kína közelmúltbeli bányászati tilalma megmutatta, hogy a Bitcoin képes alkalmazkodni és túlélni az ilyen kormányzati beavatkozásokat, gyorsan alkalmazkodva és helyreállva a hash power kieséséből.

##### Node-ok

A bányászattal ellentétben, amely jelentős pénzügyi befektetést igényel ahhoz, hogy valaki hatékonyan versenyezhessen az új blokkok kibányászásáért, vagy a kódfejlesztéssel, amely programozói szakértelmet kíván, egy node futtatása bárki számára elérhető, aki szeretné segíteni a Bitcoin decentralizációjának fenntartását.

A node-ok a Bitcoin Core szoftvert futtatják, és érvényesítik a kódban szereplő szabályokat, hogy a bányászok ne csalhassanak, például ne oszthassanak ki maguknak a megengedettnél nagyobb blokk jutalmat. Emellett érvényesítik a 21 milliós kínálati korlátot is, amely kulcsfontosságú a Bitcoin szűkösségének fenntartásához. Ahhoz, hogy egy kormány vagy rosszindulatú szereplő megállítsa a Bitcoint, minden egyes blokklánc-másolatot el kellene pusztítania, amelyek jelenleg világszerte több ezer node-on futnak – ez szinte lehetetlen feladat.

##### Emberek

A centralizáció egy másik lehetséges aspektusa az emberekhez kötődik. Minden más „altcoin”-nak van egy vezéralakja – valaki, akit potenciálisan rá lehet venni arra, hogy a Bitcoin érdekeivel ellentétes változtatásokat támogasson. Satoshi Nakamoto addig maradt, amíg biztosította, hogy a Bitcoin sikeres úton halad, majd végleg eltűnt, másokra bízva a szoftver fejlesztését és továbbfejlesztését.

Mi a helyzet azokkal, akik nagy mennyiségű Bitcoinnal rendelkeznek? A korai befektetők, akik megtartották az érméiket és nem veszítették el azokat, mostanra rendkívül gazdagok lehetnek. Fontos azonban megjegyezni, hogy ez valóban így lehet, de ez nem ad nekik nagyobb befolyást a rendszer felett, mint bárki másnak – ellentétben a „proof of stake” érmékkel, ahol a korai, már eleve gazdag résztvevők előnyöket élveznek a döntéshozatalban és a jövőbeli érmék elosztásában. Ez elkerülhetetlenül centralizációhoz vezet vagy vezetett.

##### Összefoglalás

Milyen potenciális fenyegetéseket próbálhat a decentralizáció enyhíteni?

* A kormány leállítja vagy betiltja a Bitcoint
* Olyan nem kívánt kódváltoztatások, amelyek a Bitcoinon belül egyes érdekcsoportokat részesítenek előnyben, például a blokk jutalom növelése
* A protokoll kormány vagy rosszindulatú szereplők általi befolyásolása, hogy a protokoll irányát megváltoztassák
* A bányász poolok képessége, hogy átvegyék a hálózat irányítását, és „dupla költést” hajtsanak végre – 51%-os támadás

Ahogy láthatjuk, a node-ok, a kódfejlesztők és a bányászok kombinációja, valamint a „proof of work” mechanizmus használata elegendő szintű decentralizációt biztosít a Bitcoinnak ahhoz, hogy ezek a potenciális fenyegetések ne jelentsenek komoly aggodalmat. A közösségnek azonban továbbra is figyelemmel kell kísérnie a helyzetet, hogy ez így is maradjon.
