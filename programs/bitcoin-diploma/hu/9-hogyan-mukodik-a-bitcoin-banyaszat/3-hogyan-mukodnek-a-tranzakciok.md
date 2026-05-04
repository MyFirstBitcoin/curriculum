# 9.3 Hogyan működnek a tranzakciók

Most, hogy már érted a nyilvános és privát kulcsokat, valamint a node-ok és bányászok szerepét, íme, hogyan zajlik le egy Bitcoin tranzakció az elejétől a végéig.

1. Ádám bitcoint szeretne küldeni Gergőnek. Létrehoz egy tranzakciót Gergő címével, a küldendő összeggel és egy díjjal.
1. Ádám aláírja a tranzakciót a privát kulcsával, hogy igazolja a tulajdonjogát.
1. Elküldi a tranzakciót a Bitcoin hálózatra.
1. A node-ok fogadják, és ellenőrzik, hogy megfelel-e a szabályoknak, beleértve az aláírás ellenőrzését és azt, hogy Ádámnak van-e elég bitcoinja.
1. Ha érvényes, a tranzakciót megosztják a hálózaton, és bekerül a mempoolba, ahol a függőben lévő tranzakciók várakoznak.
1. A bányászok kiválasztják a tranzakciókat a mempoolból, és beillesztik őket abba a blokkba, amelyet megpróbálnak kibányászni.
1. Amikor egy bányász sikeresen kibányászik egy blokkot, azt megosztja a hálózattal, és más node-ok is ellenőrzik.
1. Ha érvényes, a blokk hozzáadódik a blokklánchoz. Gergő megkapja a bitcoint.
1. Ahogy újabb blokkok kerülnek hozzáadásra, a tranzakció egyre több megerősítést kap, így egyre biztonságosabb lesz.

Miután bekerült egy blokkba, a tranzakció megerősítést nyer. Ádám nem költheti el újra azt a bitcoint, Gergő pedig elkötheti azt, amit kapott, egy új tranzakcióban.


> **Note**
>
> Tranzakció és díj kiválasztva → Tárca aláírja és elküldi → Node-ok terjesztik → Bányász hozzáadja a tranzakciót a blokk sablonhoz → Bányász megnyeri a Proof-of-Work versenyt → Új blokk érvényesítve → Új blokkot node-ok terjesztik


###### Források


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
