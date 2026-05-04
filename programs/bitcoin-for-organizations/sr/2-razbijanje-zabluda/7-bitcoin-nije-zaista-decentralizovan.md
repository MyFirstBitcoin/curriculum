# 2.7 Bitcoin nije zaista decentralizovan.

> Složenost kripta proističe iz pokušaja decentralizacije—distribucijom moći i upravljanja u sistemu, teoretski nema potrebe za pouzdanim posrednicima poput finansijskih institucija. To je bila osnova početnog Bitcoin white paper-a, koji je ponudio kriptografsko rešenje namenjeno omogućavanju slanja plaćanja bez uključivanja bilo koje finansijske institucije ili drugog pouzdanog posrednika. Međutim, Bitcoin je vrlo brzo postao centralizovan i sada zavisi od male grupe softverskih developera i rudarskih pool-ova da bi funkcionisao  
_Međunarodni monetarni fond_

Kao što pokazuje gornji citat iz relativno nedavne objave Međunarodnog monetarnog fonda, tradicionalna finansijska industrija i dalje tvrdi da Bitcoin nije decentralizovan, kao i da meša Bitcoin sa drugim kripto imovinama.

##### Uvod

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/b18828cef18f12a52919346f3300cbbaa2217def-161x167.svg)

Decentralizacija je ključni aspekt Bitcoina. Sposobnost održavanja pravila protokola kao što su ograničenost i distribucija bez centralnog autoriteta obezbeđuje da može funkcionisati kao novac bez dozvole za globalno društvo.

Kao što je Satoshi naveo u svojoj online prepisci, decentralizovane usluge poput BitTorrent-a su 'odolevale' vladinim pritiscima, za razliku od servisa sa identifikovanim vlasnikom i centralizovanim serverima. Očigledno je bio zabrinut zbog potencijalnog rizika da vlade ili drugi interesi ugase ili na drugi način negativno utiču na Bitcoin.

U ovom kontekstu, zanima nas decentralizacija:

* Razvoja i upravljanja kodom koji pokreće protokol; ko ima pravo da menja pravila?
* Rudarske funkcije koja kreira nove blokove u skladu sa pravilima i proverava dvostruko trošenje
* Čvorova (noda) koji proveravaju validnost transakcija i čuvaju kopiju blockchain-a

##### Programeri

Bitcoin je open-source protokol koji svako može da pogleda, preuzme, kopira ili predloži izmene. Dostupan je u GitHub biblioteci, a izvorni kod je prvobitno lansirao Satoshi Nakamoto 2009. godine. Svako može da preuzme kod i pokrene čvor, pri čemu većina koristi originalni Bitcoin Core softver, koji je vremenom ažuriran.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Izvor: https://river.com/learn/what-is-bitcoin-core/_

Razvoj Bitcoin Core-a prati najbolje prakse open source razvoja. U svakom trenutku može biti bilo koji broj programera koji pišu ili pregledaju izmene koda. Oni moraju da slušaju zabrinutosti operatora čvorova i rudara, kao i korisničke baze pre nego što naprave bilo kakvu kritičnu izmenu koda, koja će biti pregledana i dogovorena kao što je prikazano u gornjem dijagramu toka pre nego što bude uključena u kod.

Pravila Bitcoina su zatim enkodirana u ovom Bitcoin Core softveru, koji radi na svakom čvoru. Svako može predložiti izmenu pravila – pravila su kod, ali nisu_samo_kod, ona su_dogovoreni_kod. Ako se jednostrano promene, novi kod više nije deo konsenzusa i više nije deo Bitcoina. Promeniti nešto u Bitcoinu i ostati u konsenzusu je nezgodno. Predložene izmene koda spadaju u jednu od tri kategorije:

* Unutar postojećih pravila: Manja unapređenja kao što su pravopisne greške, lepši korisnički interfejs ili upravljanje podacima mogu spadati u ovu kategoriju i relativno ih je lako odobriti.
* Dodavanje novog pravila koje uvodi ograničenja u postojeća pravila – na primer, smanjenje veličine bloka. Ovo se naziva 'soft fork'. Čvorovi koji odluče da ne implementiraju izmenu koda i ostanu na staroj verziji i dalje mogu učestvovati u mreži.
* Dodavanje novog pravila koje krši trenutna pravila, npr. povećanje veličine bloka. Čvorovi koji ne nadograde na novi kod odbaciće blok kreiran u većoj veličini kao nevažeći. Ovo se naziva 'hard fork' i stvara razdvajanje lanca između čvorova koji pokreću originalni i novi kod i stvara novu kriptovalutu. Ovo se ranije dešavalo, ali nije dovelo do dugoročnog uspeha nove kriptovalute jer je većina čvorova odlučila da ostane na originalnom kodu.

Dakle, jedna strana ili grupa ljudi ne može jednostrano promeniti Bitcoin kod bez postizanja konsenzusa, u suprotnom rizikuje razdvajanje lanca i nastanak nove kriptovalute sa drugačijim pravilima.

##### Rudarenje

Rudarska funkcija proverava transakcije kao i svaki drugi čvor na mreži, ali zatim troši energiju potrebnu za kreiranje novog bloka koji ispunjava konsenzusna pravila u kodu. Uspeh omogućava rudaru da dobije nagrade u vidu transakcijskih taksi i Bitcoin nagrada (u trenutku pisanja 3,125 coina po bloku).

Rudarenje se obično obavlja putem rudarskih 'pool-ova' gde ljudi udružuju rudarsku snagu ili hash rate kako bi povećali šanse za uspešno rudarenje bloka i podelu nagrada. Postoji opasnost da jedan ili više ovih rudarskih pool-ova mogu da se udruže i postignu 51% dominacije u rudarenju i praktično preglasaju protokol validacije mreže u svoju korist kako bi dvostruko potrošili coine. Ovo bi zahtevalo ogromne resurse i velike troškove, a pojedinačni rudari mogu vrlo lako da pređu u drugi pool u bilo kom trenutku. Takav napad bi verovatno doveo i do kolapsa vrednosti bitcoina, jer bi bilo očigledno da je integritet mreže narušen. Napadač bi zato morao brzo da konvertuje bilo koji dobijeni bitcoin u fiat pre nego što vrednost opadne. To bi dodatno otežalo održavanje napada na duži period, pa je zato isplativije za rudara ili operatora pool-a da poštuje pravila i pokušava da rudari važeće blokove.

Geografska distribucija rudarske funkcije je takođe važna kako bi se izbeglo da, na primer, vlade preuzmu rudarski kapacitet ili ga ugase. Na primer, nedavna zabrana rudarenja u Kini pokazala je sposobnost Bitcoina da se prilagodi i preživi takvu vladinu intervenciju, brzo se oporavljajući od gubitka hash snage.

##### Čvorovi

Za razliku od rudarenja, koje zahteva značajnu finansijsku investiciju da bi se efikasno takmičilo u trci za rudarenje novih blokova, ili razvoja koda koji zahteva programersku stručnost, pokretanje čvora je nešto što svako ko želi da pomogne u održavanju decentralizacije Bitcoina može da uradi.

Čvorovi pokreću Bitcoin Core softver i sprovode pravila koja kod sadrži kako bi osigurali da rudari ne varaju, na primer tako što bi sebi dodelili veću nagradu po bloku nego što je dozvoljeno. Oni takođe sprovode ograničenje ponude na 21 milion, što je ključno za očuvanje oskudice Bitcoina. Da bi neka vlada ili zlonamerna strana zaustavila Bitcoin, morala bi da uništi svaku pojedinačnu kopiju blockchain-a, koji trenutno radi na hiljadama čvorova širom sveta, što je gotovo nemoguć zadatak.

##### Ljudi

Još jedan aspekt potencijalne centralizacije su ljudi. Svaki drugi 'alt-coin' ima vođu—nekoga ko bi potencijalno mogao biti primoran da zagovara promene koje nisu u najboljem interesu Bitcoina. Satoshi Nakamoto je ostao dovoljno dugo da osigura da je Bitcoin na putu uspeha pre nego što je zauvek nestao, ostavljajući ga u rukama drugih da unapređuju i prilagođavaju softver.

Šta je sa vlasnicima velikih količina Bitcoina? Rani investitori, koji su zadržali svoje coine i nisu ih izgubili, sada su izuzetno bogati. Važno je napomenuti da to možda jeste slučaj, ali im to ne daje nikakav veći uticaj na sistem od bilo koga drugog, za razliku od 'proof of stake' coina gde rani usvajači koji su već bogati u toj kriptovaluti stiču prednosti u donošenju odluka i distribuciji budućih coina. Ovo je ili će neminovno dovesti do centralizacije tokom vremena.

##### Zaključak

Koje su potencijalne pretnje koje decentralizacija može pokušati da ublaži?

* Vlada koja gasi ili zabranjuje Bitcoin
* Neželjene izmene koda koje favorizuju jedan set interesa u Bitcoinu, npr. povećanje nagrade po bloku
* Prinudno menjanje protokola od strane vlade ili zlonamernih aktera radi uticaja na smer protokola
* Mogućnost da grupa rudara preuzme mrežu i 'dvostruko potroši' Bitcoin – 51% napad

Kao što možemo videti, kombinacija čvorova, programera koda i rudara, kao i upotreba mehanizma 'proof of work', decentralizuje Bitcoin na dovoljan nivo da se ove potencijalne pretnje ne smatraju ozbiljnim rizikom. Zajednica će morati da nastavi da prati situaciju kako bi osigurala da tako i ostane.
