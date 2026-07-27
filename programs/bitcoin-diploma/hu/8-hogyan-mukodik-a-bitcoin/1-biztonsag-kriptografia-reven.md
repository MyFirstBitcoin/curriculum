# 8.1 Biztonság kriptográfia révén

> Amit a Bitcoin ad nekünk, az egy szilárd ígéret: a program pontosan az előírtak szerint fog végrehajtódni.  
_Andreas M. Antonopoulos_

#### Nyilvános/magánkulcsú kriptográfia


> **Definition – A kriptográfia definíciója**
>
> **Kriptográfia** az az eljárás, amely során az információt titokká alakítjuk, amit csak a megfelelő emberek tudnak elolvasni.


* **Titkosítás** az a folyamat, amely során az információt kódolt formára alakítjuk, hogy csak az tudja elolvasni, akinek megvan a megfelelő kulcsa.
* **Visszafejtés** az a folyamat, amely során ezt a kódolt információt ismét olvashatóvá tesszük.

A hagyományos kriptográfiában két ember, akik privát módon szeretnének kommunikálni, először meg kell, hogy osszák egymással ugyanazt a titkos kulcsot, hasonlóan egy közös jelszóhoz. Az egyik fél ezt a kulcsot használja az üzenet titkosítására, mielőtt elküldi, a másik pedig ugyanazzal a kulccsal fejti vissza és olvassa el.

A rendszer problémája, hogy mindkét félnek már előre meg kell osztania a titkos kulcsot. Ha valaki más hozzáfér ehhez a kulcshoz, el tudja olvasni bármely elfogott üzenetet.

A Bitcoin ezt a problémát egy másik megközelítéssel oldja meg, amit nyilvános kulcsú kriptográfiának neveznek, ahol a felhasználóknak nem kell előre titkos kulcsokat megosztaniuk.

A nyilvános/magánkulcsú kriptográfia megoldja a titkok megosztásának problémáját. Jelszó megosztása helyett mindenkinek két kulcsa van: egy nyilvános kulcs és egy magánkulcs.

* A **nyilvános kulcs** bárkivel megosztható.
* A **magánkulcs** mindig titokban kell maradjon.

Ha János szeretne valamit elküldeni Árminnak, használhatja Ármin nyilvános kulcsát. Csak Ármin tudja azt feloldani a saját magánkulcsával. Még ha valaki el is kapja az üzenetet, nem tudja elolvasni vagy felhasználni a magánkulcs nélkül.

A Bitcoinban ezt a rendszert digitális aláírások létrehozására használják. Egy digitális aláírás bizonyítja, hogy a magánkulcs tulajdonosa hagyta jóvá a tranzakciót, hasonlóan ahhoz, mintha aláírnánk egy dokumentumot. Ez teszi lehetővé, hogy a Bitcoin tranzakciók biztonságosak és ellenőrizhetők legyenek harmadik fél megbízhatósága nélkül.

A Bitcoin tranzakciók során a bitcoin tulajdonjoga egyik címről a másikra száll át.

A titkosítást arra használják, hogy csak a bitcoin valódi birtokosa rendelkezzen jogosultsággal arra, hogy a pénzét másnak elküldje. Ez biztosítja, hogy a tulajdonát rosszindulatú szereplőktől védje.

További védelmi intézkedésként minden Bitcoin tranzakció automatikusan EGYEDI digitális aláírást kap. Ez az egyedi digitális aláírás manipulációbiztos technológián alapul, amely segíti a hálózatot abban, hogy ellenőrizze: valóban a bitcoin tulajdonosa, és nem valaki más küldte el azt.


> **Dark**
>
> Minden felhasználónak két kulcsa van: egy **magánkulcs**, amelyet **titokban tartanak**, és egy **nyilvános kulcs**, amely **megosztható másokkal**. A **magánkulcs** azonosítóként és tulajdonjog igazolásaként szolgál, megerősítve: „Ez a cím hozzám tartozik, és én rendelkezem felette.”


###### Hogyan működik egy Bitcoin tranzakció

1. **A tranzakció létrehozása**: A felhasználó elindít egy Bitcoin tranzakciót, megadva például a fogadó címét és az elküldendő bitcoin mennyiségét.
1. **Digitális aláírás létrehozása**: A küldő egyedi **digitális aláírást** hoz létre a saját **magánkulcsával**. Ez az aláírás egy egyedi kód, amely igazolja a tranzakció hitelességét.
1. **A tranzakció továbbítása**: Az aláírt tranzakciót továbbítják a Bitcoin hálózatnak, jelezve a bitcoin tulajdonjogának átruházási szándékát a küldőtől a fogadó felé.
1. **Ellenőrzés a hálózaton**: A Bitcoin hálózat csomópontjai megkapják a tranzakciót, és a fogadó **nyilvános kulcsát** a digitális aláírás hitelességének ellenőrzésére. a tranzakció esetében. Ugyanakkor a feladó **nyilvános kulcsát** használják az **digitális aláírás** ellenőrzésére.
1. **Megerősítés a Bitcoin hálózaton**: Ha az ellenőrzés sikeres, a tranzakció bekerül a főkönyvbe, amely minden tranzakció biztonságos és átlátható nyilvántartása. Amint megerősítik, a bitcoin tulajdonjoga hivatalosan átszáll a feladótól a címzettre.


> **Callout – Összefoglalás**
>
> A **digitális aláírás**, amelyet a feladó **privát kulcsával** hoz létre, bizonyítja, hogy a tranzakciót a bitcoin tulajdonosa hagyta jóvá. A Bitcoin hálózat ezután ellenőrizheti ezt a bizonyítékot, és rögzítheti a tranzakciót.


#### A hashelés magyarázata

Ne ijedj meg a technikai kifejezésektől és matematikai fogalmaktól! Tudjuk, hogy nem mindenki rajong a matematikáért, de lehet, hogy megleped magad, és rájössz, hogy még a legösszetettebb ötletek is megérthetők egy kis erőfeszítéssel.


> **Definition – A függvény definíciója**
>
> Egy **függvény** olyan, mint egy gép, amely információt vesz be, és valami újat hoz létre belőle. Az információ, amit a függvénynek adsz, az **bemenet**. Az új információ, amit a függvény létrehoz, a **kimenet**. A függvények segítenek a számítógépeknek feladatokat elvégezni és problémákat megoldani.


##### Mi az a függvény?

A függvény egy utasítássorozat, amely egy bemenetet vesz, és egy kimenetet állít elő. Gondolj rá úgy, mint egy receptre: ha követed a lépéseket a megfelelő hozzávalókkal, mindig kiszámítható eredményt kapsz.

A Bitcoinban a függvényeket tranzakciók feldolgozására és ellenőrzésére használják. Amikor valaki bitcoint küld, kriptográfiai függvények segítenek ellenőrizni, hogy a tranzakció érvényes-e, hogy a feladónak van-e elég egyenlege, és frissítik a Bitcoin főkönyv egyenlegeit. Ha a tranzakciót ellenőrizték és blokkba került, az a blokklánc állandó részévé válik.

##### Mi az az egyirányú függvény?

Az egyirányú függvény egy speciális típusú függvény, amelyet egy irányban könnyű kiszámolni, de visszafelé rendkívül nehéz. Például egy turmix elkészítése egyszerű, de a turmixot nem tudod visszaalakítani az eredeti hozzávalókká.

A Bitcoin biztonsága egyirányú függvényeken alapul. Ezeket használják a nyilvános és privát kulcsú kriptográfiában, lehetővé téve, hogy az emberek megosszák a nyilvános kulcsukat, miközben a privát kulcsukat titokban tartják. Még ha a nyilvános kulcs látható is, lehetetlen abból a privát kulcsot levezetni. Ez teszi a Bitcoin tranzakciókat biztonságossá.

##### Mi az a hash függvény?

A **hash függvény** olyan, mint egy titkos kódgép. Egy üzenetet vesz be, és kóddá alakítja.

###### Hogyan működik a hashelés a Bitcoin tranzakciókban

A Bitcoinban minden tranzakciót hash-sé alakítanak, mielőtt bekerülne a blokkláncba. A hash a tranzakció egyedi digitális ujjlenyomata. Ha valaki akár csak egy apró részt is megváltoztat a tranzakción, a hash teljesen megváltozik. Ez lehetővé teszi a hálózat számára, hogy könnyen észrevegye a manipulációt.

###### A hashelés szerepe a Bitcoin biztonságában

A hashelés segít megvédeni a Bitcoin hálózatot azáltal, hogy a tranzakciókat könnyen ellenőrizhetővé és csendben módosíthatatlanná teszi. Mivel minden tranzakciónak saját, egyedi hash-e van, a hálózat gyorsan észreveszi, ha valamit megváltoztattak.

A hash függvény adatokat vesz be, és egy fix hosszúságú szám- és betűsort, azaz hash-t állít elő. Ugyanaz a bemenet mindig ugyanazt a hash-t adja, de már egy apró változás is teljesen más eredményt hoz. Ez a tulajdonság lehetővé teszi, hogy a számítógépek ellenőrizzék, hogy az adatokat nem módosították.


> **Definition – A hashelés definíciója**
>
> **A hashelés** olyan, mint egy digitális adat ujjlenyomatának létrehozása. Ez az a folyamat, amikor egy digitális üzenetet fix hosszúságú kóddá alakítanak, amely egyedi azonosítóként szolgál. Ahogy egy ujjlenyomat azonosít egy embert, úgy egy hash azonosít egy digitális üzenetet.


A **kimenet**, vagyis a hash, mindig ugyanolyan hosszú, függetlenül attól, hogy az eredeti információ milyen hosszú volt. A Bitcoin néhány speciális hash függvényt használ, például a **SHA-256** és a **RIPEMD160**.

Néhány példa alább:

* A(z) SHA256 hash-e ennek a szövegnek **hello world**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* A karakterlánc SHA256 hash értéke: **hello world.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Figyeld meg, hogy a bemenetben egy apró változtatás teljesen megváltoztatja a kimenetet az elsőhöz képest
* A letölthető iso fájl SHA256 hash értéke: **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Ez a bemenet egy hatalmas fájl, mégis a kimenet továbbra is ugyanakkora, fix hosszúságú

A hash-elést elképzelheted úgy is, mint egy kottát, amely megragadja egy zenemű lényegét. Ahogy egy kotta egy dallam egyedi ábrázolása, úgy a hash érték is egy adat egyedi ábrázolása.

Egy zenész a kotta és az előadás összehasonlításával meg tudja állapítani, hogy az előadás pontos-e. Hasonlóképpen, ha az átvett adat hash értékét összevetjük az eredeti hash értékkel, megállapítható, hogy az adat megváltozott-e az átvitel során.

Ahogy egy apró eltérés a zenei előadásban is máshogy hangzik, úgy az eredeti adaton végzett legkisebb változtatás is teljesen más hash értéket eredményez. Ez teszi a hash-elést hatékony eszközzé a Bitcoin tranzakciók integritásának és hitelességének biztosítására.

A **nyilvános kulcs** hash-eléssel történő kódolása növeli az információ biztonságát azáltal, hogy azt fix hosszúságú, olvashatatlan formátumba alakítja. A Bitcoin a SHA-256 és RIPEMD160 algoritmusokat használja a nyilvános címek előállításához. Az így kapott kimenet egyedi azonosítóként szolgál a **nyilvános kulcshoz** , és segít biztosítani a főkönyvben tárolt tranzakciók integritását és biztonságát. Az információ ilyen módon történő titkosításával nehezebbé válik az illetéktelenek számára az adatokhoz való hozzáférés és azok manipulálása.

##### A hash függvény tulajdonságai

* **Determinált**: Ugyanazok az összetevők mindig ugyanazt a turmixot eredményezik. Ugyanígy, ugyanaz az adat mindig ugyanazt a hash-t adja.
* **Előképkép-ellenálló**: Ha csak a turmixot látod, nem tudod kitalálni, pontosan milyen gyümölcsökből készült. Hasonlóképpen, ha csak a hash áll rendelkezésedre, nem tudod meghatározni az eredeti adatot.
* **Lavina effektus**: Ha az összetevőknek akár csak egy kis részét is megváltoztatod, teljesen más turmixot kapsz. A hash-elésnél egy nagyon apró adatváltozás is teljesen más hash-t eredményez.
* **Ütközés-ellenálló**: Rendkívül nehéz két különböző összetevő-kombinációt találni, amely pontosan ugyanazt a turmixot eredményezi. Ugyanígy, rendkívül valószínűtlen, hogy két különböző adat ugyanazt a hash-t adja.
* **Gyorsan ellenőrizhető**: A turmix elkészítése gyors, és könnyű ellenőrizni, hogy valóban turmix lett-e. A hash függvények gyorsan számíthatók és bárki számára könnyen ellenőrizhetők.

#### Gyakorlat: SHA 256 hash generálása


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Kíváncsi vagy, hogyan működik a hash-elés? Olvasd be a QR-kódot, és azonnal generálj SHA256 hash-t bármilyen általad választott szóból, mondatból vagy bemenetből. A hash függvények olyanok, mint a digitális ujjlenyomatok: egyirányúak, vagyis ha valamit hash-elsz, azt nem lehet visszafejteni. Próbáld ki, és győződj meg róla magad!
