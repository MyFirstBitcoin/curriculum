# 9.3 Jak fungují transakce

Nyní, když rozumíte veřejným a soukromým klíčům, stejně jako rolím uzlů a těžařů, zde je, jak probíhá bitcoinová transakce od začátku do konce.

1. Adam chce poslat bitcoin Jakubovi. Vytvoří transakci s Jakubovou adresou, částkou k odeslání a poplatkem.
1. Adam podepíše transakci svým soukromým klíčem, aby prokázal vlastnictví.
1. Transakci odešle do bitcoinové sítě.
1. Uzlům ji přijmou a zkontrolují, zda splňuje pravidla, včetně ověření podpisu a toho, že Adam má dostatek bitcoinů.
1. Pokud je platná, transakce se sdílí po celé síti a přidá se do mempoolu, kde čekají nevyřízené transakce.
1. Těžaři vybírají transakce z mempoolu a zahrnují je do bloku, který se snaží vytěžit.
1. Když těžař úspěšně vytěží blok, sdílí ho se sítí a ostatní uzly ho ověřují.
1. Pokud je blok platný, přidá se do blockchainu. Jakub obdrží bitcoin.
1. Jakmile se přidávají další bloky, transakce získává potvrzení, což ji činí bezpečnější.

Jakmile je transakce zahrnuta do bloku, je potvrzena. Adam už nemůže tento bitcoin znovu utratit a Jakub může to, co obdržel, použít v nové transakci.


> **Note**
>
> Transakce a poplatek vybrány → Podepsáno peněženkou a odesláno → Distribuováno uzly → Těžař přidá transakci do šablony bloku → Těžař vyhraje soutěž Proof-of-Work → Nový blok je ověřen → Nový blok je distribuován uzly


###### Zdroje


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
