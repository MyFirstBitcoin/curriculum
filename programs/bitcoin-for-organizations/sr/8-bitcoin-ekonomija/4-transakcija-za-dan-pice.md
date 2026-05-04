# 8.4 Transakcija za Dan pice

Do sada se ovaj modul fokusirao na korišćenje otvorene prirode Bitcoin glavne knjige za sastavljanje korisnih metrika iz agregiranih podataka o transakcijama. Međutim, moguće je koristiti podatke iz glavne knjige i blok eksplorere da se ispitaju stvarne transakcije i prati kretanje sredstava unutar mreže.

Svake godine, 22. maja, Bitcoin zajednica odaje priznanje Laszlu Hanječu, koji je postao prva osoba za koju je zabeleženo da je koristila bitcoin za kupovinu fizičkih dobara. Dana 18. maja 2010. godine, Hanječ je na forumu Bitcointalk.org objavio da traži picu i da je spreman da plati u BTC-u. Ponudio je 10.000 BTC svakome ko je bio voljan da uđe u tu transakciju. Čekao je nekoliko dana, dok se nije javio devetnaestogodišnji student Marko Sturdivant i poslao dve velike pice.

Transakcija za **Pizza Day** može biti pregledana od strane bilo koga i ima sledeći ID transakcije:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Unosom ovog ID-a transakcije na [mempool.space](https://mempool.space) otkriva se sledeće:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Datum i vreme transakcije: 22. maj 2010.

Mrežna naknada za transakciju: 99.000.000 satošija (u to vreme to je bilo manje od 1 srpskog dinara. U maju 2025. to iznosi 10.900,00 €)

Visina bloka: 57.043

Broj potvrda: 838.645 (ovo je broj blokova dodatih u glavnu knjigu nakon ove transakcije)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Broj ulaza u transakciji: 131

Broj izlaza u transakciji: 1

Klikom na izlazni javni ključ (koji se završava na `XaxFyQ`) za koji znamo da je pripadao Marku Sturdivantu, koji je primio 10.000 BTC za dve pice, otkriva se sledeće:

Ova adresa trenutno ima stanje od 0,00257879 BTC i izgleda da je bila uključena u 14 transakcija, od kojih je poslednja bila 13. decembra 2024.



#### 8.4.1 Aktivnost: Grupna diskusija

1. Opišite prednosti (npr. revizija, odgovornost) ili rizike (npr. zabrinutost za privatnost) za pojedince ili preduzeća koja koriste ovako transparentan i otvoren sistem transakcija.
1. Kako bi ovakav nivo finansijske transparentnosti mogao da utiče na industrije kao što su humanitarne organizacije, javne nabavke, doznake ili sprovođenje zakona?
1. Da li bi tradicionalni bankarski sistemi trebalo da ponude sličan nivo vidljivosti? Da li će ih tržište na to naterati?
