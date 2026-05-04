# 8 - Kako Bitcoin funkcioniše

Trajanje: 90 minuta

Osnovna ideja: Bezbednost Bitcoina zavisi od jednostavnih, ali moćnih tehničkih koncepata kao što su ključevi, potpisi, heširanje i UTXO-ovi, koji omogućavaju vlasništvo i proveru bez centralnog autoriteta.

#### Ciljevi učenja

Na kraju ove lekcije, učenici bi trebalo da budu u stanju da:

* Objasne kako javni i privatni ključevi pomažu u zaštiti vlasništva i transakcija Bitcoina.
* Opisu šta je digitalni potpis i kako dokazuje da je transakciju odobrio pravi vlasnik.
* Objasne, jednostavnim rečima, šta znače kriptografija, enkripcija i dekripcija u kontekstu Bitcoina.
* Definišu heširanje i opišu zašto su heš funkcije važne za bezbednost i integritet podataka u Bitcoinu.
* Prepoznaju osnovna svojstva heš funkcije, kao što su izlaz fiksne dužine, jednosmernost i osetljivost na male promene ulaza.
* Objasne UTXO model i kako se bitcoin troši, prima i vraća kao kusur kroz izlaze transakcija.
* Opišu kako čvorovi pomažu u sprečavanju dvostrukog trošenja proverom da li je izlaz već potrošen.

#### Alati i resursi

##### Vizuelna pomagala

* Poglavlje 8 - Kako Bitcoin funkcioniše

##### Pomoćna biblioteka

* Karta pojmova — Poglavlje 8 — Pojmovi: kriptografija, heš, UTXO, digitalni potpis, privatni/javni ključ, merkle stablo, blokčejn
* Biblioteka zabluda — Poglavlje 8 — Adresira: "izgubljena seed fraza može biti povraćena", "privatni ključ = lozinka", "blokčejn je anoniman"
* Tehnička objašnjenja i detaljna razmatranja — Heš funkcije, javni/privatni ključevi, UTXO model, sigurnost Proof of Work-a

#### Aktivnosti

* Transakcije u praksi
* Istraživanje mempool-a

#### Online nastava

* Koristite digitalnu tablu i crtajte svaki koncept uživo umesto da se oslanjate samo na usmeno objašnjenje.
* Predajte jednu tehničku ideju u isto vreme i često pravite pauze za proveru razumevanja.
* Koristite vizuelna pomagala za ključeve, potpise, hešove i UTXO-ove kako bi učenici mogli da prate strukturu.
* Držite se konceptualnog cilja i izbegavajte previše duboko ulazak u matematiku ili žargon.

#### Priprema

* Pripremite i plastificirajte dijagrame: parove javnog/privatnog ključa, digitalne potpise, UTXO model, heširanje (jednosmerna funkcija).
* Obeležite blokčejn istraživač i SHA-256 kalkulator heša; izaberite 2-3 prave Bitcoin transakcije za detaljnu analizu korak po korak.
* Pripremite beleške na tabli za objašnjavanje ulaza, izlaza i kako se transakcije potvrđuju na blokčejnu.

#### Postupak

Ova lekcija daje učenicima prvi uvid u tehničku stranu Bitcoina bez pretpostavke prethodnog tehničkog znanja. Vodič sada prati istu sažetu strukturu kao i Diploma, sa kriptografijom pod jednim naslovom i UTXO-ima pod drugim.

##### 8.0 Uvod, 8 minuta

Počnite postavljanjem očekivanja:

* Šta čini Bitcoin sigurnim ako ne postoji centralna banka koja ga kontroliše?
* Kako mreža može da zna da li osoba zaista poseduje bitcoin koji pokušava da pošalje?
* Šta se zapravo dešava u pozadini kada neko napravi Bitcoin transakciju?

Počistite da se ovo poglavlje fokusira na osnovne tehničke temelje Bitcoina, posebno ključeve, potpise, heširanje i UTXO-ove. Takođe, uverite učenike da ne moraju postati inženjeri da bi razumeli osnovnu logiku. Samo poglavlje to jasno ističe poređenjem Bitcoina sa internetom — mnogi ga koriste svakodnevno, a da ne razumeju svaki sloj ispod površine.

##### 8.1 Sigurnost kroz kriptografiju, 57 minuta

**Bitcoin kao knjiga računa sačuvana na mnogim računarima**

Počnite sa jednostavnim objašnjenjem iz poglavlja o Bitcoin mreži:

* Bitcoin je zapis transakcija
* taj zapis se čuva na mnogim računarima koji se zovu čvorovi
* knjiga računa je javna i pseudonimna
* prikazuje adrese i istoriju transakcija, a ne lične podatke o identitetu

Ovaj deo pomaže učenicima da se povežu sa onim što već znaju iz prethodnih poglavlja. Bitcoin se ne zasniva na skrivenim računima unutar banke. Zasniva se na zajedničkoj knjizi računa koju mnogi učesnici mogu da provere. je posebno korisno ovde jer prikazuje korisnike, novčanike i širu Bitcoin mrežu povezanu sa javnom knjigom računa.

**Javni i privatni ključevi**

Sada pređite na kriptografiju.

Objasnite da svaki korisnik Bitcoina ima:

* privatni ključ, koji mora ostati tajan
* javni ključ, koji se može deliti

Objasnite njihovu svrhu jednostavnim rečima:

* privatni ključ dokazuje kontrolu i ovlašćuje trošenje
* javni ključ pomaže drugima da provere da li je transakcija ispravno ovlašćena

Važna nastavna tačka iz ovog poglavlja je da Bitcoin koristi kriptografiju sa javnim i privatnim ključem, a ne stariji model gde dve osobe prvo moraju da podele istu tajnu. To je važno jer omogućava sigurnu proveru bez potrebe da korisnici otkrivaju tajnu koja štiti njihova sredstva.

Možete to objasniti ovako:

* privatni ključ je kao tajni dokaz da bitcoin pripada vama
* javni ključ je deo onoga što omogućava mreži da proveri vaše ovlašćenje
* ko god kontroliše privatni ključ, kontroliše mogućnost trošenja bitcoina

Pazite da ovde ne zakomplikujete jezik o enkripciji. Najvažnija stvar za učenike je vlasništvo i ovlašćenje.

**Digitalni potpisi i ovlašćivanje transakcija**

Sada objasnite šta se dešava kada neko šalje bitcoin.

Koristite redosled iz poglavlja:

* korisnik kreira transakciju
* pošiljalac generiše digitalni potpis koristeći svoj privatni ključ
* transakcija se emituje mreži
* čvorovi proveravaju da li je potpis ispravan
* kada je potvrđeno i verifikovano, vlasništvo se prenosi u knjizi

Jasno naglasite da digitalni potpis nije isto što i upisivanje imena. To je kriptografski dokaz da je pravi vlasnik ovlastio transakciju. Ovo je jedan od osnovnih mehanizama koji omogućava da Bitcoin funkcioniše bez centralnog autoriteta koji ručno odobrava transakcije. Dijagram je koristan jer vizuelno prikazuje potpisivanje i verifikaciju, kao i putanju transakcije od pošiljaoca do validacije na mreži.

Dobra rečenica za čas je:

Bitcoin transakcije nisu odobrene zato što to kaže banka. One su prihvaćene zato što mreža može da proveri validan kriptografski dokaz.

**Hešovanje i jednosmerne funkcije**

Zatim objasnite hešovanje.

Počnite jednostavno:

* funkcija uzima ulaz i proizvodi izlaz
* jednosmerna funkcija je laka za izvođenje u jednom smeru, ali je praktično nemoguće vratiti je unazad
* heš funkcija uzima podatke bilo koje veličine i pretvara ih u izlaz fiksne dužine koji se zove heš

Koristite neku od analogija iz poglavlja, onu koja je najjasnija vašoj publici:

* analogija sa smutijem za jednosmerne funkcije
* analogija sa otiskom prsta za heš vrednosti
* analogija sa muzičkom partiturom za proveru da li se nešto promenilo

Analogija sa otiskom prsta je verovatno najjasnija za većinu učenika:

* heš je kao digitalni otisak prsta za podatke
* ako se ulaz promeni i najmanje, heš se potpuno menja
* ovo pomaže računarima da provere integritet i otkriju manipulacije

Zatim objasnite zašto je hešovanje važno u Bitcoinu:

* transakcije se hešuju
* mreža koristi heš vrednosti da bi proverila integritet
* ako se transakcija promeni, menja se i heš
* ovo pomaže da se knjiga zaštiti od neprimećenih manipulacija

Vizuali na stranicama 7 do 10 su ovde veoma korisni. Poglavlje prikazuje i ideju izlaza fiksne dužine i princip „mala promena, potpuno drugačiji rezultat“, što je jedan od najvažnijih pojmova koje učenici treba da razumeju.

**Osnovna svojstva heš funkcija**

Ukratko prođite kroz svojstva istaknuta u poglavlju, bez previše akademskog pristupa:

* Deterministička: isti ulaz daje isti izlaz svaki put
* Jednosmerna / pre-image otpornost: ne možete realno vratiti proces unazad
* Osetljiva na promene: čak i mala promena ulaza daje potpuno drugačiji izlaz
* Otpornost na kolizije: izuzetno je teško pronaći dva različita ulaza sa istim izlazom
* Brza za proveru: funkcija je efikasna za izvršavanje i proveru

Nije potrebno da učenici pamte svaki termin, ali treba da razumeju osnovnu poentu: hešovanje daje Bitcoinu pouzdan način da identifikuje podatke i otkrije promene.

##### 8.2 UTXO model, 25 minuta

**UTXO model**

Sada prelazimo na drugi glavni deo poglavlja: UTXO-e, odnosno Neutrošene Izlaze Transakcija.

Objasnite to jednostavnim rečima koristeći analogiju sa gotovinom iz poglavlja:

* bitcoin se ne prati samo kao stanje na bankovnom računu
* umesto toga, sastoji se od delova koji se mogu potrošiti, zvanih UTXO-i
* kada trošite bitcoin, koristite jedan ili više postojećih UTXO-a kao ulaze
* novi UTXO-i se tada stvaraju kao izlazi

Koristite primer iz poglavlja:

* ako imate UTXO od 10 BTC
* i pošaljete 6 BTC
* novi UTXO od 6 BTC ide primaocu
* novi UTXO za kusur se vraća vama
* mali deo se plaća kao nagrada rudaru

To pomaže učenicima da shvate da Bitcoin funkcioniše više kao trošenje gotovine i dobijanje kusura nego kao prosto oduzimanje brojeva sa jednog računa. Dijagrami su ovde posebno korisni jer vizuelno prikazuju kako se jedan UTXO deli na izlaz za primaoca, izlaz za kusur i naknadu.

Istaknite dve ključne stvari:

* stanje vašeg novčanika je zbir vaših UTXO-a
* kada trošite, stari UTXO-i se troše, a novi se stvaraju

**Sprečavanje dvostrukog trošenja**

Završite sadržaj objašnjavajući jednu od najvažnijih posledica UTXO modela.

Ako neko pokuša da potroši isti izlaz dva puta, čvorovi odbijaju drugi pokušaj jer održavaju knjigu i mogu da provere da li je taj UTXO već potrošen. Tako Bitcoin sprečava dvostruko trošenje bez potrebe za centralnom platnom kompanijom koja bi vodila evidenciju. Primer je ovde veoma koristan jer prikazuje kako Ana kombinuje UTXO-e, šalje sredstva Bobanu, dobija kusur i kako potvrđena transakcija ažurira knjigu na svim čvorovima.

Jasan način da to kažete na času je:

Bitcoin sprečava dvostruko trošenje jer mreža prati koji izlazi su još uvek nepotrošeni, a koji su već iskorišćeni.

###### Završetak i provera razumevanja

Završite sa nekoliko brzih pitanja:

* Koja je razlika između javnog i privatnog ključa?
* Šta dokazuje digitalni potpis?
* Zašto je heširanje korisno u Bitcoinu?
* Šta se dešava ako se transakcija promeni nakon što je heširana?
* Šta je UTXO jednostavnim rečima?
* Kako mreža sprečava nekoga da potroši isti bitcoin dva puta?

#### Beleške za edukatore

Ovo poglavlje sadrži više tehničkog jezika nego prethodna, zato dajte prednost jasnoći, analogijama i ponavljanju.

Cilj nije da učenici postanu programeri. Cilj je da razumeju zašto Bitcoin sigurnost funkcioniše.

Najvažnije tačke na koje treba staviti akcenat, ako je vremena malo, su:

* privatni ključ naspram javnog ključa
* digitalni potpisi
* čemu služi heširanje
* UTXO-i kao delovi bitcoina koji se mogu potrošiti
* kako se sprečava dvostruko trošenje

Najkorisnije ilustracije u ovom poglavlju su:

* dijagram korisnik-novčanik-mreža
* vizuelizacija digitalnog potpisa
* primeri heširanja i dijagrami izlaza fiksne dužine na stranicama 7 do 10
* UTXO dijagrami na stranicama 10 do 12

##### Kako izgleda dobar čas

* Važno je tretirati kriptografiju kao osnovu, a ne kao misteriju, koristiti mnogo vizuelnih prikaza, izbegavati duboku matematiku, povezivati sa prethodnim poglavljima i proveravati razumevanje kroz primene kao što je „Ako neko promeni jednu transakciju, šta se kvari?“
* Edukatori treba da budu strpljivi sa učenicima kojima je teško, da razmišljaju vizuelno i sve crtaju, da budu iskreni oko onoga što učenici ne moraju da znaju, da budu spremni da kažu „Ne znam, ali evo kako bismo to saznali“, i da ostanu ohrabrujući tokom celog procesa.
* Učenici razumeju zašto Bitcoin ne može biti hakovan jer ga štiti matematika, poštuju elegantan dizajn sistema, osećaju se prijatno sa složenošću znajući da ne moraju znati svaki detalj, stiču samopouzdanje da postavljaju pitanja bez osude i prepoznaju da su napredovali u razumevanju nečega što većina ljudi ne zna.
* Ishodi učenja biće ispunjeni ako učenici mogu da objasne osnove kriptografije kao što su jednosmerne funkcije i digitalni potpisi bez duboke matematike, razumeju UTXO model koji pokazuje da posedujete novčiće, a ne račune, prepoznaju heširanje kao osnovu sigurnosti Bitcoina, razumeju anatomiju transakcije uključujući potpise i potvrde, objasne zašto je Bitcoin nepromenljiv i postavljaju kritička pitanja o potencijalnim napadima ili ranjivostima.

##### Upravljanje vremenom

Ako je vremena malo, dajte prednost:

* Privatni ključ vs javni ključ
* Digitalni potpisi
* Šta radi heširanje
* UTXO kao potrošivi delovi bitkoina
* Kako se sprečava dvostruko trošenje

Ako ste ispred, posvetite vreme:

* Dijagram korisnik-novčanik-mreža i vizuelni model bezbednosti
* Vizuelizacija digitalnog potpisa: detaljan kriptografski proces
* Merkleova stabla i bezbednost lanca
* Napredni vektori napada i zašto ne uspevaju

##### Ako se učenici muče

* Kriptografija kao preteća → „Koristiš je svakodnevno; My First Bitcoin je koristi na isti način.“
* Heširanje kao koncept → Analogija otiska prsta; jedinstven je, ne može se promeniti bez promene heša.
* Digitalni potpisi → „Dokazuje ovlašćenje bez otkrivanja lozinke.“
