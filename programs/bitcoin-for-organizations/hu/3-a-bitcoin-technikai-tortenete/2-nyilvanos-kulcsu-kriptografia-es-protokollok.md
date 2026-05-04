# 3.2 Nyilvános kulcsú kriptográfia és protokollok

A mai internet és a legtöbb modern számítógépes rendszer a kriptográfiára támaszkodik, amely egy olyan módszer, amellyel az információkat elrejtik, hogy csak a címzett tudja azokat megfejteni. A Bitcoin biztonságát szolgáló kriptográfia alapjai az 1970-es évekre vezethetők vissza.

Az első megoldandó kérdés az – hogyan lehet egy közös titkot elküldeni egy nem biztonságos csatornán.

Ezzel először Whitfield Diffie és Martin Hellman foglalkoztak.

A probléma: a két fél – akiket általában Aliznak és Bálintnak hívnak – titkos információt szeretne megosztani egy olyan hálózaton, ahol mások is lehallgathatják őket. Ennek elérésére hozták létre a Diffie-Hellman kulcscsere folyamatot.

Ez a közös titok aztán felhasználható magként számos szimmetrikus kulcs létrehozásához, amelyekkel titkosíthatják és visszafejthetik egymásnak küldött üzeneteiket anélkül, hogy magát a kulcsot nyilvánosan megosztanák.

Mivel a privát kulcsot soha nem kell megosztani, és mindkét oldalon más-más kulcsot használnak a titkosításhoz és visszafejtéshez, ezt aszimmetrikus titkosítási algoritmusnak nevezik.

Felhasználási példák:

* Aliz aláír egy üzenetet Bálint nyilvános kulcsával – ő az egyetlen, aki a saját privát kulcsával vissza tudja fejteni azt
* Aliz aláír egy üzenetet a saját privát kulcsával – ha valaki a nyilvános kulcsával visszafejti, bárki ellenőrizheti, hogy az üzenetet valóban Aliz küldte, anélkül, hogy ismerné a privát kulcsát
* E két megközelítés kombinálásával, két rétegű titkosítással, egy üzenet úgy küldhető el, hogy csak Bálint tudja visszafejteni, és ő azt is ellenőrizheti, hogy a feladó valóban Aliz volt.

Bár a tanulmányban nem tüntették fel szerzőként, Ralph Merkle kulcsszerepet játszott abban, hogy sikerült megoldani ezt az addig megoldhatatlannak tartott rejtvényt – hogyan lehet privát kommunikációt létrehozni vagy újra létrehozni egy nyílt és potenciálisan ellenséges hálózaton.

Ez a megközelítés önmagában ki van téve a brute force támadásoknak, amikor egy támadó a megosztott számokat felhasználva előbb-utóbb képes lehet újra létrehozni a közös kulcsot, ha elég ideje és erőforrása van, így önmagában nem jelent teljes megoldást.

##### Nyilvános kulcsú kriptográfiai protokollok

A fent leírt Diffie-Hellman nyilvános kulcsú rendszerhez való hozzájárulása mellett **Ralph Merkle** sok éven át tovább dolgozott ezen a területen, és kulcsszerepet játszott néhány olyan alapvető komponens kifejlesztésében, amelyeket a Bitcoin is használ.

A kriptográfiai hash függvény egy matematikai algoritmus, amely bármilyen méretű bemenetet képes feldolgozni, és összetett számításokat végezve egy hash értéket ad vissza bitekben, amelyet általában rögzített hosszúságú alfanumerikus kimenetként jelenítenek meg hexadecimális formátumban.

* A bemenet lehet bármilyen méretű
* A kimenet mindig rögzített hosszúságú és determinisztikus (ugyanaz a bemenet minden alkalommal ugyanazt a hash-t eredményezi)
* Könnyű ellenőrizni, de rendkívül nehéz visszafejteni a folyamatot, hogy meghatározzuk a bemenetet
* Az adatok legkisebb módosítása is teljesen megváltoztatja a kimenetet

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/1c5911574ad5fa83edc87fadd0ecc4511621df29-515x331.svg)

A hash-elés a Bitcoin protokoll szerves része. A Bitcoinban használt SHA-256-ot az NSA fejlesztette ki, és ez egy példa a kriptográfiai hash algoritmusokra.

* A lánc minden blokkját hash-elik, hogy az adatok ne legyenek módosíthatók – ez biztosítja az elosztott főkönyv integritását.
* A létrehozott hash-nek meg kell felelnie a „Proof of work” kritériumainak, hogy érvényes blokknak számítson.
* Merkle-fák – elágazások és hash-ek hash-einek alkalmazásával a hash-fák lehetővé teszik nagy adathalmazok ellenőrzését minimális tárhely mellett.
* Hash-alapú aláírások és kulcsok használhatók tárcákhoz, címekhez és tranzakciók engedélyezéséhez.

Az egyirányú hash-elés teszi lehetővé a blokklánc állapotainak elosztott ellenőrzését és a csak hozzáfűzhető főkönyvi modelleket, amelyek ellenállnak az utólagos módosításnak. A hash függvények megbízható, determinisztikus módszert biztosítanak az események ellenőrzésére a nyilvános főkönyveken, mint például a Bitcoin, központosított bizalmi modell nélkül.

A kriptográfia területén ezek az új képességek alkotóik szerint új innovációs hullámot indíthatnak el ezen a területen.

##### Elliptikus görbe kriptográfia

Ezek közül az egyik későbbi újítás az elliptikus görbe kriptográfia volt.

Az elliptikus görbe kriptográfiát 1985-ben két tudós, N. Koblitz és V. Miller vezette be. Azt javasolták, hogy a véges prímtartományok helyett, amelyeket a hagyományos Diffie-Hellman kulcscsere protokollban használnak, elliptikus görbék által meghatározott pontokat használjanak, feltéve, hogy a Diszkrét Logaritmus probléma feltétele teljesül. A részletek meghaladják ennek a szakasznak a kereteit, de magas szinten egy elliptikus görbe azon pontok halmaza, amelyek megfelelnek egy adott matematikai egyenletnek.

Egy elliptikus görbe egyenlete valahogy így néz ki:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Ez néhány hasznos tulajdonsággal bír:

* Vízszintes szimmetria. A görbe bármely pontja tükrözhető az x tengelyre, és ugyanazon a görbén marad.
* bármely nem függőleges egyenes legfeljebb három pontban metszi a görbét.
* A kompakt kulcsméretek elengedhetetlenek a nyilvános kulcsok hatékony tárolásához és továbbításához a blokkláncon.

Ezek a tulajdonságok lehetővé teszik kulcspárok létrehozását hasonló módon, mint a Diffie-Hellman algoritmusnál. A Bitcoin az ECDSA-t használja, amely az Elliptikus Görbe Digitális Aláírási Algoritmus rövidítése. Ez egy olyan folyamat, amely egy elliptikus görbét és egy véges mezőt használ az adatok „aláírására” úgy, hogy harmadik felek ellenőrizhetik az aláírás hitelességét, miközben az aláíró kizárólagos képessége marad az aláírás létrehozása. A bitcoin esetében az aláírt adat az a tranzakció, amely a tulajdonjogot átruházza.

A „véges” rész hasonló a Diffie-Hellman-nél alkalmazott „mod” megközelítéshez, ahol az egyenlet eredményét elosztják, és a maradékot használják fel annak biztosítására, hogy az egy adott számhalmazba essen.
