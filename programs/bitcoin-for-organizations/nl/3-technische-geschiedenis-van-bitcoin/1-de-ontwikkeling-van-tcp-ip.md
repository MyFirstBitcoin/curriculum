# 3.1 De ontwikkeling van TCP/IP

De meesten van ons zijn bekend met de TCP/IP-protocollen die tegenwoordig worden gebruikt als de basis van het internet. Hun oorsprong gaat terug tot het einde van de jaren 70, toen wetenschappers alternatieve ontwerpen voor Arpanet onderzochten – een nog eerder netwerk dat werd bedacht door het Amerikaanse Ministerie van Defensie om het delen van middelen tussen computers op afstand mogelijk te maken. TCP/IP werd in 1983 de protocolstandaard voor Arpanet, wat ertoe leidde dat het tegen het einde van de jaren 90 het dominante netwerkmodel werd en de basis vormde voor het internet waarop Bitcoin vandaag draait.


| OSI-model | TCP/IP |
| --- | --- |
| Applicatie | Applicatie |
| Presentatie | Applicatie |
| Sessie | Applicatie |
| Transport | Transport |
| Netwerk | Netwerk |
| Datalink | Datalink |
| Fysiek | Fysiek |


Tegelijkertijd met de ontwikkeling van het TCP/IP-model werd er een vergelijkbaar maar uitgebreider raamwerk ontwikkeld door de International Standards Organisation (ISO) en de telecomindustrie (CCITT). Het proces om nieuwe protocollen te ontwikkelen of wijzigingen voor te stellen verliep traag en omslachtig in vergelijking met de meer gedecentraliseerde aanpak die werd gebruikt voor de ontwikkeling van TCP/IP, wat heeft geleid tot de dominantie van deze aanpak vandaag de dag.

##### Verzoek tot wijziging

Alle voorgestelde ontwikkelingen aan bestaande protocollen of ideeën voor nieuwe kunnen in het TCP/IP-model worden voorgesteld via een **Verzoek tot wijziging** proces. Deze doorlopen een goedkeuringsproces, beheerd door de Internet Engineering Task Force (IETF), en worden open source zodra ze zijn goedgekeurd, zodat iedereen ze kan implementeren en overnemen. Enkele opmerkelijke voorbeelden:

* 1969 RFC 1 Documenteerde hoe pakketten zouden worden verzonden in het Arpanet
* 1981 RFC791 definieerde het Internet Protocol V4 – nog steeds veel gebruikt vandaag
* 1982 RFC 821 Simple Mail Transfer Protocol
* 1987 Domain Name System – hoe domeinnamen worden omgezet naar IP-adressen
* 1999 RFC 2616 Hypertext Transfer Protocol – essentieel voor het surfen op het web


> **Callout**
>
> De **Bitcoin Improvement Proposal** (BIP) volgt een vergelijkbare aanpak als RFC, maar richt zich puur op verbeteringen aan Bitcoin zelf in plaats van de ontwikkeling van nieuwe of alternatieve protocollen. Bitcoin leent ook van dit gelaagde model, en je zult extra protocollen zien die worden beschreven als laag twee of drie.


Op dezelfde manier als de basislagen van het TCP/IP-model de afgelopen decennia relatief weinig zijn veranderd, met innovatie die plaatsvindt op hogere lagen, wordt verwacht dat de basislaag van Bitcoin op dit moment zeer langzaam zal veranderen, met schaaloplossingen zoals Lightning en Liquid die daarboven plaatsvinden.

Een goed voorbeeld van hoe basislaagprotocollen na verloop van tijd moeilijk te veranderen worden, is IPv6. De verwachte uitputting van het adresbereik in IPv4 creëerde een vraag naar een nieuw protocol. De eerste conceptstandaard werd in 1998 opgesteld, maar pas in 2017 als internetstandaard bekrachtigd. Hoewel het veel problemen met IPv4 oploste en veel toekomstbestendiger is, is de adoptie ervan in de industrie vandaag nog steeds erg traag. In deze periode zijn er op de bovenste lagen veel nieuwe protocollen gedefinieerd om multimedia, e-mail, enz. mogelijk te maken.

##### De bouwstenen die door Bitcoin worden gebruikt

Deze scheiding van de problemen van onderlinge connectiviteit maakt het mogelijk dat protocollen onafhankelijk van de lagen erboven en eronder kunnen worden ontwikkeld. In plaats van oplossingen voor elke laag opnieuw te moeten uitvinden, kan het Bitcoinnetwerk vertrouwen op de onderliggende mogelijkheden van het netwerk die op de fysieke en datalinklagen worden geleverd.


| Laag | TCP/IP Oorspronkelijk |
| --- | --- |
| Applicatie | Gebruikt Domain Name System (DNS) om naburige nodes te identificeren. Poort 8333 signaleert Bitcoin-protocol. |
| Transport | UDP voor FIBRE-communicatie tussen miners voor lage latentie. TCP voor P2P-communicatie tussen nodes. |
| Transport | TOR-routing: Maakt anonimiteit en privacy mogelijk. Broadcast-protocol: Routeert verkeer over het netwerk. |
| Link | Werkt over elk medium (bijv. Ethernet, Wi-Fi, enz.) |
| Fysiek | Fysieke transmissie via draadloos, Ethernet of andere hardware-interfaces. |


##### Bitcoin is een neutraal protocol om waarde over te dragen, zoals HTTPS een protocol is om informatie over te dragen

* **HTTPS**: Beveiligde websites
* **SMTP**: E-mails verzenden
* **FTP**: Bestanden overdragen
* **DNS**: Domeinnamen beheren
* **BTC**: Waarde opslaan en overdragen

Bitcoin maakt het mogelijk om waarde betrouwbaar en zonder tussenkomst van een derde partij tussen mensen of apparaten via het internet te verplaatsen. Dit zal naar verwachting enorme waarde ontsluiten.
