# 9.2 Šta je Mempool?

**mempool**, skraćeno od „memory pool“ (memorijski bazen), je kao čekaonica za Bitcoin transakcije. Kada pošaljete bitcoin, vaša transakcija se prvo emituje mreži i smešta u mempool.

Možete to zamisliti kao čekanje u redu u restoranu. Vaše ime se upisuje na listu i čekate dok se ne oslobodi sto. Na isti način, vaša transakcija čeka u mempool-u dok je rudar ne uključi u blok.

Bitcoin čvorovi proveravaju svaku novu transakciju kako bi se uverili da je validna i da bitcoin koji se troši nije već iskorišćen. Ako je transakcija validna, ostaje u mempool-u dok ne bude potvrđena.

Rudari biraju transakcije iz mempool-a i uključuju ih u nove blokove. Obično se transakcije sa većim naknadama biraju prve.

Kada je transakcija uključena u blok, postaje potvrđena i trajno se beleži na Bitcoin blokčejnu.

#### Aktivnost: Istraživanje Mempool-a

https://qr.myfirstbitcoin.org/mempool.pdf

**Ova aktivnost upoznaje učenike sa besplatnim i otvorenim alatom koji ne zahteva tehničke veštine za korišćenje. Koristan je za Bitcoinere svih nivoa, od početnika do iskusnih.**

###### Ključne tačke

1. **Mempool** se odnosi na listu nepotvrđenih transakcija koju održava svaki Bitcoin čvor, a ne na neku određenu uslugu ili platformu.
1. Ne postoji jedan univerzalni mempool. Mempool.space je samo jedan od mnogih.
1. [Mempool.space](https://mempool.space) je otvorenog koda i poznat je po tome što je jednostavan vizuelni blok istraživač. Pruža podatke u realnom vremenu o nepotvrđenim transakcijama, visini naknada i drugim aktivnostima na mreži.

###### Savet za učenike

Mempool.space radi mnogo više od vizualizacije blokova. Istražite i druge delove Bitcoin ekosistema: npr. Lightning, rudarenje, hash rate, rudarske bazene i „naočare“ za blok prostor.
