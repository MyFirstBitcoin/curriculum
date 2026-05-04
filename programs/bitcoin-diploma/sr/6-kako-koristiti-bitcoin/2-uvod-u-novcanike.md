# 6.2 Uvod u novčanike

Za razliku od fizičkog novca, bitkoini se zapravo ne nalaze u Bitcoin novčaniku. Umesto toga, oni postoje na distribuiranoj knjizi koju Bitcoin mreža stalno proverava i obezbeđuje. Dakle, kako možete posedovati bitkoin?

Vi ste vlasnik svojih bitkoina samo ako kontrolišete privatne ključeve koji vam omogućavaju da potpisujete transakcije i prenesete vlasništvo nad svojim bitkoinima na nekog drugog. Ovo je čin slanja bitkoina.

Hajde da pogledamo dva pojma na koja mislimo kada koristimo izraz **novčanik**:

* Glavni privatni ključ, kao lozinka, iz kojeg se generišu vaši javni ključevi, kao adrese e-pošte. Svoju javnu adresu možete podeliti sa drugima da biste primali i slali bitkoin, ali nikada ne smete deliti svoj privatni ključ!
* Mobilni ili desktop interfejs koji se koristi za interakciju sa Bitcoin mrežom, proveru vašeg stanja bitkoina, slanje i primanje transakcija i njihovo emitovanje na mrežu. Različite vrste novčanika, zajedno sa njihovim prednostima i manama, biće opisane u narednim odeljcima.

#### Samostalni vs. poverenički novčanici

Pre nego što detaljno opišemo različite vrste Bitcoin novčanika i njihove karakteristike, napravimo važnu razliku između samostalnih i povereničkih novčanika. Svaka vrsta ima svoje prednosti, rizike i nivo kontrole nad bitkoinima. Samostalni znači da korisnik drži privatne ključeve i zaista kontroliše svoje bitkoine; kod povereničkih novčanika, treća strana drži bitkoine za korisnika.


| Tip | Kontrola | Prednosti | Rizici |
| --- | --- | --- | --- |
| Samostalni | Korisnik | Potpuna kontrola nad sredstvima i transakcijama, nema procesa odobravanja ili zamrzavanja naloga, nema korporativne ili državne kontrole, zaštićeno od zaplene. | Nema oporavka ako se fraza za oporavak izgubi, sva odgovornost je na korisniku. |
| Poverenički | Pružalac treće strane | Lak oporavak ako se pristup izgubi, lakša korisnička podrška. | Sredstva su povezana sa internetom, podložnija su hakerskim napadima. Poverenik može zamrznuti naloge. |


U samostalnom novčaniku (takođe nazvanom i nepoverenički novčanik), samo vi imate ključeve od novčanika i imate potpunu kontrolu nad onim što ulazi i izlazi. S druge strane, kod povereničkog novčanika neko drugi drži privatni ključ, što mu daje pun pristup da pomera bilo koji bitkoin koji taj pružalac kontroliše u vaše ime.

* Samostalno čuvanje je kao da ste sami sebi banka. Transakcije nisu podložne proveri i kontroli
* Samostalno čuvanje osigurava da treće strane ne mogu da zaplene vaše bitkoine.
* Samostalno čuvanje daje mir u vremenima neizvesnosti, jer znate da su vaši bitkoini sigurni.

Važno je izabrati pravu vrstu novčanika prema potrebama svake osobe. Ponekad je ljudima teško da razlikuju da li instaliraju samostalni ili poverenički novčanik. Ova tabela prikazuje razlike u procesu instalacije.


| Tip | Korak 1: Izaberite | Korak 2: Instalirajte | Korak 3: Kreirajte | Korak 4: Obezbedite |
| --- | --- | --- | --- | --- |
| Samostalni | Izaberite samostalni novčanik | Pratite uputstva novčanika | Generišite frazu za oporavak | Sačuvajte frazu za oporavak na sigurnom mestu |
| Poverenički | Izaberite poverenički novčanik | Pratite uputstva novčanika | Kreirajte nalog | N/A |


„**Nisu tvoji ključevi, nisu tvoji novčići**” je popularna izreka među vlasnicima bitkoina. Odnosi se na ideju da, ako nemate direktnu kontrolu nad privatnim ključevima povezanim sa vašim Bitcoin novčanikom, nemate pravo vlasništvo nad novčićima.

Ko god ima pristup vašim privatnim ključevima, ima vlasništvo nad vašim bitkoinima. Zato je izuzetno važno da ih zaštitite i držite dalje od radoznalih pogleda! Videćemo nekoliko načina kako to možete učiniti kasnije u knjizi.

U nastavku ćemo govoriti samo o samostalnim novčanicima, gde korisnik poseduje svoje ključeve i ima potpunu kontrolu nad svojim bitkoinima.

Ne brinite ako vam deluje komplikovano ili ne razumete sve — ovo je putovanje, i razumećete bolje što više budete koristili Bitcoin!

#### Različite vrste Bitcoin novčanika

Gde se vaš privatni ključ kreira i čuva određuje kako opisujemo Bitcoin novčanike. Ako su ključevi na vašem pametnom telefonu, to je **mobilni novčanik**. Ako su ključevi bezbedno sačuvani na posebnom uređaju, to je **hardverski novčanik**.


| Tip | Opis | Prednosti | Nedostaci | Primer korisnika |
| --- | --- | --- | --- | --- |
| Onlajn novčanik | Pristupa se putem veb pregledača | Dostupan sa bilo kog uređaja koji ima internet vezu | Manje bezbedan jer može biti hakovan ili kompromitovan | Mora često da pristupa svom novčaniku i nema mnogo sredstava za čuvanje |
| Mobilni novčanik | Instaliran na mobilnom uređaju | Jednostavan za korišćenje | Može biti izgubljen ako uređaj bude ukraden ili hakovan | Mora da obavlja transakcije u pokretu i nema mnogo sredstava za čuvanje |
| Desktop novčanik | Instaliran na desktop računaru | Pogodan i može mu se pristupiti sa bilo kog mesta | Može biti hakovan ako je računar zaražen malverom | Želi da čuva veću količinu bitkoina i snalazi se sa korišćenjem desktop računara |
| Hardverski novčanik | Fizički uređaj koji čuva bitkoin oflajn | Bezbedniji od onlajn novčanika i može se koristiti oflajn | Sredstva mogu biti nepovratno izgubljena | Želi da čuva veću količinu bitkoina i spreman je da plati za dodatnu bezbednost |


Pošto se ključevi mogu premeštati sa jednog uređaja na drugi, „status“ vašeg Bitcoin novčanika nije fiksan. Na primer, ako napravim ključeve svog novčanika na računaru, a kasnije ih prebacim na telefon, „desktop novčanik“ postaje „mobilni novčanik“.

Kada je reč o čuvanju vaših bitkoina, nije važno samo ko ima kontrolu nad ključevima — postoji još mnogo drugih rizika koje treba uzeti u obzir. Zato je važno pronaći rešenje za čuvanje koje je i bezbedno i praktično. Kada analizirate kompromise različitih tipova novčanika, shvatićete da ne postoji idealan novčanik koji zadovoljava sve potrebe.

##### Na šta obratiti pažnju pri izboru novčanika

* **Bezbednost**: Proverite da li novčanik ima jake mere zaštite.
* **Privatnost**: Razmislite da li novčanik zahteva lične podatke.
* **Jednostavnost korišćenja**: Izaberite novčanik koji je lak za korišćenje i snalaženje.
* **Kompatibilnost**: Proverite da li je novčanik kompatibilan sa vašim uređajem.
* **Naknade**: Uporedite naknade koje naplaćuju različiti novčanici.
* **Reputacija**: Proverite reputaciju programera kako biste bili sigurni da su pouzdani.
* **Kontrola**: Neki novčanici vam daju veću kontrolu nad vašim privatnim ključevima.

##### Otvoreni kod naspram zatvorenog koda

Još jedan važan faktor na koji treba obratiti pažnju pri izboru Bitcoin novčanika je da li je aplikacija ili softver otvorenog koda. Ovo je važno jer projekti otvorenog koda omogućavaju zajednici da pregleda kod i nastavi projekat ako tim prestane da radi na njemu. Baš kao što je kod Bitcoina potpuno otvoren za svakoga da ga pregleda, koristi i menja, tako bi trebalo da bude i kod novčanika koji koristite za upravljanje svojim bitkoinima.

#### Aktivnost: Diskusija i procena Bitcoin novčanika

https://bitcoin.org/en/choose-your-wallet

Posetite sledeći veb-sajt: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Iskoristite svoje novo znanje o Bitcoin novčanicima da izaberete onaj koji najbolje odgovara vašim potrebama na osnovu kriterijuma o kojima smo danas razgovarali.
