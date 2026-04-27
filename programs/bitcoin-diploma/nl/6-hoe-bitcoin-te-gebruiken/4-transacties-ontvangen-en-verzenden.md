# 6.4 Transacties ontvangen en verzenden

Een Bitcoin-transactie is een overdracht van eigendom van bitcoin naar een nieuwe eigenaar. Let op: het zijn niet de daadwerkelijke munten die worden overgedragen, maar het eigendom ervan: met andere woorden, het recht om ze uit te geven. Elke keer dat een transactie wordt geaccepteerd in een blok, werken alle knooppunten in het netwerk hun lokale kopie van het openbare grootboek bij om de verandering van eigendom weer te geven. In dit opzicht lijkt een Bitcoin-transactie meer op een vastgoed- (of andere eigendoms-)transactie dan op een contante transactie.

Om bitcoin te "versturen" ondertekent de verzender een bericht met zijn privésleutel, waarmee hij aan het netwerk aangeeft dat de rechtmatige eigenaar van de bitcoin het eigendom heeft overgedragen aan de ontvanger.

De bitcoin zal nu gekoppeld zijn aan het adres van de ontvanger, waardoor deze het eigendom krijgt over de bitcoin, zodat alleen de nieuwe eigenaar ze kan uitgeven met zijn of haar privésleutel.

Nieuwe Bitcoin-transacties worden overal ter wereld vanuit wallets gestart, maar er is geen centrale betalingsverwerker. In plaats daarvan strijden miners om transacties in het grootboek vast te leggen.

Stel, Jan is Eliana 0,5 BTC schuldig en is klaar om haar terug te betalen. Beiden hebben digitale wallets.

1. Eliana deelt haar adres met Jan.
1. Jan gebruikt zijn wallet-software om de transactie aan te maken, waarin Eliana’s adres, het over te maken bedrag (0,5 BTC) en een vergoeding voor de miner worden opgenomen. Hogere vergoedingen vergroten de kans dat een miner de transactie in het volgende blok opneemt.
1. Na het ondertekenen van de transactie wordt deze uitgezonden naar het netwerk, waar deze wordt geverifieerd door knooppunten. Zij controleren of Jan voldoende saldo heeft en de rechtmatige eigenaar is van de munten die hij wil uitgeven. Als dat niet zo is, wordt de transactie direct afgewezen.
1. Zodra de transactie is geverifieerd, kiezen miners of ze de transactie aan het volgende blok toevoegen, meestal op basis van de gekozen vergoeding. Zodra de transactie in een blok terechtkomt, wordt deze toegevoegd aan de blockchain en worden de fondsen overgemaakt naar Eliana's adres.
1. Het eigendom is overgedragen aan Eliana. Zij kan nu haar privésleutel gebruiken om de fondsen uit te geven.

_Het is belangrijk om te weten dat zodra de transactie is voltooid, deze niet kan worden teruggedraaid._


> **Note – Hoe een Bitcoin-transactie werkt**
>
> 1. Iemand vraagt een transactie aan
> 1. Transactie wordt uitgezonden naar P2P-computers (knooppunten)
> 1. Miners verifiëren de transactie
> 1. Transacties worden gecombineerd tot een datablock
> 1. Nieuw blok toegevoegd aan de bestaande blockchain
> 1. De transactie is voltooid



> **Note – Bitcoin-transacties ontvangen**
>
> Om bitcoin te ontvangen, moet je de verzender een Bitcoin-publiek adres geven. Dit is een unieke reeks letters en cijfers die je wallet vertegenwoordigt en wordt gebruikt om deze te identificeren op het Bitcoin-netwerk.
>
> Je kunt je publieke adres vinden door je Bitcoin-wallet te openen en te zoeken naar een optie om bitcoin te “Ontvangen” of te “Storten”.
>
> Je kunt je Bitcoin-adres vervolgens op een van de volgende manieren delen:
>
> 1. **Kopieer en plak het adres**: Je kunt het adres kopiëren door het te selecteren en op "Kopiëren" te drukken, en het vervolgens te plakken in een e-mail of bericht.
> 1. **Deel een link naar je Bitcoin-wallet**: Sommige Bitcoin-wallets laten je een link naar je wallet aanmaken die je met de verzender kunt delen. Zij kunnen dan op de link klikken om toegang te krijgen tot je wallet en bitcoin te versturen.
> 1. **Deel een QR-code**: Als de verzender een smartphone met een Bitcoin-wallet app heeft, kan hij of zij de QR-code scannen om jouw Bitcoin-adres te krijgen.


Zodra de verzender jouw adres heeft, kan hij of zij je bitcoin sturen door jouw adres en het gewenste bedrag in te voeren. De bitcoin wordt dan van hun wallet naar jouw wallet gestuurd.

De transactie wordt bevestigd door het Bitcoin-netwerk en duurt meestal ongeveer 10 minuten. Voor extra veiligheid wordt aanbevolen om te wachten op twee bevestigingen, wat ongeveer 20 minuten duurt.


> **Note – Bitcoin-transacties versturen**
>
> Om bitcoin te versturen heb je een paar dingen nodig: een Bitcoin-wallet, het publieke adres van de ontvanger en het bedrag aan bitcoin dat je wilt versturen.
>
> 1. Open je Bitcoin-wallet.
> 1. Navigeer naar de knop “Versturen” en plak het adres van de ontvanger in het veld "Aan". Je kunt eventueel ook de QR-code scannen als de ontvanger die heeft gegeven.
> 1. Voer het bedrag aan bitcoin in dat je wilt versturen in het veld “Bedrag”.
> 1. Controleer het adres van de ontvanger en het te versturen bedrag goed. Onthoud: transacties zijn onomkeerbaar!
> 1. Voordat je op “Bevestigen en Versturen” klikt, raden we aan om de transactiegegevens nog één keer goed te controleren om zeker te zijn dat je het juiste bedrag naar het juiste adres stuurt.
> 1. Zend de transactie uit en wacht tot het netwerk de transactie bevestigt.
>
> Nu weet je hoe je een zelfbewaarde Bitcoin-wallet kunt beoordelen, selecteren en instellen. Het versturen en ontvangen van bitcoin op het Bitcoin-netwerk wordt “on-chain” transacties genoemd. Dit komt omdat de transacties plaatsvinden op het hoofdnetwerk van Bitcoin en worden vastgelegd in de blockchain.
>
> On-chain transacties zijn de veiligste manier om met bitcoin te handelen vanwege de gedecentraliseerde verificatie door het netwerk.
>
> On-chain transacties zijn echter trager en kunnen aanzienlijk duurder zijn dan andere opties (waar we het over zullen hebben in Module 7) vanwege de vergoeding voor de miner.


#### Activiteit: Transacties in de praktijk

https://qr.myfirstbitcoin.org/transactions.pdf

**Dit is een samenwerkingsopdracht die de basisrollen van mensen in een Bitcoin-transactie vereenvoudigt.**

###### Belangrijkste punten

1. Er zijn vier soorten deelnemers bij elke bitcoin-transactie: de verzender, de ontvanger, de miners en de knooppuntbeheerders.
1. De verzender moet goedkeuren (cryptografisch ondertekenen) het **bedrag aan bitcoin** om te versturen EN het **specifieke adres** om naar te versturen.
1. De ontvanger moet een **geldig adres** aan de verzender geven EN controleren of de transactie succesvol is bevestigd op de blockchain.
1. Miners zorgen ervoor dat aan alle criteria is voldaan voordat ze transacties aan toekomstige blokken toevoegen.
1. Node-operators controleren of gemijnde blokken geldig zijn voordat ze hun versie van de blockchain (het grootboek) bijwerken.

###### Tip voor studenten

Draai door alle vier de rollen om te ervaren wat elke deelnemer doet.
