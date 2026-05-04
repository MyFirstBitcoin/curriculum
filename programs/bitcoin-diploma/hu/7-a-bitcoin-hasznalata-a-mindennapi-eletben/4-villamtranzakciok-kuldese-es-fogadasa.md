# 7.4 Villámtranzakciók küldése és fogadása

Egy Lightning tárcával a Bitcoin használata gyors, olcsó és privát, így két ember között könnyűvé válik a tranzakció. Gyorsan küldhetsz és fogadhatsz bitcoint mindennapi dolgokra, például kávévásárlásra.

Nézzünk néhány példát a Lightning Network működésére.

###### 1. példa

Marcia és Éva egyaránt 5 egységnyi pénzzel rendelkeznek. Marcia 2 egységet szeretne küldeni Évának. A fizetés Jeffen keresztül halad, aki segít továbbítani az összeget a Lightning Networkön. A tranzakció után Évának 7 egysége lesz, Marciának pedig 3.

Jeff segít a fizetés továbbításában, de nem tudja ellopni a pénzt. A Lightning Network kriptográfiát használ annak biztosítására, hogy csak a címzett kaphassa meg a fizetést. Jeff egyszerűen csak segíti a fizetés útját a hálózaton keresztül.

Ez megmutatja a Lightning Network egyik fő előnyét: az emberek gyorsan küldhetnek pénzt anélkül, hogy közvetítőben, például bankban kellene megbízniuk.

A Jeffhez hasonló csomópont-üzemeltetők kis díjakat is kereshetnek a fizetések továbbításáért. Ezzel segítik a hálózat decentralizáltságát és hatékonyságát.

A hagyományos Bitcoin tranzakciókhoz képest:

* **On-chain tranzakciók** közvetlenül a Bitcoin blokkláncon történnek. Nagyon biztonságosak, de lassabbak és drágábbak lehetnek.
* **Lightning tranzakciók** láncon kívül történnek, és lehetővé teszik a fizetések sokkal gyorsabb és olcsóbb lebonyolítását.

Ezért a Lightning hasznos a kis, mindennapi fizetésekhez, míg az on-chain tranzakciókat gyakran nagyobb összegek vagy hosszú távú tárolás esetén használják.

###### 2. példa

Mina szeret étterembe járni, és gyakran betér a kedvenc helyi kávézójába. Mivel sokféle fizetési lehetőség közül választhat, nem tudja, melyik a legjobb. Szerencsére már tanult egy keveset a Bitcoinról és a Lightning Networkről. Miután átgondolta a lehetőségeit, Mina rájön, hogy a Lightning fizetési mód a legjobb választás.

Mina kávét szeretne venni, de egy hagyományos Bitcoin tranzakcióval a fizetés néha időigényes lehet, és magasabb díjakkal járhat. Ehelyett úgy dönt, hogy a Lightning Networköt használja.

A Lightning Network lehetővé teszi, hogy az emberek azonnal és nagyon alacsony díjakkal küldjenek bitcoint. Ez ideálissá teszi a kis, mindennapi vásárlásokhoz, például kávéhoz.

A Lightning használatához Mina letölt egy Lightning tárcát a telefonjára. Ezután átküld némi bitcoint a hagyományos Bitcoin tárcájából a Lightning tárcájába. Ez a lépés egy normál Bitcoin tranzakció a blokkláncon. Miután a pénz megérkezett a Lightning tárcájába, már használhatja a Lightning Networkön.

Most Mina azonnal fizethet a kávézóban Lightning segítségével. A fizetés a fő Bitcoin blokkláncon kívül történik, ezért sokkal gyorsabb és olcsóbb, mint egy hagyományos on-chain tranzakció.


| Előnyök | Lightning Network | Hagyományos bankrendszer |
| --- | --- | --- |
| Sebesség | Gyors | Lassú |
| Átláthatóság | Átlátható | Átláthatatlan |
| Biztonság | Biztonságos | Sérülékeny |
| Tranzakciós díjak | Alacsony | Magas |
| Pénzügyi befogadás | Magas | Korlátozott |
| Skálázhatóság | Magas | Alacsony |
| Adatvédelem | Magas | Közepes |
| Interoperabilitás | Magas | Alacsony |
| Jogi megfelelőség | Közepes | Magas |
| Költséghatékonyság | Magas | Közepes |


Az on-chain tranzakciók közvetlenül a Bitcoin blokkláncon történnek, ezért több időt és magasabb díjat igényelhetnek. A Lightning tranzakciók láncon kívül zajlanak, így gyors és alacsony költségű fizetéseket tesznek lehetővé, miközben továbbra is bitcoint használnak.


| Visa, Inc. | Bitcoin on-chain | Lightning Network |
| --- | --- | --- |
| Kapacitás: 65 000 tranzakció másodpercenként. | Kapacitás: 7 tranzakció másodpercenként. | Kapacitás: több millió tranzakció másodpercenként. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Ez a Lightning Network teljes térképe. Több ezer Lightning node futtatónak köszönhetően satokat küldhetsz bármely felhasználónak, akinek van Bitcoin Lightning pénztárcája, bárhol is legyen a világon. A fizetés néhány másodperc alatt megérkezik, és csak néhány forintba kerül.**Próbáld ki te magad is!**

#### Gyakorlat: Lightning váltófutás

https://qr.myfirstbitcoin.org/lightning.pdf

**Ez egy gyakorlati feladat, amelyben a diákok valódi satokat küldenek és fogadnak a Lightning Network segítségével.**

###### Főbb pontok

1. Egy Lightning pénztárca használata növeli az önbizalmadat a valódi satok fogadásában és küldésében.
1. Figyelj az egységekre! Egyes pénztárcák lehetővé teszik, hogy bitcoint VAGY satot küldj (1/100 000 000 bitcoin).
1. A Lightning fizetések néha elakadhatnak az útvonalválasztás során, különösen nagyobb összegek esetén. Bár ez előfordulhat, az ilyen felhasználói élmény egyre ritkább, ahogy a hálózat fejlődik.

###### Diáktipp

Ellenőrizd az oktatóddal, hogy a jelenlegi on-chain Bitcoin tranzakciós díjak hogyan befolyásolják az általad használt konkrét Lightning pénztárcát.
