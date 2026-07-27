# 6.1 Otkrivanje digitalne oskudice

> Sa Bitcoin-om je otkrivena nova vrsta robe... vrsta digitalne robe, koju generišu računari i koja je delimično napravljena za računare. Čovečanstvo ima istoriju značajnih izuma. U istorijskim knjigama koje će biti napisane u budućnosti, Bitcoin će biti naveden kao jedan od njih.  
_Prof. dr Filip Sander_



#### 6.1.0 Oskudica u ekonomiji

U okviru ekonomije, dobro je poznato da je oskudica ključni princip koji pokreće vrednost. Dobra i usluge za kojima postoji značajna potražnja postaju vrednija ako je ponuda ograničena do te mere da se potražnja ne može lako zadovoljiti. Štaviše, oskudica podstiče povećanu konkurenciju i pokretač je otkrivanja cena na tržištu. Na tržištu slobodne, poštene i otvorene konkurencije, cene bi trebalo da se ustale na tački gde se ponuda i potražnja susreću.

Resursi za kojima postoji velika potražnja mogu se smatrati vrednijim ako su ograničeni ili teže dostupni. Ovo može podstaći dodatnu potražnju za tim resursom dok učesnici na tržištu međusobno konkurišu kako bi obezbedili pristup. Ova dinamika se može uočiti kod prirodnih resursa kao što su plemeniti metali, nafta ili takozvane 'meke robe' poput prehrambenih proizvoda. Oskudica, dakle, leži u osnovi ekonomskog odlučivanja, raspodele resursa i oportunitetnog troška. U svetu neograničenih resursa, sve bi bilo podjednako dostupno i vrlo male vrednosti. Nasuprot tome, oskudica daje vrednost i podstiče trgovinu, ulaganja i inovacije jer primorava društva da efikasno upravljaju ograničenim resursima.



#### 6.1.1 Izazov digitalne oskudice

Izazov digitalne oskudice leži u lakoći sa kojom se digitalne informacije mogu kopirati i distribuirati. Digitalne informacije su po svojoj prirodi teže za zaštitu nego fizičke, jer za razliku od fizičkih dobara - neka od

kojih prirodno poseduju oskudicu zbog materijalnih ograničenja - digitalne stavke kao što su muzičke datoteke, dokumenti ili slike mogu se beskonačno umnožavati uz praktično nikakav trošak.

Tradicionalno, mogućnost kopiranja digitalnih podataka značila je da ta sredstva ne mogu imati istu ekonomsku vrednost kao fizička, jer im je nedostajala bilo kakva primenljiva oskudica. Za digitalni novac, ovo je posebno problematično i poznato je kao problem 'dvostrukog trošenja', gde se jedna digitalna jedinica (npr. token ili valuta) može kopirati i potrošiti više puta, čime se ona obezvređuje. Ako je moguće dvostruko potrošiti valutu, ona gubi vrednost jer postaje neprepoznatljiva u odnosu na falsifikovana ili prevarantska sredstva.

Tradicionalno, centralizovane finansijske institucije poput banaka ublažavaju ovaj rizik održavanjem knjige koja verifikuje svaku transakciju i umanjuje stanje na računu, osiguravajući da, kada se novac potroši, ne može ponovo biti iskorišćen od strane istog vlasnika računa. Međutim, ovaj pristup zahteva poverenje u centralni autoritet ili 'orakl' koji upravlja i verifikuje transakcije, što stvara zavisnost i jednu tačku kontrole. Imati centralizovani orakl informacija ostavlja digitalnu imovinu ranjivom na manipulaciju i cenzuru.

Za decentralizovan, sistem sa minimalnim poverenjem kao što je Bitcoin, gde ne postoji centralni autoritet koji nadgleda transakcije, sprečavanje dvostrukog trošenja predstavlja ogroman izazov. Bez mehanizma koji obezbeđuje jedinstvenost svake transakcije, Bitcoin bi bio podložan zloupotrebama, što bi ga činilo nepraktičnim kao čuvara vrednosti i pouzdanog sredstva razmene. Bitcoin rešava problem dvostrukog trošenja putem decentralizovane knjige, gde transakcije potvrđuje hiljade učesnika mreže istovremeno. Ovaj mehanizam omogućava Bitcoinu da održava nepromenljiv zapis svake transakcije, osiguravajući da se svaki novčić može potrošiti samo jednom.

Ovo rešenje stvara digitalnu oskudicu bez oslanjanja na centralnu kontrolu. Bitcoin uvodi prvo uspešno rešenje za digitalnu oskudicu, otvarajući put ekosistemu digitalne imovine sa minimalnim poverenjem i oskudicom, na način koji se ranije smatrao nemogućim.



#### 6.1.2 Sprovođenje digitalne oskudice uz Bitcoin

> Predlažemo rešenje za problem dvostrukog trošenja koristeći peer-to-peer distribuirani server za vremensko obeležavanje, kako bismo generisali računarski dokaz hronološkog redosleda transakcija. Sistem je bezbedan sve dok pošteni čvorovi kolektivno kontrolišu više procesorske snage nego bilo koja grupa napadača koja sarađuje.  
_Satoshi Nakamoto_

Satoshi Nakamoto je stvorio Bitcoin kao inženjersko rešenje za probleme povezane sa fiat novcem. Međutim, to rešenje je zahtevalo da Satoshi pronađe način da sprovede apsolutnu digitalnu oskudicu. Da bi to postigao, Satoshi je razvio open-source komunikacioni protokol koji radi na decentralizovanoj mreži računara, odnosno čvorova. Svaki od ovih čvorova čuva lokalno proverljivu kopiju nepromenljive knjige, takozvani blockchain ili timechain. Bitcoin protokol definiše pravila, a decentralizovana mreža nezavisno verifikuje transakcije, pridržavajući se istih pravila bez potrebe za centralnim autoritetom.

Oskudica Bitcoina doprinosi njegovoj ulozi čuvara vrednosti. Slično kao zlato, Bitcoin je vredan ne samo zbog ograničene ponude, već i zbog truda potrebnog da se 'iskopa' ili proizvedu novi novčići. Rudarenje Bitcoina (proces koji održava knjigu i izdaje nove novčiće) je skup, energetski intenzivan proces koji podseća na fizičko vađenje minerala iz zemlje. Ovaj digitalni 'dokaz o radu' nameće ograničenje proizvodnje koje Bitcoin izjednačava sa opipljivim robama, dajući mu osobine trajnosti i proverljivosti koje tradicionalna digitalna dobra nemaju. Ugrađena težina i smanjenje stope izdavanja novih novčića kroz periodične 'prepolovljavanja' stvaraju ekonomsku strukturu u kojoj ponuda Bitcoina postaje sve oskudnija tokom vremena, povećavajući njegovu privlačnost kao dugoročnog čuvara vrednosti.

##### Kako se sprovodi digitalna oskudica?

Rešenje Bitcoina za problem dvostrukog trošenja leži u korišćenju decentralizovane i javno dostupne knjige. Bitcoin knjiga može se posmatrati kao nepromenljiva baza podataka koja beleži svaku transakciju u sekvencijalnom lancu vremenski obeleženih paketa, nazvanih blokovi. Svaki blok je strogo hronološki i sadrži transakcije koje su verifikovali i prihvatili učesnici mreže. Svaki blok je povezan sa prethodnim, stvarajući trajni zapis koji je distribuiran širom hiljada čvorova širom sveta. Skladištenjem i deljenjem ove knjige preko decentralizovane mreže, Bitcoin eliminiše potrebu za centralnim autoritetom za potvrdu transakcija. Kada se dogodi Bitcoin transakcija, čvorovi širom mreže je nezavisno verifikuju, osiguravajući da se svaka može potrošiti samo jednom. Ova zajednička knjiga takođe čini izuzetno teškim za napadače da hakuju mrežu ili izmene prethodne transakcije, jer bi svaka promena zahtevala odobrenje većine učesnika mreže.

Bitcoinov mehanizam Dokaza o radu (Proof-of-Work, PoW) dodatno jača zaštitu od dvostrukog trošenja tako što zahteva od rudara da reše kriptografski problem kako bi dobili dozvolu da verifikuju nove transakcije i kreiraju novi blok. Ovaj proces, poznat kao rudarenje, zahteva računarsku snagu i dodaje nivo težine i troška promeni knjige. Svaki blok dodat u knjigu mora sadržati kriptografsku vezu sa prethodnim blokom, što učvršćuje integritet lanca i sprečava manipulacije.

Uloga čvora je da čuva najnoviju kopiju knjige, koja sadrži kompletnu istoriju transakcija. Čvorovi održavaju rudare 'poštenim' jer proveravaju da nije došlo do dvostrukog trošenja i, što je važno, da su svi novčići stvoreni u skladu sa rasporedom emisije Bitcoina. Bilo koji korisnik Bitcoina može pokrenuti čvor i verifikovati svoje vlasništvo nad novčićima bez potrebe da veruje trećoj strani. Nema potrebe za autoritetima koji rešavaju sporove u Bitcoinu jer je svaka transakcija uključena u blok objektivno validna.

##### Kako bi napadač mogao da preuzme kontrolu nad Bitcoin mrežom?

Ako bi napadač želeo da izmeni prethodnu transakciju kako bi uspeo u napadu dvostrukog trošenja, morao bi da ponovo uradi Dokaz o radu za taj blok i svaki naredni blok, takmičeći se protiv ukupne računarske snage cele mreže. Ovaj bezbednosni mehanizam osigurava da, ako neko pokuša dvostruko trošenje, mora da kontroliše više od 50% rudarske snage mreže da bi uspeo. Ovo je poznato kao 51% napad.

U ranim godinama Bitcoina, kada je bilo moguće da pojedinačni učesnici kreiraju ili rudaraju nove blokove koristeći opštu računarsku opremu, barem je teoretski bilo moguće prikupiti dovoljno računarske snage za uspešan 51% napad. Danas, ukupna računarska snaga Proof-of-Work mreže prelazi 700 ExaHash/s. To znači da rudarski računari u zbiru izračunavaju više od 700 kvintiliona hešova (kriptografskih proračuna) svake sekunde. Dostigli smo tačku u kojoj su ogromni troškovi i koordinacija potrebni za prepisivanje knjige i uspešan 51% napad, što čini dvostruko trošenje neizvodljivim u praksi.

##### Potvrde i reorganizacije

Još jedan sloj zaštite (koji se ponekad zanemaruje) dolazi iz procesa potvrde transakcija u Bitcoinu. Kada se transakcija prvi put pošalje, smatra se nepotvrđenom i prikuplja se u 'mempool'-u dok čeka da bude uključena u blok i potvrđena od strane rudara. Kada se transakcija doda u blok, smatra se 'potvrđenom'. Svaki blok dodat nakon toga računa se kao dodatna potvrda za tu transakciju. Iako se transakcija smatra zvaničnom nakon jedne potvrde, ne smatra se konačnom dok se ne doda još potvrda.

Radi potpune sigurnosti, korisnici Bitcoina često čekaju više potvrda (obično šest), jer svaki dodatni blok u blockchainu dodatno osigurava transakciju, drastično smanjujući verovatnoću uspešnog pokušaja dvostrukog trošenja. Ovaj proces potvrde uspostavlja vremenski okvir tokom kojeg se transakcije finalizuju.

##### Zašto čekati šest potvrda?

Korisnici Bitcoina čekaju dodatne potvrde jer je moguće da najnoviji blok transakcija bude uklonjen iz lanca blokova, ako više nije deo najdužeg lanca. Važno je napomenuti da je rudarenje takmičenje između veoma velikih bazena računarske snage. Stoga je moguće da dva konkurentska rudara pronađu validno kriptografsko rešenje i da se odvojeni blokovi dodaju u lanac gotovo istovremeno. Ako se to dogodi, lanac se suštinski deli. Rudari će nastaviti da pokušavaju da dodaju blokove na svaku granu lanca. Međutim, kada se naredni blok izrudari, najduži lanac1 (definisan kao lanac sa najviše uloženog dokaza o radu) je onaj koji preovladava, a blok na kraćem lancu postaje 'siroče' i nevažeći je. Sve transakcije u siroče bloku vraćaju se u mempool za uključivanje u neki kasniji validan blok. Ovaj proces se naziva reorganizacija ili jednostavno, 'reorg'.

Zlonamerni akter, koji pokušava dvostruko trošenje, mora da preuzme kontrolu nad mrežom dovoljno dugo da izvrši 'reorg' lanca. Kao što smo videli gore, preuzimanje potpune kontrole zahteva ogromnu količinu računarske snage, ali šta ako velika rudarska operacija - koja hipotetički kontroliše nešto više od trećine ukupne računarske snage mreže - pokuša dvostruko trošenje novčića?

Hajde da prođemo kroz jedan primer:

Recimo, na primer, da je ukupna rudarska snaga Bitcoin mreže 550 ExaHash/s. Kompanija Rogue, koja kontroliše 200 ExaHash/s, obavlja veliku kupovinu nekretnina i namerava da plati u Bitcoin-u. Međutim, Rogue takođe planira da pokuša dvostruko trošenje istih novčića. Prodavac kaže Rogue-u da će sačekati šest potvrda pre nego što preda vlasničke listove. Da bi izvela napad dvostrukog trošenja, Rogue mora u tajnosti da izgradi alternativnu granu u lancu, kopajući duži lanac koji sadrži transakciju dvostrukog trošenja. Kada prodavac vidi šest potvrda koje sadrže njegovu transakciju i preda imovinu, Rogue tada mora da postavi sve blokove koje je iskopala u novoj grani, čineći je najdužim lancem. Koliko je ovo moguće?

U svakom trenutku, verovatnoća da Rogue iskopa sledeći blok je 200/550 = 0,36. Čak i ako je Rogue najveći rudarski bazen, verovatnoća da pošteni rudari pronađu sledeći blok je 1 - 0,36 = 0,64. Blokovi bi trebalo da se kopaju mnogo brže na poštenom lancu. Ali recimo da Rogue ima sreće, iskopa blok i zadrži ga u tajnosti. Zatim pokušava da iskopa još jedan na ovoj tajnoj grani. Međutim, pošteni lanac tada iskopa blok i preuzme prednost tako što iskopa još jedan, pre nego što Rogue iskopa svoj drugi blok.

Rogue tada odustaje. Zašto?


| Blokovi za sustizanje | 1% | 10% | 36% (Rogue) | 51% |
| --- | --- | --- | --- | --- |
| 1 | 0,010101 | 0,111111 | 0,562500 | 1,0 |
| 2 | 0,010102 | 0,012346 | 0,316406 | 1,0 |
| 3 | 1,0e-06 | 0,001372 | 0,177919 | 1,0 |
| 4 | 1,0e-08 | 0,000152 | 0,100113 | 1,0 |
| 5 | 1,0e-10 | 0,000017 | 0,056314 | 1,0 |
| 6 | 1,0e-12 | 1,9e-06 | 0,031676 | 1,0 |


**Izvor**: Na osnovu tabele iz knjige Grokking Bitcoin autora Kalle Rosenbaum

Rogue shvata da nema dovoljno hash snage da izvede dvostruko trošenje, uprkos tome što kontroliše 36% hash snage Bitcoin mreže. Da bi bio uspešan, mora da iskopa još četiri bloka kako bi pretekao pošteni lanac. Uprkos ogromnoj računarskoj snazi i kontroli nad 36% mreže, Rogue-ove šanse za uspeh su samo 0,100113.


> **Dark – Uključuje se teorija igara**
>
> Rogue-ove šanse za uspeh su užasne, ali postaje još gore. Za svaki minut pokušavanja, Rogue troši ogromnu količinu električne energije. Sve to biće uzalud. Štaviše, za svaki blok koji ne iskopa pošteno, Rogue gubi nagradu za blok, koja je trenutno 3,125 novčića po bloku, što trenutno vredi više od 300.000 €.
>
> Glavni razlog Rogue-ovog neuspeha bio je što je prodavac nekretnine zahtevao šest potvrda. Što je potrebno više potvrda, to je teže nepoštenim rudarima da izgrade alternativne lance blokova. Zaista, za veoma veliku transakciju, prodavac može zahtevati više potvrda. Na primer, deset potvrda (što bi trebalo da traje oko 100 minuta) bi smanjilo Rogue-ove šanse za uspeh na samo 0,003.
>
> Na ovaj način, teorija igara oko rudarenja obezbeđuje da su svi podstaknuti da postupaju pošteno i ne troše računarske resurse uzalud ili da ne gube nagrade za blok. Štaviše, u interesu je svih rudara da Bitcoin mreža bude sigurna i pouzdana. Ovo obezbeđuje da je njihova ogromna investicija u računarsku snagu zaštićena. Ako mreža bude uspešno napadnuta, tržišna vrednost novčića će drastično pasti jer će poverenje u mrežu biti narušeno.




#### 6.1.3 Da li je centralizacija rudarenja pretnja?

Kao što se vidi u gornjoj tabeli, centralizacija rudarenja može predstavljati potencijalnu pretnju zaštiti od dvostrukog trošenja u Bitcoin-u, jer povećava verovatnoću 51% napada – scenarija u kojem jedan rudar ili grupa rudara kontroliše više od polovine računarske snage mreže. Ako bi se to dogodilo, entitet koji kontroliše mogao bi teoretski da izmeni nedavne transakcije ili pokuša dvostruko trošenje prepravljanjem knjige, što bi mu omogućilo da iste novčiće potroši više puta.

Takva situacija podriva integritet Bitcoin mreže jer daje nesrazmeran uticaj na validaciju transakcija nekolicini aktera. Međutim, iako je teoretski moguće, sprovođenje 51% napada bi i dalje bilo izuzetno složeno i skupo, zahtevajući ogromne računarske resurse, električnu energiju i koordinaciju, što bi verovatno prevazišlo potencijalne koristi pokušaja dvostrukog trošenja.

Postoje zaštitne mere koje pomažu u ograničavanju rizika od centralizacije rudarenja. Rudarski bazeni, na primer, omogućavaju manjim rudarima da udruže resurse i dele nagrade za blok, smanjujući dominaciju bilo kog pojedinačnog entiteta. Iako je ovo koristan način za male rudare da učestvuju u mreži, postoji rizik da entitet koji kontroliše bazen može zloupotrebiti i pokušati da napadne mrežu. Međutim, transparentnost Bitcoin knjige takođe znači da je svaka koncentracija rudarske snage vidljiva, upozoravajući zajednicu na potencijalne rizike i omogućavajući protivmere. Rudari su veoma svesni da svaki napad na Bitcoin mrežu ozbiljno ugrožava njenu vrednost, pa je vrlo jednostavno za male rudare da pređu u novi bazen kako bi izbegli da njihova rudarska snaga bude zloupotrebljena. Iako rizik nije nula, otvorena i distribuirana priroda Bitcoin ekosistema, u kombinaciji sa visokim troškovima napada, čini centralizaciju rudarenja više teorijskom pretnjom nego neposrednom, jer bi održavanje takve kontrole tokom dužeg perioda bilo finansijski neodrživo za bilo kog napadača.



#### 6.1.4 Širi uticaj digitalne oskudice

Bitcoin je promenio način na koji razmišljamo o oskudici u digitalnom svetu. Zato što digitalna dobra – kao što su softver, muzički fajlovi, e-knjige i onlajn sadržaj – poseduju karakteristike koje ih razlikuju od fizičkih dobara, mogu se reprodukovati uz zanemarljive troškove i deliti trenutno. Za razliku od fizičkih predmeta, koji su ograničeni materijalnim uslovima kao što su troškovi proizvodnje i ograničenja skladištenja, digitalna dobra postoje kao podaci koji se mogu beskonačno kopirati bez gubitka kvaliteta. To znači da su fizička dobra po svojoj prirodi oskudna zbog ovih materijalnih ograničenja, dok su digitalna dobra tradicionalno bila obilna, bez ugrađenih mehanizama za ograničavanje ponude.

Važno je napomenuti da su digitalna dobra nerivalna. To znači da konzumacija digitalnog dobra od strane jedne osobe ne umanjuje dostupnost tog dobra za druge. Na primer, kada se pesma preuzme, može se kopirati i distribuirati neograničen broj puta bez gubitka korisnosti. Istorijski gledano, ovo obilje predstavlja izazov za stvaranje vrednosti, jer se tradicionalni ekonomski model ponude i potražnje iskrivljuje kada je ponuda, barem teoretski, neograničena. Kao odgovor na to, upravljanje digitalnim pravima (DRM) i druge mere veštačke oskudice pokušale su da ograniče pristup. Međutim, ti mehanizmi mogu biti zaobiđeni i poverenje prebacuju na centralizovane autoritete. Inovacija Bitcoina leži u tome što ovaj problem rešava izvorno, čineći ga prvim digitalnim sredstvom koje ugrađuje oskudicu kroz decentralizovanu tehnologiju, bez oslanjanja na ova tradicionalna ograničenja.

Bitcoin igra transformativnu ulogu u uspostavljanju digitalne oskudice uvođenjem protokola koji nameće ograničenu ponudu. Limit od 21 milion novčića je ugrađen u protokol i ovo ograničenje ne može biti promenjeno bez konsenzusa mreže, tj. svih hiljada učesnika širom sveta koji pokreću Bitcoin čvorove. Na ovaj način, Bitcoin je stvorio sredstvo koje oponaša konačnu prirodu fizičkih dobara, kao što je zlato, dok u potpunosti postoji u digitalnom svetu. Ograničenje ponude je fundamentalno za vrednost Bitcoina i održava se kombinacijom kriptografije, mehanizama konsenzusa i transparentnog, otvorenog koda. Ovo obezbeđuje da svi učesnici na mreži poštuju ista pravila, kao i da ih pokreće ključni ekonomski podsticaj da osiguraju da je ponuda novčića apsolutno i dokazivo konačna.

Rešavanjem problema dvostrukog trošenja, Bitcoin sprečava inflaciju ili dupliranje sredstva, što je bio izazov koji je mučio prethodne eksperimente sa digitalnim novcem. U okviru Bitcoina, nijedan pojedinačni autoritet ne kontroliše ponudu, što ga čini imunim na centralizovanu manipulaciju kakva se viđa u sistemu fiat novca, kao što je proizvoljno štampanje novca ili devalvacija. Ova inovacija omogućava Bitcoinu da služi kao čuvar vrednosti i zaštita od inflacije, omogućavajući mu da zauzme jedinstvenu poziciju sličnu 'digitalnom zlatu' – oskudnom digitalnom resursu sa proverljivom vrednošću.



#### 6.1.5 Zaključak

Zaključno, sve je šire shvaćeno da je inovacija Bitcoina u digitalnoj oskudici redefinisala pojam novca. Ipak, ponekad se zanemaruje da je Bitcoin takođe transformisao digitalni pejzaž rešavanjem dugotrajnog problema stvaranja oskudice u suštinski obilnom digitalnom svetu. Bitcoin je efektivno uveo novu kategoriju digitalne imovine koja odražava osobine fizičkih dobara.

Ovo otkriće pokazuje da decentralizovani sistem može uspostaviti oskudicu, nepromenljivost i vrednost nezavisno od bilo kog centralnog autoriteta. Štaviše, može imati primenu i van novca, jer je inspirisao čitavo polje istraživanja i razvoja oko ove tehnologije.

Gledajući unapred, model digitalne oskudice Bitcoina oblikuje budućnost novca i čuvanja vrednosti. Kako zabrinutost zbog inflacije i pitanja oko upravljanja fiat valutom postaju sve prepoznatljivija, fiksirana ponuda Bitcoina ga čini sve privlačnijim kao zaštitu od tradicionalne finansijske nestabilnosti.

Na kraju, otkriće digitalne oskudice kroz Bitcoin može označiti početak promene paradigme, gde digitalna sredstva sa prepoznatom oskudicom i proverljivim poverenjem stiču priznanje kao vredne komponente moderne ekonomije, postavljajući temelje za budućnost decentralizovanih finansija i digitalnog vlasništva. Ovo ima značajne implikacije za oblast ekonomije – Bitcoin je dao model kako oskudica i vrednost mogu postojati u digitalnom obliku.

> Pored digitalne oskudice, Bitcoin je takođe prvi primer apsolutne oskudice, jedina likvidna roba (digitalna ili fizička) sa unapred određenom fiksnom količinom koja se ne može zamislivo povećati. Do izuma Bitcoina, oskudica je uvek bila relativna, nikada apsolutna.  
_Saša_



###### Beleške

1. Najduži lanac Bitcoin čvorovi prihvataju kao najvalidniju verziju glavne knjige i definiše se kao lanac za čiju izgradnju je bilo potrebno najviše truda (ili najveći dokaz o radu). Više informacija ovde: [https://learnmeabitcoin.com/technical/blockchain/longest-chain/](https://learnmeabitcoin.com/technical/blockchain/longest-chain/)
