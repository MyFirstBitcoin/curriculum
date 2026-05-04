# 3.1 Razvoj TCP/IP-a

Većina nas je upoznata sa TCP/IP protokolima koji se danas koriste kao osnova interneta. Njihovo poreklo datira iz kasnih 70-ih godina kada su naučnici istraživali alternativne dizajne za Arpanet – još raniju mrežu koju je osmislilo Ministarstvo odbrane SAD kako bi omogućilo deljenje resursa između udaljenih računara. TCP/IP je postao standardni protokol za Arpanet 1983. godine, što je dovelo do toga da do kraja 1990-ih postane dominantni model umrežavanja i osnova interneta na kojem danas funkcioniše Bitcoin.


| OSI model | TCP/IP |
| --- | --- |
| Aplikacija | Aplikacija |
| Prezentacija | Aplikacija |
| Sesija | Aplikacija |
| Transport | Transport |
| Mreža | Mreža |
| Povezivanje podataka | Povezivanje podataka |
| Fizički sloj | Fizički sloj |


U isto vreme kada se razvijao TCP/IP model, razvijan je sličan, ali obuhvatniji okvir od strane Međunarodne organizacije za standardizaciju (ISO) i telekom industrije (CCITT). Proces razvoja novih protokola ili predlaganja izmena bio je spor i nezgrapan u poređenju sa decentralizovanijim pristupom koji je korišćen za razvoj TCP/IP-a, što je dovelo do dominacije ovog pristupa danas.

##### Zahtev za izmenu

Bilo kakav predlog za razvoj postojećih protokola ili ideje za nove mogu se predložiti u TCP/IP modelu kroz **Zahtev za izmenu** proces. Oni prolaze kroz proces odobravanja, kojim upravlja Internet Engineering Task Force (IETF), i postaju otvorenog koda kada budu odobreni, kako bi svako mogao da ih implementira i usvoji. Neki značajni primeri:

* 1969 RFC 1 Dokumentovao je kako će paketi biti slati u Arpanetu
* 1981 RFC791 definisao je Internet protokol V4 – i danas široko korišćen
* 1982 RFC 821 Protokol za jednostavan prenos elektronske pošte
* 1987 Sistem imena domena – kako se imena domena prevode u IP adrese
* 1999 RDC 2616 Protokol za prenos hiperteksta – ključan za pretraživanje interneta


> **Callout**
>
> The **Bitcoin Improvement Proposal** (BIP) prati sličan pristup kao RFC, ali se fokusira isključivo na unapređenja samog Bitcoina, a ne na razvoj novih ili alternativnih protokola. Bitcoin takođe preuzima ovaj slojeviti model, pa ćete videti dodatne protokole opisane kao drugi ili treći sloj.


Na isti način na koji se osnovni slojevi TCP/IP modela malo menjaju poslednjih decenija, dok se inovacije dešavaju na višim slojevima, očekuje se da se osnovni Bitcoin sloj sada veoma sporo menja, dok se rešenja za skaliranje kao što su Lightning i Liquid razvijaju iznad njega.

Dobar primer kako osnovni protokoli postaju teško promenjivi tokom vremena je IPv6. Očekivano iscrpljivanje adresnog prostora u IPv4 stvorilo je potrebu za novim protokolom. Prvi nacrt standarda napravljen je 1998. godine, ali nije ratifikovan kao internet standard do 2017. godine. Iako je rešio mnoge probleme IPv4 i mnogo je otporniji na buduće promene, i dalje se veoma sporo usvaja u industriji danas. Za to vreme, mnogi novi protokoli su definisani na višim slojevima kako bi omogućili multimediju, e-poštu itd.

##### Građevinski blokovi koje koristi Bitcoin

Ova podela problema međusobnog povezivanja omogućava da se protokoli razvijaju nezavisno od slojeva iznad i ispod. Umesto da se za svaki sloj iznova izmišljaju rešenja, Bitcoin mreža može da se osloni na osnovne mogućnosti mreže koje pružaju fizički i sloj za povezivanje podataka.


| Sloj | TCP/IP original |
| --- | --- |
| Aplikacija | Koristi sistem imena domena (DNS) za identifikaciju susednih čvorova. Port 8333 signalizira Bitcoin protokol. |
| Transport | UDP za FIBRE komunikaciju između rudara radi niske latencije. TCP za P2P komunikaciju između čvorova. |
| Transport | TOR rutiranje: Omogućava anonimnost i privatnost. Protokol za emitovanje: Usmerava saobraćaj kroz mrežu. |
| Veza | Radi preko bilo kog medijuma (npr. Ethernet, Wi-Fi, itd.) |
| Fizički sloj | Fizički prenos putem bežične veze, Ethernet-a ili drugih hardverskih interfejsa. |


##### Bitcoin je neutralni protokol za prenos vrednosti kao što je HTTPS protokol za prenos informacija

* **HTTPS**: Sigurni sajtovi
* **SMTP**: Šaljite e-poštu
* **FTP**: Prenosite fajlove
* **DNS**: Upravljajte domenima
* **BTC**: Čuvajte i prenosite vrednost

Bitcoin omogućava pouzdan prenos vrednosti između ljudi ili uređaja preko Interneta, bez potrebe za trećom stranom. Očekuje se da će ovo otključati ogroman potencijal.
