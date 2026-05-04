# 8.0 Bevezetés

> A Bitcoin nem "szabályozatlan"; algoritmus szabályozza, nem pedig kormányzati bürokráciák. Korrupciómentes.  
_Andreas M. Antonopoulos_

Ebben a modulban közelebbről megvizsgáljuk a Bitcoin technikai oldalát. Egyszerűen elmagyarázzuk azt a kriptográfiát, amely a protokollt védi, és bemutatjuk, hogyan működnek a tranzakciók. Néhány fogalom technikainak tűnhet, de ne aggódj. Sokan használják nap mint nap az internetet anélkül, hogy teljesen értenék, hogyan működik.

A Bitcoin technikai oldalának elsajátítása hosszú út, amit nem mindenkinek kell végigjárnia. Bár bátorítjuk a folyamatos tanulást, ez a modul a legfontosabb alapokra koncentrál.

A Bitcoin hálózat egy megosztott tranzakciós nyilvántartás, amelyet sok számítógép, úgynevezett csomópontok (node-ok) tárolnak. Ezt a nyilvántartást Bitcoin főkönyvnek hívják, és pszeudonim. Nem tartalmaz személyes adatokat, mint például neveket vagy életkort, csak tranzakciós adatokat és Bitcoin-címeket. A főkönyv minden tranzakciót nyomon követ a blokklánc kezdetétől fogva.

##### A Bitcoin protokoll működése

* Munkabizonyíték (Proof-of-Work)
* Kriptográfiai időbélyegek
* Nehézségi szint igazítása
* Peer-to-peer hálózati architektúra
* Hash függvények és Merkle-fák
* Nyilvános kulcsú kriptográfia
* Blokkjutalom felezése
