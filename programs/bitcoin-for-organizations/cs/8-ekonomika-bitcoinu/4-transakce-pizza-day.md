# 8.4 Transakce Pizza Day

Doposud se tento modul zaměřoval na využití otevřené povahy bitcoinové účetní knihy k sestavování užitečných metrik z agregovaných dat o transakcích. Je však možné využít data z účetní knihy a blokové průzkumníky k prozkoumání skutečných transakcí a sledování pohybu prostředků v rámci sítě.

Každý rok 22. května si bitcoinová komunita připomíná Laszla Hanyecze, který se stal prvním člověkem, o němž je známo, že použil bitcoin k nákupu fyzického zboží. Dne 18. května 2010 Hanyecz oznámil na fóru Bitcointalk.org, že má chuť na pizzu a je ochoten za ni zaplatit v BTC. Nabídl 10 000 BTC komukoliv, kdo bude ochoten tuto transakci uskutečnit. Čekal několik dní, až nakonec devatenáctiletý student Jakub Novák souhlasil a poslal dvě velké pizzy.

Transakce **Pizza Day** je dostupná ke zhlédnutí pro kohokoliv a má následující ID transakce:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Zadáním tohoto ID transakce do [mempool.space](https://mempool.space) se zobrazí následující:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Datum a čas transakce: 22. května 2010

Síťový poplatek za transakci: 99 000 000 satů (v té době to bylo méně než 1 cent v USD. V květnu 2025 to činí 95 072,67 USD)

Výška bloku: 57 043

Počet potvrzení: 838 645 (to je počet bloků přidaných do účetní knihy po této transakci)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Počet vstupů transakce: 131

Počet výstupů transakce: 1

Kliknutím na veřejný klíč výstupu (končící na `XaxFyQ`), o kterém víme, že patřil Jakubu Novákovi, který obdržel 10 000 BTC za dvě pizzy, se zobrazí následující:

Tato adresa má aktuálně zůstatek 0,00257879 BTC a zdá se, že byla zapojena do 14 transakcí, z nichž poslední proběhla 13. prosince 2024.



#### 8.4.1 Aktivita: Skupinová diskuse

1. Popište výhody (např. auditovatelnost, odpovědnost) nebo rizika (např. obavy o soukromí) pro jednotlivce nebo firmy využívající takto transparentní a otevřený systém transakcí.
1. Jak by tento druh finanční transparentnosti mohl ovlivnit odvětví jako jsou charita, vládní zakázky, remitence nebo vymáhání práva?
1. Měly by tradiční bankovní systémy nabízet podobnou úroveň viditelnosti? Budou k tomu donuceny trhem?
