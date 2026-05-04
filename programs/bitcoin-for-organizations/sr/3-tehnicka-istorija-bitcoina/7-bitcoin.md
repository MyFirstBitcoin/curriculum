# 3.7 Bitcoin

Nakon mnogo godina i neuspešnih pokušaja, Sajferpankeri su uglavnom počeli da gube interesovanje za ideju digitalne valute bez dozvole, kada je Adam Back primio imejl sa linkom ka nacrtu belog papira pod nazivom ‘elektronski novac bez treće strane’ od anonimne osobe koja se predstavljala kao Satoshi Nakamoto.

Da rezimiramo do ovog trenutka, imamo bar sledeće ideje:

* Kriptografski potpisi koji mogu obezbediti određeni nivo privatnosti i anonimnosti
* Koncept valute bez pokrića (B-Money)
* Predlozi (ali ne i način) za ograničavanje izdavanja nove valute
* Digitalni novčići čije je vlasništvo određeno javnim ključevima (B-Money) i koji se mogu prenositi potpisivanjem i preusmeravati na osnovu adrese primaoca (RPOW i Hashcash)
* Svi čvorovi održavaju kopiju potpuno distribuirane knjige (B-Money) (u to vreme odbačeno kao nepraktično)
* Protokol vremenskog žiga – korišćenje Merkle stabla za heširanje radi matematički dokazive hronologije događaja koju je teško falsifikovati ako svi korisnici čuvaju iste zapise
* Dokaz o radu kao način povezivanja stvarnog truda sa sistemom (ali korišćenjem samog heša kao valute)
* Potpuno decentralizovane mreže gde su svi učesnici ravnopravni i mogu slobodno dolaziti i odlaziti iz mreže (BitTorrent)
* Koncept povezivanja novih heševa sa prethodnim heševima (Bit Gold i vremensko žigosanje)

Ono što je u tom trenutku nedostajalo uključivalo je:

* Izvodljivo rešenje za ‘problem vizantijskih generala’
* Metod za ograničavanje količine novca u opticaju uprkos stalnim hardverskim unapređenjima
* Sistem podsticaja za učešće ljudi (problem ‘kokoška ili jaje’)

Druga velika razlika između nedavnih pokušaja i Bitcoina bila je ta što je Satoshi neko vreme radio na kodu u pravom duhu ‘Sajferpankeri pišu kod’ pre nego što ga je objavio na mejling listama, za razliku od Bit Gold i B-Money koji su bili više konceptualni.

Koja je bila inovacija koja je izdvojila Bitcoin od prethodnih pokušaja elektronskog novca?

Dokaz o radu bi se koristio kao mehanizam konsenzusa i način obezbeđivanja sigurnosti i nepromenljivosti: Umesto da se heš koristi kao oblik novca, koristio bi se kroz novi konceptualni proces nazvan rudarenje, gde bi čvor grupisao skup transakcija, dodao nasumičan broj i zatim primenio heširanje na ‘blok’ podataka. Validan blok koji ispunjava zahtev za heš bi se zatim oglašavao mreži. Ovi blokovi bi se povezivali korišćenjem heša prethodnog bloka u svakom, a najduži blokčejn bi se koristio u slučaju podele gde različiti čvorovi istovremeno validiraju i oglašavaju različite blokove, stvarajući razdvajanje lanca. Dokaz o radu je postao distribuirani mehanizam za rešavanje problema vizantijskih generala.

Ovi rudari su takođe dobijali podsticaj da obezbede potrebnu procesorsku snagu za dokaz o radu tako što su im dodeljivani novi bitcoini za svaki blok. Količina Bitcoina koju dobijaju je takođe programirana da se smanjuje otprilike svakih 4 godine dok svi Bitcoini ne budu stvoreni, čime se postavlja čvrsta granica na ukupnu količinu Bitcoina koja će ikada biti u opticaju na 21 milion.

Najoriginalnija ideja bila je način na koji je rešio pitanje koliko novca se stvara kako se hardver unapređuje i više snage može biti primenjeno na mrežu. Vremenski žigovi određenog broja blokova (2016) bi se prosečno izračunavali, i ako se blokovi stvaraju prebrzo, heš potreban za kreiranje novog bloka bi se otežavao, a ako previše sporo, olakšavao. Ovo je ugrađeno u decentralizovani protokol koji svi čvorovi pokreću, tako da bi svaki rudar koji to ignoriše trošio energiju uzalud jer bi njegov blok bio odbijen od strane ostatka mreže. Ovo podešavanje obezbeđuje da kreiranje novih blokova ostane u planiranom rasporedu izdavanja i pruža podsticaje rudarima da ‘igraju po pravilima’.

####   
Rezime

Mnogi delovi slagalice potrebni za izgradnju decentralizovanog peer-to-peer elektronskog novčanog sistema zasnovanog na principima zdravog novca bili su već postavljeni pre nego što je Satoshi objavio svoj beli papir i ubrzo nakon početnog izdanja koda.

> Priroda Bitcoina je takva da je, kada je verzija 0.1 objavljena, osnovni dizajn bio zacrtan za ceo njegov životni vek  
_Satoshi Nakamoto_

Iako su mnoge ideje za poboljšanja (BIP-ovi) predlagane i usvajane, Bitcoin radi u pozadini još od 2009. godine prateći protokol ugrađen u početno izdanje i gotovo bez ikakvih prekida. Sva poboljšanja su urađena tako da omogućavaju kompatibilnost unazad sa svim prethodnim verzijama.



##### Beleške

1. Za objašnjenje problema vizantijskih generala - pogledajte [https://en.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
