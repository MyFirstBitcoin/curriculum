# 3.7 Bitcoin

Sok évnyi próbálkozás és kudarc után a Cypherpunkok többsége már kezdte elveszíteni az érdeklődését a digitális, engedély nélküli pénz ötlete iránt, amikor Adam Back kapott egy e-mailt, amely egy 'elektronikus pénz harmadik fél nélkül' című fehér könyv tervezetéhez vezetett, egy Satoshi Nakamoto nevű, ismeretlen személytől.

Összefoglalva eddig, legalább az alábbi ötletekkel rendelkezünk:

* Kriptográfiai aláírások, amelyek bizonyos szintű magánszférát és anonimitást biztosíthatnak
* A fedezet nélküli pénz koncepciója (B-Money)
* Javaslatok (de nincs megvalósítás) az új pénz kibocsátásának korlátozására
* Digitális érmék, amelyek tulajdonjogát nyilvános kulcsokhoz rendelték (B-Money), és amelyek mozgathatók voltak aláírással, valamint újra hozzárendelhetők a címzett címéhez (RPOW és Hashcash)
* Minden csomópont egy teljesen elosztott főkönyv másolatát tartja fenn (B-Money) (akkoriban kivitelezhetetlennek tartották)
* Időbélyegző protokoll – Merkle-fa hash-elés használata, hogy matematikailag bizonyítható eseménysorrendet biztosítson, amelyet nehéz meghamisítani, ha minden felhasználó ugyanazokat a feljegyzéseket tartja fenn
* Proof of work, hogy a való világban végzett munkát összekapcsolja a rendszerrel (de magát a hash-t használva pénzként)
* Teljesen decentralizált hálózatok, ahol minden résztvevő egyenrangú, és szabadon csatlakozhat vagy kiléphet a hálózatból (BitTorrent)
* Az új hash-ek előző hash-ekhez kötésének koncepciója (Bit Gold és időbélyegzés)

Ami ebben az időben hiányzott:

* Egy életképes megoldás a 'bizánci tábornokok' problémájára
* Egy módszer a forgalomban lévő pénz mennyiségének korlátozására a folyamatos hardverfejlődés ellenére
* Ösztönző rendszer az emberek részvételéhez (tyúk-tojás probléma)

A másik jelentős különbség a korábbi próbálkozások és a Bitcoin között az volt, hogy Satoshi már jó ideje dolgozott a kódon a valódi 'Cypherpunkok kódot írnak' eredeti szellemiségében, mielőtt bejelentette volna a levelezőlistákon, ellentétben a Bit Gold és B-Money koncepciókkal, amelyek inkább elméletiek voltak.

Mi volt az az újítás, amely megkülönböztette a Bitcoint a korábbi elektronikus pénz próbálkozásoktól?

A proof of work-öt konszenzusmechanizmusként, valamint a biztonság és a megváltoztathatatlanság biztosításának eszközeként használták: Ahelyett, hogy a hash-t pénzként használnák, egy új, bányászatnak nevezett eljárásban alkalmazták, ahol egy csomópont összegyűjt egy tranzakciócsomagot, hozzáad egy véletlenszámot, majd a teljes 'blokk' adatot hash-eli. Egy érvényes blokk, amely megfelel a hash-követelménynek, ezután meghirdetésre kerül a hálózaton. Ezeket a blokkokat egymáshoz kapcsolják az előző blokk hash-ével, és a leghosszabb blokkláncot használják döntetlen esetén, amikor különböző csomópontok egyszerre érvényesítenek és hirdetnek különböző blokkokat, lánc szétválást okozva. A proof of work lett a decentralizált döntőbíró a bizánci tábornokok problémájának megoldására.

Ezek a bányászok ösztönzést is kaptak, hogy biztosítsák a proof-of-work elvégzéséhez szükséges CPU-t, mivel minden blokkért új bitcoin-t kaptak. Az általuk kapott Bitcoin mennyisége is úgy van programozva, hogy körülbelül négyévente csökkenjen, amíg az összes Bitcoin létre nem jön, így kemény felső határt szabva a forgalomban lévő Bitcoin teljes mennyiségének, ami 21 millió.

A legeredetibb ötlet az volt, ahogyan megoldotta azt a problémát, hogy mennyi pénz jön létre, ahogy a hardver fejlődik, és egyre nagyobb teljesítmény áll rendelkezésre a hálózat számára. Egy meghatározott számú blokk (2016) időbélyegét átlagolják, és ha túl gyorsan jönnek létre, a következő blokk létrehozásához szükséges hash nehezebbé válik, ha túl lassan, akkor könnyebbé. Ez be van építve a decentralizált protokollba, amelyet minden csomópont futtat, így minden bányász, aki ezt figyelmen kívül hagyja, energiát pazarol egy olyan blokk kibányászására, amelyet a hálózat többi része elutasít. Ez a beállítás biztosítja, hogy az új blokkok létrehozása a tervezett kibocsátási ütem szerint történjen, és ösztönzi a bányászokat, hogy 'tartsák be a szabályokat'.

####   
Összefoglalás

A decentralizált, peer-to-peer elektronikus pénzrendszer felépítéséhez szükséges kirakós darabok nagy része már megvolt, mielőtt Satoshi kiadta volna a fehér könyvét, és nem sokkal később a kód első verzióját.

> A Bitcoin természete olyan, hogy amint a 0.1-es verzió megjelent, a magterv a továbbiakban kőbe vésetté vált  
_Satoshi Nakamoto_

Bár számos fejlesztési ötletet (BIP) javasoltak és fogadtak el, a Bitcoin 2009 óta a háttérben működik, követve a kezdeti kiadásban lefektetett protokollt, szinte bármiféle fennakadás nélkül. Minden fejlesztés úgy történt, hogy visszafelé kompatibilis maradt az összes korábbi verzióval.



##### Jegyzetek

1. A bizánci tábornokok problémájának magyarázatához lásd: [https://hu.wikipedia.org/wiki/Biz%C3%A1nci_hiba](https://en.wikipedia.org/wiki/Byzantine_fault)
