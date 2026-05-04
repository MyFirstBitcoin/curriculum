# 8.2 Maatstaven voor het analyseren van het grootboek

Omdat de transparantie van Bitcoin anders is dan die van traditionele financiële systemen — waar het grootste deel van de geldstromen achter gesloten institutionele deuren plaatsvindt — ontstaat er een rijk veld van on-chain analyse, waarbij netwerkdata een lens wordt om gebruikersgedrag, geldstromen en langetermijntrends te begrijpen. Deze statistieken kunnen helpen om specifieke vragen te beantwoorden, zoals hoe actief het netwerk wordt gebruikt, of munten worden geaccumuleerd of verkocht, en of het netwerk veiliger wordt.

Het begrijpen van deze statistieken is niet alleen nuttig voor Bitcoin-gebruikers, maar ook voor onderzoekers of beleidsmakers die inzicht willen krijgen in dit uniek transparante financiële systeem.

Deze sectie bevat enkele veelgebruikte statistieken voor het analyseren van Bitcoin-activiteit, gegroepeerd in subcategorieën. Het is geen volledige lijst. Bezoek [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) voor een uitgebreidere lijst en beschrijvingen.



#### 8.2.1 Adresstatistieken

Adresstatistieken zijn nuttig om in de tijd te volgen, omdat ze het activiteitsniveau op het Bitcoin-netwerk aangeven. Naarmate Bitcoin bijvoorbeeld meer wordt geadopteerd, neemt het aantal actieve adressen toe. We kunnen dit verder onderzoeken door het aantal adressen te bekijken dat een minimaal gespecificeerd bedrag aan Bitcoin bezit, bijvoorbeeld 0,1 BTC, binnen een bepaalde periode, zoals één jaar. Hoewel dit een beeld geeft van de adoptie van Bitcoin in de tijd, is het niet perfect, omdat een individu meerdere Bitcoin-adressen kan bezitten. Omgekeerd kunnen beurzen of ETF's als één entiteit verschijnen terwijl ze fondsen voor grote aantallen individuen beheren.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adressen die Bitcoin > X BTC vasthouden per jaar. Bron: Bitcoin Magazine Pro._

Door adressen te vergelijken met de huidige marktprijs van BTC is het mogelijk om het percentage van alle Bitcoin-adressen dat winst maakt te bekijken. Dit stelt ons in staat om het marktsentiment te volgen, omdat we kunnen zien welk deel van de markt BTC vasthoudt met winst of verlies.

Bijvoorbeeld, de **Percentage Onverwezenlijkte Winst** grafiek hieronder toont het aandeel van alle ledger-adressen met een onverwezenlijkte winst gemeten in Amerikaanse dollars. Merk op dat, aangezien de onderstaande grafiek is genomen vlak bij het hoogste punt ooit van Bitcoin, het percentage adressen met een onverwezenlijkte winst dicht bij honderd procent ligt. We zien ook dat langdurige periodes waarin het Percentage Onverwezenlijkte Winst onder één standaarddeviatie van het gemiddelde ligt, ongebruikelijk zijn. Daarom kan een daling onder deze lijn een goed instapmoment voor kopers suggereren.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Percentage Onverwezenlijkte Winst. Bron: checkonchain.com_



#### 8.2.2 On-Chain Indicatoren

On-chain indicatoren zijn nuttig omdat ze inzicht geven in netwerkgedrag, verder dan wat prijs- en adresstatistieken alleen kunnen laten zien. Ze helpen analisten de acties en het sentiment van verschillende soorten deelnemers te begrijpen, zoals langetermijnhouders versus kortetermijnhandelaren, door te volgen hoe munten worden vastgehouden, verplaatst of gewaardeerd in de tijd. Deze indicatoren maken gebruik van de transparantie van het grootboek om verborgen marktmechanismen te onthullen, zoals accumulatie, distributie of zelfs investeerdersovertuiging. Dit maakt ze bijzonder nuttig voor het identificeren van structurele trends, het beoordelen of de markt oververhit of ondergewaardeerd is, en het anticiperen op keerpunten in een marktcyclus.

Door bijvoorbeeld de waarde van BTC-bezit te onderzoeken sinds ze voor het laatst zijn verhandeld, kunnen we afleiden of de markt onder druk staat (zoals tijdens een dieptepunt in een grote cyclus). Deze statistiek staat bekend als **Gerealiseerde Prijs** en geeft ons een ‘gemiddelde kostprijs’ van alle BTC in omloop. Als de marktprijs onder de Gerealiseerde Prijs zakt, betekent dit dat het merendeel van de adressen gemiddeld genomen een papieren verlies heeft.

Door grootboekdata verder te groeperen in leeftijdsbanden, kunnen we laten zien hoe de hoeveelheid BTC in de loop van de tijd tussen adressen beweegt, wat golfachtige patronen op een grafiek creëert die bekend staan als **HODL-golven**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL-golven. Bron: Bitcoin Magazine Pro._

De HODL-golven laten zien wat langetermijn-, middellangetermijn- en kortetermijnhouders doen met hun BTC. In de bovenstaande grafiek worden kortetermijnhouders bijvoorbeeld weergegeven in rood en oranje, en we zien pieken in activiteit wanneer deze groep haastig koopt bij marktpieken. Aan de andere kant zien we dat zeer langetermijnhouders (in paars en blauw) hun aandeel in het netwerk gestaag vergroten, wat wijst op een hoge overtuiging binnen deze groepen. De grafiek is niet perfect, omdat sommige munten van oude naar nieuwe adressen kunnen verplaatsen onder controle van dezelfde gebruiker. Toch geeft het een interessant beeld van de overtuiging van langetermijnhouders.

Een andere manier om het ‘slimme geld’ van langetermijnhouders te onderzoeken is door te kijken naar **Coin Days Destroyed** (CDD). Het concept ‘Coin Days’ is een vermenigvuldiging van het aantal BTC met het aantal dagen sinds de munten voor het laatst zijn verplaatst. Bijvoorbeeld, 5 BTC die 100 dagen niet is verplaatst, heeft 500 coin days opgebouwd en 10 BTC die 10 dagen niet is verplaatst, heeft 100 coin days opgebouwd. Op deze manier geven we extra gewicht aan munten die langer worden vastgehouden. Wanneer deze munten worden verplaatst, worden die coin days ‘vernietigd’. Deze indicator laat stijgingen in CDD zien bij significante prijsbewegingen, wat analisten een manier biedt om routinematige marktactiviteit te onderscheiden van betekenisvolle verschuivingen in het sentiment van langetermijnhouders.

Een andere statistiek die kan helpen bepalen of de markt BTC onder- of overwaardeert, is de Market-Value to Realised Value of **MVRV**. Deze wordt eenvoudig berekend als de verhouding van Marktwaarde (aantal BTC in omloop vermenigvuldigd met de marktprijs) gedeeld door de Gerealiseerde Waarde (de som van alle BTC sinds ze voor het laatst zijn verplaatst). Een hoge MVRV suggereert dat meer munten winst maken (vaak gezien bij marktpieken) en een lage MVRV geeft aan dat veel munten met verlies worden vastgehouden (gezien bij marktdepressies).



#### 8.2.3 Miningstatistieken

Miningstatistieken zijn nuttig om het beveiligingsniveau, de economische prikkels en de algehele gezondheid van het Bitcoin-netwerk te begrijpen. Statistieken zoals hashrate, inkomsten van miners, moeilijkheidsgraad en fee-verhoudingen laten zien hoeveel rekenkracht de blockchain beveiligt en hoe goed miners worden beloond voor hun activiteiten.

De **Hashrate** van het Bitcoin-netwerk is misschien wel de meest genoemde indicator van de netwerkgezondheid en de sterkte van de beveiliging. Omdat het miningproces het netwerk beveiligt en bevestigt dat transacties op het grootboek geldig zijn, geldt: hoe meer rekenkracht (of hashing power) er is, hoe moeilijker het wordt voor een kwaadwillende partij om het netwerk te overmeesteren en aan te vallen.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Bron: Bitcoin Magazine Pro._

De bovenstaande grafiek laat zien dat in mei 2025 de totale rekenkracht van het netwerk rond de 900 TeraHash/s ligt (900 biljoen cryptografische ‘hash’-berekeningen per seconde). Als de hashrate stijgt, betekent dit dat het netwerk veiliger wordt, wat geruststellend is voor gebruikers.

De Puell Multiple (bedacht door David Puell) bekijkt de marktcyclus vanuit het perspectief van miners en hun inkomsten. De statistiek wordt berekend door de dagelijkse uitgifte van BTC (in USD) te delen door het voortschrijdend gemiddelde van 365 dagen van de dagelijkse uitgiftewaarde. De statistiek helpt om periodes van stress of verlichting voor miners te identificeren. Historisch gezien is een multiple boven de 3 voorafgegaan aan een daling van de marktwaarde van BTC, omdat dit aangeeft dat miners zeer winstgevend zijn. Een waarde onder de 0,5 duidt op stress en heeft historisch gezien marktdepressies voor de waarde van BTC aangegeven.
