# 9.1 Bitcoin čvorovi i rudari

Bitcoin čvorovi možda zvuče tehnički, ali oni su jednostavno softver koji čuva kopiju Bitcoin blokčejna na računaru. Blokčejn je zajednički zapis svih Bitcoin transakcija.

Kada pokrećete svoj čvor, sami proveravate Bitcoin transakcije umesto da verujete nekome drugom. Ovo vam daje više nezavisnosti i pomaže da Bitcoin mreža ostane decentralizovana.

Možete zamisliti Bitcoin čvor kao digitalnog saobraćajca sa nekoliko važnih zadataka.

1. On čuva kopiju blokčejna, što je istorija svih Bitcoin transakcija.
1. Čvorovi se povezuju sa drugim čvorovima širom sveta i razmenjuju informacije. Jedan primer je lista novih transakcija koje čekaju potvrdu, a koja se zove mempool.
1. Čvorovi proveravaju da li svaka transakcija poštuje Bitcoin pravila. Ako je transakcija nevažeća, čvor je odbacuje.

Čvorovi takođe pomažu novim čvorovima da se priključe mreži tako što im dele blokčejn. Ipak, svaki novi čvor samostalno proverava sva pravila.

Svako može pokrenuti čvor instaliranjem softvera kao što je Bitcoin Core i preuzimanjem blokčejna. Kada je sve podešeno, čvor nastavlja da prima nove blokove otprilike svakih 10 minuta i proverava ih pre nego što ih doda u svoju kopiju blokčejna.

Pokretanjem čvora pomažete da Bitcoin mreža bude sigurnija i decentralizovanija, jer više ljudi nezavisno proverava sistem.

#### Šta je Bitcoin čvor?

> Svrha rudarenja nije stvaranje novih bitkoina; to je sistem podsticaja. Rudarenje je mehanizam kojim se bezbednost Bitcoina decentralizuje.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Rudari sakupljaju nepotvrđene transakcije, formiraju blok i koriste energiju da pronađu ključ koji dodaje i obezbeđuje blok.


Rudari se takmiče da dodaju sledeći blok transakcija u blokčejn. Da bi to uradili, moraju pronaći poseban broj koji stvara važeći heš bloka. Možete to zamisliti kao potragu za pravim ključem među milijardama mogućnosti. Prvi rudar koji pronađe ispravan heš pobeđuje u trci i dobija pravo da doda svoj blok u blokčejn.

Kada rudar pronađe važeći heš, deli svoj blok sa mrežom. Ostali rudari brzo proveravaju da li je rešenje ispravno. Ako jeste, blok se dodaje u blokčejn, pomažući da Bitcoinova javna knjiga ostane sigurna.

Rudari zarađuju bitcoin na dva načina:

* **Nagrada za blok:** Novi bitkoini se stvaraju i dodeljuju rudaru koji uspešno doda blok u blokčejn.
* **Naknade za transakcije:** Kada ljudi šalju bitcoin, uključuju malu naknadu. Rudar koji doda blok dobija naknade od transakcija uključenih u taj blok.

#### Bitcoin prepolovljenja


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Nagrade za rudare za završavanje jednog bloka prepolove se na svakih 210.000 blokova, otprilike svake četiri godine.


Bitcoin ima fiksno maksimalno snabdevanje od 21.000.000 bitkoina, ali svi oni nisu stvoreni kada je Bitcoin počeo. Umesto toga, novi bitkoini se postepeno uvode u opticaj kroz **rudarenje**.

Kada rudari uspešno dodaju novi blok transakcija u Bitcoin mrežu, dobijaju **nagradu za blok** u bitkoinima. U ranim danima Bitcoina, ova nagrada je bila 50 bitkoina po bloku. Ova nagrada je podsticala ljude da koriste računarsku snagu i električnu energiju kako bi pomogli u obezbeđivanju mreže.

Otprilike na svakih 210.000 blokova (približno svake 4 godine), nagrada za blok se prepolovi. Ovaj događaj se zove **prepolovljenje**. Prepolovljenje usporava stvaranje novih bitkoina i pomaže da se obezbedi da ukupna količina nikada ne pređe 21 milion. Vremenom, ovo čini bitcoin sve ređim.


> **Definition – Količina u opticaju**
>
> **Količina u opticaju** odnosi se na ukupnu dostupnu količinu valute. Kod Bitcoina, ukupna količina u opticaju je broj novčića koji su izrudarenii nalaze se u opticaju u bilo kom trenutku.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/e8e931863cb07995c410ff8fbe437451129efaf6-292x200.svg)


> **Definition – Raspored snabdevanja Bitcoinom**
>
> **Raspored snabdevanja Bitcoinom** je unapred određen i javan plan za puštanje novih bitkoina u opticaj, osmišljen da održi retkost Bitcoina tokom vremena.


Nakon svakog prepolovljenja, nagrada u bitkoinima koju rudari dobijaju za dodavanje bloka se prepolovi. Ovo smanjuje stopu po kojoj se stvaraju novi bitkoini.

Rudari i dalje zarađuju naknade za transakcije iz transakcija koje su uključene u blok koji izrudare. Vremenom se očekuje da će ove naknade postati veći deo prihoda rudara.

Prepolovljenja su ugrađena u Bitcoin protokol i dešavaju se automatski otprilike svake četiri godine. Zbog toga je raspored izdavanja Bitcoina predvidljiv i transparentan.

Tabela prikazuje predstojeća prepolovljenja, uključujući približan datum, broj bloka kada se dešavaju, novu nagradu za blok i procenat ukupne količine bitcoina koji je do tada iskopan.


| Događaj | Datum | Blok | Nagrada | Iskopano |
| --- | --- | --- | --- | --- |
| Peto prepolovljenje | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| Šesto prepolovljenje | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| Sedmo prepolovljenje | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Kako se kopa sve više bitcoina, količina u opticaju nastavlja da raste dok se ne dostigne maksimalna količina od 21.000.000 bitcoina, što se očekuje oko 2140. godine. Pošto se tokom vremena stvara sve manje novih bitcoina, ako potražnja poraste, cena Bitcoina može rasti. Ovo takođe podstiče rudare da nastave da obezbeđuju mrežu svojim računarima.

#### Šta je važeći hash bloka u Bitcoinu?

U Bitcoinu, rudari se takmiče da pronađu poseban kod koji se zove **hash bloka**. Ovaj kod identifikuje blok transakcija i omogućava mu da bude dodat u blokčejn.

Svaki blok sadrži informacije o nedavnim transakcijama i takođe uključuje hash prethodnog bloka. Ovo povezuje svaki blok, formirajući lanac od prvog bloka (Genesis Block) do najnovijeg.

Hash funkcioniše kao **digitalni otisak prsta** za podatke u bloku. Ako bi se bilo koja informacija u bloku promenila, otisak prsta bi se takođe promenio. Ovo omogućava svakome da lako proveri da istorija transakcija na blokčejnu nije izmenjena i pomaže u očuvanju sigurnosti mreže.


> **Callout**
>
> Satoshi Nakamoto, tvorac Bitcoina, iskopao je Genesis Block, čime je otključano ukupno 50 bitcoina.


#### Trka za kopanje bloka

Rudari se takmiče da pronađu važeći hash bloka. Prvi rudar koji ga pronađe dobija priliku da doda novi blok u blokčejn i dobije nagradu u bitcoinu.

Da bi bio važeći, hash bloka mora biti manji od broja koji je mreža postavila i koji se zove cilj težine. Pošto su hash vrednosti nasumične, rudari moraju stalno da pokušavaju različite ulaze dok ne pronađu onaj koji odgovara.

Ako se previše rudara takmiči, blokovi bi se pronalazili prebrzo. Ako učestvuje premalo rudara, pronalaženje blokova bi trajalo predugo. Da bi sistem radio glatko, Bitcoin automatski podešava težinu svakih 2.016 blokova (otprilike svake dve nedelje).

Ovo podešavanje obezbeđuje da se u proseku novi blok dodaje u blokčejn otprilike svakih 10 minuta.


> **Definition – Definicija nivoa težine**
>
> **nivo težine** u Bitcoin rudarenju meri koliko je teško pronaći važeći hash bloka. Mreža podešava ovu težinu svakih 2.016 blokova (otprilike svake dve nedelje) tako da se novi blokovi dodaju u blokčejn otprilike svakih 10 minuta. Što je veća težina, to je rudari teže da pronađu važeći blok.


Pronalaskom važećeg hash-a bloka, rudar dokazuje da je obavio potreban rad da bi dodao novi blok u blokčejn. Ovaj proces se zove **Dokaz o radu** (PoW). To je sigurnosni mehanizam koji omogućava Bitcoinu da potvrdi transakcije i doda nove blokove u blokčejn. Rudar koji prvi pronađe važeći hash dobija nagradu u bitcoinu, koja uključuje nagradu za blok i naknade za transakcije iz tog bloka.

Dokaz o radu (PoW) pomaže da Bitcoin ostane siguran tako što čini izuzetno skupim za bilo koga da pokuša da prevari ili preuzme kontrolu nad mrežom. Umesto toga, mnogo je isplativije poštovati pravila.

Rudari imaju četiri glavne uloge:

1. **Prikupljaju transakcije**: Rudari biraju transakcije koje su poslate mreži i stavljaju ih u kandidat blok.
1. **Izvršavaju dokaz o radu**: Rudari se takmiče da reše težak matematički zadatak pronalaženjem važećeg hash-a bloka.
1. **Emituj blok**: Prvi rudar koji pronađe ispravno rešenje deli novi blok sa mrežom.
1. **Zaradi nagrade**: Ako je blok ispravan, dodaje se u blokčejn i rudar dobija novoizdati bitcoin plus naknade za transakcije.

Mnogi rudari širom sveta pokušavaju da naprave sledeći blok u isto vreme. Kada jedan rudar pronađe ispravno rešenje, mreža proverava blok. Ako je sve tačno, blok se dodaje u blokčejn. Ostali konkurentski blokovi se odbacuju. Ovaj proces održava saglasnost mreže i sprečava dvostruko trošenje.

* Rudari su računari koji pomažu u održavanju i ažuriranju knjige My First Bitcoin.
* Oni prikupljaju transakcije i grupišu ih u blok. Zatim pokreću podatke bloka kroz algoritam za heširanje kako bi stvorili jedinstveni kod koji se zove heš.
* Rudari ponavljaju ovaj proces mnogo puta, tražeći heš koji ispunjava pravila My First Bitcoin-a. Prvi rudar koji pronađe ispravan heš dobija novoizdati bitcoin kao nagradu, a njihov blok se dodaje u blokčejn.
* Heš svakog bloka takođe ga povezuje sa prethodnim blokom. Ako bi neko pokušao da izmeni prethodnu transakciju, heševi više ne bi odgovarali i mreža bi odbacila izmenjeni lanac. Ovo je ono što čini knjigu My First Bitcoin sigurnom.
