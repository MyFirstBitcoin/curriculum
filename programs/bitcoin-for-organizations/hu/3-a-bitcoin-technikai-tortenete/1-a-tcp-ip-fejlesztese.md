# 3.1 A TCP/IP fejlesztése

A legtöbben ismerjük a ma használt TCP/IP protokollokat, amelyek az internet alapját képezik. Eredetük az 1970-es évek végére nyúlik vissza, amikor tudósok alternatívákat kerestek az Arpanethez – egy még korábbi hálózathoz, amelyet az Egyesült Államok Védelmi Minisztériuma hozott létre a távoli számítógépek közötti erőforrás-megosztás érdekében. 1983-ban a TCP/IP lett az Arpanet protokoll szabványa, ami ahhoz vezetett, hogy a TCP/IP a 90-es évek végére a domináns hálózati modellé vált, és ez lett az alapja annak az internetnek, amelyen ma a Bitcoin is működik.


| OSI modell | TCP/IP |
| --- | --- |
| Alkalmazás | Alkalmazás |
| Megjelenítés | Alkalmazás |
| Munkamenet | Alkalmazás |
| Szállítási | Szállítási |
| Hálózati | Hálózati |
| Adatkapcsolati | Adatkapcsolati |
| Fizikai | Fizikai |


Ugyanabban az időben, amikor a TCP/IP modellt fejlesztették, egy hasonló, de átfogóbb keretrendszert dolgozott ki a Nemzetközi Szabványügyi Szervezet (ISO) és a távközlési ipar (CCITT). Az új protokollok kidolgozásának vagy módosításának folyamata lassú és nehézkes volt a decentralizáltabb TCP/IP fejlesztési megközelítéshez képest, ami végül a TCP/IP dominanciájához vezetett napjainkban.

##### Módosítási kérelem

Bármilyen fejlesztési javaslat a meglévő protokollokhoz vagy új ötletekhez a TCP/IP modellben egy **Módosítási kérelem** folyamatán keresztül történhet. Ezek jóváhagyási folyamaton mennek keresztül, amelyet az Internet Engineering Task Force (IETF) kezel, és jóváhagyás után nyílt forráskódúvá válnak, hogy bárki megvalósíthassa és alkalmazhassa őket. Néhány figyelemre méltó példa:

* 1969 RFC 1 Dokumentálta, hogyan küldik a csomagokat az Arpanetben
* 1981 RFC791 meghatározta az Internet protokoll V4-et – amelyet ma is széles körben használnak
* 1982 RFC 821 Egyszerű levéltovábbítási protokoll
* 1987 Domain Name System – hogyan fordítjuk le a domain neveket IP-címekre
* 1999 RDC 2616 Hypertext Transfer Protocol – alapvető a web böngészéséhez


> **Callout**
>
> A **Bitcoin Improvement Proposal** (BIP) hasonló megközelítést követ, mint az RFC, de kizárólag a Bitcoin fejlesztésére összpontosít, nem pedig új vagy alternatív protokollok kidolgozására. A Bitcoin is átveszi ezt a rétegzett modellt, és további protokollokat is láthatunk, amelyeket második vagy harmadik rétegként írnak le.


Ugyanúgy, ahogy a TCP/IP modell alaprétegei az elmúlt évtizedekben viszonylag keveset változtak, és az innováció a magasabb rétegekben történt, a Bitcoin alaprétege is várhatóan nagyon lassan fog változni, miközben a skálázási megoldások, mint a Lightning és a Liquid, a felsőbb rétegekben jelennek meg.

Jó példa arra, hogy az alapszintű protokollokat idővel milyen nehéz megváltoztatni, az IPv6. Az IPv4 címterének várható kimerülése új protokoll iránti igényt teremtett. Az első szabványtervezet 1998-ban készült el, de csak 2017-ben ratifikálták internetes szabványként. Bár sok problémát megoldott az IPv4-gyel kapcsolatban, és sokkal inkább jövőbiztos, az iparágban mégis nagyon lassan terjedt el. Ez idő alatt számos új protokollt határoztak meg a felsőbb rétegekben a multimédia, e-mail stb. lehetővé tételére.

##### A Bitcoin által használt építőelemek

Az összekapcsolhatóság problémáinak ilyen szétválasztása lehetővé teszi, hogy a protokollokat függetlenül fejlesszék a felette és alatta lévő rétegektől. Ahelyett, hogy minden réteghez újra kellene találni a megoldásokat, a Bitcoin hálózat támaszkodhat a fizikai és adatkapcsolati rétegek által biztosított hálózati képességekre.


| Réteg | TCP/IP eredeti |
| --- | --- |
| Alkalmazás | A Domain Name System (DNS) segítségével azonosítja a szomszédos csomópontokat. A 8333-as port jelzi a Bitcoin protokollt. |
| Szállítási | UDP a FIBRE kommunikációhoz a bányászok között az alacsony késleltetés érdekében. TCP a csomópontok közötti P2P kommunikációhoz. |
| Szállítási | TOR útvonalválasztás: Anonimitást és adatvédelmet biztosít. Broadcast protokoll: Forgalom irányítása a hálózaton keresztül. |
| Kapcsolati | Bármilyen közegen működik (pl. Ethernet, Wi-Fi, stb.) |
| Fizikai | Fizikai átvitel vezeték nélküli, Ethernet vagy más hardveres interfészeken keresztül. |


##### A Bitcoin egy semleges protokoll az érték átvitelére, ahogy a HTTPS egy protokoll az információ átvitelére

* **HTTPS**: Biztonságos weboldalak
* **SMTP**: E-mailek küldése
* **FTP**: Fájlok átvitele
* **DNS**: Domain nevek kezelése
* **BTC**: Érték tárolása és átvitele

A Bitcoin lehetővé teszi az érték megbízható átvitelét emberek vagy eszközök között az interneten keresztül, harmadik fél bevonása nélkül. Várhatóan ez óriási értéket szabadít fel.
