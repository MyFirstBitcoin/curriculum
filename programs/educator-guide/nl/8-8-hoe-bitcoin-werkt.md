# 8 - Hoe Bitcoin Werkt

Duur: 90 minuten

Kernidee: De veiligheid van Bitcoin is gebaseerd op eenvoudige maar krachtige technische concepten zoals sleutels, handtekeningen, hashing en UTXO's, die eigendom en verificatie mogelijk maken zonder een centrale autoriteit.

#### Leerdoelen

Aan het einde van deze les moeten studenten in staat zijn om:

* Uitleggen hoe publieke en private sleutels helpen om het eigendom en de transacties van Bitcoin te beveiligen.
* Beschrijven wat een digitale handtekening is en hoe deze bewijst dat een transactie is goedgekeurd door de rechtmatige eigenaar.
* In eenvoudige bewoordingen uitleggen wat cryptografie, encryptie en decryptie betekenen in de context van Bitcoin.
* Hashing definiëren en beschrijven waarom hashfuncties belangrijk zijn voor de veiligheid en gegevensintegriteit van Bitcoin.
* De basiskenmerken van een hashfunctie benoemen, zoals vaste lengte van de uitvoer, eenrichtingskarakter en gevoeligheid voor kleine veranderingen in de invoer.
* Het UTXO-model uitleggen en hoe bitcoin wordt uitgegeven, ontvangen en als wisselgeld wordt teruggegeven via transactie-uitgangen.
* Beschrijven hoe nodes helpen om dubbel uitgeven te voorkomen door te controleren of een output al is uitgegeven.

#### Hulpmiddelen & Bronnen

##### Visuele hulpmiddelen

* Hoofdstuk 8 - Hoe Bitcoin Werkt

##### Ondersteunende bibliotheek

* Woordenkaart — Hoofdstuk 8 — Termen: cryptografie, hash, UTXO, digitale handtekening, private/publieke sleutel, merkleboom, blockchain
* Misvattingenbibliotheek — Hoofdstuk 8 — Adres: "verloren seed phrase kan worden hersteld," "private key = wachtwoord," "blockchain is anoniem"
* Technische uitleg & diepgang — Hashfuncties, publieke/private sleutels, UTXO-model, Proof of Work-beveiliging

#### Activiteiten

* Transacties in de praktijk
* De mempool verkennen

#### Online lesgeven

* Gebruik een digitaal whiteboard en teken elk concept live in plaats van alleen mondeling uit te leggen.
* Behandel telkens één technisch concept en pauzeer regelmatig voor controlevragen.
* Gebruik visuele hulpmiddelen voor sleutels, handtekeningen, hashes en UTXO's zodat studenten de structuur kunnen volgen.
* Houd het doel conceptueel en ga niet te diep in op wiskunde of jargon.

#### Voorbereiding

* Bereid gelamineerde diagrammen voor: publieke/private sleutelpaar, digitale handtekeningen, UTXO-model, hashing (eenrichtingsfunctie).
* Zet een blockchain explorer en SHA-256 hash calculator in de favorieten; selecteer 2-3 echte Bitcoin-transacties om stap voor stap door te nemen.
* Bereid whiteboardnotities voor om inputs, outputs en hoe transacties worden bevestigd op de blockchain uit te leggen.

#### Procedure

Deze les geeft studenten een eerste blik op de technische kant van Bitcoin zonder dat er technische voorkennis wordt verwacht. De handleiding volgt nu dezelfde compacte structuur als het Diploma, waarbij cryptografie onder één kopje is gegroepeerd en UTXO's onder het andere.

##### 8.0 Introductie, 8 minuten

Begin met het scheppen van verwachtingen:

* Wat maakt Bitcoin veilig als er geen centrale bank is die het beheert?
* Hoe kan het netwerk weten of iemand echt de eigenaar is van de bitcoin die hij probeert te versturen?
* Wat gebeurt er eigenlijk achter de schermen als iemand een Bitcoin-transactie doet?

Maak duidelijk dat dit hoofdstuk zich richt op de fundamentele technische basis van Bitcoin, vooral sleutels, handtekeningen, hashing en UTXO's. Stel studenten gerust dat ze geen ingenieur hoeven te worden om de essentiële logica te begrijpen. Het hoofdstuk zelf maakt dit duidelijk door Bitcoin te vergelijken met het internet: veel mensen gebruiken het dagelijks zonder elke onderliggende laag volledig te begrijpen.

##### 8.1 Beveiliging door cryptografie, 57 minuten

**Bitcoin als een grootboek opgeslagen op veel computers**

Begin met de eenvoudige uitleg van het hoofdstuk over het Bitcoinnetwerk:

* Bitcoin is een registratie van transacties
* die registratie wordt opgeslagen op veel computers, zogenaamde nodes
* het grootboek is openbaar en pseudoniem
* het toont adressen en transactiegeschiedenis, geen persoonlijke identiteitsgegevens

Dit gedeelte helpt studenten om aan te sluiten bij wat ze al weten uit eerdere hoofdstukken. Bitcoin is niet gebaseerd op verborgen rekeningen binnen een bank. Het is gebaseerd op een gedeeld grootboek dat door veel deelnemers kan worden gecontroleerd. is hier vooral nuttig omdat het gebruikers, wallets en het bredere Bitcoinnetwerk laat zien die verbonden zijn met het openbare grootboek.

**Publieke en private sleutels**

Ga nu verder met cryptografie.

Leg uit dat elke Bitcoin-gebruiker het volgende heeft:

* een private sleutel, die geheim moet blijven
* een publieke sleutel, die gedeeld kan worden

Verduidelijk hun doel in eenvoudige bewoordingen:

* de privésleutel bewijst het bezit en autoriseert het uitgeven
* de publieke sleutel helpt anderen te verifiëren dat de transactie correct is geautoriseerd

Een belangrijk leerpunt uit het hoofdstuk is dat Bitcoin gebruikmaakt van publieke/privésleutelcryptografie, niet het oudere model waarbij twee mensen eerst hetzelfde geheime sleutel moeten delen. Dat is belangrijk omdat het veilige verificatie mogelijk maakt zonder dat gebruikers het geheim hoeven prijs te geven dat hun geld beschermt.

Je kunt het zo uitleggen:

* de privésleutel is als het geheime bewijs dat de bitcoin van jou is
* de publieke sleutel is onderdeel van wat het netwerk in staat stelt jouw autorisatie te verifiëren
* wie de privésleutel beheert, beheert de mogelijkheid om de bitcoin uit te geven

Wees hier voorzichtig om de encryptietaal niet te ingewikkeld te maken. Het belangrijkste punt voor studenten is eigendom en autorisatie.

**Digitale handtekeningen en transactie-autorisatie**

Leg nu uit wat er gebeurt als iemand bitcoin verstuurt.

Gebruik de volgorde uit het hoofdstuk:

* een gebruiker maakt een transactie aan
* de verzender genereert een digitale handtekening met zijn privésleutel
* de transactie wordt uitgezonden naar het netwerk
* nodes verifiëren of de handtekening geldig is
* na verificatie en bevestiging wordt het eigendom overgedragen op het grootboek

Maak duidelijk dat een digitale handtekening niet hetzelfde is als het typen van een naam. Het is een cryptografisch bewijs dat de echte eigenaar de transactie heeft geautoriseerd. Dit is een van de kernmechanismen waardoor Bitcoin kan werken zonder dat een centrale autoriteit transacties handmatig goedkeurt. Het diagram is nuttig omdat het het ondertekenen en verifiëren visueel toont, evenals het pad van de transactie van verzender tot netwerkvalidatie.

Een goede zin voor in de klas is:

Bitcointransacties worden niet goedgekeurd omdat een bank dat zegt. Ze worden geaccepteerd omdat het netwerk geldig cryptografisch bewijs kan verifiëren.

**Hashing en eenrichtingsfuncties**

Leg vervolgens hashing uit.

Begin eenvoudig:

* een functie neemt een invoer en produceert een uitvoer
* een eenrichtingsfunctie is makkelijk in één richting uit te voeren, maar in de praktijk onmogelijk om om te keren
* een hashfunctie neemt data van elke grootte en verandert die in een uitvoer van vaste lengte, een zogenaamde hash

Gebruik een van de analogieën uit het hoofdstuk, welke het duidelijkst is voor jouw publiek:

* de smoothie-analogie voor eenrichtingsfuncties
* de vingerafdruk-analogie voor hashes
* de bladmuziek-analogie om te controleren of iets is veranderd

De vingerafdruk-analogie is waarschijnlijk het duidelijkst voor de meeste klassen:

* een hash is als een digitale vingerafdruk voor data
* als de invoer zelfs maar een beetje verandert, verandert de hash volledig
* dit helpt computers om integriteit te controleren en knoeien te detecteren

Leg daarna uit waarom hashing belangrijk is in Bitcoin:

* transacties worden gehasht
* het netwerk gebruikt hashes om integriteit te helpen verifiëren
* als een transactie wordt veranderd, verandert de hash
* dit helpt het grootboek te beschermen tegen ongemerkte manipulatie

De afbeeldingen op pagina's 7 tot 10 zijn hier erg nuttig. Het hoofdstuk laat zowel het idee van vaste lengte als het principe van "kleine verandering, compleet ander resultaat" zien, wat een van de belangrijkste concepten is voor studenten om te begrijpen.

**Basiskenmerken van hashfuncties**

Loop kort door de eigenschappen die in het hoofdstuk worden benadrukt, zonder ze te academisch te maken:

* Deterministisch: dezelfde invoer geeft elke keer dezelfde uitvoer
* Eenrichtingsverkeer / pre-image weerstand: je kunt het proces in de praktijk niet omkeren
* Gevoelig voor verandering: zelfs een kleine verandering in de invoer geeft een heel andere uitvoer
* Botsingsbestendig: het is extreem moeilijk om twee verschillende invoeren met dezelfde uitvoer te vinden
* Snel te verifiëren: de functie is efficiënt om uit te voeren en te controleren

Studenten hoeven niet elk begrip uit het hoofd te leren, maar ze moeten het algemene punt begrijpen: hashing geeft Bitcoin een betrouwbare manier om data te identificeren en veranderingen te detecteren.

##### 8.2 Het UTXO-model, 25 minuten

**Het UTXO-model**

Ga nu verder met het tweede hoofdonderdeel van het hoofdstuk: UTXO's, oftewel Unspent Transaction Outputs (onbestede transactie-uitgangen).

Leg het eenvoudig uit met behulp van de cash-analogie uit het hoofdstuk:

* bitcoin wordt niet gevolgd als een bankrekening-saldo alleen
* in plaats daarvan bestaat het uit besteedbare stukjes die UTXO's worden genoemd
* wanneer je bitcoin uitgeeft, gebruik je een of meer bestaande UTXO's als input
* nieuwe UTXO's worden dan aangemaakt als output

Gebruik het voorbeeld uit het hoofdstuk:

* als je een UTXO van 10 BTC hebt
* en je stuurt 6 BTC
* gaat er een nieuwe UTXO van 6 BTC naar de ontvanger
* komt er een nieuwe wisselgeld-UTXO terug naar jou
* een klein deel wordt betaald als vergoeding voor de miners

Dat helpt studenten inzien dat Bitcoin meer werkt als het uitgeven van contant geld en het ontvangen van wisselgeld, dan als het aftrekken van getallen van een simpele rekening. De diagrammen zijn hier vooral sterk omdat ze visueel laten zien hoe één UTXO wordt opgesplitst in een ontvangersoutput, wisselgeldoutput en vergoeding.

Maak twee kernpunten expliciet:

* je wallet-saldo is de som van je UTXO's
* wanneer je uitgeeft, worden oude UTXO's verbruikt en nieuwe aangemaakt

**Voorkomen van dubbel uitgeven**

Sluit de inhoud af door een van de belangrijkste gevolgen van het UTXO-model uit te leggen.

Als iemand probeert om dezelfde output twee keer uit te geven, weigeren nodes de tweede poging omdat zij het grootboek bijhouden en kunnen controleren of die UTXO al is uitgegeven. Dit is hoe Bitcoin dubbel uitgeven voorkomt zonder dat er een centrale betaaldienst nodig is om de administratie te beheren. Het voorbeeld is hier erg nuttig omdat het laat zien hoe Alice UTXO's combineert, geld naar Bob stuurt, wisselgeld ontvangt en hoe de bevestigde transactie het grootboek bij alle nodes bijwerkt.

Een duidelijke manier om het in de klas te zeggen is:

Bitcoin voorkomt dubbel uitgeven omdat het netwerk bijhoudt welke outputs nog niet zijn uitgegeven en welke al gebruikt zijn.

###### Afronding en controle van begrip

Sluit af met een paar snelle vragen:

* Wat is het verschil tussen een publieke sleutel en een private sleutel?
* Wat bewijst een digitale handtekening?
* Waarom is hashen nuttig in Bitcoin?
* Wat gebeurt er als een transactie wordt gewijzigd nadat deze is gehasht?
* Wat is een UTXO in eenvoudige bewoordingen?
* Hoe voorkomt het netwerk dat iemand dezelfde bitcoin twee keer uitgeeft?

#### Aantekeningen voor docenten

Dit hoofdstuk bevat meer technische taal dan eerdere, dus geef prioriteit aan duidelijkheid, analogieën en herhaling.

Het doel is niet om studenten tot ontwikkelaars te maken. Het doel is om ze te laten begrijpen waarom de beveiliging van Bitcoin werkt.

De belangrijkste punten om te benadrukken als de tijd kort is, zijn:

* private key versus public key
* digitale handtekeningen
* wat hashen doet
* UTXO's als besteedbare stukjes bitcoin
* hoe dubbel uitgeven wordt voorkomen

De meest bruikbare visuals in dit hoofdstuk zijn:

* het gebruiker-wallet-netwerkdiagram
* de visualisatie van de digitale handtekening
* de hash-voorbeelden en diagrammen van vaste lengte op pagina's 7 tot 10
* de UTXO-diagrammen op pagina's 10 tot 12

##### Hoe ziet goed onderwijs eruit

* Het is belangrijk om cryptografie te behandelen als een fundament en geen mysterie, veel visuals te gebruiken, diepe wiskunde te vermijden, terug te koppelen naar eerdere hoofdstukken en het begrip te testen met toepassingen zoals "Als iemand één transactie verandert, wat gaat er dan mis?"
* Docenten moeten geduldig zijn met studenten die moeite hebben, visueel denken en alles tekenen, eerlijk zijn over wat studenten niet hoeven te begrijpen, bereid zijn te zeggen "Ik weet het niet, maar zo zouden we het uitzoeken," en gedurende het hele proces bemoedigend blijven.
* Studenten begrijpen waarom Bitcoin niet gehackt kan worden omdat het beschermd wordt door wiskunde, respecteren het elegante ontwerp van het systeem, voelen zich comfortabel met complexiteit wetende dat ze niet elk detail hoeven te kennen, krijgen vertrouwen om vragen te stellen zonder oordeel, en herkennen dat ze een hoger niveau van begrip hebben bereikt dan de meeste mensen.
* Leerdoelen zijn behaald als studenten cryptografie-basisprincipes zoals eenrichtingsfuncties en digitale handtekeningen kunnen uitleggen zonder diepe wiskunde, het UTXO-model begrijpen waarbij je munten bezit en geen rekeningen, hashen herkennen als de basis van Bitcoins beveiliging, de anatomie van transacties begrijpen inclusief handtekeningen en bevestigingen, kunnen uitleggen waarom Bitcoin onveranderlijk is, en kritische vragen kunnen stellen over mogelijke aanvallen of kwetsbaarheden.

##### Tijdmanagement

Als de tijd kort is, prioriteer dan:

* Privésleutel versus publieke sleutel
* Digitale handtekeningen
* Wat hashing doet
* UTXO's als besteedbare stukjes bitcoin
* Hoe dubbel uitgeven wordt voorkomen

Als je voorloopt, neem dan de tijd voor:

* Gebruiker-portemonnee-netwerkdiagram en visueel beveiligingsmodel
* Digitale handtekening visueel: gedetailleerd cryptografisch proces
* Merkle-bomen en ketenbeveiliging
* Geavanceerde aanvalsvectoren en waarom ze falen

##### Als studenten moeite hebben

* Cryptografie als bedreigend → "Je gebruikt het dagelijks; Bitcoin gebruikt het op dezelfde manier."
* Hashing als concept → Vingerafdruk-analogie; uniek, kan niet veranderen zonder hash-verandering.
* Digitale handtekeningen → "Bewijst autorisatie zonder wachtwoord te onthullen."
