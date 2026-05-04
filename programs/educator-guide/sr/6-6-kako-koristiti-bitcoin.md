# 6 - Kako koristiti Bitcoin

Trajanje: 90 minuta

Osnovna ideja: Korišćenje Bitcoina na lancu uči učenike kako vlasništvo, samostalno čuvanje i verifikacija funkcionišu u praksi, pretvarajući teoriju u direktnu finansijsku akciju.

#### Ciljevi učenja

Na kraju ove lekcije, učenici bi trebalo da budu u stanju da:

* Prepoznaju uobičajene načine za sticanje i razmenu bitcoina, uključujući peer-to-peer i metode centralizovanih menjačnica.
* Objasne razliku između samostalnih i skrbničkih novčanika, i zašto je samostalno čuvanje važno u Bitcoinu.
* Opisu svrhu privatnih ključeva, javnih adresa, seed fraza i interfejsa novčanika.
* Uporede različite tipove novčanika i procene njihove prednosti i mane na osnovu bezbednosti, praktičnosti, privatnosti i kontrole.
* Postave mobilni Bitcoin novčanik i objasne osnovni proces oporavka.
* Pokažu kako da prime i pošalju bitcoin transakciju na lancu.

Primene princip "Ne veruj, proveri" pri izboru novčanika, transakcijama i širem korišćenju Bitcoina.

#### Alati i resursi

##### Vizuelna pomagala

* Poglavlje 6 - Kako koristiti Bitcoin

##### Pomoćna biblioteka

* Karta sa rečnikom — Poglavlje 6 — Pojmovi: novčanik, privatni ključ, javna adresa, seed fraza, skrbnički, samostalni, UTXO, naknada za transakciju
* Tabele za poređenje i referentni listovi — Poređenje tipova novčanika (skrbnički, mobilni, hardverski, papirni)
* Tehnička objašnjenja i detaljna analiza — Javni/privatni ključevi, UTXO model, potvrda transakcije
* Detaljna analiza bezbednosti privatnog ključa — Seed fraze, derivacija ključeva, metode bekapa, vektori napada
* Vodič kroz anatomiju transakcije — Primer korak po korak kako funkcioniše Bitcoin transakcija
* Kontrolna lista najboljih bezbednosnih praksi — Pre početka, kreiranje novčanika, primanje, slanje, prevencija fišinga

#### Aktivnosti

* Transakcije u praksi
* Lightning štafeta
* Istraživanje mempool-a

#### Online nastava

* Od početka jasno stavite do znanja da li učenici gledaju demonstraciju ili sami podešavaju novčanik.
* Koristite velike, čitljive snimke ekrana za svaki korak podešavanja novčanika.
* Pauzirajte posle svakog koraka i tražite od učenika da potvrde razumevanje u četu pre nego što nastavite.
* Dajte direktno upozorenje pre dela o seed frazi i podsetite učenike da nikada ne dele osetljive informacije na internetu.

#### Priprema

* Preuzmite i testirajte aplikaciju za mobilni novčanik (Blue Wallet ili Muun); pripremite snimke ekrana ključnih koraka podešavanja.
* Pripremite vodič za podešavanje novčanika (preuzimanje → kreiranje → bekap seed fraze → primanje) za referencu.
* Proverite da li mreža/WiFi radi; pripremite demo adresu i QR kod za prikazivanje.

#### Procedura

Ova lekcija prelazi iz teorije u direktnu praksu. Sada se direktno poklapa sa strukturom Diplome tako da se sticanje, novčanici, podešavanje, transakcije i verifikacija pojavljuju pod istim glavnim naslovima kao i vodič za učenike. Dodatna podrška za nastavnike ostaje u okviru tih sekcija.

##### 6.0 Uvod, 8 minuta

Počnite povezivanjem ovog poglavlja sa prethodnim:

* Ako je Bitcoin novac, kako ga ljudi zapravo dobijaju i koriste?
* Šta znači zaista kontrolisati svoj bitcoin?
* Zašto je korišćenje Bitcoina drugačije od korišćenja aplikacije banke?

Objasnite da je ovo poglavlje o praktičnoj upotrebi. Učenici više ne uče samo šta je Bitcoin, već uče kako da direktno stupe u interakciju sa njim.

##### 6.1 Sticanje i razmena Bitcoina, 12 minuta

Objasnite da ljudi mogu steći bitcoin na različite načine, uključujući:

* primanje plate u bitcoinu
* rudarenje bitcoina
* zamenu dinara za bitcoin uživo
* zamenu dinara za bitcoin putem interneta

Zatim se fokusirajte na dva glavna načina sticanja koja su obrađena u poglavlju:

* peer-to-peer, uživo
* peer-to-peer, online
* centralizovane berze

Jasno istaknite kompromise.

Za P2P uživo, naglasite direktnu razmenu bez banke ili posrednika, ali takođe pomenite praktične rizike sastajanja sa ljudima radi trgovine za gotovinu.

Za P2P online, objasnite escrow jednostavnim rečima, kao način da se smanji rizik od druge strane, a da se i dalje omogući direktna razmena između korisnika.

Za centralizovane berze, jasno recite da su praktične, ali zahtevaju da korisnici veruju kompaniji, često dele lične podatke i ostavljaju sredstva pod kontrolom treće strane dok ih ne povuku. Ovo je dobar trenutak da naglasite da pogodnost često dolazi uz kompromise po pitanju privatnosti i suvereniteta.

##### 6.2 Uvod u Bitcoin novčanike, 35 minuta

**Šta je zapravo Bitcoin novčanik**

Odmah razjasnite čestu zabludu: bitcoin se ne čuva unutar aplikacije novčanika kao fizički novac u torbi.  
Bitcoin postoji na glavnoj knjizi koju održava mreža. Ono što korisnik kontroliše je mogućnost da ga potroši putem privatnih ključeva.

Zatim objasnite dve stvari na koje ljudi često misle kada kažu "novčanik":

* sistem privatnih ključeva, iz kojeg se generišu adrese
* aplikacija ili interfejs koji se koristi za interakciju sa mrežom

Koristite analogiju sa e-poštom iz ovog poglavlja ako je korisna:

* javna adresa = kao imejl adresa koju možete deliti
* privatni ključ = kao lozinka koju morate čuvati

Budite veoma jasni ovde: ko god kontroliše privatne ključeve, kontroliše bitcoin. To je osnovni koncept koji studenti moraju da razumeju.

**Samostalno čuvanje vs. čuvanje kod treće strane**

Ovo je jedan od najvažnijih delova poglavlja.

Jasno objasnite razliku:

* Samostalni novčanik: korisnik kontroliše privatne ključeve
* Novčanik kod treće strane: treća strana kontroliše privatne ključeve u ime korisnika

Zatim prođite kroz kompromise:

Samostalno čuvanje

* potpuna kontrola nad sredstvima
* nema procesa odobravanja
* zaštita od proizvoljne zaplene
* veća odgovornost
* nema lakog oporavka ako se seed fraza izgubi

Čuvanje kod treće strane

* lakši oporavak i podrška
* jednostavnije za početnike
* veća izloženost blokadi naloga, hakerskim napadima i kontroli treće strane
* korisnik zapravo ne drži bitcoin

Ovo je pravi trenutak da naglasite frazu:

"Not your keys, not your coins."

Studenti treba da iz ovog dela razumeju ne samo slogan, već i šta on zapravo znači u praksi.

**Različite vrste novčanika i kako izabrati jedan**

Predstavite vrste novčanika obrađene u ovom poglavlju:

* online novčanik
* mobilni novčanik
* desktop novčanik
* hardverski novčanik
* papirni novčanik

Nemojte nijedan predstavljati kao savršen. Umesto toga, objasnite da svaki ima kompromise između:

* bezbednosti
* privatnosti
* praktičnosti
* kompatibilnosti
* provizija
* kontrole
* ugled

Takođe jasno naglasite da preporučujemo obraćanje pažnje na to da li je softver novčanika otvorenog koda, jer alati otvorenog koda mogu biti pregledani, provereni i unapređivani od strane zajednice. Ovo je direktno povezano sa principom verifikacije u Bitcoinu.

##### 6.3 Podešavanje Bitcoin novčanika na mobilnom telefonu, 10 minuta

Provedite učenike kroz osnovni proces prikazan u ovom poglavlju:

* preuzmite novčanik
* kreirajte novi novčanik
* generišite i zapišite rezervnu frazu
* potvrdite rezervnu frazu
* dodajte dodatnu zaštitu ako je dostupna
* otvorite novčanik i pronađite opciju za primanje

Upozorenje o seed frazi mora biti veoma jasno:

* ako se seed fraza izgubi, pristup sredstvima može biti izgubljen
* ako neko drugi dođe do seed fraze, može preuzeti sredstva

Ako učenici ovo rade praktično, edukator treba da zastane na svakom koraku i proveri da li svi razumeju šta rade. Ako je čas više konceptualan, ovaj deo se može objasniti kao demonstracija umesto izvođenja uživo. Opcija za oporavak prikazana u poglavlju je takođe korisna za objašnjenje da novčanici mogu biti vraćeni ako je seed fraza pravilno sačuvana.

##### 6.4 Primanje i slanje transakcija, 17 minuta

**Primanje i slanje transakcija na lancu**

Sada objasnite kako funkcionišu transakcije na lancu.

Za primanje bitcoina:

* otvorite novčanik
* pritisnite na primi ili depozit
* kopirajte adresu, podelite link ili pokažite QR kod

Za slanje bitcoina:

* otvorite novčanik
* nalepite ili skenirajte adresu primaoca
* unesite iznos
* proverite sve detalje još jednom
* pošaljite transakciju
* sačekajte potvrdu

Jasno istaknite ove ključne tačke:

* transakcija prenosi vlasništvo, a ne fizičke novčiće
* transakcije su nepovratne
* čvorovi proveravaju ispravnost
* rudari uključuju transakcije u blokove
* naknade utiču na prioritet potvrde
* transakcije na lancu su generalno sigurne, ali sporije i često skuplje od Lightning transakcija

Dijagram toka transakcije u poglavlju je posebno koristan ovde, jer pomaže učenicima da vizualizuju put od zahteva iz novčanika do potvrde na mreži.

**Transakcije u praksi i vežba kroz uloge**

Koristite kooperativnu vežbu iz poglavlja da ojačate razumevanje. Objasnite četiri uloge koje su uključene:

* pošiljalac
* primalac
* rudar
* operator čvora

Jednostavan pristup u učionici je da se podele uloge i prođe kroz jednu transakciju korak po korak. Ovo pomaže učenicima da shvate da Bitcoin transakcija nije magija, već koordinisan proces koji uključuje odobravanje, proveru, uključivanje u blok i ažuriranje knjige.

Cilj ovde nije tehnička dubina. Cilj je da učenici razumeju ko šta radi u transakciji i zašto je verifikacija važna.

##### 6.5 Ne veruj, proveri, 8 minuta

Objasnite da se ovo odnosi na:

* novčanike
* menjačnice
* aplikacije
* detalje transakcije
* tvrdnje o "lakim profitima"
* projekti koji se pretvaraju da su kao Bitcoin

Jasno stavite do znanja da Bitcoin zahteva od korisnika da kritički razmišljaju, proveravaju ono što koriste i izbegavaju slepo poverenje. Takođe objasnite zašto su alati otvorenog koda važni u ovom kontekstu: oni omogućavaju nezavisnu proveru.

###### Završetak i provera razumevanja

Završite sa nekoliko brzih pitanja:

* Koja je razlika između kustodijalnog i samokustodijalnog novčanika?
* Zašto je seed fraza toliko važna?
* Šta se dešava kada pošaljete on-chain transakciju?
* Zašto su on-chain transakcije sporije od nekih drugih Bitcoin plaćanja?
* Šta u praksi znači "Ne veruj, proveri"?

#### Beleške za edukatore

Ovo poglavlje je veoma praktično, zato dajte prednost jasnoći, bezbednosti i ponavljanju.

Studenti ne moraju da savladaju sve tipove novčanika na jednom času. Glavni ciljevi su:

* razumevanje osnova novčanika
* razumevanje samokustodije
* učenje osnovnog toka transakcije
* usvajanje odgovornog načina provere

Budite posebno pažljivi kada govorite o seed frazama i podešavanju novčanika. Studenti treba da odu sa časa shvatajući da ovo nisu sitnice, već osnova vlasništva nad Bitcoin-om.

Najkorisniji vizuali i aktivnosti u ovom poglavlju su:

* poređenje samokustodijalnog i kustodijalnog novčanika
* tabela kompromisa tipova novčanika
* vežba postepenog podešavanja novčanika
* dijagram toka transakcije
* aktivnost transakcije po ulogama

##### Kako izgleda dobar rezultat

* Važno je da studenti zaista podešavaju novčanik ili gledaju pažljivu demonstraciju, da seed fraza bude u centru sa "Ovih 12 reči JESU tvoj Bitcoin", da se testiraju scenariji kao što je "Šta se dešava ako izgubiš telefon?" i da vežbaju prepoznavanje fišinga.
* Edukatori treba da budu praktični vodiči koji su ovo već radili, da budu svesni bezbednosti bez paranoje i da budu iskreni o težini i potrebnom učenju.
* Studenti osećaju da su naučili stvarnu veštinu koju mogu da koriste, razumeju da je seed fraza stvarna i važna, a ne apstraktna, osećaju se sposobnim da drže svoj Bitcoin i shvataju da decentralizacija zahteva ličnu odgovornost.
* Ishodi učenja su ispunjeni ako studenti mogu da podešavaju novčanik i razumeju razliku između javnih i privatnih ključeva, razumeju kompromise između kustodijalnih i samokustodijalnih novčanika, objasne kako funkcioniše transakcija uključujući ulaze, izlaze i naknade, pokažu svest o bezbednosti uključujući zaštitu seed fraze i postavljaju kritička pitanja o vlasništvu i kontroli.

##### Upravljanje vremenom

Ako je vremena malo, dajte prednost:

* Razumevanju osnova novčanika
* Razumevanju samokustodije
* Učenju osnovnog toka transakcije
* Usvajanju odgovornog načina provere

Ako ste ispred sa vremenom, posvetite vreme:

* Tabeli poređenja samokustodijalnog i kustodijalnog novčanika
* Tabeli kompromisa tipova novčanika
* Vežbi postepenog podešavanja novčanika sa demonstracijom uživo
* Dijagramu toka transakcije sa proračunom naknada
* Naprednim bezbednosnim praksama i razmatranju hardverskih novčanika

##### Ako studenti imaju poteškoća

* Seed fraze kao "stvarne" → "Ova fraza JE tvoj bitcoin; nema korisničke podrške."
* Javni vs. privatni ključevi → Analogija sa emailom (adresa vs. lozinka).
* Zašto je teško → "Ti kontrolišeš; ti si odgovoran." Priznajte kompromis.
