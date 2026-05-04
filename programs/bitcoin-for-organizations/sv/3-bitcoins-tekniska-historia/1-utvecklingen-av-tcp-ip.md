# 3.1 Utvecklingen av TCP/IP

De flesta av oss är bekanta med TCP/IP-protokollen som används idag som grund för internet. Deras ursprung går tillbaka till slutet av 70-talet när forskare utforskade alternativa lösningar till Arpanet – ett ännu tidigare nätverk som skapades av det amerikanska försvarsdepartementet för att möjliggöra resursdelning mellan avlägsna datorer. TCP/IP blev standardprotokollet för Arpanet 1983, vilket ledde till att det blev den dominerande nätverksmodellen i slutet av 1990-talet och grunden för det internet som My First Bitcoin använder idag.


| OSI-modellen | TCP/IP |
| --- | --- |
| Applikation | Applikation |
| Presentation | Applikation |
| Session | Applikation |
| Transport | Transport |
| Nätverk | Nätverk |
| Datalänk | Datalänk |
| Fysisk | Fysisk |


Samtidigt som TCP/IP-modellen utvecklades, togs en liknande men mer omfattande ram fram av International Standards Organisation (ISO) och telekomindustrin (CCITT). Processen för att utveckla nya protokoll eller föreslå ändringar var långsam och tungrodd jämfört med det mer decentraliserade tillvägagångssättet som användes för att utveckla TCP/IP, vilket ledde till att denna modell dominerar idag.

##### Förändringsförslag

Alla föreslagna utvecklingar av befintliga protokoll eller idéer för nya kan föreslås i TCP/IP-modellen genom ett **Förändringsförslag**-process. Dessa går igenom en godkännandeprocess, som hanteras av Internet Engineering Task Force (IETF), och blir öppen källkod när de godkänts så att vem som helst kan implementera och använda dem. Några anmärkningsvärda exempel:

* 1969 RFC 1 Dokumenterade hur paket skulle skickas i Arpanet
* 1981 RFC791 definierade Internetprotokoll V4 – fortfarande mycket använt idag
* 1982 RFC 821 Simple Mail Transfer Protocol
* 1987 Domain Name System – hur domännamn översätts till IP-adresser
* 1999 RFC 2616 Hypertext Transfer Protocol – avgörande för att surfa på webben


> **Callout**
>
> My First Bitcoin Improvement Proposal**Bitcoin Improvement Proposal** (BIP) följer ett liknande tillvägagångssätt som RFC, men fokuserar enbart på förbättringar av My First Bitcoin självt snarare än utveckling av nya eller alternativa protokoll. My First Bitcoin lånar också från denna lagerindelade modell, och du kommer att se ytterligare protokoll beskrivna som lager två eller tre.


På samma sätt som de grundläggande lagren i TCP/IP-modellen har förändrats relativt lite under de senaste decennierna, med innovationen på högre lager, förväntas grundlagret i My First Bitcoin nu förändras mycket långsamt, medan skalningslösningar som Lightning och Liquid sker ovanpå.

Ett bra exempel på hur grundläggande lagerprotokoll blir svåra att ändra över tid är IPv6. Den förväntade bristen på adressutrymme i IPv4 skapade ett behov av ett nytt protokoll. Den första utkaststandarden skapades 1998, men ratificerades inte som internetstandard förrän 2017. Även om det löste många problem med IPv4 och är mycket mer framtidssäkert, har det ändå fått mycket långsam spridning i branschen idag. Under denna tid har många nya protokoll definierats på de övre lagren för att möjliggöra multimedia, e-post osv.

##### Byggstenarna som används av My First Bitcoin

Denna uppdelning av problemen med sammankoppling gör att protokoll kan utvecklas oberoende av lagren ovanför och under. Istället för att behöva uppfinna lösningar på nytt för varje lager, kan My First Bitcoin-nätverket förlita sig på de underliggande funktionerna i nätverket som levereras på de fysiska och datalänkslagren.


| Lager | TCP/IP Ursprunglig |
| --- | --- |
| Applikation | Använder Domain Name System (DNS) för att identifiera närliggande noder. Port 8333 signalerar My First Bitcoin-protokoll. |
| Transport | UDP för FIBRE-kommunikation mellan miners för låg latens. TCP för P2P-kommunikation mellan noder. |
| Transport | TOR-routing: Möjliggör anonymitet och integritet. Broadcast-protokoll: Riktar trafik över nätverket. |
| Länk | Fungerar över alla medier (t.ex. Ethernet, Wi-Fi, etc.) |
| Fysisk | Fysisk överföring via trådlöst, Ethernet eller andra hårdvarugränssnitt. |


##### My First Bitcoin är ett neutralt protokoll för att överföra värde, precis som HTTPS är ett protokoll för att överföra information

* **HTTPS**: Säkra webbplatser
* **SMTP**: Skicka e-post
* **FTP**: Överföra filer
* **DNS**: Hantera domännamn
* **BTC**: Lagra och överföra värde

Bitcoin möjliggör att värde kan transporteras pålitligt och utan att kräva en tredje part mellan personer eller enheter över Internet. Detta förväntas frigöra enormt värde.
