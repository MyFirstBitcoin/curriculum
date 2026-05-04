# 2.4 A Bitcoinban nincs innováció.

> Ezer erdő teremtése egyetlen makkból indul ki.   
_Ralph Waldo Emerson_

A kritikusok gyakran próbálják azt állítani, hogy a Bitcoin „régi” vagy „halott” technológia, mert nem változtatja meg az alapszintű protokollt olyan gyakran, mint a versengő blokkláncok. Ez az állítás figyelmen kívül hagyja mind azokat az okokat, amiért a Bitcoin változásait lassan fogadják el, mind pedig azt az innovációs mennyiséget, amely a hálózat skálázására történik a magasabb rétegeken, például a Lightning Networkön. Azt is figyelmen kívül hagyja, hogy sok leginkább rugalmas és tartós technológiánk sem skálázódik gyorsan az alapszinten.

Például a Transmission Control Protocol (TCP) esetében sincs már innováció, amely az internet alapját képezi. A TCP-t először 1974-ben hozták létre. Utoljára 1982-ben frissítették. Azt teszi, amire szükség van. Nem tökéletes, és vannak viták arról, hogy frissíteni kellene-e az IPv4-et a jövőbeli internetes fejlesztések támogatására. Azonban azt állítani, hogy 1982 óta nem történt innováció az interneten, rendkívüli kijelentés lenne. Minden innováció a TCP „fölött” történt, nem pedig „benne”.

Az innovációk túlnyomó többsége nem „a” Bitcoinban, hanem „a” Bitcoinon történik. Egy nap valószínűleg már nem lesz innováció „a” Bitcoinban, és ennek célnak kell lennie, nem pedig kritikának, hiszen ez azt tükrözi majd, mennyire alapvetővé vált a globális gazdaság támogatásában azáltal, hogy alapot nyújt a globális, semleges és engedélymentes, stabil pénzhez. Olyan pénzhez, amely gazdasági értelemben is stabil, mert fix a kínálata és megmásíthatatlan a főkönyve, de technológiai értelemben is stabil, mert nem változik, és a működése évek óta megszakítás nélkül zajlik. A Bitcoin az elmúlt 10 évben már elérte a 100%-os rendelkezésre állást.

Az viszont aggasztó lenne, ha nem történne innováció „a” Bitcoinon. Nézzük meg, mi történt ezen a téren az elmúlt 10 évben:



#### „A” Bitcoinban

A Segregated Witness (SegWit) 2017-ben került bevezetésre, hogy megvédje a tranzakciókat a módosíthatóságtól, és növelje a blokkok kapacitását. A SegWit szükséges előfeltétele volt a lightning és néhány side chain hatékony működésének is.

A Taproot 2021-ben került bevezetésre, hogy lehetővé tegye több aláírás csoportosítását és érvényesítését Schnorr-aláírások beépítésével, egy szkriptnyelv bevezetésével, amely összetettebb funkciókat tesz lehetővé, valamint növeli a tranzakciók magánszféráját és cenzúraállóságát.



#### „A” Bitcoinon

##### Liquid Sidechain

A Liquid sidechain 2018-ban került bevezetésre. A Liquid, akárcsak más side chain-ek, egy külön blokklánc főkönyv, amely előre meghatározott szabályok szerint kapcsolódik a fő Bitcoin blokklánchoz. Ezek a szabályok elég rugalmasak ahhoz, hogy a Liquid lánc idővel fejlesztéseket és skálázhatósági újításokat vezessen be. Ugyanakkor a Bitcoin blokklánchoz való kapcsolódás biztosítja, hogy a bitcoin teljes, 21 milliós kínálati korlátja mindkét láncon következetes maradjon.

A Liquidben lévő eszköz, az L-BTC, kétirányú peg-gel kapcsolódik a fő láncon lévő bitcoinhoz. Költség-, sebesség-, adatvédelmi és biztonsági kompromisszumok vannak, amelyek miatt az L-BTC bizonyos alkalmazásokhoz ideális. Az L-BTC költsége, sebessége és adatvédelme mind javul, cserébe azonban bizonyos mértékű bizalmat kell helyezni a Liquid Szövetséget alkotó szervezetekbe, akik egy 15-ből 11-es multisig folyamaton keresztül irányítják az L-BTC és a bitcoin közötti átváltást.

##### Lightning Network

A Lightning Network 2018-ban került bevezetésre. A Lightning célja, hogy peer-to-peer fizetési hálózat legyen, amely csatornákon keresztül összekapcsolt csomópontok gráfjaként működik; nem blokklánc. A bitcoinokat egy csomópont futtató zárolja a fő blokkláncon, hogy elérhetővé tegye azokat a Lightning Networkön, ez biztosítja, hogy csak „valódi” bitcoin legyen használatban. A csomópontok ezután likviditási csatornákat nyithatnak egymással multisig okosszerződéseken keresztül. A fizetések útvonalat találnak a hálózaton keresztül a forrástól a célig, optimalizálva a költséget azzal a feltétellel, hogy minden lépésnél elegendő likviditás álljon rendelkezésre a megfelelő irányban. A Lightning Network jelentősen javítja a költséget, a sebességet és az adatvédelmet, cserébe viszont csökken a biztonság (vagy nő a szükséges bizalom) és nő a komplexitás. Ugyanakkor ezt nagy volumenű, kis értékű, mindennapi fizetésekre szánják, így ez nagyon ésszerű kompromisszumnak számít a napi több millió tranzakcióért (forrás: River, 2023).

##### Chaumian eCash Mints

A Fedimint-ek közösségi határok közé szorított lightning hálózatként foghatók fel. Az a céljuk, hogy kihasználják azokat a bizalmi viszonyokat, amelyek bizonyos közösségekben (pl. családok, falvak, baráti társaságok) természetesen léteznek, cserébe egyszerűsítik a komplexitást és növelik a felhasználók adatvédelmét. Ezek moduláris, nyílt forráskódú protokollok a bitcoin közösségi környezetben történő letétkezelésére és tranzaktálására. Magával a Lightning Networkkel is interoperábilisak.

**Cashu** egy bemutatóra szóló token, amely tárolható például egy mobiltelefonon; a tervezés célja, hogy a fizikai készpénz előnyeit digitális formában reprodukálja. A Cashu a Chaumian eCash egyik példája, amely a Bitcoinra épül, és növeli az adatvédelmet, a cenzúraállóságot, valamint csökkenti a komplexitást, cserébe viszont bizalmat kell helyezni a használt eCash mintbe. A Cashu minták eCash tokeneket bocsátanak ki, amelyek a bitcoint képviselik, és a felhasználók úgy költhetik el őket, hogy nem fedik fel személyazonosságukat. A Cashu interoperábilis a Lightning Networkkel.

Valószínűleg a jövőben még sok más 2. rétegbeli alkalmazás fog épülni, amelyekre aztán további, 3. rétegbeli alkalmazások épülnek majd.

A Lightningra épülő alkalmazások hihetetlen számának szemléltetésére íme egy részlet a River Lightning Network kutatási jelentéséből.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
