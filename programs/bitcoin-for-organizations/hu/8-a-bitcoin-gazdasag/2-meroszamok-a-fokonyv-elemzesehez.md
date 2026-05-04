# 8.2 Mérőszámok a főkönyv elemzéséhez

Mivel a Bitcoin átláthatósága eltér a hagyományos pénzügyi rendszerekétől — ahol a pénzmozgások nagy része intézményi ajtók mögött, zárt körben zajlik —, ezért egy gazdag on-chain analitikai területet hoz létre, ahol a hálózati szintű adatok betekintést nyújtanak a felhasználói viselkedésbe, a pénzáramlásokba és a hosszú távú trendekbe. Ezek a mutatók segíthetnek konkrét kérdések megválaszolásában, például hogy mennyire aktív a hálózat, éppen felhalmozzák vagy eladják a bitcoinokat, illetve hogy a hálózat egyre biztonságosabbá válik-e.

Ezeknek a mutatóknak a megértése nemcsak a Bitcoin felhasználók számára hasznos, hanem kutatók vagy döntéshozók számára is, akik betekintést szeretnének nyerni ebbe a páratlanul átlátható pénzügyi rendszerbe.

Ez a szakasz néhány gyakran használt mutatót tartalmaz a Bitcoin aktivitás elemzéséhez, alcsoportokba rendezve. Ez nem egy teljes lista. Látogass el a következő oldalra: [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) a teljesebb lista és leírások megtekintéséhez.



#### 8.2.1 Cím (address) mutatók

A címekkel kapcsolatos mutatók hasznosak a hálózati aktivitás időbeli nyomon követésére, mivel jelzik a Bitcoin hálózat aktivitásának szintjét. Például, ahogy a Bitcoin elterjedtebbé válik, az aktív címek száma növekszik. Ezt tovább vizsgálhatjuk úgy, hogy megszámoljuk, hány cím tart legalább egy meghatározott mennyiségű Bitcoint, például 0,1 BTC-t, egy adott időszakban, például egy év alatt. Bár ez képet ad a Bitcoin elterjedéséről az idő múlásával, nem tökéletes, mivel egy személy több Bitcoin címet is birtokolhat. Ezzel szemben a tőzsdék vagy ETF-ek egyetlen entitásként jelenhetnek meg, miközben sok ember pénzét kezelik.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Bitcoin-t tartó címek > X BTC évente. Forrás: Bitcoin Magazine Pro._

Ha összevetjük a címeket a BTC aktuális piaci árával, láthatjuk, hogy a Bitcoin címek mekkora százaléka van nyereségben. Ez lehetővé teszi a piaci hangulat követését, mivel láthatjuk, hogy a piac mekkora része tartja a BTC-t nyereséggel vagy veszteséggel.

Például a **Nem realizált nyereség százaléka** alábbi grafikon azt mutatja, hogy a főkönyv összes címének mekkora aránya rendelkezik nem realizált nyereséggel, amerikai dollárban mérve. Fontos megjegyezni, hogy mivel az alábbi grafikon közel készült a Bitcoin mindenkori csúcsához, a nem realizált nyereséget mutató címek aránya közel száz százalék. Azt is láthatjuk, hogy a nem realizált nyereség százalékának tartósan egy szórás alá esése ritka. Ezért, ha ez a vonal alá esik, az jó beszállási pontot jelezhet a vásárlók számára.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Nem realizált nyereség százaléka. Forrás: checkonchain.com_



#### 8.2.2 On-chain indikátorok

Az on-chain indikátorok azért hasznosak, mert betekintést nyújtanak a hálózat viselkedésébe, túl azon, amit az ár- és címadatok önmagukban mutatnak. Segítenek az elemzőknek megérteni a különböző típusú résztvevők — például a hosszú távú tartók és a rövid távú kereskedők — tevékenységét és hangulatát, azáltal, hogy nyomon követik, hogyan tartják, mozgatják vagy értékelik a bitcoinokat az idő múlásával. Ezek az indikátorok a főkönyv átláthatóságára támaszkodva tárják fel a rejtett piaci dinamikákat, mint például a felhalmozás, elosztás vagy akár a befektetői meggyőződés. Ez különösen hasznossá teszi őket a szerkezeti trendek azonosításában, annak felmérésében, hogy a piac túlfűtött vagy alulértékelt-e, illetve a piaci ciklus fordulópontjainak előrejelzésében.

Például, ha megvizsgáljuk a BTC állományok értékét attól kezdve, hogy utoljára elmozdultak, következtethetünk arra, hogy a piac stressz alatt van-e (mint például egy nagyobb ciklus mélypontján). Ezt a mutatót hívják **Realizált árnak**, és ez adja meg az összes forgalomban lévő BTC „átlagos bekerülési költségét”. Ha a piaci ár a Realizált ár alá esik, az azt mutatja, hogy összességében a legtöbb cím papírveszteséget tart.

Ha tovább csoportosítjuk a főkönyvi adatokat életkor szerinti sávokba, megmutathatjuk, hogyan mozog a BTC mennyisége a címek között az idő múlásával, ami hullámszerű mintákat hoz létre a grafikonon, ezeket hívják **HODL hullámoknak**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL hullámok. Forrás: Bitcoin Magazine Pro._

A HODL hullámok megmutatják, hogy a hosszú, közép- és rövid távú tartók mit tesznek a BTC-jükkel. Például a fenti grafikonon a rövid távú tartók pirossal és naranccsal vannak jelölve, és láthatjuk, hogy aktivitásuk megugrik, amikor ez a csoport a piaci csúcsok közelében vásárol. A másik oldalon láthatjuk, hogy a nagyon hosszú távú tartók (lilával és kékkel) folyamatosan növelik a hálózatban elfoglalt arányukat, ami magas meggyőződést jelez ezeknél a csoportoknál. A grafikon nem tökéletes, mivel néhány érme régi címről újra kerülhet ugyanannak a felhasználónak az irányítása alatt. Mégis érdekes képet ad a hosszú távú tartók meggyőződéséről.

A hosszú távú tartók „okos pénzének” vizsgálatára egy másik módszer a **Coin Days Destroyed** (CDD) elemzése. A „Coin Days” fogalma a BTC mennyiségének és az utolsó mozgatás óta eltelt napok számának szorzata. Például 5 BTC, amely 100 napja nem mozdult, 500 coin day-t halmozott fel, míg 10 BTC, amely 10 napja nem mozdult, 100 coin day-t. Így nagyobb súlyt adunk a hosszabb ideje tartott érméknek. Amikor ezek az érmék elmozdulnak, ezek a coin day-ek „megsemmisülnek”. Ez a mutató a CDD növekedését mutatja jelentős ármozgások idején, ami lehetőséget ad az elemzőknek arra, hogy megkülönböztessék a rutinszerű piaci aktivitást a hosszabb távú tartók hangulatának jelentős változásaitól.

Egy másik mutató, amely segíthet annak azonosításában, hogy a piac alul- vagy túlértékeli-e a BTC-t, a piaci érték és a realizált érték aránya, vagyis az **MVRV**. Ezt egyszerűen úgy számítják ki, hogy a piaci értéket (a forgalomban lévő BTC-k száma szorozva a piaci árral) elosztják a realizált értékkel (az összes BTC értéke az utolsó mozgatásuk óta). A magas MVRV azt jelzi, hogy több érme van nyereségben (gyakran a piaci csúcsok közelében), míg az alacsony MVRV azt mutatja, hogy sok érme veszteségben van (piaci mélypontoknál).



#### 8.2.3 Bányászati mutatók

A bányászati mutatók hasznosak a Bitcoin hálózat biztonságának, gazdasági ösztönzőinek és általános egészségének megértéséhez. Az olyan mutatók, mint a hashráta, a bányászok bevétele, a nehézség és a díj arányok megmutatják, mennyi számítási teljesítmény védi a blokkláncot, és mennyire vannak jól megfizetve a bányászok a tevékenységükért.

A **Hashrate** a Bitcoin hálózatának talán leggyakrabban emlegetett mutatója a hálózat egészségének és biztonságának erősségére. Mivel a bányászat folyamata biztosítja a hálózatot és igazolja a főkönyvi tranzakciók érvényességét, minél nagyobb a számítási (vagy hash-) teljesítmény, annál nehezebb lenne egy rosszindulatú szereplőnek túlerővel támadni a hálózatot.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Forrás: Bitcoin Magazine Pro._

A fenti grafikon azt mutatja, hogy 2025 májusában a hálózat teljes számítási kapacitása körülbelül 900 TeraHash/s (900 billió kriptográfiai „hash” számítás másodpercenként). Ha a hashráta növekszik, az azt mutatja, hogy a hálózat egyre biztonságosabbá válik, ami megnyugtató a felhasználók számára.

A Puell-multiplikátor (David Puell által kidolgozva) a piaci ciklust a bányászok és bevételeik szemszögéből vizsgálja. A mutatót úgy számítják ki, hogy a napi BTC kibocsátást (USD-ben) elosztják a napi kibocsátás 365 napos mozgóátlagával. Ez a mutató segít azonosítani a bányászok stresszes vagy könnyebb időszakait. Történelmileg a 3 feletti érték a BTC piaci értékének csökkenését előzte meg, mivel ez azt jelzi, hogy a bányászok nagyon nyereségesek. Az 0,5 alatti érték stresszt jelez, és történelmileg a BTC értékének piaci mélypontjait jelezte.
