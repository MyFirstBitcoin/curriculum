# 9 - Kako funkcioniše rudarenje Bitcoina

Trajanje: 90 minuta

Osnovna ideja: Rudarenje Bitcoina i validacija čvorova zajedno rade na obezbeđivanju mreže, potvrđivanju transakcija i sprovođenju pravila sistema putem Dokaza o radu (Proof of Work).

#### Ciljevi učenja

Na kraju ove lekcije, učenici bi trebalo da budu u stanju da:

* Objasne razliku između uloge Bitcoin čvorova i uloge Bitcoin rudara.
* Opisu kako čvorovi proveravaju transakcije, dele informacije i pomažu u sprovođenju Bitcoin pravila.
* Objasne šta rade rudari, uključujući izbor transakcija, izgradnju kandidatskih blokova i takmičenje u pronalaženju važećeg heša bloka.
* Definišu mempool i objasne zašto funkcioniše kao čekaonica za nepotvrđene transakcije.
* Opisu kako naknade za transakcije utiču na izbor rudara i brzinu potvrde.
* Objasne Proof of Work kao mehanizam koji obezbeđuje Bitcoin tako što napadi postaju skupi.
* Opisu kako prilagođavanje težine pomaže u održavanju prosečnog vremena bloka od oko 10 minuta.
* Prođu kroz ceo životni ciklus Bitcoin transakcije, od kreiranja i potpisivanja do potvrde u bloku.

#### Alati i resursi

##### Vizuelna pomagala

* Poglavlje 9 - Kako funkcioniše rudarenje Bitcoina?

##### Pomoćna biblioteka

* Karta pojmova — Poglavlje 9 — Pojmovi: rudarenje, Proof of Work, heš zagonetka, prilagođavanje težine, nagrada za blok, mempool, 51% napad
* Biblioteka zabluda — Poglavlje 9 — Obraditi: "rudari stvaraju Bitcoin ni iz čega", "rudari kontrolišu Bitcoin", "više rudarenja = manje bezbednosti"
* Tabele poređenja i referentni listovi — Ekonomija rudarenja: prihodi, troškovi, usklađenost podsticaja; prilagođavanje težine
* Tehnička objašnjenja i detaljna analiza — Bezbednost Proof of Work; zašto su napadi skupi; prag od 51%

#### Aktivnosti

* Istraživanje mempool-a
* Transakcije u praksi

#### Online nastava

* Koristite jedan jasan dijagram toka transakcije od potpisivanja u novčaniku do potvrde.
* Tokom cele lekcije, vizuelno odvojite čvorove i rudare na ekranu.
* Koristite mempool.space ili snimak ekrana da prikažete nepotvrđene transakcije i pritisak naknada.
* Napravite pauzu posle svake faze procesa rudarenja i postavite jedno kratko pitanje za razumevanje.

#### Priprema

* Pripremite dijagram procesa rudarenja (mempool → izbor transakcija → kreiranje bloka → prilagođavanje težine) za prikaz.
* Obeležite mempool.space ili blockchain.com stranicu za rudarenje; pripremite snimke ekrana sa trenutnim statistikama rudarenja i prilagođavanjima težine.
* Napravite vizuelno objašnjenje Proof of Work kao mehanizma bezbednosti; prikažite prilagođavanje težine u poslednjih 3-6 meseci.

#### Procedura

Ova lekcija detaljnije razmatra kako Bitcoin transakcije prolaze kroz mrežu i postaju deo blokčejna. Sada direktno prati strukturu Diplome tako da se glavni delovi poklapaju sa vodičem za učenike, dok se unutar svakog dela zadržava detaljnije objašnjenje za edukatore.

##### 9.0 Uvod, 8 minuta

Započnite povezivanjem ovog poglavlja sa prethodnim:

* Ako korisnik potpiše transakciju privatnim ključem, šta se dešava sledeće?
* Ko proverava da li je ta transakcija ispravna?
* Kako se dodaje u blokčejn?
* Zašto su Bitcoinu potrebni i čvorovi i rudari?

Počistite da ovo poglavlje objašnjava kako mreža u praksi obrađuje transakcije i kako rudarenje obezbeđuje sistem bez centralnog autoriteta.

##### 9.1 Bitcoin čvorovi i rudari, 47 minuta

**Čvorovi i rudari, različite uloge**

Počnite jasnim razdvajanjem ove dve uloge.

Bitcoin čvorovi:

* čuvaju kopiju blokčejna
* proveravaju da li transakcije poštuju pravila
* dele informacije sa drugim čvorovima
* pomažu novčanicima i drugom softveru da pristupe podacima sa blokčejna
* mogu da odbace nevažeće transakcije ili nevažeće blokove

Poglavlje opisuje čvorove kao čuvare validacije i proširuje to analogijom „digitalnog saobraćajca“. To je korisno jer prikazuje čvorove kao proveravače i koordinatore, a ne kao vladare. Dijagram takođe naglašava da mnogi čvorovi čuvaju kopije glavne knjige širom sveta.

Bitcoin rudari:

* prikupljaju validne transakcije
* sastavljaju kandidatske blokove
* takmiče se da pronađu validan heš bloka
* emituju validne blokove kada pobede
* dobijaju nagrade za blok i naknade za transakcije

Ključna pouka iz poglavlja je da svrha rudarenja nije samo stvaranje novih bitkoina, već decentralizacija bezbednosti Bitcoina. Novi bitkoin je podsticaj, dok je sam proces rudarenja mehanizam bezbednosti.

**Šta čvorovi zapravo rade**

Nadogradite deo o čvorovima listom funkcija čvorova iz poglavlja:

* Čuvari validacije: proveravaju da li transakcije i blokovi poštuju pravila
* Komunikacioni čvor: povezuju se međusobno i dele podatke o transakcijama
* Kontrolor kvaliteta: odbacuju nevalidne informacije
* Informator o blokčejnu: pružaju podatke drugom softveru kao što su novčanici
* Dobrodošlica novim čvorovima: pomažu novim čvorovima da preuzmu blokčejn, dok svaki novi čvor i dalje samostalno proverava podatke

Ovo je dobar trenutak da naglasite da pokretanje čvora korisniku daje veću nezavisnost. Umesto da se u potpunosti oslanjaju na spoljne servise da im kažu stanje mreže, mogu to sami da provere. jasno ističe ovu poentu, uključujući i pominjanje Bitcoin Core-a kao jedne od implementacija koju korisnici mogu pokrenuti.

**Šta rudari zapravo rade**

Sada pažljivije objasnite rudarenje.

Rudari:

* prikupljaju proverene, ali nepotvrđene transakcije
* grupišu ih u kandidatski blok
* više puta hešuju podatke bloka u potrazi za validnim hešom bloka
* emituju pobednički blok mreži
* zarađuju nagrade ako blok bude prihvaćen

Koristite analogiju iz poglavlja o „ogromnoj plastu ključeva“ ako pomaže. Ona daje studentima konkretnu sliku rudarske trke. Glavna ideja nije da rudari rešavaju koristan matematički problem u uobičajenom smislu, već da dokazuju da su potrošili stvarnu energiju i računarsku snagu da bi obezbedili sistem.

Ovo je takođe pravo mesto da objasnite nagrade za rudare:

* nagrada za blok: novoizdati bitkoin
* naknade za transakcije: naknade priložene transakcijama koje korisnici žele da budu potvrđene

Počistite da rudari obično daju prednost transakcijama sa većim naknadama, jer one povećavaju njihovu nagradu. Poglavlje ovde takođe objašnjava prepolovljenja, pa možete ukratko napomenuti da se nagrada za blok smanjuje na svakih 210.000 blokova, otprilike svake četiri godine, prema javnom rasporedu ponude Bitcoina. Strane 5 i 6 sadrže raspored ponude i tabelu narednih prepolovljenja, što može pomoći da se ojača predvidljivo izdavanje Bitcoina.

**Validan heš bloka, dokaz o radu i prilagođavanje težine**

Ovaj deo je srž poglavlja.

Objasnite da rudari traže validan heš bloka, što znači heš bloka koji ispunjava cilj mreže. Poglavlje ovo objašnjava kao pronalaženje broja manjeg od cilja koji postavlja mreža.

Zatim jasno objasnite dokaz o radu:

* rudari moraju da obavljaju ponovljene računarske operacije
* prvi koji pronađe validan heš dokazuje da je obavio taj rad
* to čini prepravljanje ili napad na glavnu knjigu skupim
* čvorovi zatim proveravaju blok pre nego što ga prihvate

Snažna rečenica za nastavu je:

Dokaz o radu obezbeđuje Bitcoin tako što čini nepoštenje skupim, a proveru lakom.

Takođe objasnite prilagođavanje težine:

* mreža prilagođava težinu rudarenja na svakih 2.016 blokova
* to se dešava otprilike svake dve nedelje
* cilj je da prosečno vreme bloka ostane blizu 10 minuta
* ako se priključi više računarske snage, težina raste
* ako je prisutno manje računarske snage, težina opada

Strane 7 i 8 objašnjavaju ovaj proces i pokazuju kako teži ciljevi zahtevaju više rada. Ovo pomaže studentima da shvate da vreme Bitcoina ne kontroliše centralna vlast, već pravila protokola koja automatski reaguju na uslove mreže.

##### 9.2 Šta je mempul?, 15 minuta

Sada pređite na mempul.

Objasnite da je mempul čekaonica za validne, nepotvrđene transakcije. Kada korisnik emituje transakciju, čvorovi je prvo proveravaju. Ako je validna, dodaju je u svoj mempul i dele je sa drugim čvorovima. Zatim rudari mogu da biraju među tim transakcijama koje čekaju kada prave blok. Strane 10 i 11 direktno objašnjavaju ovaj proces.

Važne tačke koje treba naglasiti:

* mempool nije blokčejn
* transakcije tamo su još uvek nepotvrđene
* svaki čvor održava svoj sopstveni mempool
* ne postoji jedan univerzalni mempool
* transakcije sa većom naknadom će verovatno biti brže izabrane

Poglavlje takođe objašnjava uobičajene razloge zbog kojih transakcija može ostati nepotvrđena duže vreme:

* niska naknada
* zagušenje mreže
* pokušaj dvostrukog trošenja
* pogrešni ili nepotpuni podaci
* neispravno formirana transakcija

Ako je korisno, spomenite aktivnost sa mempool.space kao praktičan način za vizuelizaciju nepotvrđenih transakcija i nivoa naknada. Takođe jasno naglasite da je mempool.space samo jedan explorer, a ne sam mempool.

##### 9.3 Kako funkcionišu Bitcoin transakcije, 20 minuta

Sada povežite sve koristeći korak-po-korak sekvencu iz poglavlja.

Jasna verzija za učionicu je:



1. Pošiljalac bira UTXO i kreira transakciju
1. Pošiljalac dodaje adresu primaoca i naknadu
1. Pošiljalac potpisuje transakciju svojim privatnim ključem
1. Transakcija se emituje na mrežu
1. Čvorovi je proveravaju i dodaju u svoje mempoole
1. Rudari je biraju za kandidat blok
1. Rudari se takmiče kroz Proof of Work
1. Jedan rudar pronalazi validan hash bloka i emituje blok
1. Čvorovi proveravaju blok i dodaju ga u blokčejn
1. Transakcija dobija potvrde kako se dodaju novi blokovi
1. Jasno naglasite završnu poentu:
1. kada je transakcija uključena u validan blok, ona je potvrđena
1. potrošeni ulazi više nisu upotrebljivi
1. primalac sada kontroliše nove UTXO-e koje je ta transakcija kreirala

Dijagram sažetka je ovde posebno koristan jer vizuelno povezuje ceo proces od potpisivanja u novčaniku, preko uključivanja od strane rudara, do validacije čvorova i distribucije blokova.

###### Završetak i provera razumevanja

Završite sa nekoliko brzih pitanja:

* Koja je razlika između čvora i rudara?
* Šta je mempool?
* Zašto se neke transakcije potvrđuju brže od drugih?
* Šta dokazuje Proof of Work?
* Zašto Bitcoin podešava težinu rudarenja?
* Koji su glavni koraci između slanja transakcije i dobijanja potvrde?

#### Beleške za edukatore

Držite glavnu nit predavanja jasnom: čvorovi verifikuju, rudari se takmiče, Proof of Work obezbeđuje, a mempool čuva validne transakcije dok ne budu potvrđene.

Ovo poglavlje može delovati tehnički, zato često koristite analogije i dijagrame.

Izbegavajte da rudarenje zvuči kao „stvaranje bitkoina ni iz čega.“ Budite precizni da je nagrada podsticaj, dok sam proces rudarenja obezbeđuje mrežu.

Najvažnije tačke na koje treba staviti akcenat, ako je vremena malo, su:



1. Uloge čvora i rudara
1. Mempool kao čekaonica
1. Proof of Work
1. Podešavanje težine
1. Tok transakcije od potpisivanja do potvrde

##### Kako izgleda dobar odgovor

* Važno je odmah razjasniti da Rudari ≠ Čvorovi, prikazati rudarenje kao ekonomsku aktivnost sa stvarnim hardverskim troškovima i troškovima električne energije, koristiti podešavanje težine i Proof of Work za objašnjenje mehanizma bezbednosti i proveriti razumevanje kroz scenarije o promenama u mreži.
* Edukatori treba da koriste stvarne brojeve kako bi utemeljili diskusije, budu izuzetno jasni i ponavljaju razliku između rudara i čvorova, budu realni u vezi sa zabrinutostima oko centralizacije rudarskih bazena, i poštuju stvarnu složenost koja je uključena.
* Studenti razumeju da je rudarenje posao pametnih ljudi koji rade složen posao jer zarađuju Bitcoin, prepoznaju da podsticaji podstiču pošteno ponašanje jer profit rudara zavisi od uspeha Bitcoina, vide da se sistem samoreguliše automatskim podešavanjem težine, shvataju da je rudarenje pravi biznis, a ne dobrotvorni rad, i cene to što bezbednost Bitcoina košta stvarnu električnu energiju i novac.
* Ishodi učenja biće ispunjeni ako studenti mogu da razlikuju rudare koji prave blokove od čvorova koji ih verifikuju, razumeju Proof of Work kao mehanizam bezbednosti koji napade čini eksponencijalno skupim, prepoznaju da podešavanje težine održava vreme bloka na otprilike 10 minuta, razumeju podsticaje rudara oko nagrada za blok i naknada, objasne zašto 51% napad ne uspeva, i vide rudarenje kao ekonomsku aktivnost sa stvarnim troškovima i koristima.

##### Upravljanje vremenom

Ako je vremena malo, prioritet su:

* Uloge čvora i rudara (ključna razlika)
* Mempool kao čekaonica
* Mehanizam Proof of Work
* Podešavanje težine (samoregulišući sistem)
* Tok transakcije od potpisivanja do potvrde

Ako ste ispred plana, posvetite vreme:

* Ekonomiji rudarenja i specifikama hardvera
* Dinamici rudarskih bazena i zabrinutostima oko centralizacije
* Scenarijima 51% napada i zašto matematički ne uspevaju
* Dugoročnoj bezbednosti kroz usklađivanje podsticaja

##### Ako se studenti muče

* Rudari vs. čvorovi (zbunjenost) → "Čvorovi verifikuju, rudari predlažu; sudije vs. igrači."
* Proof of Work je rasipnički → "Skupa bezbednost sprečava napade; čini ih besmislenim."
* Podešavanje težine → "Više rudara = brži blokovi = raste težina; sistem diše."
