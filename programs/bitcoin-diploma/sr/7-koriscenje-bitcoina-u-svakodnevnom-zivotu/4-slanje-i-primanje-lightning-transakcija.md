# 7.4 Slanje i primanje Lightning transakcija

Sa Lightning novčanikom, korišćenje Bitcoina je brzo, jeftino i privatno, što olakšava transakcije između dvoje ljudi. Možete brzo slati i primati bitcoin za svakodnevne stvari kao što je kupovina kafe.

Hajde da pogledamo nekoliko primera kako Lightning mreža funkcioniše u praksi.

###### Primer 1

I Marija i Eva imaju po 5 jedinica valute. Marija želi da pošalje 2 jedinice Evi. Plaćanje prolazi kroz Jovana, koji pomaže da se uplata prenese preko Lightning mreže. Nakon što je plaćanje završeno, Eva ima 7 jedinica, a Marija 3.

Jovan pomaže u rutiranju plaćanja, ali ne može da ukrade sredstva. Lightning mreža koristi kriptografiju kako bi osigurala da samo predviđeni primalac može da primi uplatu. Jovan samo pomaže da uplata prođe kroz mrežu.

Ovo pokazuje ključnu prednost Lightning mreže: ljudi mogu brzo da šalju uplate bez poverenja u posrednike kao što su banke.

Operatori čvorova kao što je Jovan mogu takođe zaraditi male naknade za pomoć u rutiranju uplata. Na taj način pomažu da mreža ostane decentralizovana i efikasna.

U poređenju sa običnim Bitcoin transakcijama:

* **Transakcije na lancu** dešavaju se direktno na Bitcoin blokčejnu. Veoma su bezbedne, ali mogu biti sporije i skuplje.
* **Lightning transakcije** dešavaju se van lanca i omogućavaju da uplate budu mnogo brže i sa mnogo nižim troškovima.

Zbog toga je Lightning koristan za male, svakodnevne uplate, dok se transakcije na lancu često koriste za veće transfere ili dugoročno čuvanje.

###### Primer 2

Mina voli da jede napolju i često svraća u svoj omiljeni lokalni kafić. Sa toliko različitih opcija plaćanja, nije sigurna koja je najbolji izbor. Srećom, naučila je ponešto o Bitcoinu i Lightning mreži. Nakon što je razmotrila svoje opcije, Mina shvata da je korišćenje Lightning metode plaćanja najbolja opcija.

Mina želi da kupi kafu, ali plaćanje običnom Bitcoin transakcijom ponekad može potrajati i zahtevati veće naknade. Umesto toga, odlučuje da koristi Lightning mrežu.

Lightning mreža omogućava ljudima da šalju bitcoin trenutno i uz veoma niske naknade. Ovo je čini idealnom za male, svakodnevne kupovine kao što je kafa.

Da bi počela da koristi Lightning, Mina preuzima Lightning novčanik na svoj telefon. Zatim šalje malo bitcoina iz svog običnog Bitcoin novčanika u Lightning novčanik. Ovaj korak koristi standardnu Bitcoin transakciju na blokčejnu. Kada sredstva stignu u njen Lightning novčanik, mogu se koristiti na Lightning mreži.

Sada Mina može da plati kafić trenutno koristeći Lightning. Plaćanje se dešava van glavnog Bitcoin blokčejna, zbog čega je mnogo brže i jeftinije od obične transakcije na lancu.


| Prednosti | Lightning mreža | Tradicionalni bankarski sistem |
| --- | --- | --- |
| Brzina | Brzo | Sporo |
| Transparentnost | Transparentno | Netransparentno |
| Bezbednost | Bezbedno | Ranljivo |
| Naknade za transakcije | Niske | Visoke |
| Finansijska inkluzija | Visoka | Ograničena |
| Skalabilnost | Visoka | Niska |
| Privatnost | Visoka | Umerena |
| Interoperabilnost | Visoka | Niska |
| Pravna usklađenost | Umerena | Visoka |
| Isplativost | Visok | Umeren |


On-chain transakcije se dešavaju direktno na Bitcoin blockchain-u i mogu zahtevati više vremena i veće naknade. Lightning transakcije se odvijaju van lanca, omogućavajući brza i jeftina plaćanja, dok se i dalje koristi bitcoin.


| Visa, Inc. | Bitcoin On-chain | Lightning mreža |
| --- | --- | --- |
| Kapacitet od 65.000 transakcija u sekundi. | Kapacitet od 7 transakcija u sekundi. | Kapacitet od miliona transakcija u sekundi. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Ovo je mapa cele Lightning mreže. Zahvaljujući hiljadama pokretača Lightning čvorova, možete poslati sate bilo kom korisniku sa Bitcoin Lightning novčanikom, gde god da se nalazi u svetu. Plaćanje će stići za nekoliko sekundi i koštaće samo nekoliko dinara.**Pogledajte sami!**

#### Aktivnost: Lightning štafeta

https://qr.myfirstbitcoin.org/lightning.pdf

**Ovo je praktična vežba u kojoj učenici šalju i primaju prave sate koristeći Lightning mrežu.**

###### Ključne tačke

1. Korišćenje Lightning novčanika će vam pomoći da steknete samopouzdanje u primanju i slanju pravih sata.
1. Obratite pažnju na jedinice. Neki novčanici omogućavaju korisnicima da šalju bitcoin ILI sate (1/100.000.000 bitcoina).
1. Lightning plaćanja se ponekad mogu zaglaviti u rutiranju, posebno kod većih uplata. Iako je to moguće, ovakvo korisničko iskustvo postaje sve ređe kako mreža sazreva.

###### Savet za učenike

Proverite sa svojim instruktorom da li i kako trenutne naknade za on-chain Bitcoin transakcije utiču na Lightning novčanik koji koristite.
