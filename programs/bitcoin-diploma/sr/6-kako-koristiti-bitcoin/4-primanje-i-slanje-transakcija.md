# 6.4 Primanje i slanje transakcija

Bitcoin transakcija je prenos vlasništva bitcoina na novog vlasnika. Imajte na umu da se ne prenose stvarni novčići, već vlasništvo nad njima: drugim rečima, pravo da ih potrošite. Svaki put kada se transakcija prihvati u blok, svi čvorovi u mreži ažuriraju svoju lokalnu kopiju javne knjige kako bi odrazili promenu vlasništva. U tom smislu, Bitcoin transakcija je sličnija transakciji nekretnina (ili druge imovine) nego gotovinskoj transakciji.

Da bi "poslao" bitcoin, pošiljalac potpisuje poruku svojim privatnim ključem, signalizirajući mreži da je pravi vlasnik bitcoina preneo vlasništvo na primaoca.

Bitcoin će sada biti vezan za adresu primaoca, dajući mu vlasništvo nad bitcoinom, tako da samo novi vlasnik može da ih potroši koristeći svoj privatni ključ.

Nove Bitcoin transakcije pokreću se iz novčanika širom sveta, ali ne postoji centralni procesor plaćanja. Umesto toga, rudari se takmiče da zabeleže transakcije u knjizi.

Recimo da Marko duguje Jeleni 0,5 BTC i spreman je da joj vrati dug. Oboje imaju digitalne novčanike.

1. Jelena deli svoju adresu sa Markom.
1. Marko koristi softver svog novčanika da kreira transakciju, koja uključuje Jeleninu adresu, iznos koji se prenosi (0,5 BTC) i naknadu za rudara. Veće naknade povećavaju verovatnoću da će rudar uključiti transakciju u sledeći blok.
1. Nakon potpisivanja transakcije, ona se emituje mreži, gde je čvorovi proveravaju. Oni proveravaju da li Marko ima dovoljno sredstava i da li je pravi vlasnik novčića koje želi da potroši. Ako nije, odmah odbijaju transakciju.
1. Kada se transakcija verifikuje, rudari biraju da li će je dodati u sledeći blok, obično na osnovu izabrane naknade. Kada transakcija uđe u blok, dodaje se u blokčejn i sredstva se prenose na Jeleninu adresu.
1. Vlasništvo je preneto na Jelenu. Ona sada može koristiti svoj privatni ključ da potroši sredstva.

_Važno je napomenuti da, kada je transakcija završena, ne može se poništiti._


> **Light – Kako funkcioniše Bitcoin transakcija**
>
> 1. Neko zahteva transakciju
> 1. Transakcija se emituje P2P računarima (čvorovima)
> 1. Rudari verifikuju transakciju
> 1. Transakcije se kombinuju da formiraju blok podataka
> 1. Novi blok se dodaje postojećem blokčejnu
> 1. Transakcija je završena



> **Light – Primanje Bitcoin transakcija**
>
> Da biste primili bitcoin, potrebno je da pošiljaocu date Bitcoin javnu adresu. To je jedinstveni niz slova i brojeva koji predstavlja vaš novčanik i koristi se za njegovo prepoznavanje na Bitcoin mreži.
>
> Svoju javnu adresu možete pronaći tako što otvorite svoj Bitcoin novčanik i potražite opciju „Primanje“ ili „Depozit“ bitcoina.
>
> Svoju Bitcoin adresu možete podeliti na nekoliko načina:
>
> 1. **Kopirajte i nalepite adresu**: Možete kopirati adresu tako što je označite i pritisnete "Kopiraj", a zatim je nalepite u e-mail ili poruku.
> 1. **Podelite link ka svom Bitcoin novčaniku**: Neki Bitcoin novčanici omogućavaju da kreirate link ka svom novčaniku koji možete podeliti sa pošiljaocem. On tada može kliknuti na link da pristupi vašem novčaniku i pošalje bitcoin.
> 1. **Podelite QR kod**: Ako pošiljalac ima pametni telefon sa instaliranom Bitcoin aplikacijom, može skenirati QR kod da dobije vašu Bitcoin adresu.


Kada pošiljalac ima vašu adresu, može vam poslati bitcoin tako što unese vašu adresu i iznos koji želi da pošalje. Bitcoin se tada šalje iz njegovog novčanika u vaš.

Transakciju potvrđuje Bitcoin mreža i obično traje oko 10 minuta. Radi veće sigurnosti, preporučuje se da sačekate dve potvrde, što traje oko 20 minuta.


> **Light – Slanje Bitcoin transakcija**
>
> Da biste poslali bitcoin, potrebno vam je nekoliko stvari: Bitcoin novčanik, javna adresa primaoca i iznos bitcoina koji želite da pošaljete.
>
> 1. Otvorite svoj Bitcoin novčanik.
> 1. Idite na dugme „Pošalji“ i nalepite adresu primaoca u polje "Za". Alternativno, možete skenirati QR kod ako ga primalac obezbedi.
> 1. Unesite iznos bitcoina koji želite da pošaljete u polje „Iznos“.
> 1. Pažljivo proverite adresu primaoca i iznos koji šaljete. Zapamtite da su transakcije nepovratne!
> 1. Pre nego što kliknete na „Potvrdi i pošalji“, preporučujemo da još jednom proverite detalje transakcije kako biste bili sigurni da šaljete ispravan iznos bitcoina na ispravnu adresu.
> 1. Emitujte transakciju i sačekajte da mreža potvrdi transakciju.
>
> Sada znate kako da procenite, izaberete i podesite samostalni Bitcoin novčanik. Slanje i primanje bitcoina na Bitcoin mreži naziva se „on-chain“ transakcijama. To je zato što se transakcije odvijaju na glavnoj Bitcoin mreži i beleže u blokčejnu.
>
> On-chain transakcije su najsigurniji način za transakcije sa bitcoinom zbog decentralizovane verifikacije koju pruža mreža.
>
> Međutim, on-chain transakcije su sporije i mogu biti znatno skuplje od drugih opcija (o kojima ćemo govoriti u Modulu 7) zbog naknade za rudare.


#### Aktivnost: Transakcije u praksi


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Ovo je zajednička vežba koja pojednostavljuje osnovne uloge ljudi uključenih u Bitcoin transakciju.**

###### Ključne tačke

1. U svakoj bitcoin transakciji postoje četiri tipa učesnika: pošiljalac, primalac, rudari i operateri čvorova.
1. Pošiljalac mora da odobri (kriptografski potpiše) **iznos bitcoina** za slanje I **određenu adresu** na koju šalje.
1. Primalac mora da pošalje **važeću adresu** pošiljaocu I da proveri da li je transakcija uspešno potvrđena na blokčejnu.
1. Majneri proveravaju da li su svi kriterijumi ispravni pre nego što dodaju transakcije u buduće blokove.
1. Operatori čvorova proveravaju da li su iskopani blokovi ispravni pre nego što ažuriraju svoju verziju blokčejna (glavne knjige).

###### Savet za učenike

Rotirajte kroz sve četiri uloge kako biste iskusili šta svaki učesnik radi.
