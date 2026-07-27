# 8.1 Bezbednost putem kriptografije

> Ono što nam Bitcoin daje jeste čvrsto obećanje: program će se izvršiti tačno onako kako je navedeno.  
_Andreas M. Antonopoulos_

#### Javna/Privatna Ključna Kriptografija


> **Definition – Definicija Kriptografije**
>
> **Kriptografija** je praksa pretvaranja informacija u tajnu koju mogu pročitati samo pravi ljudi.


* **Enkripcija** je proces pretvaranja informacija u kodirani oblik tako da ih može pročitati samo onaj ko ima ispravan ključ.
* **Dekripcija** je proces vraćanja te kodirane informacije u čitljiv oblik.

U tradicionalnoj kriptografiji, dve osobe koje žele da komuniciraju privatno moraju prvo da podele isti tajni ključ, slično kao zajednička lozinka. Jedna osoba koristi taj ključ da šifruje poruku pre slanja, a druga koristi isti ključ da je dešifruje i pročita.

Problem sa ovim sistemom je što obe osobe moraju već da dele tajni ključ. Ako neko drugi dođe do tog ključa, može da pročita sve presretnute poruke.

Bitcoin rešava ovaj problem koristeći drugačiji pristup koji se zove kriptografija javnog ključa, gde korisnici ne moraju unapred da dele tajne ključeve.

Kriptografija javnog/privatnog ključa rešava problem deljenja tajni. Umesto deljenja lozinke, svaka osoba ima dva ključa: javni i privatni ključ.

* **javni ključ** može se podeliti sa bilo kim.
* **privatni ključ** mora uvek ostati tajan.

Ako Marko želi da pošalje nešto Ani, može koristiti Anin javni ključ. Samo Ana može to otključati koristeći svoj privatni ključ. Čak i ako neko presretne poruku, ne može je pročitati niti koristiti bez privatnog ključa.

U Bitcoinu, ovaj sistem se koristi za kreiranje digitalnih potpisa. Digitalni potpis dokazuje da je vlasnik privatnog ključa odobrio transakciju, slično kao kada potpisujete svoje ime na dokumentu. To omogućava da Bitcoin transakcije budu sigurne i proverljive bez potrebe za poverenjem trećoj strani.

Bitcoin transakcije podrazumevaju prenos vlasništva nad bitcoinom sa jedne adrese na drugu.

Enkripcija se koristi kako bi se osiguralo da samo pravi vlasnik bitcoina ima ovlašćenje da pošalje svoj novac nekome drugom. To osigurava da je njihova imovina zaštićena od zlonamernih aktera.

Kao dodatna mera zaštite, svaka Bitcoin transakcija automatski dobija JEDINSTVEN digitalni potpis. Ovaj jedinstveni digitalni potpis pokreće tehnologija otporna na manipulacije koja pomaže mreži da proveri da je pravi vlasnik bitcoina, a ne neko drugi, poslao sredstva.


> **Dark**
>
> Svaki korisnik ima dva ključa: **privatni ključ**, koji se **čuva u tajnosti**, i **javni ključ** koji se može **podeliti sa drugima**. **Privatni ključ** služi kao oblik identifikacije i dokaza vlasništva, potvrđujući: „Ova adresa pripada meni i ja imam kontrolu nad njom.“


###### Kako funkcioniše Bitcoin transakcija

1. **Kreiranje transakcije**: Korisnik pokreće Bitcoin transakciju tako što navodi detalje kao što su adresa primaoca i količina bitcoina koja se šalje.
1. **Generisanje digitalnog potpisa**: Pošiljalac generiše jedinstven **digitalni potpis** koristeći svoj **privatni ključ**. Ovaj potpis je jedinstven kod koji potvrđuje autentičnost transakcije.
1. **Slanje transakcije**: Potpisana transakcija se šalje Bitcoin mreži, čime se pokazuje namera da se vlasništvo nad bitcoinom prenese sa pošiljaoca na primaoca.
1. **Verifikacija na mreži**: Čvorovi na Bitcoin mreži primaju transakciju i koriste **javni ključ** da bi se proverila autentičnost potpisa transakcije. Istovremeno, koristi se pošiljalčev **javni ključ** da bi se proverio **digitalni potpis**.
1. **Potvrda na Bitcoin mreži**: Ako je verifikacija uspešna, transakcija će biti dodata u knjigu, koja služi kao siguran i transparentan zapis svih transakcija. Kada se potvrdi, vlasništvo nad bitcoinom se zvanično prenosi sa pošiljaoca na primaoca.


> **Callout – Rezime**
>
> Digitalni potpis**digitalni potpis**, kreiran pošiljalčevim **privatnim ključem**, dokazuje da je transakciju odobrio vlasnik bitcoina. Bitcoin mreža zatim može da proveri ovaj dokaz i zabeleži transakciju.


#### Objašnjenje heširanja

Molimo vas da vas ne uplaše tehnički termini i matematički koncepti koji slede. Razumemo da nisu svi zaljubljeni u matematiku, ali možda ćete se iznenaditi i videti da čak i najkompleksnije ideje mogu biti shvaćene uz malo truda.


> **Definition – Definicija funkcije**
>
> Funkcija**funkcija** je kao mašina koja uzima neku informaciju i pretvara je u nešto novo. Informacija koju dajete funkciji je **ulaz**. Nova informacija koju funkcija stvori je **izlaz**. Funkcije pomažu računarima da obavljaju zadatke i rešavaju probleme.


##### Šta je funkcija?

Funkcija je skup instrukcija koji uzima ulaz i proizvodi izlaz. Možete je zamisliti kao recept: pratite korake sa određenim sastojcima i uvek dobijete predvidljiv rezultat.

U Bitcoinu, funkcije se koriste za obradu i verifikaciju transakcija. Kada neko šalje bitcoin, kriptografske funkcije pomažu da se proveri da li je transakcija validna, potvrđuju da pošiljalac ima dovoljno sredstava i ažuriraju stanja na Bitcoin knjizi. Kada se transakcija verifikuje i doda u blok, ona postaje deo trajnog zapisa na blokčejnu.

##### Šta je jednosmerna funkcija?

Jednosmerna funkcija je posebna vrsta funkcije koja se lako izračunava u jednom smeru, ali je izuzetno teško vratiti je unazad. Na primer, lako je napraviti smuti od sastojaka, ali ne možete ponovo razdvojiti smuti na originalne sastojke.

Bezbednost Bitcoina se oslanja na jednosmerne funkcije. One se koriste u kriptografiji javnog i privatnog ključa, omogućavajući ljudima da dele javni ključ dok svoj privatni ključ drže u tajnosti. Iako je javni ključ vidljiv, nemoguće je iz njega izvesti privatni ključ. To je ono što čini Bitcoin transakcije sigurnim.

##### Šta je heš funkcija?

Heš funkcija**heš funkcija** je kao mašina za tajne kodove. Uzima poruku i pretvara je u kod.

###### Kako heširanje funkcioniše u Bitcoin transakcijama

U Bitcoinu, svaka transakcija se pretvara u heš pre nego što se doda na blokčejn. Heš je jedinstveni digitalni otisak transakcije. Ako neko pokuša da promeni i najmanji deo transakcije, heš će se potpuno promeniti. Ovo omogućava mreži da lako otkrije pokušaje menjanja podataka.

###### Uloga heširanja u bezbednosti Bitcoina

Heširanje pomaže u zaštiti Bitcoin mreže tako što transakcije čini lakim za proveru i nemogućim za tiho menjanje. Pošto svaka transakcija ima svoj jedinstveni heš, mreža može brzo da otkrije ako je nešto izmenjeno.

Heš funkcija uzima podatke i pretvara ih u fiksni niz brojeva i slova koji se zove heš. Isti ulaz će uvek proizvesti isti heš, ali čak i najmanja promena u ulazu stvara potpuno drugačiji rezultat. Ovo svojstvo omogućava računarima da provere da li podaci nisu promenjeni.


> **Definition – Definicija heširanja**
>
> **Heširanje** je kao pravljenje otiska prsta za digitalne podatke. To je proces uzimanja digitalne poruke i pretvaranja u kod fiksne dužine, koji služi kao jedinstveni identifikator. Kao što otisak prsta može identifikovati osobu, tako heš može identifikovati digitalnu poruku.


Izlaz**izlaz**, ili heš, uvek je iste dužine, bez obzira koliko je originalna informacija bila dugačka. Bitcoin koristi nekoliko specifičnih tipova heš funkcija kao što su **SHA-256** i **RIPEMD160**.

Nekoliko primera je ispod:

* SHA256 heš stringa **zdravo svete**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256 heš stringa **zdravo svete.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Primeti da mala promena ulaza potpuno menja izlaz u poređenju sa prvim primerom
* SHA256 heš preuzete iso datoteke **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Ovaj ulaz je ogromna datoteka, ali izlaz je i dalje iste fiksne dužine

Možeš takođe zamisliti heširanje kao muzičku partituru koja hvata suštinu muzičkog dela. Kao što je partitura jedinstvena reprezentacija melodije, tako je i heš vrednost jedinstvena reprezentacija podataka.

Upoređujući partituru muzičkog dela sa stvarnim izvođenjem, muzičar može da utvrdi da li je izvođenje tačno. Slično tome, upoređujući heš vrednost primljenih podataka sa originalnom heš vrednošću, može se utvrditi da li su podaci izmenjeni tokom prenosa.

Kao što i najmanje odstupanje u muzičkom izvođenju može učiniti da zvuči drugačije, tako i najmanja promena originalnih podataka dovodi do potpuno drugačije heš vrednosti. Ovo čini heširanje moćnim alatom za obezbeđivanje integriteta i autentičnosti Bitcoin transakcije.

Proces kodiranja **javnog ključa** kroz heširanje koristi se za poboljšanje bezbednosti informacija tako što ih pretvara u format fiksne dužine koji nije čitljiv. Bitcoin koristi SHA-256 i RIPEMD160 algoritme za generisanje javnih adresa. Dobijeni izlaz služi kao jedinstveni identifikator za **javni ključ** i pomaže u obezbeđivanju integriteta i sigurnosti transakcija koje se čuvaju u glavnoj knjizi. Šifrovanjem informacija na ovaj način, postaje mnogo teže neovlašćenim osobama da pristupe i manipulišu podacima.

##### Svojstva heš funkcije

* **Deterministička**: Isti sastojci uvek prave isti smuti. Na isti način, isti podaci će uvek proizvesti isti heš.
* **Otpornost na pre-image**: Ako imaš samo smuti, ne možeš da otkriješ tačno koje voće je korišćeno. Slično, ako imaš samo heš, ne možeš da utvrdiš originalne podatke.
* **Avalanš efekat**: Promena čak i najmanjeg dela sastojaka pravi potpuno drugačiji smuti. Kod heširanja, vrlo mala promena podataka daje potpuno drugačiji heš.
* **Otpornost na koliziju**: Izuzetno je teško pronaći dva različita skupa sastojaka koji prave potpuno isti smuti. Na isti način, izuzetno je malo verovatno da će dva različita podatka proizvesti isti heš.
* **Brzo za proveru**: Praviti smuti je brzo, i lako je proveriti da li je rezultat smuti. Heš funkcije se brzo računaju i svako može lako da proveri rezultat.

#### Aktivnost: Generiši SHA 256 heš


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Zanima te kako funkcioniše heširanje? Skeniraj QR kod i odmah generiši SHA256 heš od bilo koje reči, rečenice ili unosa po tvom izboru. Heš funkcije su kao digitalni otisci prsta: jednosmerne su, što znači da kada se nešto hešira, ne može se vratiti nazad. Probaj i uveri se sam!
