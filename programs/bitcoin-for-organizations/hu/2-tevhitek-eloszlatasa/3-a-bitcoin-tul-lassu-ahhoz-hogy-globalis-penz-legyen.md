# 2.3 A Bitcoin túl lassú ahhoz, hogy globális pénz legyen.

> A jövőbelátók egy olyan jövőt látnak, ahol az emberek otthonról dolgoznak, interaktív könyvtárak és multimédiás tantermek léteznek. Elektronikus városi gyűlésekről és virtuális közösségekről beszélnek… Az igazság az, hogy egyetlen online adatbázis sem fogja helyettesíteni a napi újságodat, egyetlen CD-ROM sem veheti át egy hozzáértő tanár szerepét, és egyetlen számítógépes hálózat sem fogja megváltoztatni a kormányzat működését.  
_Clifford Stroll_

17 évvel később a Newsweek megszüntette a nyomtatott kiadást, és kizárólag online lett elérhető. Képzeld el, milyen lehetett 1974-ben élni, amikor először létrehozták a Transmission Control Protocolt (TCP).

Senki sem látta előre az okostelefont, az összes alkalmazásával, a kezedben. Senki sem számított a navigációs rendszerre az autódban.

Az internet nem egy lépésben jelent meg, hanem fokozatosan, protokollok és rétegek fejlődéseként. Ezek a fejlődések az alapokra épültek, de főként nem változtatták meg a TCP-t.

> Ahogy a jövő kommunikációs platformjaira való átállást nézem, látom, hogy az internetes protokollok szépsége abban rejlik, hogy elválasztják a szolgáltatás és a technológia rétegeit.  
_Michael K Powell_



##### Hasonlítsd össze a Bitcoin fejlődését az internetével

A TCP szükséges volt, de nem volt elégséges minden más internetes dolog megjelenéséhez. A Bitcoin fejlődése hasonló utat látszik követni. A nyílt rendszerek ellenállóbbnak és sikeresebbnek tűnnek, ha rétegekben fejlesztik őket, bár az alapok lerakása és az elterjedés között sok idő is eltelhet. Az egyben megoldások nem tűnnek olyan hatékonynak a nyílt rendszerekben, mint azok, amelyeket protokollokra épülő rétegekben hoznak létre. Ahogy senkinek sem kellett újraépítenie az internetet csak azért, mert a filmeket nem lehetett TCP-n keresztül streamelni, valószínűleg így lesz ez a Bitcoinnal is.

Már most is számos második rétegű protokoll létezik a Bitcoin tetején, és sok alkalmazás működik ezekre a második rétegű protokollokra építve (lásd a 201.4-es szakaszt ezek részleteiért).

Ahelyett, hogy arra koncentrálnánk, mit nem tud ma a bitcoin és a Bitcoin hálózat, gondoljunk arra, hogy mit lehet már most is megtenni, és hasonlítsuk össze azzal, amit 10 évvel ezelőtt tudott. Végezze el ezt a gyakorlatot az internettel is 1985-től 1995-ig, majd nézze meg, mennyivel gyorsabb lett az internet a következő 30 évben, és milyen alkalmazások váltak lehetővé. Ezt a felismerést használja fel arra, hogy előrevetítse a Bitcoin jövőjét, és képzelje el, milyen lehet akár csak 10 év múlva, vagy 30 év múlva, ha a képzelete addig elér.



##### Hasonlítsd össze a Bitcoint a jelenlegi globális pénzrendszerrel

Az a központi állítás, hogy a Bitcoin túl lassú ahhoz, hogy globális pénz legyen, vitathatóan igaz, ha csak a Bitcoin alapszintjére korlátozódunk. Az is igaz, hogy a jelenlegi pénzrendszereink alapszintje is túl lassú lenne globális pénznek, ha hasonló korlátozás azt jelentené, hogy nem épülne rá semmilyen fizetési infrastruktúra a magánbankok és fizetési szolgáltatók, például a Visa és a Mastercard által. A jelenlegi rendszerünk is rétegekre épül, így várható, hogy a jövő is hasonló lesz. Bizonyos tervezési kompromisszumok, például a bizalom, a sebesség és a költség között, átültethetők lehetnek a rendszerek között, amelyek ugyanazokat a megoldásokat szállítják, bár különböző értékjelzőket mozgatnak.

A meglévő második rétegű megoldások közül néhány közvetlenül kezeli a sebesség problémáját, például a Liquid és a Lightning Network (lásd a 201.4-es szakaszt a részletekért). A Liquid gyorsabb és olcsóbb, mint a Bitcoin blokklánc, a Lightning Network pedig még gyorsabb és olcsóbb, mint a Liquid. A második rétegek elterjedése, mindegyik különböző kompromisszumokkal, várható és egészséges.

Valószínűleg még több második és harmadik réteg lesz, és ezekre épülő alkalmazások robbanásszerűen fognak megjelenni, ahogy az internet fejlődése során is történt.



##### Motiváció

Amikor ez a kritika felmerül, érdemes megfontolni, hogy a kritikusnak van-e más motivációja. Például, van-e egy új vagy eltérő blokklánc projektje? Ez hasonlítható ahhoz, mintha valaki egy jobb Transmission Control Protocolt próbálna eladni.

A skálázhatósági, vagy blokklánc trilemmát először Vitalik Buterin vetette fel 2017-ben. Eszerint a blokklánc tervezésében mindig kompromisszum van a decentralizáció, a biztonság és a skálázhatóság tulajdonságai között. Bárki, aki azt kritizálja, hogy a Bitcoin túl lassú, és hogy van egy gyorsabb megoldása egy első rétegű blokkláncban, az valamilyen biztonságot vagy decentralizációt fog feláldozni ennek érdekében. Bár egy más célra tervezett blokklánc esetében ez a kompromisszum értelmes lehet, egy globális pénz esetében a prioritási sorrendnek a következőnek kell lennie:


> **Light**
>
> * **Decentralizáció**
>   * Lehetővé teszi a megbízható közvetítők eltávolítását
> * **Biztonság**
>   * Megakadályozza, hogy rosszindulatú szereplők manipulálják a tranzakciókat vagy a főkönyvet
> * **Skálázhatóság**
>   * Lehetővé teszi, hogy a rendszer gazdaságosan bővüljön felhasználókban és sebességben


Az első két tulajdonság teremti meg azt a környezetet, ahol kibocsátás lehetséges kibocsátók nélkül, fizetés közvetítők nélkül és letétkezelés kezelők nélkül.

A Bitcoin a három blokklánc tervezési tulajdonság közül a megfelelő kompromisszumot választja, tekintve, hogy célzott felhasználása a globális pénz, és a skálázhatósági és sebességbeli kompromisszumokat rétegekkel kezeli.

> Satoshi rájött, hogyan lehet a digitális pénz integritását megvédeni megbízható közvetítők nélkül – nincs szükség kibocsátókra, közvetítőkre vagy kezelőkre.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
