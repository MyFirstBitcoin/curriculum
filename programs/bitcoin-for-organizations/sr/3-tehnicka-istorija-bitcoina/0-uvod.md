# 3.0 Uvod

> **Dark – Apstrakt Bitcoin White Papera**
>
> **Isključivo peer-to-peer verzija elektronskog novca** omogućila bi da se online plaćanja šalju direktno od jedne strane drugoj bez posredovanja finansijske institucije. **Digitalni potpisi predstavljaju deo rešenja**, ali se glavni benefiti gube ako je **pouzdana treća strana** i dalje potrebna da bi se sprečilo dvostruko trošenje. Predlažemo rešenje problema dvostrukog trošenja korišćenjem **peer-to-peer mreže**. **Mreža vremenski obeležava transakcije** tako što ih hešira u kontinuirani lanac **dokaza o radu zasnovanog na hešu,** formirajući zapis koji ne može biti promenjen bez ponovnog izvršavanja **dokaza o radu**. Najduži lanac ne služi samo kao dokaz redosleda događaja kojima se svedočilo, već i kao dokaz da potiče iz najvećeg skupa CPU snage. Sve dok većinu CPU snage kontrolišu čvorovi koji ne sarađuju u napadu na mrežu, oni će generisati najduži lanac i nadmašiti napadače. **Sama mreža zahteva minimalnu strukturu. Poruke se emituju po principu najbolje namere, a čvorovi mogu napustiti i ponovo se priključiti mreži po želji**, prihvatajući najduži lanac dokaza o radu kao dokaz onoga što se desilo dok su bili odsutni.


Bitcoin se nije pojavio iz vakuuma, već je izgrađen na radu mnogih iz prethodnih decenija. Ovaj modul će istražiti osnove interneta na kojima je Bitcoin izgrađen, kao i istraživanja i razvoj koji su priznati u whitepaper-u.

Sedamdesetih godina, grupa pojedinaca je primetila kako američka vlada, posebno, pokušava da ograniči pristup kriptografiji, i odlučila da obezbedi da ova tehnologija bude dostupna svim ljudima radi zaštite njihove privatnosti na internetu. Neki od ovih ranih pionira su se takođe fokusirali na potencijalne prednosti digitalnog sistema 'zdravog novca' koji bi mogao da se koristi za čuvanje i razmenu vrednosti preko novonastajućeg interneta. Fridrih Hajek – vodeći predstavnik austrijske ekonomske škole – zamislio je kako bi idealna valuta zasnovana na slobodnom tržišnom takmičenju izgledala mnogo pre pojave interneta, ali je zaključio da je to tehnički i politički neizvodljivo. Osim digitalne privatnosti, ova grupa, koja je kasnije postala poznata kao Cypherpunks, pokušala je da ostvari Hajekovu viziju digitalnog novca, ali ti pokušaji nisu uspeli sve dok Satoshi nije objavio svoje ideje na mejling listi.

* TCP/IP protokol (1976)
* Protokoli za javne kriptosisteme - Ralph Merkle (1980)
* Digicash - David Chaum (1989)
* Digitalno vremensko obeležavanje (devedesete)
* Hashcash - Adam Back (1997)
* BitTorrent - Bram Cohen (2001)
* Ponovno upotrebljiv POW - Hal Finney (2004)
* Bitcoin Whitepaper - Satoshi Nakamoto (2008)

Ključni uticaj na razvoj Bitcoina bio je nastanak Cypherpunk pokreta devedesetih godina. Oni su razvili nekoliko kriptografskih tehnologija uključujući kriptografiju sa javnim ključem, koja omogućava korisnicima da sigurno i privatno komuniciraju i dele informacije. Mnogi od ovde opisanih razvoja i ljudi koji su u njima učestvovali bili su deo ove grupe.

Potreba za digitalnim novcem je takođe prepoznata i bilo je nekoliko pokušaja da se on stvori, ali su ti pokušaji imali ograničenja koja su ih sprečila da budu uspešni. Genijalnost Satoshija Nakamota bila je u tome što je sve ove mogućnosti spojio, i uz neke svoje inovacije, izgradio na njima Bitcoin protokol koji se danas koristi. U narednim odeljcima ćemo istražiti neke od ovih razvoja i objasniti kako su oni doprineli dizajnu Bitcoina. Takođe ćemo razgovarati o tome koji su to nedostajući delovi slagalice koje je Satoshi uspeo da reši.
