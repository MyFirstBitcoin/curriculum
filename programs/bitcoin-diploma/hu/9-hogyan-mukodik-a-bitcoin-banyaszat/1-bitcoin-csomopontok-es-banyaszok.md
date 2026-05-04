# 9.1 Bitcoin csomópontok és bányászok

A Bitcoin node-ok technikainak tűnhetnek, de valójában csak olyan szoftverek, amelyek egy számítógépen tárolják a Bitcoin blokklánc másolatát. A blokklánc a Bitcoin tranzakciók közös nyilvántartása.

Ha saját node-ot futtatsz, akkor magad ellenőrzöd a Bitcoin tranzakciókat, nem pedig másban bízol. Ez nagyobb függetlenséget ad, és segít a Bitcoin hálózat decentralizáltságának megőrzésében.

A Bitcoin node-ot elképzelheted úgy, mint egy digitális forgalomirányítót, amelynek néhány fontos feladata van.

1. Tárolja a blokklánc másolatát, ami az összes Bitcoin tranzakció története.
1. A node-ok világszerte más node-okhoz kapcsolódnak, és megosztják egymással az információkat. Egy példa erre az új, megerősítésre váró tranzakciók listája, amit mempoolnak hívnak.
1. A node-ok ellenőrzik, hogy minden tranzakció megfelel-e a Bitcoin szabályainak. Ha egy tranzakció érvénytelen, a node elutasítja azt.

A node-ok abban is segítenek, hogy új node-ok csatlakozhassanak a hálózathoz, megosztva velük a blokkláncot. Azonban minden új node önállóan ellenőrzi az összes szabályt.

Bárki futtathat node-ot, ha telepít egy szoftvert, például a Bitcoin Core-t, és letölti a blokkláncot. Miután beállítottad, a node körülbelül 10 percenként fogad új blokkokat, és ellenőrzi őket, mielőtt hozzáadná a saját blokklánc-másolatához.

A node futtatása segít biztonságosabbá és decentralizáltabbá tenni a Bitcoin hálózatot, mert így többen ellenőrzik függetlenül a rendszert.

#### Mi az a Bitcoin node?

> A bányászat célja nem az új bitcoin létrehozása; az csak az ösztönző rendszer. A bányászat az a mechanizmus, amely által a Bitcoin biztonsága decentralizált.  
_Andreas M. Antonopoulos_


> **Callout**
>
> A bányászok összegyűjtik a megerősítetlen tranzakciókat, létrehoznak egy blokkot, és energiát használnak fel ahhoz, hogy megtalálják azt a kulcsot, amely hozzáadja és biztosítja a blokkot.


A bányászok versenyeznek, hogy ki adhatja hozzá a következő tranzakciós blokkot a blokklánchoz. Ehhez meg kell találniuk egy speciális számot, amely érvényes blokk hash-t hoz létre. Ezt úgy képzelheted el, mintha a megfelelő kulcsot keresnéd milliárdnyi lehetőség közül. Az első bányász, aki megtalálja a helyes hash-t, megnyeri a versenyt, és joga van hozzáadni a saját blokkját a blokklánchoz.

Amikor egy bányász érvényes hash-t talál, megosztja a blokkját a hálózattal. A többi bányász gyorsan ellenőrzi, hogy a megoldás helyes-e. Ha igen, a blokkot hozzáadják a blokklánchoz, ezzel segítve a Bitcoin nyilvános főkönyvének biztonságát.

A bányászok kétféleképpen keresnek bitcoint:

* **Blokk jutalom:** Új bitcoin jön létre, és azt a bányász kapja, aki sikeresen hozzáad egy blokkot a blokklánchoz.
* **Tranzakciós díjak:** Amikor valaki bitcoint küld, egy kis díjat is mellékel. Az a bányász, aki hozzáadja a blokkot, megkapja az abban a blokkban szereplő tranzakciók díjait.

#### Bitcoin felezések


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> A bányászok jutalma minden 210 000 blokk után felére csökken, ami körülbelül négyévente történik.


A Bitcoinnak rögzített, legfeljebb 21 000 000 darabos maximális kínálata van, de ezek nem mind jöttek létre a Bitcoin indulásakor. Ehelyett az új bitcoin fokozatosan kerül forgalomba **bányászat** révén.

Amikor a bányászok sikeresen hozzáadnak egy új tranzakciós blokkot a Bitcoin hálózathoz, **blokk jutalmat** kapnak bitcoinban. A Bitcoin korai időszakában ez a jutalom 50 bitcoin volt blokkonként. Ez a jutalom ösztönözte az embereket, hogy számítási kapacitást és áramot használjanak a hálózat biztonságához.

Nagyjából minden 210 000 blokk után (körülbelül 4 évente) a blokk jutalom felére csökken. Ezt az eseményt nevezik **felezésnek**. A felezés lassítja az új bitcoin létrehozását, és segít biztosítani, hogy a teljes kínálat soha ne haladja meg a 21 milliót. Idővel ez egyre ritkábbá teszi a bitcoint.


> **Definition – Forgalomban lévő kínálat**
>
> **A forgalomban lévő kínálat** az adott pénznem elérhető teljes mennyiségét jelenti. A Bitcoinnál a teljes forgalomban lévő kínálat az a mennyiség, amit már kibányásztak, és egy adott pillanatban forgalomban van.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/ce42c8d0f8969b8c5f4e9c81dd53a4c28b471d1f-292x200.svg)


> **Definition – A Bitcoin kínálati ütemterve**
>
> A **Bitcoin kínálati ütemterve** az előre meghatározott és nyilvános terv az új bitcoin forgalomba hozatalára, amelynek célja, hogy hosszú távon fenntartsa a Bitcoin ritkaságát.


Minden felezési esemény után a bányászok által blokkonként kapott bitcoin jutalom felére csökken. Ez csökkenti az új bitcoinok létrehozásának ütemét.

A bányászok továbbra is kapnak tranzakciós díjakat azokból a tranzakciókból, amelyek bekerülnek az általuk bányászott blokkba. Idővel ezek a díjak várhatóan a bányászok bevételének nagyobb részét fogják kitenni.

A felezések be vannak építve a Bitcoin protokolljába, és automatikusan megtörténnek körülbelül négyévente. Emiatt a Bitcoin kínálati ütemezése kiszámítható és átlátható.

A táblázat a közelgő felezéseket mutatja, beleértve a hozzávetőleges dátumot, a blokk számát, amikor megtörténnek, az új blokk jutalmat, valamint azt a százalékot, amely a teljes bitcoin készletből már ki lett bányászva.


| Esemény | Dátum | Blokk | Jutalom | Kitermelve |
| --- | --- | --- | --- | --- |
| 5. felezés | 2028 | 1 050 000 | 1,5625 BTC | 98,44 % |
| 6. felezés | 2032 | 1 260 000 | 0,78125 BTC | 99,22 % |
| 7. felezés | 2036 | 1 470 000 | 0,390625 BTC | 99,61 % |


Ahogy egyre több bitcoint bányásznak ki, a forgalomban lévő mennyiség folyamatosan nő egészen addig, amíg el nem éri a 21 000 000 bitcoin maximális készletet, amely várhatóan 2140 körül következik be. Mivel idővel egyre kevesebb új bitcoin jön létre, ha a kereslet növekszik, a Bitcoin ára emelkedhet. Ez arra is ösztönzi a bányászokat, hogy továbbra is biztosítsák a hálózatot a számítási kapacitásuk hozzájárulásával.

#### Mi az érvényes blokk hash a Bitcoinban?

A Bitcoinban a bányászok egy speciális kódot próbálnak megtalálni, amit úgy hívnak, hogy **blokk hash**. Ez a kód azonosítja a tranzakciós blokkot, és lehetővé teszi, hogy hozzáadják a blokklánchoz.

Minden blokk tartalmaz információkat a legutóbbi tranzakciókról, valamint az előző blokk hash-ét is. Ez összekapcsolja az összes blokkot, így egy láncot alkotnak az első blokktól (Genesis Block) a legfrissebbig.

A hash úgy működik, mint egy **digitális ujjlenyomat** az adott blokk adatainak. Ha bármilyen információ megváltozna a blokkban, az ujjlenyomat is megváltozna. Ez megkönnyíti bárki számára annak ellenőrzését, hogy a blokklánc tranzakciós előzményeit nem módosították, és segít a hálózat biztonságának fenntartásában.


> **Callout**
>
> Satoshi Nakamoto, a Bitcoin megalkotója bányászta ki a Genesis Blockot, amely összesen 50 bitcoint szabadított fel.


#### A verseny egy blokk kibányászásáért

A bányászok versenyeznek, hogy érvényes blokk hash-t találjanak. Az első bányász, aki megtalálja, hozzáadhatja az új blokkot a blokklánchoz, és megkapja a bitcoin jutalmat.

Ahhoz, hogy érvényes legyen, a blokk hash-nek alacsonyabbnak kell lennie, mint egy, a hálózat által meghatározott szám, amit nehézségi célnak hívnak. Mivel a hash-ek véletlenszerűek, a bányászoknak folyamatosan új bemeneteket kell próbálgatniuk, amíg nem találnak megfelelőt.

Ha túl sok bányász versenyezne, a blokkok túl gyorsan készülnének el. Ha túl kevés bányász venne részt, a blokkok megtalálása túl sokáig tartana. Azért, hogy a rendszer zökkenőmentesen működjön, a Bitcoin automatikusan módosítja a nehézségi szintet minden 2 016 blokk után (körülbelül kéthetente).

Ez a beállítás biztosítja, hogy átlagosan körülbelül 10 percenként kerüljön új blokk a blokkláncra.


> **Definition – A nehézségi szint meghatározása**
>
> A **nehézségi szint** a Bitcoin bányászatban azt méri, hogy mennyire nehéz érvényes blokk hash-t találni. A hálózat ezt a nehézséget minden 2 016 blokk után (körülbelül kéthetente) módosítja, hogy az új blokkok átlagosan 10 percenként kerüljenek a blokkláncra. Minél magasabb a nehézség, annál nehezebb a bányászoknak érvényes blokkot találni.


Azáltal, hogy érvényes blokk hash-t talál, a bányász bizonyítja, hogy elvégezte a szükséges munkát egy új blokk hozzáadásához a blokklánchoz. Ezt a folyamatot **Proof of Work** (PoW) néven ismerjük. Ez az a biztonsági mechanizmus, amely lehetővé teszi, hogy a Bitcoin megerősítse a tranzakciókat és új blokkokat adjon a blokklánchoz. Az a bányász, aki elsőként találja meg az érvényes hash-t, bitcoin jutalmat kap, amely tartalmazza a blokk jutalmat és az adott blokkban szereplő tranzakciós díjakat.

A Proof of Work (PoW) segít a Bitcoin biztonságának fenntartásában azáltal, hogy rendkívül költségessé teszi bárki számára a csalást vagy a hálózat irányításának átvételét. Ehelyett sokkal jövedelmezőbb a szabályokat követni.

A bányászok négy fő szerepet töltenek be:

1. **Tranzakciók gyűjtése**: A bányászok kiválasztják a hálózatra beküldött tranzakciókat, és egy jelölt blokkba helyezik őket.
1. **Proof of Work végrehajtása**: A bányászok versenyeznek, hogy megoldjanak egy nehéz matematikai feladványt egy érvényes blokk hash megtalálásával.
1. **A blokk sugárzása**: Az első bányász, aki érvényes megoldást talál, megosztja az új blokkot a hálózattal.
1. **Jutalmak szerzése**: Ha a blokk érvényes, hozzáadják a blokklánchoz, és a bányász újonnan létrehozott bitcoint, valamint tranzakciós díjakat kap jutalmul.

Világszerte sok bányász próbálja egyszerre létrehozni a következő blokkot. Amikor egy bányász érvényes megoldást talál, a hálózat ellenőrzi a blokkot. Ha minden rendben van, hozzáadják a blokklánchoz. A többi versengő blokkot elvetik. Ez a folyamat biztosítja a hálózat egyetértését és megakadályozza a dupla költést.

* A bányászok olyan számítógépek, amelyek segítenek fenntartani és frissíteni a Bitcoin főkönyvét.
* Összegyűjtik a tranzakciókat, és egy blokkba csoportosítják őket. Ezután a blokk adatait egy hash algoritmuson futtatják át, hogy létrehozzanak egy egyedi kódot, amit hash-nek neveznek.
* A bányászok ezt a folyamatot sokszor megismétlik, hogy olyan hash-t találjanak, amely megfelel a Bitcoin szabályainak. Az első bányász, aki érvényes hash-t talál, újonnan létrehozott bitcoint kap jutalmul, és az ő blokkja kerül be a blokkláncba.
* Minden blokk hash-e az előző blokkhoz is kapcsolódik. Ha valaki megpróbálna megváltoztatni egy korábbi tranzakciót, a hash-ek már nem egyeznének, és a hálózat elutasítaná a módosított láncot. Ez az, ami biztonságossá teszi a Bitcoin főkönyvét.
