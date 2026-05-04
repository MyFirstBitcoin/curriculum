# 8 - Hogyan működik a Bitcoin

Időtartam: 90 perc

Alapötlet: A Bitcoin biztonsága egyszerű, de erőteljes technikai elveken alapul, mint például a kulcsok, aláírások, hash-elés és UTXO-k, amelyek lehetővé teszik a tulajdonjogot és az ellenőrzést központi hatóság nélkül.

#### Tanulási célok

A lecke végére a diákok képesek lesznek:

* Elmagyarázni, hogyan segítik a nyilvános és privát kulcsok a Bitcoin tulajdonjogának és tranzakcióinak biztonságát.
* Leírni, mi az a digitális aláírás, és hogyan bizonyítja, hogy egy tranzakciót a jogos tulajdonos hagyott jóvá.
* Egyszerűen elmagyarázni, mit jelent a kriptográfia, titkosítás és visszafejtés a Bitcoin esetében.
* Meghatározni a hash-elést, és leírni, miért fontosak a hash-függvények a Bitcoin biztonsága és adatainak épsége szempontjából.
* Azonosítani egy hash-függvény alapvető tulajdonságait, mint például a fix hosszúságú kimenet, egyirányúság és az érzékenység a bemenet apró változásaira.
* Elmagyarázni az UTXO modellt, és hogy a bitcoint hogyan költik el, fogadják, illetve hogyan tér vissza visszajáróként a tranzakciók kimenetein keresztül.
* Leírni, hogyan segítenek a node-ok megelőzni a dupla költést azáltal, hogy ellenőrzik, egy kimenetet már elköltöttek-e.

#### Eszközök és források

##### Vizuális segédletek

* 8. fejezet – Hogyan működik a Bitcoin

##### Támogató könyvtár

* Szókártya — 8. fejezet — Fogalmak: kriptográfia, hash, UTXO, digitális aláírás, privát/nyilvános kulcs, merkle-fa, blokklánc
* Tévhitek könyvtára — 8. fejezet — Címek: „az elveszett seed phrase visszaállítható”, „privát kulcs = jelszó”, „a blokklánc anonim”
* Technikai magyarázatok és mélyebb elemzések — Hash-függvények, nyilvános/privát kulcsok, UTXO modell, Proof of Work biztonság

#### Tevékenységek

* Tranzakciók működés közben
* A Mempool felfedezése

#### Online oktatás

* Használj digitális táblát, és rajzold le élőben az egyes fogalmakat, ne csak szóban magyarázz.
* Egyszerre csak egy technikai fogalmat taníts, és gyakran állj meg ellenőrző kérdésekhez.
* Használj vizuális segédleteket a kulcsokhoz, aláírásokhoz, hash-ekhez és UTXO-khoz, hogy a diákok követni tudják a felépítést.
* Maradj a fogalmi szinten, és kerüld a túl mély matematikai vagy szakzsargonba való elmerülést.

#### Felkészülés

* Készítsd elő és lamináld le a diagramokat: nyilvános/privát kulcspárok, digitális aláírások, UTXO modell, hash-elés (egyirányú függvény).
* Könyvjelzőzd be a blokklánc böngészőt és a SHA-256 hash kalkulátort; válassz ki 2-3 valódi Bitcoin tranzakciót, amelyeken lépésről lépésre végig tudtok menni.
* Készíts jegyzeteket a táblára a bemenetek, kimenetek és a tranzakciók blokkláncon való megerősítésének magyarázatához.

#### Folyamat

Ez a lecke bevezeti a diákokat a Bitcoin technikai oldalába anélkül, hogy előzetes technikai tudást feltételezne. Az útmutató most már a Diploma tömör szerkezetét követi, a kriptográfiát egy, az UTXO-kat egy másik fejezet alá csoportosítva.

##### 8.0 Bevezetés, 8 perc

Kezdd az elvárások tisztázásával:

* Mitől biztonságos a Bitcoin, ha nincs központi bank, ami irányítaná?
* Honnan tudja a hálózat, hogy valaki valóban birtokolja-e a bitcoint, amit el akar küldeni?
* Mi történik valójában a háttérben, amikor valaki Bitcoin tranzakciót hajt végre?

Tisztázd, hogy ez a fejezet a Bitcoin alapvető technikai alapjaira koncentrál, különösen a kulcsokra, aláírásokra, hash-elésre és UTXO-kra. Nyugtasd meg a diákokat, hogy nem kell mérnökké válniuk ahhoz, hogy megértsék a lényegi logikát. Maga a fejezet is világosan rámutat erre, amikor a Bitcoint az internethez hasonlítja: sokan használják nap mint nap anélkül, hogy minden rétegét teljesen értenék.

##### 8.1 Biztonság kriptográfiával, 57 perc

**Bitcoin mint főkönyv, amely sok számítógépen tárolódik**

Kezdd a fejezet egyszerű megfogalmazásával a Bitcoin hálózatról:

* A Bitcoin egy tranzakciós nyilvántartás
* ez a nyilvántartás sok számítógépen, úgynevezett node-okon tárolódik
* a főkönyv nyilvános és pszeudonim
* címeket és tranzakciós előzményeket mutat, nem személyes adatokat

Ez a rész segít a diákoknak visszacsatolni ahhoz, amit korábbi fejezetekből már tudnak. A Bitcoin nem rejtett bankszámlákon alapul. Egy megosztott főkönyvre épül, amelyet sok résztvevő ellenőrizhet.  itt különösen hasznos, mert bemutatja a felhasználókat, tárcákat és a szélesebb Bitcoin hálózatot, amelyek a nyilvános főkönyvhöz kapcsolódnak.

**Nyilvános és privát kulcsok**

Most térj át a kriptográfiára.

Magyarázd el, hogy minden Bitcoin felhasználónak van:

* egy privát kulcsa, amelyet titokban kell tartani
* egy nyilvános kulcs, amely megosztható

Egyszerűen fogalmazva tisztázd a céljukat:

* a privát kulcs igazolja a tulajdonjogot és engedélyezi a költést
* a nyilvános kulcs segít másoknak ellenőrizni, hogy a tranzakciót helyesen engedélyezték

A fejezet egyik erős tanítási pontja, hogy a Bitcoin nyilvános/privát kulcsú titkosítást használ, nem pedig a régebbi modellt, ahol két embernek először ugyanazt a titkos kulcsot kell megosztania. Ez azért fontos, mert így biztonságos ellenőrzés lehetséges anélkül, hogy a felhasználóknak fel kellene fedniük azt a titkot, amely a pénzüket védi.

Így magyarázhatod el:

* a privát kulcs olyan, mint a titkos bizonyíték arra, hogy a bitcoin a tiéd
* a nyilvános kulcs része annak, ami lehetővé teszi a hálózat számára, hogy ellenőrizze a jogosultságodat
* aki birtokolja a privát kulcsot, az tudja elkölteni a bitcoint

Itt ügyelj arra, hogy ne bonyolítsd túl a titkosítási nyelvezetet. A legfontosabb pont a diákok számára a tulajdonjog és az engedélyezés.

**Digitális aláírások és tranzakció engedélyezése**

Most magyarázd el, mi történik, amikor valaki bitcoint küld.

Használd a fejezet lépéseit:

* a felhasználó létrehoz egy tranzakciót
* a küldő digitális aláírást generál a privát kulcsával
* a tranzakciót továbbítják a hálózatra
* a csomópontok ellenőrzik, hogy az aláírás érvényes-e
* ha ellenőrizték és megerősítették, a tulajdonjog átkerül a főkönyvön

Tedd világossá, hogy a digitális aláírás nem ugyanaz, mint egy név begépelése. Ez kriptográfiai bizonyíték arra, hogy a valódi tulajdonos engedélyezte a tranzakciót. Ez az egyik alapvető mechanizmus, amely lehetővé teszi, hogy a Bitcoin központi hatóság manuális jóváhagyása nélkül működjön. Az ábra hasznos, mert vizuálisan mutatja be az aláírást és az ellenőrzést, valamint a tranzakció útját a küldőtől a hálózati érvényesítésig.

Egy jó mondat az órán:

A Bitcoin tranzakciókat nem azért hagyják jóvá, mert egy bank azt mondja. Azért fogadják el, mert a hálózat érvényes kriptográfiai bizonyítékot tud ellenőrizni.

**Hash-elés és egyirányú függvények**

Ezután magyarázd el a hash-elést.

Kezdd egyszerűen:

* egy függvény bemenetet vesz, és kimenetet ad
* egy egyirányú függvény egy irányba könnyen futtatható, de visszafelé gyakorlatilag lehetetlen
* egy hash függvény bármilyen méretű adatot vesz, és egy fix hosszúságú kimenetet, úgynevezett hash-t készít belőle

Használd a fejezet egyik analógiáját, amelyik a legérthetőbb a közönségednek:

* a turmix analógia az egyirányú függvényekhez
* az ujjlenyomat analógia a hash-ekhez
* a kottás példa annak ellenőrzésére, hogy valami megváltozott-e

Az ujjlenyomat analógia valószínűleg a legtisztább a legtöbb osztály számára:

* a hash olyan, mint egy digitális ujjlenyomat az adatokhoz
* ha a bemenet akár egy kicsit is változik, a hash teljesen megváltozik
* ez segít a számítógépeknek ellenőrizni az integritást és észlelni a manipulációt

Ezután magyarázd el, miért fontos a hash-elés a Bitcoinban:

* a tranzakciókat hash-elik
* a hálózat hash-eket használ az integritás ellenőrzésére
* ha egy tranzakció megváltozik, a hash is megváltozik
* ez segít megvédeni a főkönyvet a rejtett manipulációtól

A 7–10. oldalon lévő ábrák itt nagyon hasznosak. A fejezet bemutatja mind a fix hosszúságú kimenet elvét, mind a „kis változás, teljesen más eredmény” elvet, ami az egyik legfontosabb fogalom, amit a diákoknak meg kell érteniük.

**A hash függvények alapvető tulajdonságai**

Röviden menj végig a fejezetben kiemelt tulajdonságokon, anélkül, hogy túl tudományosnak tűnnének:

* Determinált: ugyanaz a bemenet minden alkalommal ugyanazt a kimenetet adja
* Egyirányú / előkép-ellenálló: a folyamatot gyakorlatilag nem lehet visszafordítani
* Érzékeny a változásra: már egy kis bemeneti változás is teljesen más kimenetet eredményez
* Ütközésálló: rendkívül nehéz két különböző bemenetet találni, amelyek ugyanazt a kimenetet adják
* Gyorsan ellenőrizhető: a függvény hatékonyan futtatható és ellenőrizhető

Nem kell, hogy a diákok minden kifejezést megjegyezzenek, de értsék a lényeget: a hash-elés megbízható módot ad a Bitcoin számára az adatok azonosítására és a változások észlelésére.

##### 8.2 Az UTXO modell, 25 perc

**A UTXO modell**

Most lépjünk át a fejezet második fő részébe: a UTXO-khoz, vagyis az Elköltetlen Tranzakciós Kimenetekhez.

Magyarázd el egyszerűen a fejezet készpénzes hasonlatával:

* a bitcoint nem úgy követik nyomon, mint egy bankszámla-egyenleget
* helyette elköltető darabokból áll, amelyeket UTXO-knak hívnak
* amikor bitcoint költesz, egy vagy több meglévő UTXO-t használsz bemenetként
* új UTXO-k jönnek létre kimenetként

Használd a fejezet példáját:

* ha van egy 10 BTC-s UTXO-d
* és elküldesz 6 BTC-t
* egy új 6 BTC-s UTXO kerül a címzetthez
* egy új visszajáró UTXO jön vissza hozzád
* egy kis részt bányász díjként fizetsz ki

Ez segít a diákoknak megérteni, hogy a Bitcoin inkább úgy működik, mint a készpénz elköltése és visszajáró kapása, nem pedig egyszerű számlaegyenlegből való kivonás. A diagramok itt különösen erősek, mert vizuálisan mutatják be, ahogy egy UTXO feloszlik címzett kimenetre, visszajáróra és díjra.

Tedd világossá a két legfontosabb pontot:

* a tárcád egyenlege az UTXO-id összege
* amikor költesz, a régi UTXO-k elhasználódnak, és újak jönnek létre

**A dupla költés megakadályozása**

Zárd le a tartalmat azzal, hogy elmagyarázod a UTXO modell egyik legfontosabb következményét.

Ha valaki megpróbálja ugyanazt a kimenetet kétszer elkölteni, a node-ok elutasítják a második próbálkozást, mert ők vezetik a főkönyvet, és ellenőrizni tudják, hogy az adott UTXO-t már elköltötték-e. Így akadályozza meg a Bitcoin a dupla költést anélkül, hogy központi fizetési cég kezelné a nyilvántartást. A példa itt nagyon hasznos, mert végigvezeti, ahogy Anna összevonja az UTXO-it, pénzt küld Bélának, visszajárót kap, és a megerősített tranzakció frissíti a főkönyvet a node-ok között.

Egyértelműen így lehet elmondani az órán:

A Bitcoin azért akadályozza meg a dupla költést, mert a hálózat nyilvántartja, mely kimenetek maradtak elköltetlenek, és melyeket használtak már fel.

###### Összefoglalás és megértés ellenőrzése

Zárd le néhány gyors kérdéssel:

* Mi a különbség a nyilvános kulcs és a privát kulcs között?
* Mit bizonyít a digitális aláírás?
* Miért hasznos a hash-elés a Bitcoinban?
* Mi történik, ha egy tranzakciót megváltoztatnak a hash-elés után?
* Mi az a UTXO egyszerűen elmagyarázva?
* Hogyan akadályozza meg a hálózat, hogy valaki ugyanazt a bitcoint kétszer költse el?

#### Oktatói jegyzetek

Ez a fejezet technikaibb nyelvezetet tartalmaz, mint a korábbiak, ezért a világosság, a hasonlatok és az ismétlés legyen a prioritás.

A cél nem az, hogy a diákok fejlesztőkké váljanak. A cél az, hogy megértsék, miért működik a Bitcoin biztonsága.

A legerősebb pontok, amelyeket időhiány esetén is ki kell emelni:

* privát kulcs vs nyilvános kulcs
* digitális aláírások
* mit csinál a hash-elés
* a UTXO-k mint a bitcoin elköltető darabjai
* hogyan akadályozzák meg a dupla költést

A leghasznosabb vizuális elemek ebben a fejezetben:

* a felhasználó-tárca-hálózat diagram
* a digitális aláírás vizuálja
* a hash-elési példák és a fix hosszúságú kimenet diagramjai a 7-10. oldalon
* a UTXO diagramok a 10-12. oldalon

##### Mit jelent a jó megoldás

* Fontos, hogy a kriptográfiát alapnak, ne rejtélynek tekintsük, sok vizuális elemet használjunk, kerüljük a mély matematikát, kapcsolódjunk vissza a korábbi fejezetekhez, és teszteljük a megértést olyan alkalmazásokkal, mint például: „Ha valaki megváltoztat egy tranzakciót, mi romlik el?”
* Az oktatóknak türelmesnek kell lenniük a nehezebben haladó diákokkal, vizuálisan kell gondolkodniuk és mindent le kell rajzolniuk, őszintének kell lenniük abban, hogy mit nem kell a diákoknak megérteniük, készeknek kell lenniük azt mondani: „Nem tudom, de így tudnánk kideríteni”, és végig bátorítónak kell maradniuk.
* A diákok megértik, miért nem lehet feltörni a Bitcoint, mert azt a matematika védi, tisztelik a rendszer elegáns felépítését, kényelmesen érzik magukat a komplexitással, tudva, hogy nem kell minden részletet ismerniük, magabiztosan mernek kérdezni ítélkezés nélkül, és felismerik, hogy szintet léptek valami olyan megértésében, amit a legtöbben nem tudnak.
* A tanulási eredmények teljesülnek, ha a diákok el tudják magyarázni a kriptográfia alapjait, mint az egyirányú függvényeket és a digitális aláírásokat mély matematika nélkül, megértik a UTXO modellt, amely megmutatja, hogy érméket birtokolnak, nem számlákat, felismerik a hash-elést a Bitcoin biztonságának alapjaként, értik a tranzakciók felépítését, beleértve az aláírásokat és a megerősítéseket, el tudják magyarázni, miért változtathatatlan a Bitcoin, és kritikus kérdéseket tudnak feltenni a lehetséges támadásokról vagy sebezhetőségekről.

##### Időbeosztás

Ha kevés az idő, ezeket részesítsd előnyben:

* Privát kulcs vs nyilvános kulcs
* Digitális aláírások
* Mit csinál a hash-elés
* UTXO-k mint elkölthető bitcoin-darabok
* Hogyan előzik meg a dupla költést

Ha előrébb jársz, ezekre szánj több időt:

* Felhasználó-tárca-hálózat diagram és vizuális biztonsági modell
* Digitális aláírás vizuálisan: részletes kriptográfiai folyamat
* Merkle-fák és a lánc biztonsága
* Fejlett támadási módszerek és miért nem működnek

##### Ha a diákok nehézségekbe ütköznek

* A kriptográfia fenyegetőnek tűnik → „Naponta használod; a Bitcoin is ugyanígy használja.”
* A hash-elés mint fogalom → Ujjlenyomat hasonlat; egyedi, nem lehet megváltoztatni anélkül, hogy a hash is változna.
* Digitális aláírások → „Igazolja a jogosultságot anélkül, hogy felfedné a jelszót.”
