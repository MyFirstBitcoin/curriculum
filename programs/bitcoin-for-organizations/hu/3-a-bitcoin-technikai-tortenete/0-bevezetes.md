# 3.0 Bevezetés

> **Dark – A Bitcoin White Paper összefoglalója**
>
> **Egy tisztán peer-to-peer alapú elektronikus készpénz** lehetővé tenné, hogy az online fizetések közvetlenül egyik féltől a másikhoz jussanak el pénzügyi intézmény közbeiktatása nélkül.**A digitális aláírások a megoldás egyik részét biztosítják**, de a fő előnyök elvesznek, ha egy **megbízható harmadik fél** továbbra is szükséges a dupla költés megakadályozásához. Mi egy megoldást javaslunk a dupla költés problémájára egy **peer-to-peer hálózat** segítségével. A **hálózat időbélyeggel látja el a tranzakciókat**, azáltal, hogy azokat egy folyamatosan növekvő láncba hash-eli, amely **hash-alapú proof-of-work** bizonyítékot használ, így olyan nyilvántartás jön létre, amelyet nem lehet megváltoztatni anélkül, hogy újra el ne végeznénk a **proof-of-work** műveletet. A leghosszabb lánc nemcsak az események sorrendjének bizonyítékaként szolgál, hanem annak is, hogy az a legnagyobb CPU teljesítményből származik. Amíg a CPU teljesítmény többségét olyan csomópontok irányítják, amelyek nem működnek együtt a hálózat megtámadásában, ők fogják létrehozni a leghosszabb láncot és megelőzik a támadókat.**Maga a hálózat minimális struktúrát igényel. Az üzenetek legjobb tudás szerint kerülnek továbbításra, és a csomópontok szabadon elhagyhatják vagy újra csatlakozhatnak a hálózathoz**, elfogadva a leghosszabb proof-of-work láncot annak bizonyítékaként, hogy mi történt, amíg távol voltak.


A Bitcoin nem a semmiből jelent meg, hanem sokak korábbi munkájára épült az elmúlt évtizedekben. Ez a modul bemutatja azokat az internetes alapokat, amelyekre a Bitcoin épít, valamint azokat a kutatásokat és fejlesztéseket, amelyeket a whitepaper is elismer.

A 70-es években egy csoport felismerte, hogy különösen az amerikai kormány igyekszik korlátozni a kriptográfia elérhetőségét, ezért elhatározták, hogy ezt a technológiát mindenki számára elérhetővé teszik, hogy megvédhessék magánéletüket az interneten. Ezek közül a korai úttörők közül néhányan egy digitális, 'jó pénz' rendszer lehetőségeit is vizsgálták, amely érték tárolására és cseréjére szolgálhatott volna a kibontakozó interneten. Friedrich Hayek – az osztrák közgazdaságtan egyik vezető alakja – már jóval az internet előtt elképzelte, milyen lenne egy szabadpiaci versenyen alapuló ideális valuta, de úgy vélte, hogy ez technikailag és politikailag kivitelezhetetlen. Ez a csoport, amely később Cypherpunkként vált ismertté, a digitális magánélet mellett Hayek digitális pénzre vonatkozó vízióját is megpróbálta megvalósítani, de ezek a próbálkozások mindaddig kudarcot vallottak, amíg Satoshi meg nem osztotta ötleteit a levelezőlistán.

* TCP/IP protokoll (1976)
* Nyilvános kulcsú kriptográfiai protokollok – Ralph Merkle (1980)
* Digicash – David Chaum (1989)
* Digitális időbélyegzés (90-es évek)
* Hashcash – Adam Back (1997)
* BitTorrent – Bram Cohen (2001)
* Újrahasználható POW – Hal Finney (2004)
* Bitcoin Whitepaper – Satoshi Nakamoto (2008)

A Bitcoin fejlődésére nagy hatással volt a Cypherpunk mozgalom megjelenése az 1990-es években. Több kriptográfiai technológiát fejlesztettek ki, köztük a nyilvános kulcsú kriptográfiát, amely lehetővé tette a felhasználók számára, hogy biztonságosan és privát módon kommunikáljanak és osszanak meg információkat. Az itt bemutatott fejlesztések és a résztvevő személyek többsége ennek a csoportnak a tagja volt.

A digitális készpénz iránti igényt is felismerték, és több próbálkozás történt a létrehozására, de ezeknek voltak olyan korlátai, amelyek miatt nem lettek sikeresek. Satoshi Nakamoto zsenialitása abban rejlett, hogy ezeket a képességeket összefogta, és néhány saját innovációjával kiegészítve megalkotta a ma is használt Bitcoin protokollt. A következő szakaszokban bemutatunk néhány ilyen fejlesztést, és elmagyarázzuk, hogyan járultak hozzá a Bitcoin tervezéséhez. Megbeszéljük azt is, hogy mik voltak azok a hiányzó láncszemek, amelyeket Satoshi sikeresen megoldott.
