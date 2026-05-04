# 7.1 Lightning mreža

Lightning Network je platni sistem koji omogućava korisnicima da šalju i primaju bitcoin brzo i jeftino. Funkcioniše tako što se postavi zajednički novčanik u koji obe strane deponuju deo svog bitcoina. Zatim mogu međusobno obavljati neograničen broj transakcija bez potrebe da se svaka pojedinačno beleži na glavnom blockchainu. Na taj način zaobilaze potrebu da se svaka transakcija verifikuje i uključi u blok, što čini proces i brzim i isplativim. Niže naknade znače da se Lightning Network može koristiti za male uplate koje nisu uvek isplative na lancu. Kada strane odluče da završe saradnju, samo konačno stanje se beleži na blockchainu.

Zamislite dan kada radite u kafiću. Planirate da ostanete duže, pa otvarate račun i unapred plaćate umesto da plaćate svaku porudžbinu posebno. Na kraju dana, vi i vlasnik pregledate račun da biste izmirili dug. Ako je vaš depozit veći od onoga što ste potrošili, dobijate razliku nazad; ako ste potrošili više, plaćate ono što još dugujete.

Ova šema može da se proširi i na više učesnika. Na primer, tokom jedne od vaših poseta kafiću, dovodite prijatelja kojeg barmen ne poznaje i ne može mu otvoriti račun. Vi nudite svom prijatelju da koristi vaš postojeći račun za svoje troškove, i dogovarate se da će vam on kasnije privatno vratiti novac. Zamislite sada hiljade ljudi koji rade isto u isto vreme, omogućavajući drugima da koriste postojeće račune kako bi se povezali sa još više ljudi — tako funkcioniše Lightning Network!

Uz Lightning, možete slati uplate bilo kome na mreži, ne samo osobi sa kojom direktno delite račun — pod uslovom da postoji ruta između dve strane. Vaša uplata može proći kroz mrežu dok ne stigne do odredišta, čak i ako nemate otvoren kanal direktno sa primaocem.

Pogledajmo razliku između on-chain i off-chain transakcija.

##### On-chain transakcije

Ovo su transakcije koje se dešavaju direktno na Bitcoin blockchainu. Potrebno je oko 10 minuta da se potvrde, a naknade zavise od veličine transakcije u virtuelnim bajtovima. One su sigurnije, ali sporije, jer zahtevaju konsenzus mreže.

##### Lightning Network transakcije

Ove transakcije se odvijaju na posebnoj mreži izgrađenoj na vrhu Bitcoin blockchaina. One se izvršavaju brže i uz niže naknade. Najčešće se koriste tamo gde su brzina i trošak transakcija važniji. U poređenju sa on-chain transakcijama, manje su sigurne.


|  | Bitcoin mreža | Lightning Network |
| --- | --- | --- |
| Definicija | Decentralizovana digitalna mreža koja koristi kriptografiju za obezbeđivanje finansijskih transakcija. | Protokol za plaćanje drugog sloja koji funkcioniše na vrhu Bitcoin blockchaina, omogućavajući brže i jeftinije transakcije. |
| Prednosti | Decentralizovano i sigurno. Nema povraćaja novca ili prevara. Može se koristiti pod pseudonimom. Globalno prihvaćeno. | Brže i jeftinije transakcije. Veća skalabilnost. Off-chain transakcije ne opterećuju blockchain. |
| Nedostaci | Sporo vreme transakcija. Visoke naknade za određene vrste transakcija. Složeno za početnike. | Može zahtevati poverenje u operatere kanala. Potrebna je on-chain transakcija za otvaranje i zatvaranje kanala. |
