# 6.4 Tranzakciók fogadása és küldése

A Bitcoin-tranzakció a bitcoin tulajdonjogának átruházása egy új tulajdonosra. Fontos megjegyezni, hogy nem maguk az érmék kerülnek átruházásra, hanem azok tulajdonjoga: más szóval, a jog, hogy el lehessen költeni őket. Minden alkalommal, amikor egy tranzakció bekerül egy blokkba, a hálózat összes csomópontja frissíti a nyilvános főkönyv helyi másolatát, hogy tükrözze a tulajdonosváltást. Ebben a tekintetben a Bitcoin-tranzakció inkább hasonlít egy ingatlan (vagy más vagyontárgy) adásvételére, mint egy készpénzes tranzakcióra.

A bitcoin "elküldéséhez" a küldő aláír egy üzenetet a privát kulcsával, jelezve a hálózatnak, hogy a bitcoin jogos tulajdonosa átruházta annak tulajdonjogát a címzettre.

A bitcoin mostantól a címzett címéhez kötődik, így ő lesz a bitcoin tulajdonosa, és csak az új tulajdonos költheti el őket a saját privát kulcsával.

Új Bitcoin-tranzakciókat indítanak el világszerte a pénztárcákból, de nincs központi fizetési feldolgozó. Ehelyett a bányászok versenyeznek azért, hogy rögzítsék a tranzakciókat a főkönyvben.

Tegyük fel, hogy Gábor tartozik Elenának 0,5 BTC-vel, és készen áll arra, hogy visszafizesse. Mindkettőjüknek van digitális pénztárcája.

1. Elena megosztja a címét Gáborral.
1. Gábor a pénztárca szoftverével létrehozza a tranzakciót, amely tartalmazza Elena címét, az átutalandó összeget (0,5 BTC), valamint a bányász díját. A magasabb díjak növelik annak esélyét, hogy egy bányász a következő blokkba beilleszti a tranzakciót.
1. A tranzakció aláírása után azt továbbítják a hálózatra, ahol a csomópontok ellenőrzik. Megnézik, hogy Gábornak van-e elegendő fedezete, és valóban ő-e az érmék jogos tulajdonosa, amelyeket el akar költeni. Ha nem, azonnal elutasítják a tranzakciót.
1. Miután a tranzakciót ellenőrizték, a bányászok eldöntik, hogy hozzáadják-e a következő blokkhoz, általában a kiválasztott díj alapján. Amint a tranzakció bekerül egy blokkba, hozzáadják a blokklánchoz, és az összeg átkerül Elena címére.
1. A tulajdonjog átkerült Elenához. Most már a saját privát kulcsával költheti el az összeget.

_Fontos megjegyezni, hogy ha a tranzakció befejeződött, azt nem lehet visszafordítani._


> **Note – Hogyan működik egy Bitcoin-tranzakció**
>
> 1. Valaki tranzakciót kezdeményez
> 1. A tranzakciót továbbítják a P2P számítógépekhez (csomópontokhoz)
> 1. A bányászok ellenőrzik a tranzakciót
> 1. A tranzakciókat egy adatblokkba kombinálják
> 1. Az új blokk hozzáadódik a meglévő blokklánchoz
> 1. A tranzakció befejeződött



> **Note – Bitcoin-tranzakciók fogadása**
>
> A bitcoin fogadásához meg kell adnod a küldőnek egy Bitcoin nyilvános címet. Ez egy egyedi betű- és számsorozat, amely a pénztárcádat jelöli, és a Bitcoin-hálózaton azonosítja azt.
>
> A nyilvános címedet megtalálod, ha megnyitod a Bitcoin pénztárcádat, és keresel egy "Fogadás" vagy "Befizetés" lehetőséget.
>
> Ezután többféleképpen is megoszthatod a Bitcoin-címedet:
>
> 1. **Cím másolása és beillesztése**: Kijelölheted a címet, majd a "Másolás" gombra kattintva kimásolhatod, és beillesztheted egy e-mailbe vagy üzenetbe.
> 1. **Oszd meg a Bitcoin pénztárcád linkjét**: Egyes Bitcoin pénztárcák lehetővé teszik, hogy létrehozz egy linket a pénztárcádhoz, amit megoszthatsz a küldővel. Ők rákattinthatnak a linkre, hogy elérjék a pénztárcádat és küldjenek bitcoint.
> 1. **Oszd meg a QR-kódot**: Ha a küldőnek van okostelefonja Bitcoin pénztárca alkalmazással, be tudja olvasni a QR-kódot, hogy megkapja a Bitcoin-címedet.


Miután a küldő megkapta a címedet, elküldheti neked a bitcoint úgy, hogy beírja a címedet és a kívánt összeget. A bitcoin ezután az ő pénztárcájából a tiédbe kerül.

A tranzakciót a Bitcoin-hálózat megerősíti, ami általában körülbelül 10 percet vesz igénybe. Nagyobb biztonság érdekében ajánlott két megerősítésre várni, ami körülbelül 20 perc.


> **Note – Bitcoin-tranzakciók küldése**
>
> A bitcoin küldéséhez néhány dologra lesz szükséged: egy Bitcoin pénztárcára, a címzett nyilvános címére, és a küldeni kívánt bitcoin mennyiségére.
>
> 1. Nyisd meg a Bitcoin pénztárcádat.
> 1. Navigálj a "Küldés" gombra, és illeszd be a címzett címét a "Címzett" mezőbe. Alternatívaként be is olvashatod a QR-kódot, ha a címzett ilyet ad meg.
> 1. Írd be a küldeni kívánt bitcoin mennyiségét az "Összeg" mezőbe.
> 1. Ellenőrizd le még egyszer a címzett címét és a küldendő összeget. Ne feledd, a tranzakciók visszafordíthatatlanok!
> 1. Mielőtt a "Megerősítés és küldés" gombra kattintanál, javasoljuk, hogy még egyszer ellenőrizd a tranzakció részleteit, hogy biztosan a megfelelő összeget küldöd a megfelelő címre.
> 1. Továbbítsd a tranzakciót, és várd meg, amíg a hálózat megerősíti azt.
>
> Most már tudod, hogyan értékeld, válaszd ki és állítsd be az önállóan kezelt Bitcoin pénztárcádat. A bitcoin küldését és fogadását a Bitcoin-hálózaton "on-chain" tranzakcióknak nevezik. Ez azért van, mert ezek a tranzakciók a fő Bitcoin-hálózaton történnek, és a blokkláncban kerülnek rögzítésre.
>
> Az on-chain tranzakciók a legbiztonságosabb módjai a bitcoin használatának, mivel a hálózat decentralizált ellenőrzést biztosít.
>
> Azonban az on-chain tranzakciók lassabbak, és a bányász díja miatt jelentősen drágábbak is lehetnek más lehetőségekhez képest (amelyekről a 7. modulban lesz szó).


#### Tevékenység: Tranzakciók működés közben

https://qr.myfirstbitcoin.org/transactions.pdf

**Ez egy együttműködésen alapuló gyakorlat, amely leegyszerűsíti a Bitcoin-tranzakcióban részt vevő emberek alapvető szerepeit.**

###### Főbb pontok

1. Minden bitcoin tranzakcióban négyféle résztvevő van: a küldő, a címzett, a bányászok és a csomópont üzemeltetők.
1. A küldőnek jóvá kell hagynia (kriptográfiailag alá kell írnia) a **bitcoin mennyiségét** amit küldeni akar, ÉS a **konkrét címet** amire küldeni akar.
1. A címzettnek meg kell adnia egy **érvényes címet** a küldőnek, ÉS ellenőriznie kell, hogy a tranzakció sikeresen megerősítésre került-e a blokkláncon.
1. A bányászok gondoskodnak arról, hogy minden feltétel érvényes legyen, mielőtt a tranzakciókat a jövőbeli blokkokhoz adnák.
1. A node üzemeltetők ellenőrzik, hogy a kibányászott blokkok érvényesek-e, mielőtt frissítenék a blokklánc (a főkönyv) saját verzióját.

###### Diáktipp

Forgassatok végig mind a négy szerepet, hogy megtapasztaljátok, mit csinál minden résztvevő.
