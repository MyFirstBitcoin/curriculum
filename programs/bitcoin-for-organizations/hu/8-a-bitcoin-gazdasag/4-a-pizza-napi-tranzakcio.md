# 8.4 A Pizza-napi tranzakció

Eddig ez a modul arra összpontosított, hogy a Bitcoin főkönyv nyitott jellegét felhasználva hasznos mutatókat állítsunk össze az összesített tranzakciós adatokból. Azonban lehetséges a főkönyvi adatok és blokkböngészők segítségével valós tranzakciókat is megvizsgálni, és nyomon követni a pénzeszközök mozgását a hálózaton belül.

Minden évben május 22-én a Bitcoin közösség megemlékezik Laszlo Hanyeczről, aki az első ismert személy volt, aki bitcoinnal fizetett fizikai árucikkért. 2010. május 18-án Hanyecz bejelentette a Bitcointalk.org fórumon, hogy pizzát keres, és hajlandó BTC-vel fizetni érte. 10 000 BTC-t ajánlott fel bárkinek, aki hajlandó részt venni az ügyletben. Több napig várt, míg egy 19 éves diák, akit a példában nevezzünk Gergőnek, elfogadta az ajánlatot, és küldött két nagy pizzát.

A **Pizza Day** tranzakciót bárki megtekintheti, és a következő tranzakcióazonosítóval rendelkezik:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Ha ezt a tranzakcióazonosítót beírjuk a [mempool.space](https://mempool.space) oldalra, a következőket láthatjuk:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



A tranzakció dátuma és időpontja: 2010. május 22.

A hálózati tranzakciós díj: 99 000 000 sat (akkoriban ez kevesebb volt, mint 1 amerikai cent. 2025 májusában ez 95 072,67 USD-t ér).

A blokk magassága: 57 043

A megerősítések száma: 838 645 (ez azt jelzi, hány blokk került a főkönyvbe e tranzakció után)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

A tranzakció bemeneteinek száma: 131

A tranzakció kimeneteinek száma: 1

Ha rákattintunk a kimeneti nyilvános kulcsra (amelynek vége `XaxFyQ`), amelyről tudjuk, hogy Gergő tulajdonában volt, aki 10 000 BTC-t kapott két pizzáért, a következőket láthatjuk:

Ennek a címnek jelenleg 0,00257879 BTC az egyenlege, és úgy tűnik, hogy 14 tranzakcióban vett részt, amelyek közül a legutóbbi 2024. december 13-án történt.



#### 8.4.1 Tevékenység: Csoportos megbeszélés

1. Írd le az előnyöket (pl. auditálás, elszámoltathatóság) vagy kockázatokat (pl. adatvédelmi aggályok), amelyek egy ilyen átlátható és nyitott tranzakciós rendszer használatával járnak magánszemélyek vagy vállalkozások számára.
1. Hogyan befolyásolhatja az ilyen pénzügyi átláthatóság a jótékonysági szervezeteket, az állami beszerzéseket, a hazautalásokat vagy a bűnüldözést?
1. A hagyományos bankrendszereknek is hasonló szintű átláthatóságot kellene biztosítaniuk? Rákényszerítheti őket erre a piac?
