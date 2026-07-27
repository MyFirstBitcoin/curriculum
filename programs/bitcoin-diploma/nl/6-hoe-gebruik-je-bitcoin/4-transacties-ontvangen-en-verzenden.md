# 6.4 Transacties ontvangen en verzenden

Een Bitcoin-transactie is een overdracht van het eigendom van bitcoins aan een nieuwe eigenaar. Let wel: het zijn niet de daadwerkelijke munten die worden overgedragen, maar het eigendom ervan: met andere woorden, het recht om ze uit te geven. Telkens wanneer een transactie in een blok wordt opgenomen, werken alle knooppunten in het netwerk hun lokale kopie van het openbare grootboek bij om de eigendomsoverdracht weer te geven. In dit opzicht lijkt een Bitcoin-transactie meer op een transactie in onroerend goed (of andere eigendommen) dan op een contante transactie.

Om bitcoin te „verzenden”, ondertekent de afzender een bericht met zijn privésleutel, waarmee hij aan het netwerk aangeeft dat de rechtmatige eigenaar van de bitcoin het eigendom ervan aan de ontvanger heeft overgedragen.

De bitcoin wordt nu gekoppeld aan het adres van de ontvanger, waardoor deze eigenaar wordt van de bitcoin, zodat alleen de nieuwe eigenaar deze kan uitgeven met behulp van zijn privésleutel.

Nieuwe Bitcoin-transacties worden geïnitieerd vanuit wallets over de hele wereld, maar er is geen centrale betalingsverwerker. In plaats daarvan concurreren miners met elkaar om transacties in het grootboek vast te leggen.

Stel dat Jim Eliana 0,5 BTC verschuldigd is en bereid is om haar terug te betalen. Beiden hebben een digitale portemonnee.

1. Eliana geeft haar adres aan Jim.
1. Jim gebruikt zijn wallet-software om de transactie aan te maken, waarin het adres van Eliana, het over te maken bedrag (0,5 BTC) en een vergoeding voor de miner zijn opgenomen. Hoe hoger de vergoeding, hoe groter de kans dat een miner de transactie in het volgende blok opneemt.
1. Nadat de transactie is ondertekend, wordt deze naar het netwerk verzonden, waar ze door de knooppunten wordt geverifieerd. Zij controleren of Jim over voldoende saldo beschikt en de rechtmatige eigenaar is van de munten die hij wil uitgeven. Als dat niet het geval is, wordt de transactie onmiddellijk afgewezen.
1. Zodra de transactie is geverifieerd, beslissen miners of ze de transactie aan het volgende blok toevoegen, meestal op basis van de gekozen vergoeding. Zodra de transactie in een blok is opgenomen, wordt deze aan de blockchain toegevoegd en wordt het geld overgemaakt naar het adres van Eliana.
1. Het eigendom is overgedragen aan Eliana. Ze kan nu haar privésleutel gebruiken om het geld uit te geven.

_Het is belangrijk om te weten dat de transactie, zodra deze is voltooid, niet meer ongedaan kan worden gemaakt._

###### Hoe een Bitcoin-transactie werkt

1. De transactie wordt naar het netwerk verzonden
1. Mijnwerkers bundelen transacties in een blok
1. Het blok wordt aan de blockchain toegevoegd
1. De transactie is bevestigd


> **Light – Bitcoin-transacties ontvangen**
>
> Om bitcoin te ontvangen, moet je de afzender een openbaar Bitcoin-adres geven. Dit is een unieke reeks letters en cijfers die je wallet vertegenwoordigt en die wordt gebruikt om deze op het Bitcoin-netwerk te identificeren.
>
> Je kunt je openbare adres vinden door je Bitcoin-portemonnee te openen en te zoeken naar een optie om bitcoin te ‘ontvangen’ of te ‘storten’.
>
> Je kunt je Bitcoin-adres vervolgens op verschillende manieren delen:
>
> 1. **Kopieer en plak het adres**: Je kunt het adres kopiëren door het te markeren en op "Kopiëren" te klikken; vervolgens kun je het in een e-mail of bericht plakken.
> 1. **Deel een link naar je Bitcoin-portemonnee**: Bij sommige Bitcoin-wallets kun je een link naar je wallet aanmaken die je met de afzender kunt delen. Die kan dan op de link klikken om toegang te krijgen tot je wallet en bitcoin te versturen.
> 1. **Een QR-code delen**: Als de afzender een smartphone heeft waarop een Bitcoin-wallet-app is geïnstalleerd, kan hij of zij de QR-code scannen om je Bitcoin-adres te verkrijgen.


Zodra de afzender je adres heeft, kan hij of zij je bitcoin sturen door je adres en het bedrag dat hij of zij wil sturen in te voeren. De bitcoin wordt vervolgens vanuit zijn of haar portemonnee naar jouw portemonnee gestuurd.

De transactie wordt door het Bitcoin-netwerk bevestigd en duurt doorgaans ongeveer 10 minuten. Voor extra veiligheid wordt aangeraden om te wachten tot er twee bevestigingen zijn, wat ongeveer 20 minuten duurt.


> **Light – Bitcoin-transacties verzenden**
>
> Om bitcoin te versturen, heb je een aantal dingen nodig: een Bitcoin-wallet, het openbare adres van de ontvanger en het bedrag aan bitcoin dat je wilt versturen.
>
> 1. Open je Bitcoin-portemonnee.
> 1. Ga naar de knop ‘Verzenden’ en plak het adres van de ontvanger in het veld ‘Aan’. Je kunt ook de QR-code scannen als de ontvanger die heeft verstrekt.
> 1. Voer het bedrag aan bitcoin dat u wilt versturen in het veld „Bedrag“ in.
> 1. Controleer nogmaals het adres van de ontvanger en het over te maken bedrag. Vergeet niet dat transacties onomkeerbaar zijn!
> 1. Voordat u op ‘Bevestigen en verzenden’ klikt, raden wij u aan de transactiegegevens nogmaals goed te controleren om er zeker van te zijn dat u het juiste bedrag aan bitcoin naar het juiste adres verstuurt.
> 1. Verzend de transactie en wacht tot het netwerk de transactie bevestigt.
>
> Nu weet je hoe je een Bitcoin-wallet met eigen beheer kunt beoordelen, kiezen en instellen. Het verzenden en ontvangen van bitcoin via het Bitcoin-netwerk wordt aangeduid als ‘on-chain’-transacties. Dit komt doordat de transacties plaatsvinden op het hoofdnetwerk van Bitcoin en worden vastgelegd in de blockchain.
>
> Transacties op de blockchain zijn de veiligste manier om met bitcoin te handelen, dankzij de gedecentraliseerde verificatie die door het netwerk wordt geboden.
>
> Transacties op de blockchain verlopen echter trager en kunnen aanzienlijk duurder zijn dan andere opties (die we in module 7 zullen bespreken) vanwege de miner-vergoeding.


#### Activiteit: Transacties in de praktijk


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Dit is een gezamenlijke oefening waarin de basisrollen van de betrokkenen bij een Bitcoin-transactie worden vereenvoudigd.**

###### Belangrijkste punten

1. Bij elke bitcointransactie zijn er vier soorten deelnemers: de afzender, de ontvanger, miners en knooppuntbeheerders.
1. De afzender moet het volgende goedkeuren (cryptografisch ondertekenen): **hoeveelheid bitcoin** om te verzenden EN de **specifiek adres** naar wie het moet worden verzonden.
1. De ontvanger moet een **geldig adres** naar de afzender EN controleren of de transactie met succes is bevestigd op de blockchain.
1. Mijnwerkers controleren of aan alle criteria is voldaan voordat ze transacties aan toekomstige blokken toevoegen.
1. Knooppuntbeheerders controleren of de geminde blokken geldig zijn voordat ze hun versie van de blockchain (het grootboek) bijwerken.

###### Tip voor studenten

Wissel de vier rollen af om te ervaren wat elke deelnemer doet.
