# 3.2 Javna ključna kriptografija i protokoli

Danasšnji internet i većina savremenih računarskih sistema oslanjaju se na kriptografiju, metodu prikrivanja informacija tako da samo primalac može da ih dešifruje. Osnove kriptografije koja se koristi za zaštitu Bitcoina mogu se pratiti unazad do sedamdesetih godina.

Prvo pitanje koje treba rešiti je – kako poslati zajedničku tajnu preko nebezbednog kanala.

Ovim su se prvi put bavili Vitfild Difi i Martin Helman.

Problem: dve strane – obično nazvane Ana i Bob – žele da podele tajnu informaciju preko mreže na kojoj drugi mogu da prisluškuju. Da bi to postigli, kreirali su Difi-Helman proces razmene ključeva.

Ova zajednička tajna može se koristiti kao početna vrednost za kreiranje brojnih simetričnih ključeva za šifrovanje i dešifrovanje poruka koje šalju jedno drugom, bez potrebe da se ključ deli javno.

Pošto se privatni ključ nikada ne deli, a različiti ključevi se koriste na svakom kraju za šifrovanje i dešifrovanje, ovo se naziva asimetrični algoritam šifrovanja.

Primeri upotrebe:

* Ana potpisuje poruku Bobovim javnim ključem – samo on može da je dešifruje koristeći svoj privatni ključ
* Ana potpisuje poruku svojim privatnim ključem – dešifrovanjem njenim javnim ključem svako može da proveri da je poruku poslala Ana, bez otkrivanja njenog privatnog ključa
* Kombinovanjem ova dva pristupa sa dva sloja šifrovanja, poruka može biti poslata tako da samo Bob može da je dešifruje, a on zatim može da proveri da je pošiljalac zaista bila Ana

Iako nije potpisan na radu, Ralf Merkl je bio ključan u rešavanju onoga što se do tada smatralo nerešivom zagonetkom – kako uspostaviti ili ponovo uspostaviti privatnu komunikaciju preko otvorene i potencijalno neprijateljske mreže.

Ovaj pristup sam po sebi je podložan napadu grubom silom, gde napadač može uzeti zajedničke brojeve i na kraju rekonstruisati zajednički ključ ako ima dovoljno vremena i resursa, tako da ovo nije potpuno rešenje samo po sebi.

##### Protokoli za kriptosisteme sa javnim ključem

Pored doprinosa Difi-Helman sistemu javnog ključa opisanom iznad, **Ralf Merkl** nastavio je da doprinosi ovom polju dugi niz godina i bio je ključan u razvoju nekih važnih komponenti koje koristi Bitcoin.

Kriptografska heš funkcija je matematički algoritam koji prima ulaze bilo koje veličine i obrađuje složene proračune da bi vratio heš vrednost u bitovima, koja se obično prikazuje kao izlaz fiksne dužine u alfanumeričkom obliku koristeći heksadecimalni format.

* Ulazi mogu biti bilo koje veličine
* Izlaz je uvek fiksne dužine i deterministički (isti ulaz daje isti heš svaki put)
* Lako je proveriti, ali je izuzetno teško obrnuti proces i odrediti ulaz
* Mala izmena podataka potpuno menja izlaz

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/836bc2305274e9d71101de6b596d1892bc661dea-515x331.svg)

Heširanje je sastavni deo Bitcoin protokola. SHA-256, koji koristi Bitcoin, kreirala je NSA i to je primer kriptografske heš funkcije.

* Svaki blok u lancu se hešira tako da podaci ne mogu biti promenjeni – čime se obezbeđuje integritet distribuirane knjige
* Generisani heš mora da zadovolji kriterijum „Dokaza o radu“ da bi blok bio validan
* Merkleova stabla – korišćenjem grananja i hešova hešova, stabla hešova omogućavaju verifikaciju velikih skupova podataka uz minimalno skladištenje
* Heš zasnovani potpisi i ključevi mogu se koristiti za novčanike, adrese i autorizaciju transakcija

Distribuirana verifikacija stanja blokčejna i modela knjige koja se može samo dopunjavati, otpornih na izmene, omogućena je jednostranim heširanjem. Heš funkcije pružaju pouzdan, deterministički način za proveru događaja na javnim knjigama kao što je Bitcoin, bez centralizovanog modela poverenja.

Ove nove mogućnosti u oblasti kriptografije njihovi tvorci su očekivali da će doneti novi talas inovacija u ovom polju.

##### Kriptografija eliptičkih krivih

Jedna od kasnijih inovacija pojavila se u obliku kriptografije eliptičkih krivih.

Kriptografija eliptičkih krivih predstavljena je 1985. godine od strane dva naučnika, N. Koblitz-a i V. Miller-a. Oni su predložili ideju korišćenja tačaka definisanih eliptičkim krivama umesto konačnih prostih polja tako da pretpostavka problema diskretnog logaritma važi, kao što se obično koristi u standardnom Difi-Helman protokolu razmene ključeva. Detalji kako ovo funkcioniše prevazilaze opseg ovog odeljka, ali na visokom nivou, eliptička kriva je skup tačaka koje zadovoljavaju određenu matematičku jednačinu.

Jednačina za eliptičku krivu izgleda otprilike ovako:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Ovo ima nekoliko korisnih osobina:

* Horizontalna simetrija. Svaka tačka na krivi može se preslikati preko x ose i ostaje na istoj krivi.
* bilo koja nenvertikalna prava seče krivu u najviše tri tačke.
* Kompaktne veličine ključeva su ključne za efikasno skladištenje i prenos javnih ključeva u blokčejnu.

Ove osobine mogu se koristiti za kreiranje parova ključeva na sličan način kao kod Difi-Helman algoritma. Bitcoin koristi ECDSA, što je skraćenica za Digitalni potpisni algoritam eliptičkih krivih. To je proces koji koristi eliptičku krivu i konačno polje za „potpisivanje“ podataka na takav način da treća lica mogu da provere autentičnost potpisa, dok potpisnik zadržava isključivu mogućnost da kreira potpis. Kod bitcoina, podaci koji se potpisuju su transakcije koje prenose vlasništvo.

„Konačni“ deo je sličan „mod“ pristupu kod Difi-Helmana, gde se izlaz jednačine deli i koristi se ostatak kako bi se osiguralo da rezultat ostaje u okviru određenog raspona brojeva.
