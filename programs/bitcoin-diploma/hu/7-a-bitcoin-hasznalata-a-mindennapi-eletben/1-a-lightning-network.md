# 7.1 A Lightning Network

A Lightning Network egy fizetési rendszer, amely lehetővé teszi a felhasználók számára, hogy gyorsan és olcsón küldjenek és fogadjanak bitcoint. Úgy működik, hogy létrehoznak egy közös pénztárcát, ahová mindkét fél elhelyez némi bitcoint. Ezután korlátlan számú tranzakciót hajthatnak végre egymás között anélkül, hogy mindegyiket rögzíteni kellene a fő blokkláncon. Így elkerülik, hogy minden egyes tranzakciót ellenőrizni és blokkokba foglalni kelljen, ami gyorsabbá és költséghatékonyabbá teszi a folyamatot. Az alacsonyabb díjaknak köszönhetően a Lightning Network kis összegű fizetésekre is alkalmas, amelyek láncon nem mindig lennének megvalósíthatók. Amikor a felek úgy döntenek, hogy befejezik az együttműködést, csak a végső egyenleget rögzítik a blokkláncon.

Képzelj el egy napot egy kávézóban dolgozva. Mivel hosszabb ideig maradsz, nyitsz egy számlát, és előre fizetsz, ahelyett, hogy minden rendelésnél külön fizetnél. A nap végén te és a tulajdonos átnézitek a számlát, hogy rendezzétek a végösszeget. Ha a letéted több, mint amennyit elköltöttél, visszakapod a különbözetet; ha többet költöttél, akkor kifizeted a fennmaradó összeget.

Ez a rendszer több résztvevőre is kiterjeszthető. Például egyik alkalommal, amikor a kávézóba mész, magaddal viszel egy barátot, akit a pultos nem ismer, így nem tud neki számlát nyitni. Felajánlod a barátodnak, hogy a te meglévő számládat használja a fogyasztására, és megegyeztek, hogy ő majd külön rendezi veled. Most képzeld el, hogy emberek ezrei teszik ugyanezt egyszerre, lehetővé téve, hogy mások is használják a meglévő számlákat, hogy még több emberhez kapcsolódjanak — így működik a Lightning Network!

A Lightning segítségével bárkinek küldhetsz fizetést a hálózaton, nem csak annak, akivel közvetlenül megosztott számlád van — feltéve, hogy található útvonal a két fél között. A fizetésed végighalad a hálózaton, amíg el nem jut a címzetthez, még akkor is, ha nincs közvetlen csatornád vele.

Nézzük meg, mi a különbség a láncon (on-chain) és a láncon kívüli (off-chain) tranzakciók között.

##### Láncon történő tranzakciók

Ezek a tranzakciók közvetlenül a Bitcoin blokkláncon történnek. Általában körülbelül 10 percet vesz igénybe a megerősítésük, és a díjak a tranzakció méretétől (virtuális bájtban) függenek. Ezek biztonságosabbak, de lassabbak, mivel a hálózat konszenzusára van szükség.

##### Lightning Network tranzakciók

Ezek a tranzakciók egy külön hálózaton zajlanak, amely a Bitcoin blokkláncára épül. Gyorsabban és alacsonyabb díjakkal teljesülnek. Olyan esetekben használják őket, amikor a tranzakciók sebessége és költsége fontosabb szempont. A láncon történő tranzakciókhoz képest kevésbé biztonságosak.


|  | Bitcoin hálózat | Lightning Network |
| --- | --- | --- |
| Meghatározás | Egy decentralizált digitális hálózat, amely kriptográfiát használ a pénzügyi tranzakciók biztonságossá tételéhez. | Egy második rétegű fizetési protokoll, amely a Bitcoin blokkláncán működik, lehetővé téve a gyorsabb és olcsóbb tranzakciókat. |
| Előnyök | Decentralizált és biztonságos. Nincsenek visszaterhelések vagy csalások. Használható álnéven is. Globális elfogadottság. | Gyorsabb és olcsóbb tranzakciók. Nagyobb skálázhatóság. A láncon kívüli tranzakciók nem terhelik a blokkláncot. |
| Hátrányok | Lassú tranzakciós idők. Magas díjak bizonyos tranzakciótípusoknál. Bonyolult a kezdők számára. | Előfordulhat, hogy meg kell bízni a csatorna üzemeltetőiben. A csatornák megnyitásához és lezárásához láncon történő tranzakció szükséges. |
