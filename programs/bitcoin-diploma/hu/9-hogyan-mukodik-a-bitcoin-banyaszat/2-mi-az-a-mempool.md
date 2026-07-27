# 9.2 Mi az a Mempool?

A **mempool**, a „memória pool” rövidítése, olyan, mint egy váróterem a Bitcoin tranzakciók számára. Amikor bitcoint küldesz, a tranzakciódat először továbbítja a hálózat, és elhelyezi a mempoolban.

Úgy képzelheted el, mintha sorban állnál egy étteremben. A neved felkerül egy listára, és vársz, amíg felszabadul egy asztal. Ugyanígy a tranzakciód is várakozik a mempoolban, amíg egy bányász be nem illeszti egy blokkba.

A Bitcoin node-ok minden új tranzakciót ellenőriznek, hogy érvényes-e, és hogy az elköltött bitcoinokat még nem használták-e fel korábban. Ha a tranzakció érvényes, a mempoolban marad, amíg meg nem erősítik.

A bányászok a mempoolból választanak tranzakciókat, és ezeket beillesztik az új blokkokba. Általában a magasabb díjjal rendelkező tranzakciókat választják először.

Amint egy tranzakció bekerül egy blokkba, megerősítetté válik, és véglegesen rögzítik a Bitcoin blokkláncon.

#### Tevékenység: A Mempool felfedezése


https://qr.myfirstbitcoin.org/mempool.pdf

_Activity: Mempool_


**Ez a tevékenység egy ingyenes és nyílt forráskódú eszközt mutat be a diákoknak, amelynek használatához nincs szükség technikai tudásra. Hasznos minden szintű Bitcoiner számára, kezdőtől a haladóig.**

###### Főbb pontok

1. **Mempool** az egyes Bitcoin node-ok által fenntartott, megerősítetlen tranzakciók listájára utal, nem pedig egy konkrét szolgáltatásra vagy platformra.
1. Nincs egyetlen, univerzális mempool. A Mempool.space csak egy a sok közül.
1. [Mempool.space](https://mempool.space) nyílt forráskódú, és jól ismert arról, hogy könnyen használható, vizuális blokkböngésző. Valós idejű adatokat nyújt a megerősítetlen tranzakciókról, díjszintekről és egyéb hálózati aktivitásról.

###### Diáktipp

A Mempool.space sokkal többet tud, mint blokkokat megjeleníteni. Fedezd fel a Bitcoin ökoszisztéma más részeit is: például a Lightning hálózatot, a bányászatot, a hash rátát, a bányász poolokat és a blokktér „szemüveget”.
