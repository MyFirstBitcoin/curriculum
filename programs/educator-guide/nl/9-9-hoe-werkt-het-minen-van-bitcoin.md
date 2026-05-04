# 9 - Hoe werkt het minen van Bitcoin

Duur: 90 minuten

Kernidee: Bitcoin-mining en node-validatie werken samen om het netwerk te beveiligen, transacties te bevestigen en de regels van het systeem af te dwingen via Proof of Work.

#### Leerdoelen

Aan het einde van deze les moeten studenten in staat zijn om:

* Leg het verschil uit tussen de rol van Bitcoin-nodes en de rol van Bitcoin-miners.
* Beschrijf hoe nodes transacties valideren, informatie delen en helpen de regels van Bitcoin af te dwingen.
* Leg uit wat miners doen, waaronder het selecteren van transacties, het bouwen van kandidaat-blokken en het concurreren om een geldige block-hash te vinden.
* Definieer de mempool en leg uit waarom deze werkt als een wachtruimte voor onbevestigde transacties.
* Beschrijf hoe transactiekosten de selectie door miners en de snelheid van bevestiging beïnvloeden.
* Leg Proof of Work uit als het mechanisme dat Bitcoin beveiligt door aanvallen duur te maken.
* Beschrijf hoe de moeilijkheidsaanpassing helpt om een gemiddelde bloktijd van ongeveer 10 minuten te behouden.
* Loop door de volledige levenscyclus van een Bitcoin-transactie, van aanmaak en ondertekening tot bevestiging in een blok.

#### Hulpmiddelen & Bronnen

##### Visuele hulpmiddelen

* Hoofdstuk 9 - Hoe werkt Bitcoin-mining?

##### Ondersteunende bibliotheek

* Woordenkaart — Hoofdstuk 9 — Termen: mining, Proof of Work, hash-puzzel, moeilijkheidsaanpassing, blokbeloning, mempool, 51%-aanval
* Misvattingen-bibliotheken — Hoofdstuk 9 — Adres: "miners creëren Bitcoin uit het niets," "miners controleren Bitcoin," "meer mining = minder veilig"
* Vergelijkingsschema's & referentiebladen — Mining-economie: inkomsten, kosten, prikkeluitlijning; moeilijkheidsaanpassing
* Technische uitleg & diepgaande analyses — Proof of Work-beveiliging; waarom aanvallen duur is; 51%-drempel

#### Activiteiten

* De mempool verkennen
* Transacties in actie

#### Online lesgeven

* Gebruik één duidelijk transactiestroomschema van wallet-ondertekening tot bevestiging.
* Houd nodes en miners visueel gescheiden op het scherm gedurende de hele les.
* Gebruik mempool.space of een screenshot daarvan om onbevestigde transacties en fee-druk te tonen.
* Pauzeer na elke fase van het miningproces en stel één korte begripsvraag.

#### Voorbereiding

* Bereid een diagram van het miningproces voor (mempool → transactieselectie → blokcreatie → moeilijkheidsaanpassing) om te tonen.
* Bookmark mempool.space of de miningpagina van blockchain.com; bereid screenshots voor van actuele miningstatistieken en moeilijkheidsaanpassingen.
* Maak een visuele uitleg van Proof of Work als beveiligingsmechanisme; toon moeilijkheidsaanpassing over de afgelopen 3-6 maanden.

#### Procedure

Deze les kijkt van dichtbij naar hoe Bitcoin-transacties door het netwerk bewegen en onderdeel worden van de blockchain. De les volgt nu direct de structuur van het Diploma, zodat de hoofdsecties aansluiten bij de studentengids, terwijl de uitgebreidere uitleg voor docenten binnen elke sectie behouden blijft.

##### 9.0 Introductie, 8 minuten

Begin met het verbinden van dit hoofdstuk aan het vorige:

* Als een gebruiker een transactie ondertekent met een privésleutel, wat gebeurt er dan?
* Wie controleert of die transactie geldig is?
* Hoe wordt deze toegevoegd aan de blockchain?
* Waarom heeft Bitcoin zowel nodes als miners nodig?

Maak duidelijk dat dit hoofdstuk uitlegt hoe het netwerk transacties in de praktijk verwerkt en hoe mining het systeem beveiligt zonder centrale autoriteit.

##### 9.1 Bitcoin-nodes en miners, 47 minuten

**Nodes en miners, verschillende rollen**

Begin met het duidelijk scheiden van de twee rollen.

Bitcoin-nodes:

* houden een kopie van de blockchain bij
* controleren of transacties aan de regels voldoen
* delen informatie met andere nodes
* helpen wallets en andere software toegang te krijgen tot blockchaingegevens
* kunnen ongeldige transacties of ongeldige blokken afwijzen

Het hoofdstuk beschrijft nodes als poortwachters van validatie, en breidt dat uit met de analogie van de "digitale verkeersagent". Dat is nuttig omdat het laat zien dat nodes controleurs en coördinatoren zijn, geen heersers. Het diagram benadrukt ook dat veel nodes kopieën van het grootboek over de hele wereld bewaren.

Bitcoin miners:

* verzamelen geldige transacties
* stellen kandidaat-blokken samen
* concurreren om een geldige blok-hash te vinden
* zenden geldige blokken uit wanneer ze winnen
* ontvangen blokbeloningen en transactiekosten

Een belangrijk leerpunt uit het hoofdstuk is dat het doel van mining niet simpelweg is om nieuwe bitcoin te creëren, maar om de beveiliging van Bitcoin te decentraliseren. De nieuwe bitcoin is de stimulans, terwijl het miningproces zelf het beveiligingsmechanisme is.

**Wat nodes daadwerkelijk doen**

Bouw voort op het node-gedeelte met de lijst van node-functies uit het hoofdstuk:

* Poortwachters van validatie: ze controleren of transacties en blokken aan de regels voldoen
* Communicatieknooppunt: ze verbinden met elkaar en delen transactiegegevens
* Kwaliteitscontroleur: ze wijzen ongeldige informatie af
* Blockchain-informant: ze leveren gegevens aan andere software zoals wallets
* Nieuwe node-verwelkomer: ze helpen nieuwe nodes om de blockchain te verkrijgen, terwijl elke nieuwe node de gegevens toch onafhankelijk verifieert

Dit is een goed moment om te benadrukken dat het draaien van een node de gebruiker meer onafhankelijkheid geeft. In plaats van volledig afhankelijk te zijn van externe diensten om hen de staat van het netwerk te vertellen, kunnen ze het zelf verifiëren.  maakt dit punt duidelijk, inclusief de vermelding van Bitcoin Core als een implementatie die gebruikers kunnen draaien.

**Wat miners daadwerkelijk doen**

Leg nu mining zorgvuldiger uit.

Miners:

* verzamelen geverifieerde maar onbevestigde transacties
* groeperen deze in een kandidaat-blok
* hasht herhaaldelijk blokgegevens terwijl ze zoeken naar een geldige blok-hash
* zenden het winnende blok uit naar het netwerk
* verdienen beloningen als het blok wordt geaccepteerd

Gebruik de analogie van het hoofdstuk met de "enorme hooiberg van sleutels" als dat helpt. Het geeft studenten een concreet beeld van de miningrace. Het belangrijkste idee is niet dat miners een nuttig wiskundig probleem oplossen in de gewone zin, maar dat ze bewijzen dat ze echte energie en rekenkracht hebben besteed om het systeem te beveiligen.

Dit is ook het juiste moment om miner-beloningen uit te leggen:

* blokbeloning: nieuw uitgegeven bitcoin
* transactiekosten: kosten die zijn toegevoegd aan transacties die gebruikers bevestigd willen hebben

Verduidelijk dat miners meestal transacties met hogere kosten prioriteren, omdat die hun beloning verhogen. Het hoofdstuk legt hier ook halvings uit, dus je kunt kort vermelden dat de blokbeloning elke 210.000 blokken afneemt, ongeveer elke vier jaar, volgens het openbare uitgifteschema van Bitcoin. Pagina's 5 en 6 bevatten het uitgifteschema en de aankomende halveringstabel, wat kan helpen om Bitcoin's voorspelbare uitgifte te benadrukken.

**Geldige blok-hash, Proof of Work en moeilijkheidsaanpassing**

Deze sectie is de kern van het hoofdstuk.

Leg uit dat miners zoeken naar een geldige blok-hash, wat betekent een blok-hash die voldoet aan het doel van het netwerk. Het hoofdstuk legt dit uit als het vinden van een getal dat lager is dan het doel dat door het netwerk is ingesteld.

Leg daarna Proof of Work duidelijk uit:

* miners moeten herhaaldelijk rekenwerk verrichten
* degene die als eerste een geldige hash vindt, bewijst dat hij dat werk heeft gedaan
* dit maakt het duur om het grootboek te herschrijven of aan te vallen
* nodes verifiëren vervolgens het blok voordat ze het accepteren

Een sterke zin om te onderwijzen is:

Proof of Work beveiligt Bitcoin door oneerlijkheid duur te maken en verificatie gemakkelijk.

Leg ook de moeilijkheidsaanpassing uit:

* het netwerk past de mining-moeilijkheid aan elke 2.016 blokken aan
* dit gebeurt ongeveer elke twee weken
* het doel is om de gemiddelde bloktijd dicht bij 10 minuten te houden
* als er meer rekenkracht aan het netwerk wordt toegevoegd, stijgt de moeilijkheidsgraad
* als er minder rekenkracht is, daalt de moeilijkheidsgraad

Pagina's 7 en 8 leggen dit proces uit en laten zien hoe moeilijkere doelen meer werk vereisen. Dit helpt studenten te begrijpen dat de timing van Bitcoin niet wordt gecontroleerd door een centrale autoriteit, maar door protocolregels die automatisch reageren op netwerkcondities.

##### 9.2 Wat is de mempool?, 15 minuten

Ga nu verder naar de mempool.

Leg uit dat de mempool de wachtruimte is voor geldige, onbevestigde transacties. Wanneer een gebruiker een transactie uitzendt, verifiëren nodes deze eerst. Als deze geldig is, voegen ze hem toe aan hun mempool en delen ze hem met andere nodes. Daarna kunnen miners uit deze wachtende transacties kiezen bij het bouwen van een blok. Pagina's 10 en 11 leggen dit proces direct uit.

Belangrijke punten om te benadrukken:

* de mempool is niet de blockchain
* transacties daar zijn nog niet bevestigd
* elke node onderhoudt zijn eigen mempool
* er is niet één enkele universele mempool
* transacties met een hogere vergoeding worden waarschijnlijk sneller geselecteerd

Het hoofdstuk legt ook uit waarom een transactie soms lang onbevestigd blijft:

* lage vergoeding
* netwerkcongestie
* poging tot double-spend
* onjuiste of onvolledige gegevens
* ongeldig gevormde transactie

Indien nuttig, noem de activiteit met mempool.space als een praktische manier om onbevestigde transacties en vergoedingen te visualiseren. Maak ook duidelijk dat mempool.space slechts één explorer is, niet de mempool zelf.

##### 9.3 Hoe Bitcoin-transacties werken, 20 minuten

Breng nu alles samen met behulp van de stapsgewijze volgorde uit het hoofdstuk.

Een duidelijke versie voor in de klas is:



1. De verzender selecteert een UTXO en maakt een transactie
1. De verzender voegt het ontvangstadres en de vergoeding toe
1. De verzender ondertekent de transactie met zijn privésleutel
1. De transactie wordt uitgezonden naar het netwerk
1. Nodes verifiëren deze en voegen hem toe aan hun mempools
1. Miners selecteren hem voor een kandidaatblok
1. Miners concurreren via Proof of Work
1. Eén miner vindt een geldige blokhash en zendt het blok uit
1. Nodes verifiëren het blok en voegen het toe aan de blockchain
1. De transactie ontvangt bevestigingen naarmate er meer blokken worden toegevoegd
1. Maak het laatste punt expliciet:
1. zodra de transactie is opgenomen in een geldig blok, is deze bevestigd
1. de gebruikte inputs zijn niet langer bruikbaar
1. de ontvanger beheert nu de nieuwe UTXO's die door die transactie zijn aangemaakt

Het overzichtsdiagram is hier vooral nuttig omdat het het hele proces visueel verbindt: van ondertekening in de wallet tot opname door de miner, validatie door de node en distributie van het blok.

###### Afronding en controle van begrip

Sluit af met een paar snelle vragen:

* Wat is het verschil tussen een node en een miner?
* Wat is de mempool?
* Waarom worden sommige transacties sneller bevestigd dan andere?
* Wat bewijst Proof of Work?
* Waarom past Bitcoin de mining-moeilijkheid aan?
* Wat zijn de belangrijkste stappen tussen het versturen van een transactie en het ontvangen van een bevestiging?

#### Aantekeningen voor docenten

Houd de belangrijkste leslijn duidelijk: nodes verifiëren, miners concurreren, Proof of Work beveiligt, en de mempool houdt geldige transacties vast tot ze bevestigd zijn.

Dit hoofdstuk kan technisch aanvoelen, dus gebruik vaak analogieën en diagrammen.

Voorkom dat mining klinkt als "bitcoin uit het niets creëren." Wees precies dat de beloning het incentive is, terwijl het miningproces het netwerk beveiligt.

De belangrijkste punten om te benadrukken als de tijd kort is, zijn:



1. Rollen van node versus miner
1. Mempool als wachtruimte
1. Proof of Work
1. Aanpassing van de moeilijkheidsgraad
1. Transactiestroom van ondertekening tot bevestiging

##### Hoe ziet goed onderwijs eruit

* Het is belangrijk om direct duidelijk te maken dat Miners ≠ Nodes, mining te tonen als economische activiteit met echte hardwarekosten en elektriciteitsverbruik, moeilijkheidsaanpassing en Proof of Work te gebruiken om het beveiligingsmechanisme uit te leggen, en het begrip te testen met scenario's over netwerkveranderingen.
* Onderwijzers moeten echte cijfers gebruiken om discussies te onderbouwen, glashelder en herhaaldelijk zijn over het verschil tussen Miners en Nodes, realistisch zijn over centralisatieproblemen bij mining pools, en respect tonen voor de daadwerkelijke complexiteit die erbij komt kijken.
* Studenten begrijpen dat mining slimme mensen zijn die complex werk doen omdat ze Bitcoin verdienen, erkennen dat prikkels eerlijk gedrag stimuleren omdat de winst van miners afhangt van het succes van Bitcoin, zien dat het systeem zichzelf reguleert via automatische moeilijkheidsaanpassing, begrijpen dat mining een echt bedrijf is en geen liefdadigheid, en waarderen dat de beveiliging van Bitcoin echte elektriciteit en geld kost.
* Leerdoelen zijn behaald als studenten het verschil kunnen maken tussen miners die blokken maken en nodes die ze valideren, Proof of Work begrijpen als een beveiligingsmechanisme dat aanvallen exponentieel duur maakt, herkennen dat moeilijkheidsaanpassing de bloktijd op ongeveer 10 minuten houdt, de prikkels van miners rond blokbeloningen en transactiekosten begrijpen, kunnen uitleggen waarom een 51%-aanval niet werkt, en mining zien als een economische activiteit met echte kosten en baten.

##### Tijdbeheer

Als de tijd beperkt is, geef prioriteit aan:

* Node versus miner rollen (het cruciale verschil)
* Mempool als wachtruimte
* Proof of Work mechanisme
* Moeilijkheidsaanpassing (zelfregulerend systeem)
* Transactiestroom van ondertekening tot bevestiging

Als je voorloopt, neem dan de tijd voor:

* Mining economie en hardware specifieke details
* Dynamiek van mining pools en centralisatieproblemen
* 51%-aanval scenario's en waarom ze wiskundig falen
* Langetermijnbeveiliging door prikkelafstemming

##### Als studenten moeite hebben

* Miners versus nodes (verwarring) → "Nodes valideren, miners stellen voor; scheidsrechters versus spelers."
* Proof of Work verspilling → "Dure beveiliging voorkomt aanvallen; maakt ze zinloos."
* Moeilijkheidsaanpassing → "Meer miners = snellere blokken = moeilijkheid stijgt; het systeem ademt."
