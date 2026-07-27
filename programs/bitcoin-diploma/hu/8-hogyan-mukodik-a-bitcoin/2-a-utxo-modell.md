# 8.2 A UTXO modell

##### Mik azok az UTXO-k?

Ne ijedj meg a furcsa névtől! Az UTXO-kat úgy képzelheted el, mint a bitcoin darabjait, hasonlóan a pénztárcádban lévő bankjegyekhez és érmékhez. Például, ha egy 2 000 Ft-os terméket egy 5 000 Ft-os bankjeggyel fizetsz ki, 3 000 Ft visszajárót kapsz. A bitcoin is hasonlóan működik.

Az összes bitcoinod különböző UTXO-kból áll össze. Amikor bitcoint küldesz, a tárcád egy vagy több ilyen darabot használ fel a fizetéshez.

Ha az általad elköltött darab nagyobb, mint a küldött összeg, a fennmaradó érték visszajáróként, egy új UTXO formájában visszakerül hozzád. Ugyanakkor a címzett is kap egy új UTXO-t, amely a tőled kapott bitcoint képviseli.

A tárcád egyenlege egyszerűen az összes általad birtokolt UTXO összértéke.


> **Callout – Adatvédelem**
>
> Nem célszerű másokkal tudatni, hogy milyen UTXO-id vannak, mert ha valaki ismeri ezeket, nyomon tudja követni a tranzakcióidat, és végül azt is megtudja, mennyi pénzed van.


###### Példa

1. Anna 5 BTC-t szeretne küldeni Balázsnak.
1. A tárcája két UTXO-t használ fel, amelyek együtt 6 BTC-t érnek.
1. A tranzakció elküldi **5 BTC-t Balázsnak**, létrehozva egy új UTXO-t Balázs tárcájában.
1. A fennmaradó **0,99 BTC visszajáróként visszakerül Annához**, miután levonta a **0,01 BTC tranzakciós díjat**.
1. Miután a tranzakció megerősítést nyer, bekerül a Bitcoin főkönyvébe, és az Anna által felhasznált UTXO-k elköltöttnek minősülnek, így azokat már nem lehet újra felhasználni.

###### Források


[▶ Nézd meg a „How Bitcoin Works under the Hood” című videót](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
