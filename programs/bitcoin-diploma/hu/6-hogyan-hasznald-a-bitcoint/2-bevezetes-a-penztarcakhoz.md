# 6.2 Bevezetés a pénztárcákhoz

A fizikai pénzzel ellentétben a bitcoinok valójában nincsenek egy Bitcoin tárcában. Ehelyett a Bitcoin hálózat által folyamatosan ellenőrzött és biztosított elosztott főkönyvön léteznek. Akkor hogyan lehet birtokolni bitcoint?

Csak akkor vagy a bitcoinod tulajdonosa, ha te irányítod azokat a privát kulcsokat, amelyek lehetővé teszik, hogy tranzakciókat írj alá, és a bitcoinod tulajdonjogát másnak átadd. Ez maga a bitcoin küldésének folyamata.

Nézzünk meg két fogalmat, amelyekre a következő kifejezés használatakor hivatkozunk: **tárca**:

* Egy mester privát kulcs, amely olyan, mint egy jelszó, ebből generálódnak a publikus kulcsok, amelyek olyanok, mint az e-mail címek. A publikus címedet megoszthatod másokkal, hogy bitcoint fogadj vagy küldj, de a privát kulcsodat soha ne oszd meg!
* A mobil vagy asztali felület, amelyen keresztül kapcsolatba léphetsz a Bitcoin hálózattal, ellenőrizheted a bitcoin egyenlegedet, tranzakciókat küldhetsz és fogadhatsz, valamint továbbíthatod azokat a hálózatra. A különböző típusú tárcákat, azok előnyeit és hátrányait a következő szakaszokban ismertetjük.

#### Önőrzéses vs Letétkezelő Tárcák

Mielőtt részleteznénk a különböző Bitcoin tárcatípusokat és azok jellemzőit, fontos különbséget tenni az önőrzéses és a letétkezelő tárcák között. Mindegyik típusnak megvannak a maga előnyei, kockázatai és a bitcoin feletti ellenőrzés szintje. Az önőrzéses azt jelenti, hogy a felhasználó birtokolja a privát kulcsokat, és valóban ő irányítja a bitcoinját; a letétkezelő tárcáknál egy harmadik fél tartja a bitcoint a felhasználó nevében.


| Típus | Ellenőrzés | Előnyök | Kockázatok |
| --- | --- | --- | --- |
| Önőrzéses | A felhasználó | Teljes ellenőrzés a pénz és a tranzakciók felett, nincs jóváhagyási folyamat vagy számlafagyasztás, nincs vállalati vagy állami kontroll, védett az elkobzás ellen. | Nincs visszaállítás, ha az emlékeztető kifejezés elveszik, a teljes felelősség a felhasználóra hárul. |
| Letétkezelő | A harmadik fél szolgáltató | Könnyű visszaállítás, ha elveszik a hozzáférés, egyszerűbb ügyfélszolgálat. | A pénz az internethez kapcsolódik, így sérülékenyebb a hackelésre. A letétkezelő befagyaszthatja a számlákat. |


Egy önőrzéses tárcában (más néven nem letétkezelő tárca) csak te rendelkezel a tárca kulcsaival, és teljes mértékben te irányítod, mi kerül be vagy ki. Ezzel szemben egy letétkezelő tárcában valaki más birtokolja a privát kulcsot, így teljes hozzáférése van ahhoz a bitcoinhoz, amit az a szolgáltató a nevedben kezel.

* Az önőrzés olyan, mintha saját bankod lennél. A tranzakciókat nem érinti a felügyelet és az ellenőrzés
* Az önőrzés biztosítja, hogy harmadik felek ne kobozhassák el a bitcoinodat.
* Az önőrzés nyugalmat ad bizonytalan időkben, mert tudod, hogy a bitcoinod biztonságban van.

Fontos, hogy mindenki a saját igényeinek megfelelő tárcatípust válasszon. Néha nehéz megkülönböztetni, hogy önőrzéses vagy letétkezelő tárcát telepítünk-e. Ez a táblázat bemutatja a különbségeket a telepítési folyamatban.


| Típus | 1. lépés: Válassz | 2. lépés: Telepítsd | 3. lépés: Hozd létre | 4. lépés: Biztosítsd |
| --- | --- | --- | --- | --- |
| Önőrzéses | Válassz önőrzéses tárcát | Kövesd a tárca utasításait | Generálj egy helyreállítási kifejezést | Tárold a helyreállítási kifejezést biztonságos helyen |
| Letétkezelő | Válassz letétkezelő tárcát | Kövesd a tárca utasításait | Hozz létre egy fiókot | N/A |


„**Nem a te kulcsaid, nem a te pénzed**” – ez egy népszerű mondás a bitcoin tulajdonosok körében. Arra utal, hogy ha nincs közvetlen irányításod a Bitcoin tárcádhoz tartozó privát kulcsok felett, akkor nincs valódi tulajdonod a coinok felett.

Aki hozzáfér a privát kulcsaidhoz, az birtokolja a bitcoinodat. Ezért rendkívül fontos, hogy megvédd őket, és távol tartsd a kíváncsi szemektől! A könyv későbbi részében bemutatunk néhány módszert, hogyan teheted ezt meg.

A továbbiakban kizárólag önőrzéses tárcákról lesz szó, ahol a felhasználó birtokolja a kulcsait, és teljes ellenőrzése van a bitcoinja felett.

Ne aggódj, ha bonyolultnak tűnik, vagy nem értesz mindent — ez egy utazás, és minél többet használod a Bitcoint, annál jobban meg fogod érteni!

#### A Bitcoin tárcák különböző típusai

Az, hogy hol jön létre és hol tárolódik a privát kulcsod, meghatározza, hogyan nevezzük a Bitcoin tárcákat. Ha a kulcsok az okostelefonodon vannak, akkor ez egy **mobil tárca**. Ha biztonságosan, egy dedikált eszközön vannak tárolva, akkor ez egy **hardveres tárca**.


| Típus | Leírás | Előnyök | Hátrányok | Példa felhasználó |
| --- | --- | --- | --- | --- |
| Online tárca | Webböngészőn keresztül érhető el | Bármilyen internetkapcsolattal rendelkező eszközről elérhető | Kevésbé biztonságos, mert feltörhető vagy kompromittálható | Gyakran kell hozzáférnie a tárcájához, és nem tárol benne sok pénzt |
| Mobil tárca | Mobil eszközre telepítve | Könnyen használható | Elveszhet, ha az eszközt ellopják vagy feltörik | Útközben kell tranzakciókat végeznie, és nem tárol benne sok pénzt |
| Asztali tárca | Asztali számítógépre telepítve | Kényelmes, és bárhonnan elérhető | Feltörhető, ha a számítógép fertőzött kártevővel | Nagyobb mennyiségű bitcoint szeretne tárolni, és magabiztosan használ asztali számítógépet |
| Hardveres tárca | Egy fizikai eszköz, amely offline tárolja a bitcoint | Biztonságosabb, mint az online tárcák, és offline is használható | Az eszközön lévő pénz elveszhet, ha nem visszaállítható | Nagyobb mennyiségű bitcoint szeretne tárolni, és hajlandó fizetni a nagyobb biztonságért |


Mivel a kulcsokat át lehet vinni egyik eszközről a másikra, a Bitcoin tárcád „státusza” nem állandó. Például, ha a tárcakulcsokat számítógépen hozom létre, majd később áthelyezem a telefonomra, az „asztali tárca” „mobil tárcává” válik.

A bitcoinod tárolásánál nem csak az számít, hogy ki rendelkezik a kulcsokkal — sok más kockázatot is figyelembe kell venni. Ezért fontos olyan tárolási megoldást találni, amely egyszerre biztonságos és kényelmes. Ha megvizsgálod a különböző tárcatípusok előnyeit és hátrányait, látni fogod, hogy nincs olyan tökéletes tárca, amely minden igényt kielégít.

##### Mire figyeljünk tárca választásakor

* **Biztonság**: Győződj meg róla, hogy a tárca erős biztonsági intézkedésekkel rendelkezik.
* **Adatvédelem**: Fontold meg, hogy a tárca igényel-e személyes adatokat.
* **Használhatóság**: Olyan tárcát válassz, amely könnyen használható és átlátható.
* **Kompatibilitás**: Győződj meg róla, hogy a tárca kompatibilis az eszközöddel.
* **Díjak**: Hasonlítsd össze a különböző tárcák által felszámított díjakat.
* **Hírnév**: Ellenőrizd a fejlesztők hírnevét, hogy megbízhatóak-e.
* **Ellenőrzés**: Egyes tárcák nagyobb kontrollt adnak a privát kulcsok felett.

##### Nyílt forráskódú vagy zárt forráskódú

Egy másik fontos szempont a Bitcoin tárca kiválasztásakor, hogy az alkalmazás vagy szoftver nyílt forráskódú-e. Ez azért lényeges, mert a nyílt forráskódú projektek lehetővé teszik a közösség számára a kód átvizsgálását és a projekt folytatását, ha a fejlesztőcsapat abbahagyja a munkát. Ahogyan a Bitcoin kódja is teljesen nyitott mindenki számára, hogy átnézze, használja és módosítsa, ugyanígy a tárcád kódjának is nyílt forráskódúnak kellene lennie, ha abban tárolod a bitcoinodat.

#### Tevékenység: Bitcoin tárcák megbeszélése és értékelése


https://bitcoin.org/en/choose-your-wallet

_QR Code: Choose your wallet_


Látogasd meg a következő weboldalt: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Használd fel az újonnan megszerzett tudásodat a Bitcoin tárcákról, és válaszd ki azt, amelyik a legjobban megfelel az igényeidnek a ma megbeszélt szempontok alapján.
