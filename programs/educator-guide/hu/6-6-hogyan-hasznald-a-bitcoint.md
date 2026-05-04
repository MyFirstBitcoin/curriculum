# 6 - Hogyan használd a Bitcoint

Időtartam: 90 perc

Alapötlet: A Bitcoin láncon történő használata megtanítja a diákokat arra, hogyan működik a tulajdonjog, az önálló letétkezelés és az ellenőrzés a gyakorlatban, így az elméletet közvetlen pénzügyi cselekvéssé alakítja.

#### Tanulási célok

Az óra végére a diákok képesek lesznek:

* Felismerni a bitcoin megszerzésének és cseréjének általános módjait, beleértve a személyes és a központosított tőzsdei módszereket.
* Elmagyarázni az önálló letétkezelésű és a letétkezelő pénztárcák közötti különbséget, és hogy miért fontos az önálló letétkezelés a Bitcoin esetében.
* Leírni a privát kulcsok, nyilvános címek, seed phrase-ek és pénztárca felületek célját.
* Összehasonlítani a különböző pénztárcatípusokat, és értékelni azok előnyeit és hátrányait a biztonság, kényelem, adatvédelem és kontroll szempontjából.
* Beállítani egy mobil Bitcoin pénztárcát, és elmagyarázni az alapvető helyreállítási folyamatot.
* Bemutatni, hogyan lehet fogadni és küldeni egy láncon történő bitcoin tranzakciót.

Alkalmazni a "Ne bízz, ellenőrizz!" elvet a pénztárcaválasztásban, tranzakciókban és a Bitcoin szélesebb körű használatában.

#### Eszközök és források

##### Vizuális segédletek

* 6. fejezet – Hogyan használd a Bitcoint

##### Támogató könyvtár

* Szókártya — 6. fejezet — Fogalmak: pénztárca, privát kulcs, nyilvános cím, seed phrase, letétkezelő, önálló letétkezelő, UTXO, tranzakciós díj
* Összehasonlító táblázatok és segédletek — Pénztárcatípusok összehasonlítása (letétkezelő, mobil, hardver, papír)
* Technikai magyarázatok és mélyebb elemzések — Nyilvános/privát kulcsok, UTXO modell, tranzakció megerősítés
* Privát kulcs biztonsági mélyelemzés — Seed phrase-ek, kulcsszármaztatás, biztonsági mentési módszerek, támadási vektorok
* Tranzakció anatómiája útmutató — Lépésről lépésre bemutatott példa arra, hogyan működik egy Bitcoin tranzakció
* Biztonsági legjobb gyakorlatok ellenőrzőlista — Indulás előtt, pénztárca létrehozása, fogadás, küldés, adathalászat elleni védelem

#### Tevékenységek

* Tranzakciók működés közben
* Lightning váltóverseny
* A Mempool felfedezése

#### Online oktatás

* Az elejétől fogva tedd egyértelművé, hogy a diákok csak bemutatót néznek, vagy maguk is pénztárcát állítanak be.
* Használj nagy, jól olvasható képernyőképeket minden pénztárca-beállítási lépéshez.
* Minden lépés után állj meg, és kérd meg a diákokat, hogy chatben jelezzék, értik-e, mielőtt továbbléptek.
* Adj közvetlen figyelmeztetést a seed phrase szekció előtt, és emlékeztesd a diákokat, hogy soha ne osszanak meg érzékeny információkat online.

#### Felkészülés

* Tölts le és tesztelj egy mobil pénztárca alkalmazást (Blue Wallet vagy Muun); készíts képernyőképeket a fő beállítási lépésekről.
* Készíts pénztárca-beállítási útmutatót (letöltés → létrehozás → seed mentése → fogadás) referenciaként.
* Győződj meg róla, hogy a hálózat/WiFi működik; legyen egy bemutató cím és QR-kód készen a bemutatáshoz.

#### Folyamat

Ez a lecke az elmélettől a közvetlen gyakorlathoz vezet. Most már közvetlenül illeszkedik a Diploma szerkezetéhez, így a megszerzés, pénztárcák, beállítás, tranzakciók és ellenőrzés ugyanazok alatt a főcímek alatt jelennek meg, mint a diák útmutatóban. A további oktatási támogatás ezekben a szekciókban marad beágyazva.

##### 6.0 Bevezetés, 8 perc

Kezdd azzal, hogy összekapcsolod ezt a fejezetet az előzővel:

* Ha a Bitcoin pénz, hogyan szerzik és használják azt az emberek valójában?
* Mit jelent igazán uralni a saját bitcoinodat?
* Miért más a Bitcoin használata, mint egy banki alkalmazásé?

Tisztázd, hogy ez a fejezet a gyakorlati használatról szól. A diákok már nem csak azt tanulják, mi a Bitcoin, hanem azt is, hogyan léphetnek vele közvetlen kapcsolatba.

##### 6.1 Bitcoin megszerzése és cseréje, 12 perc

Magyarázd el, hogy az emberek különböző módokon szerezhetnek bitcoint, például:

* bitcoinban kapnak fizetést
* bitcoint bányásznak
* fiat pénzt cserélnek bitcoinra személyesen
* fiat pénzt cserélnek bitcoinra online

Ezután összpontosíts a fejezetben tárgyalt két fő megszerzési módra:

* személyes, peer-to-peer
* peer-to-peer, online
* központosított tőzsdék

Tedd egyértelművé a kompromisszumokat.

A személyes P2P esetén hangsúlyozd a közvetlen cserét bank vagy közvetítő nélkül, de említsd meg a készpénzes találkozók gyakorlati kockázatait is.

Az online P2P esetén magyarázd el egyszerűen az escrow (letét) fogalmát, mint egy módot arra, hogy csökkentsük a partnerkockázatot, miközben továbbra is közvetlen csere történik a felek között.

A központosított tőzsdéknél tedd világossá, hogy kényelmesek, de a felhasználóknak meg kell bízniuk egy cégben, gyakran meg kell osztaniuk személyes adataikat, és a pénzeszközök harmadik fél ellenőrzése alatt maradnak a visszavonásig. Itt jó hangsúlyozni, hogy a kényelem gyakran együtt jár a magánélet és a szuverenitás kompromisszumaival.

##### 6.2 Bevezetés a Bitcoin tárcákhoz, 35 perc

**Mi is valójában egy Bitcoin tárca**

Azonnal tisztázz egy gyakori félreértést: a bitcoin nem a tárca alkalmazásban van tárolva, mint a készpénz egy táskában.  
A bitcoin a hálózat által vezetett főkönyvön létezik. Amit a felhasználó irányít, az a költés lehetősége a privát kulcsokon keresztül.

Ezután magyarázd el azt a két dolgot, amit az emberek gyakran értenek a "tárca" alatt:

* a privát kulcs rendszerét, amelyből a címek generálódnak
* az alkalmazást vagy felületet, amellyel a hálózathoz kapcsolódunk

Használd a fejezet e-mailes hasonlatát, ha segít:

* nyilvános cím = mint egy e-mail cím, amit megoszthatsz
* privát kulcs = mint egy jelszó, amit védened kell

Itt legyél nagyon egyértelmű: aki a privát kulcsokat birtokolja, az irányítja a bitcoint. Ez az a kulcsfontosságú fogalom, amit a tanulóknak meg kell érteniük.

**Önőrzéses vs. letétkezelői tárcák**

Ez a fejezet egyik legfontosabb része.

Magyarázd el világosan a különbséget:

* Önőrzéses tárca: a felhasználó irányítja a privát kulcsokat
* Letétkezelői tárca: egy harmadik fél irányítja a privát kulcsokat a felhasználó nevében

Ezután vezesd végig a kompromisszumokat:

Önőrzéses

* teljes ellenőrzés a pénz felett
* nincs jóváhagyási folyamat
* védelem az önkényes elkobzás ellen
* nagyobb felelősség
* nincs egyszerű visszaállítás, ha a seed kifejezés elveszik

Letétkezelői

* könnyebb visszaállítás és támogatás
* egyszerűbb kezdőknek
* jobban ki van téve a számlafagyasztásnak, feltöréseknek és harmadik fél általi ellenőrzésnek
* a felhasználó valójában nem birtokolja a bitcoint

Ez a megfelelő pillanat, hogy hangsúlyozd ezt a mondatot:

"Nem a te kulcsaid, nem a te coinjaid."

A tanulóknak ebből a részből nemcsak a szlogent kell megérteniük, hanem azt is, hogy ez mit jelent a gyakorlatban.

**Különböző tárcatípusok és hogyan válasszunk**

Mutasd be a fejezetben tárgyalt tárcatípusokat:

* online tárca
* mobil tárca
* asztali tárca
* hardveres tárca
* papír tárca

Ne állítsd be egyiket sem tökéletesnek. Ehelyett magyarázd el, hogy mindegyik kompromisszumot jelent a következők között:

* biztonság
* magánélet
* kényelem
* kompatibilitás
* díjak
* ellenőrzés
* hírnév

Tegyük egyértelművé azt is, hogy javasoljuk odafigyelni arra, hogy a tárcaszoftver nyílt forráskódú-e, mert a nyílt forráskódú eszközöket a közösség átnézheti, auditálhatja és továbbfejlesztheti. Ez közvetlenül kapcsolódik a Bitcoin ellenőrzési elvéhez.

##### 6.3 Mobil Bitcoin tárca beállítása, 10 perc

Vezesd végig a diákokat a fejezetben bemutatott alapvető folyamaton:

* töltsd le a tárcát
* hozz létre egy új tárcát
* generáld le és írd fel a helyreállítási kifejezést
* erősítsd meg a helyreállítási kifejezést
* adj hozzá extra biztonsági lépést, ha elérhető
* nyisd meg a tárcát és keresd meg a fogadás funkciót

Tedd a magmondat (seed phrase) figyelmeztetést nagyon egyértelművé:

* ha a magmondat elveszik, a pénzhez való hozzáférés is elveszhet
* ha valaki más megszerzi a magmondatot, elviheti a pénzt

Ha a diákok ezt gyakorlatban végzik, az oktatónak minden lépésnél meg kell állnia, és ellenőriznie kell, hogy mindenki érti-e, mit csinál. Ha az óra inkább elméleti, ezt a részt magyarázatként is el lehet mondani, nem kell élőben végrehajtani. A fejezetben bemutatott helyreállítási lehetőség arra is jó példa, hogy elmagyarázzuk: a tárcák visszaállíthatók, ha a magmondatot megfelelően lementették.

##### 6.4 Fogadás és küldés tranzakciók, 17 perc

**Fogadás és küldés láncon (on-chain) történő tranzakciókkal**

Most magyarázd el, hogyan működnek a láncon történő tranzakciók.

Bitcoin fogadásához:

* nyisd meg a tárcát
* érintsd meg a fogadás vagy befizetés gombot
* másold ki a címet, oszd meg a linket, vagy mutasd meg a QR-kódot

Bitcoin küldéséhez:

* nyisd meg a tárcát
* illeszd be vagy olvasd be a címzett címét
* írd be az összeget
* ellenőrizd le kétszer az összes adatot
* küldd el a tranzakciót
* várj a visszaigazolásra

Tedd világossá ezeket a kulcspontokat:

* a tranzakció tulajdonjogot ad át, nem fizikai érméket
* a tranzakciók visszafordíthatatlanok
* a csomópontok ellenőrzik az érvényességet
* a bányászok beillesztik a tranzakciókat a blokkokba
* a díjak befolyásolják a visszaigazolás sorrendjét
* a láncon történő tranzakciók általában biztonságosak, de lassabbak és gyakran drágábbak, mint a Lightning tranzakciók

A fejezetben található tranzakciós folyamatábra itt különösen hasznos, mert segít a diákoknak elképzelni az utat a tárca kérésétől a hálózati visszaigazolásig.

**Tranzakciók működés közben és szerepalapú gyakorlat**

Használd a fejezetben bemutatott kooperatív gyakorlat szerkezetét a megértés elmélyítésére. Magyarázd el a négy érintett szerepet:

* küldő
* fogadó
* bányász
* csomópont üzemeltető

Egy egyszerű osztálytermi megközelítés, ha kiosztjuk a szerepeket, és lépésről lépésre végigmegyünk egy tranzakción. Ez segít a diákoknak megérteni, hogy egy Bitcoin tranzakció nem varázslat, hanem egy összehangolt folyamat, amely jóváhagyásból, ellenőrzésből, blokkba foglalásból és főkönyvi frissítésből áll.

Itt nem a technikai mélység a cél. Az a fontos, hogy a diákok megértsék, ki mit csinál egy tranzakcióban, és miért fontos az ellenőrzés.

##### 6.5 Ne bízz, ellenőrizz, 8 perc

Magyarázd el, hogy ez vonatkozik:

* tárcákra
* tőzsdékre
* alkalmazásokra
* tranzakciós adatokra
* "könnyű nyereségről" szóló állítások
* projektek, amelyek úgy tesznek, mintha a Bitcoinhoz hasonlók lennének

Tedd világossá, hogy a Bitcoin használata kritikus gondolkodást, ellenőrzést és a vak bizalom elkerülését igényli. Magyarázd el azt is, miért fontosak az open-source eszközök ebben a kontextusban: ezek teszik lehetővé a független ellenőrzést.

###### Összefoglalás és megértés ellenőrzése

Zárd le néhány gyors kérdéssel:

* Mi a különbség a letétkezelő és az önálló (self-custodial) tárca között?
* Miért olyan fontos a seed phrase (helyreállító kifejezés)?
* Mi történik, amikor láncon (on-chain) küldesz tranzakciót?
* Miért lassabbak a láncon történő tranzakciók, mint néhány más Bitcoin fizetés?
* Mit jelent a gyakorlatban a "Ne bízz, ellenőrizz!"?

#### Oktatói jegyzetek

Ez a fejezet nagyon gyakorlati, ezért a világosságot, a biztonságot és az ismétlést helyezd előtérbe.

A diákoknak nem kell minden tárcatípust egyetlen órán elsajátítaniuk. A fő célok:

* a tárcák alapjainak megértése
* az önálló tárolás (self-custody) megértése
* az alapvető tranzakciós folyamat elsajátítása
* felelősségteljes, ellenőrző szemlélet kialakítása

Légy különösen óvatos, amikor a seed phrase-ről és a tárca beállításáról beszélsz. A diákoknak úgy kell távozniuk, hogy megértik: ezek nem apró részletek, hanem a Bitcoin tulajdonjogának alapjai.

A leghasznosabb vizuális elemek és tevékenységek ebben a fejezetben:

* az önálló és letétkezelő tárcák összehasonlítása
* a tárcatípusok előnyeit és hátrányait bemutató táblázat
* a lépésről lépésre történő tárca beállítási gyakorlat
* a tranzakciós folyamat ábrája
* a szerepalapú tranzakciós tevékenység

##### Mit jelent a jó gyakorlat?

* Fontos, hogy a diákok ténylegesen állítsanak be egy tárcát, vagy nézzenek meg egy alapos bemutatót, a seed phrase legyen a középpontban a "Ez a 12 szó A te Bitcoinod" üzenettel, próbáljanak ki olyan helyzeteket, mint "Mi történik, ha elveszíted a telefonod?", és gyakorolják az adathalászat felismerését.
* Az oktatóknak gyakorlott, segítőkész vezetőknek kell lenniük, akik már csinálták ezt korábban, biztonságtudatosak, de nem paranoiásak, és őszinték a nehézségi görbével és a szükséges tanulással kapcsolatban.
* A diákok úgy érzik, valódi, használható készséget tanultak, megértik, hogy a seed phrase valós és fontos, nem csak elvont dolog, képesnek érzik magukat saját Bitcoin tartására, és megértik, hogy a decentralizáció személyes felelősséget igényel.
* A tanulási eredmények akkor teljesülnek, ha a diákok képesek tárcát beállítani, megértik a nyilvános és privát kulcsok közötti különbséget, felismerik a letétkezelő és önálló tárcák közötti kompromisszumokat, el tudják magyarázni a tranzakció működését (bemenetek, kimenetek, díjak), biztonságtudatosak (különösen a seed phrase védelmében), és kritikus kérdéseket tudnak feltenni a tulajdonjoggal és az ellenőrzéssel kapcsolatban.

##### Időbeosztás

Ha kevés az idő, ezekre fókuszálj:

* A tárcák alapjainak megértése
* Az önálló tárolás megértése
* Az alapvető tranzakciós folyamat elsajátítása
* Felelősségteljes, ellenőrző szemlélet kialakítása

Ha előrébb jártok, szánjatok időt ezekre:

* Az önálló és letétkezelő tárcák összehasonlító táblázata
* A tárcatípusok előnyeit és hátrányait bemutató táblázat
* Lépésről lépésre történő tárca beállítási gyakorlat élő bemutatóval
* Tranzakciós folyamat ábrája díjszámítással
* Haladó biztonsági gyakorlatok és hardveres tárcák megfontolásai

##### Ha a diákok nehezen boldogulnak

* A seed phrase mint "valódi" → "Ez a kifejezés A te bitcoinod; nincs ügyfélszolgálat."
* Nyilvános vs. privát kulcs → E-mail hasonlat (cím vs. jelszó).
* Miért nehéz → "Te irányítod; te vagy a felelős." Ismerd el a kompromisszumot.
