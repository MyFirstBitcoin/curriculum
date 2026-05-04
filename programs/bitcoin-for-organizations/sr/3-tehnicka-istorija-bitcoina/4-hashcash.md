# 3.4 Hashcash

Hashcash je kreirao Adam Back, još jedan od ranih inovatora u ovoj oblasti. Adam je imao snažno interesovanje za slobodna tržišta i privatnost na internetu, i naišao je na Cypherpunks mejling listu kojoj se pridružio i postao aktivan učesnik.

Bio je veoma zainteresovan za digitalni novac i dao je neke predloge kako bi grupa možda mogla bliže da sarađuje na DigiCash-u sa Chaumom, ali to nije dovelo ni do čega. Zatim je svoju pažnju usmerio na drugi problem koji se pojavljivao – neželjenu poštu (spam) u elektronskoj pošti. On i ostali iz Cypherpunks grupe želeli su da pronađu rešenje za problem spama, gde je spamerima bilo trivijalno da kreiraju i pošalju hiljade mejlova koji zagušuju mreže. Njegovo inovativno rešenje zasnivalo se na heširanju – mogućnosti kriptografije da bilo koji podatak pretvori u jedinstveni i nasumični niz određene dužine, kako bi se stvorio ekvivalent digitalne 'markice' koja je morala biti dodata mejlu da bi bio validan i prosleđen kroz mrežu. Beznačajan trošak za pravi mejl, ali nepremostiv za spamere.

Ključna inovacija koju je Hashcash doneo bila je povezivanje resursa iz stvarnog sveta – računarske snage – sa digitalnom mrežom. Dok su se digitalni resursi do tada mogli neograničeno kopirati, broj 'hashcash' tokena bio je ograničen time koliko su ljudi bili spremni da ulože energije u njihovo stvaranje.

Iako je rešenje ispunjavalo neke od kriterijuma za koje je Adam smatrao da su potrebni za digitalni novčani sistem; bilo je anonimno, otporno i nije zahtevalo poverenje, svaki hashcash nije mogao ponovo da se koristi i nije bio zaista redak. Predložio je druge načine na koje bi se ti problemi mogli rešiti korišćenjem eksternih trećih strana.

##### BitGold

Nick Szabo je nadogradio koncept Hashcash-a i dokaz rada (proof of work) kako bi predložio alternativno rešenje, koje je opisao na mejling listi godinu dana nakon što je Hashcash objavljen, 1998.

Iako je bio bliži rešenju, ovaj predlog je i dalje imao nekoliko izazova.

* Ko bi vodio registar vlasništva nad hash-ovima i kako im se može verovati?
* Heširanje bi generalno postajalo jeftinije tokom vremena, što je bio izazov i za HashCash.

Pošto bi povezani hash-ovi bili vremenski obeleženi, predložio je neku vrstu istorijskog praćenja težine heširanja u to vreme; raniji hash bi zahtevao više procesorske snage nego kasniji, jer su troškovi opadali. Nažalost, to je značilo da hash-ovi ne bi bili 'zamjenjivi', tj. iste vrednosti, što se smatra ključnom osobinom digitalnog novca. Da bi to rešio, Nick je predložio neku vrstu 'slobodnog bankarstva' na vrhu BitGold-a, koje bi moglo da agregira različite grupe hash-ova koji bi imali istu vrednost.

##### B-Money

Ubrzo nakon Bit Gold predloga, Wei Dai je predložio slično rešenje. Već je razvio nekoliko drugih alata za Cypherpunks i imao je svoje ideje o digitalnom novcu.

Njegov predlog je ličio na Bit Gold po tome što je koristio digitalne potpise za prenos novca, a zapisi o transakcijama bi se čuvali u knjizi (ledgeru), koja sadrži javne ključeve i iznos novčanih jedinica dodeljenih svakom. Kao i kod Bit-Gold-a, pouzdane treće strane su smatrane sigurnosnim rupama, i verovalo se da elektronski novčani sistem ne bi trebalo da zavisi od jedne entiteta za praćenje stanja, transakcija ili sprečavanje dvostrukog trošenja.

Wei Dai je predložio nekoliko rešenja za ove probleme, od kojih je jedno bilo da umesto centralnog entiteta (ili više njih) koji održava knjigu, SVI čvorovi održavaju kopiju. Ako svi korisnici proveravaju svoju knjigu i validnost svake transakcije, dokle god su svi čvorovi ažurirani, knjige bi trebalo da ostanu sinhronizovane kroz mrežu. Ovakav visoko distribuirani sistem bi bilo teško kompromitovati.

Wei Dai je prepoznao da ovo ne rešava problem vizantijskih generala (1), jer čvorovi lako mogu izgubiti sinhronizaciju ili jednostavno lagati. Predložio je alternativne metode kao što su podskup 'pouzdanih' servera koji održavaju knjigu, i stvaranje finansijskih podsticaja da ti serveri ostanu pošteni.

Za monetarnu politiku, predložio je da se kupovna moć B-Money-a veže za neku vrstu eksternog indeksa potrošačkih cena. Želeo je da ista količina B-Money-a može da kupi isti deo indeksa tokom vremena, obezbeđujući određenu stabilnost cena. Tako je svako mogao da generiše nove novčane jedinice pružanjem validnog hash-a, ali težina generisanja hash-a bi se mogla menjati tokom vremena u zavisnosti od troškova procesora i cenovnog indeksa, tako da bi svaka jedinica bila 'nepromenljiva'.
