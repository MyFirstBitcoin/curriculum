# 3.4 Hashcash

A Hashcash-t Adam Back hozta létre, aki szintén az egyik korai újító volt ezen a területen. Adam erősen érdeklődött a szabad piacok és az internetes magánélet iránt, és rátalált a Cypherpunks levelezőlistára, amelyhez csatlakozott, és aktív résztvevője lett.

Nagyon érdekelte a digitális pénz, és javaslatokat tett arra, hogyan működhetne együtt szorosabban a csoport a DigiCash-en Chaummal, de ezek nem vezettek eredményre. Ezután figyelmét egy másik felmerülő problémára fordította – az e-mail spamekre. Ő és a többi Cypherpunk megoldást akart találni a spam problémájára, ahol a spammerek számára triviális volt több ezer e-mailt létrehozni és elküldeni, amelyek elárasztják a hálózatokat. Innovatív megoldása a hashelésen alapult – a kriptográfia azon képességén, hogy bármilyen adatot egyedi és véletlenszerű, meghatározott hosszúságú karakterlánccá alakítson, létrehozva egy digitális „bélyeget”, amelyet az e-mailhez kellett csatolni, hogy azt érvényesnek tekintsék, és továbbítsák a hálózaton. Egy valódi e-mail esetén ez elhanyagolható költség, de a spammerek számára megakadályozó tényező.

A Hashcash kulcsfontosságú újítása az volt, hogy a való világ erőforrásait – a számítási teljesítményt – kötötte össze egy digitális hálózattal. Míg a digitális erőforrásokat addig korlátlanul lehetett másolni, a létrehozott „hashcash” mennyiségét az korlátozta, hogy az emberek mennyi energiát voltak hajlandók befektetni.

Bár a megoldás megfelelt néhány olyan kritériumnak, amelyet Adam egy digitális pénzrendszerben szükségesnek tartott; anonim, ellenálló és bizalommentes volt, minden hashcash nem volt újrahasználható és nem volt valóban ritka. Javasolt más módszereket is ezeknek a problémáknak a kezelésére, külső harmadik felek bevonásával.

##### BitGold

Nick Szabo a Hashcash és a proof of work koncepciójára építve egy alternatív megoldást javasolt, amelyet egy levelezőlistán írt le egy évvel a Hashcash megjelenése után, 1998-ban.

Bár közelebb került a megoldáshoz, ez a javaslat még mindig több kihívással küzdött.

* Ki működtetné a hash tulajdonjogának nyilvántartását, és hogyan lehetne bennük megbízni?
* A hashelés általában idővel olcsóbbá válik, ami a HashCash számára is kihívást jelentett.

Mivel a kapcsolódó hasheket időbélyeggel látták el, valamilyen történeti nyilvántartást javasolt a hashelés nehézségéről az adott időpontban; egy korábbi hash előállítása több számítási költséget igényelt, mint egy későbbi, mivel a költségek idővel csökkentek. Sajnos ez azt jelentette, hogy a hashek nem voltak „helyettesíthetők”, vagyis nem voltak egyenértékűek, pedig ez a digitális pénz egyik kulcsfontosságú tulajdonsága. Ennek megoldására Nick valamilyen „szabad bankrendszert” javasolt a BitGold fölé, amely különböző hash-csoportokat tudott volna összevonni, hogy azok azonos értékűek legyenek.

##### B-Money

Nem sokkal a Bit Gold javaslat után Wei Dai egy hasonló megoldást vetett fel. Már több más eszközt is kifejlesztett a Cypherpunks számára, és saját elképzelései voltak a digitális pénzről.

Javaslata hasonlított a Bit Goldhoz abban, hogy digitális aláírásokat használt a pénz átutalásához, és a tranzakciók nyilvántartását egy főkönyvben tárolták, amely tartalmazta a nyilvános kulcsokat és az egyesekhez rendelt pénzegységek számát. Ahogy a Bit-Gold esetében is, a megbízható harmadik feleket biztonsági résnek tekintették, és az volt a meggyőződés, hogy egy elektronikus pénzrendszernek nem szabad egyetlen entitásra támaszkodnia az egyenlegek, tranzakciók nyilvántartására vagy a dupla költés megakadályozására.

Wei Dai több megoldást is javasolt ezekre a problémákra, ezek egyike az volt, hogy a főkönyvet ne egy központi entitás(ok) vezesse, hanem MINDEN csomópont tartson fenn egy másolatot. Ha minden felhasználó ellenőrzi a saját főkönyvét és minden tranzakció érvényességét, akkor amíg minden csomópont naprakész marad, a főkönyvek szinkronban maradnak a hálózaton. Ez a rendkívül elosztott rendszer nehezen lenne korrumpálható.

Wei Dai felismerte, hogy ez nem oldja meg a bizánci tábornokok problémáját (1), mivel a csomópontok könnyen elveszíthetik a szinkront, vagy egyszerűen hazudhatnak. Alternatív módszereket javasolt, például egy „megbízható” szerverekből álló részhalmazt, amely fenntartja a főkönyvet, valamint pénzügyi ösztönzők létrehozását, hogy ezek a szerverek őszinték maradjanak.

A monetáris politikára azt javasolta, hogy a B-Money vásárlóerejét valamilyen külső fogyasztói árindexhez kössék. Azt szerette volna, hogy ugyanannyi B-Money idővel ugyanakkora részesedést tudjon vásárolni az indexből, így biztosítva némi árstabilitást. Tehát bárki létrehozhatott új pénzegységeket egy érvényes hash bemutatásával, de a hash előállításának nehézsége idővel változhatott a CPU költségek és az árindex alapján, hogy minden egység „változatlan” maradjon.
