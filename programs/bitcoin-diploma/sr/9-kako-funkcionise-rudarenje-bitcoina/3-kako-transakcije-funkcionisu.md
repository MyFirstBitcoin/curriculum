# 9.3 Kako transakcije funkcionišu

Sada kada razumeš javne i privatne ključeve, kao i uloge čvorova i rudara, evo kako funkcioniše Bitcoin transakcija od početka do kraja.

1. Adam želi da pošalje bitcoin Gerardu. On pravi transakciju sa Gerardovom adresom, iznosom koji želi da pošalje i naknadom.
1. Adam potpisuje transakciju svojim privatnim ključem kako bi dokazao vlasništvo.
1. On šalje transakciju Bitcoin mreži.
1. Čvorovi je primaju i proveravaju da li poštuje pravila, uključujući proveru potpisa i da li Adam ima dovoljno bitcoina.
1. Ako je ispravna, transakcija se deli po mreži i dodaje u mempool, gde čekaju transakcije koje još nisu obrađene.
1. Rudari biraju transakcije iz mempool-a i uključuju ih u blok koji pokušavaju da iskopaju.
1. Kada rudar uspešno iskopa blok, on se deli sa mrežom i proveravaju ga drugi čvorovi.
1. Ako je ispravan, blok se dodaje u blokčejn. Gerard dobija bitcoin.
1. Kako se dodaju novi blokovi, transakcija dobija potvrde, što je čini sigurnijom.

Kada je transakcija uključena u blok, ona je potvrđena. Adam više ne može da potroši taj bitcoin, a Gerard može da potroši ono što je primio u novoj transakciji.


> **Light**
>
> Transakcija i naknada izabrane → Potpisuje je novčanik i šalje → Distribuiraju čvorovi → Rudar dodaje transakciju u šablon bloka → Rudar pobeđuje u Proof-of-Work takmičenju → Novi blok se validira → Novi blok distribuiraju čvorovi


###### Resursi


[▶ Pogledaj ovaj video o Bitcoin čvorovima](https://www.youtube.com/watch?v=xc_TxlByxeY)
