# 8.1 Priroda Bitcoinove knjige evidencije

Bitcoinova knjiga transakcija (poznata i kao timechain ili blockchain) je javno dostupna, vremenski označena evidencija svake validne transakcije koja se ikada dogodila na mreži. U tradicionalnom finansijskom sistemu, interne transakcije su vidljive samo ovlašćenim učesnicima, kao što su banke, regulatori ili operateri podataka poput SWIFT-a, BACS-a ili SEPA-e. Pristup podacima o plaćanju u tradicionalnim sistemima može biti veoma ograničen i skup.

Nasuprot tome, u okviru Bitcoin mreže, svako sa internet vezom može da vidi svaku transakciju, od najveće vrednosti pa do pojedinačnog Satoshija. Učesnici mogu u realnom vremenu pratiti ukupnu ponudu bitcoina, nadgledati aktivnosti adresa i novčanika, kao i videti nagrade rudara i ponašanje naknada. Iako je vidljiva aktivnost na knjizi vezana za javne adrese ključeva, a ne za pojedinačne identitete, moguće je agregirati velike skupove podataka o potrošačkom ponašanju, što omogućava svima da prikupljaju i istražuju ekonomsku aktivnost u realnom vremenu. Kako mreža raste i postaje sve prihvaćenija kao izvor ekonomske istine, možemo očekivati manju zavisnost od državnih tela i trećih strana za izradu statističkih analiza i izveštaja o potrošačkom ponašanju.



#### 8.1.1 Čvorovi i blok eksploreri

Svako ko želi nezavisno da verifikuje Bitcoin knjigu i pristupi njenim podacima treba da pokrene pun čvor (full node). Pun čvor se često opisuje kao najosnovniji način učešća i verifikacije Bitcoin ekonomije. On je globalno dostupan kao open-source softver koji, kada se pokrene, preuzima i verifikuje celu Bitcoin knjigu od 'Genesis bloka', objavljenog u januaru 2009. godine, pa sve do danas. Takođe doprinosi bezbednosti Bitcoin mreže pomažući u verifikaciji novih transakcija koje se dodaju u knjigu. Pristupom Bitcoin knjizi na ovaj način, pun čvor služi kao izvor istine za istraživače i revizore mreže. Za korisnike Bitcoina, pun čvor predstavlja 'suvereni' pristup informacijama o transakcijama u Bitcoin ekonomiji jer poboljšava privatnost i bezbednost uklanjanjem zavisnosti od usluga trećih strana.

Dok puni čvorovi preuzimaju sirove podatke, blok eksploreri kao što su mempool.space ili blockstream.info nude vizuelni interfejs za pretragu i tumačenje aktivnosti na knjizi. Blok eksplorer omogućava praćenje pojedinačnih transakcija, pregled stanja i istorije novčanika. Takođe prikazuje metrike aktivnosti rudara kao što su nagrade za blokove i podaci o naknadama za transakcije.

Zajedno, puni čvorovi i blok eksploreri su alati koji čine transparentnost Bitcoin mreže upotrebljivom.



#### 8.1.2 Aktivnost: Istraživanje Bitcoin knjige

1. Otvorite [mempool.space](https://mempool.space) i istražite početnu stranicu.
  * Koja je visina najnovijeg bloka?
  * Kolika je trenutna naknada za transakciju (niski, srednji i visoki prioritet)?
  * Koliko transakcija čeka u mempool-u za sledeći blok?
1. Pristupite najnovijem bloku u knjizi.
  * Koliko transakcija je uključeno?
  * Kako se zove rudar ovog bloka?
  * Kolika je bila nagrada za blok?
1. Pristupite jednoj transakciji u bloku.
  * Koliko ulaza i izlaza ima transakcija?
  * Kolika je vrednost transakcije u BTC i EUR?

Diskutujte o razlikama između načina na koji novac cirkuliše u tradicionalnom sistemu i načina na koji preduzeće ili vlada koristi ovakvu vrstu transparentnosti.
