# 9.1 Bitcoin-nodes en miners

Bitcoin-nodes klinken misschien technisch, maar het zijn simpelweg programma’s die een kopie van de Bitcoin-blockchain op een computer bewaren. De blockchain is een gedeeld register van alle Bitcoin-transacties.

Wanneer je je eigen node draait, verifieer je Bitcoin-transacties zelf in plaats van iemand anders te vertrouwen. Dit geeft je meer onafhankelijkheid en helpt het Bitcoin-netwerk gedecentraliseerd te houden.

Je kunt een Bitcoin-node zien als een digitale verkeersagent met een paar belangrijke taken.

1. Het bewaart een kopie van de blockchain, oftewel de geschiedenis van alle Bitcoin-transacties.
1. Nodes verbinden met andere nodes over de hele wereld en delen informatie. Een voorbeeld hiervan is de lijst met nieuwe transacties die wachten op bevestiging, ook wel de mempool genoemd.
1. Nodes controleren of elke transactie voldoet aan de regels van Bitcoin. Als een transactie ongeldig is, wijst de node deze af.

Nodes helpen ook nieuwe nodes om zich bij het netwerk aan te sluiten door de blockchain met hen te delen. Elke nieuwe node controleert echter alsnog alle regels zelfstandig.

Iedereen kan een node draaien door software zoals Bitcoin Core te installeren en de blockchain te downloaden. Zodra deze is ingesteld, ontvangt de node ongeveer elke 10 minuten nieuwe blokken en verifieert deze voordat ze aan zijn kopie van de blockchain worden toegevoegd.

Het draaien van een node helpt het Bitcoin-netwerk veiliger en gedecentraliseerder te maken, omdat meer mensen het systeem onafhankelijk verifiëren.

#### Wat is een Bitcoin-node?

> Het doel van mining is niet het creëren van nieuwe bitcoin; dat is het beloningssysteem. Mining is het mechanisme waarmee de beveiliging van Bitcoin wordt gedecentraliseerd.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Miners verzamelen onbevestigde transacties, vormen een blok en gebruiken energie om een sleutel te vinden die het blok toevoegt en beveiligt.


Miners strijden om het volgende blok transacties aan de blockchain toe te voegen. Hiervoor moeten ze een speciaal getal vinden dat een geldige blok-hash oplevert. Je kunt het je voorstellen als het zoeken naar de juiste sleutel tussen miljarden mogelijkheden. De eerste miner die de juiste hash vindt, wint de race en krijgt het recht om zijn blok aan de blockchain toe te voegen.

Wanneer een miner een geldige hash vindt, deelt hij zijn blok met het netwerk. Andere miners controleren snel of de oplossing klopt. Als dat zo is, wordt het blok aan de blockchain toegevoegd, wat helpt om het openbare grootboek van Bitcoin veilig te houden.

Miners verdienen bitcoin op twee manieren:

* **Blokbeloningen:** Nieuwe bitcoin worden gecreëerd en gegeven aan de miner die succesvol een blok aan de blockchain toevoegt.
* **Transactiekosten:** Wanneer mensen bitcoin versturen, voegen ze een kleine vergoeding toe. De miner die het blok toevoegt ontvangt de vergoedingen van de transacties die in dat blok zijn opgenomen.

#### Bitcoin-halveringen


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Info**
>
> De beloningen voor miners voor het voltooien van één blok halveren elke 210.000 blokken, ongeveer elke vier jaar.


Bitcoin heeft een maximale vaste voorraad van 21.000.000 bitcoin, maar ze zijn niet allemaal gecreëerd toen Bitcoin begon. In plaats daarvan worden nieuwe bitcoin geleidelijk in omloop gebracht via **mining**.

Wanneer miners met succes een nieuw blok transacties aan het Bitcoin-netwerk toevoegen, ontvangen ze een **blokbeloning** in bitcoin. In de beginjaren van Bitcoin was deze beloning 50 bitcoin per blok. Deze beloning moedigde mensen aan om rekenkracht en elektriciteit te gebruiken om het netwerk te beveiligen.

Ongeveer elke 210.000 blokken (ongeveer elke 4 jaar) wordt de blokbeloning gehalveerd. Dit evenement heet de **halvering**. De halvering vertraagt de creatie van nieuwe bitcoin en helpt ervoor te zorgen dat het totale aanbod nooit meer dan 21 miljoen zal zijn. Na verloop van tijd maakt dit bitcoin steeds schaarser.


> **Definition – Circulerend aanbod**
>
> **Circulerend aanbod** verwijst naar de totale beschikbare hoeveelheid van een valuta. Bij Bitcoin is het totale circulerende aanbod het aantal munten dat is gemined en op elk moment in omloop is.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/9f32eb028a622db06db1c92a9f866c5f558dfeb8-292x200.svg)


> **Definition – Bitcoin-aanbodschema**
>
> Het **Bitcoin-aanbodschema** is het vooraf bepaalde en openbare plan voor de uitgifte van nieuwe bitcoin in omloop, ontworpen om de schaarste van Bitcoin in de loop van de tijd te behouden.


Na elke halvering wordt de bitcoin-beloning die miners ontvangen voor het toevoegen van een blok gehalveerd. Dit vermindert het tempo waarmee nieuwe bitcoins worden gecreëerd.

Miners verdienen nog steeds transactiekosten van de transacties die in het blok dat ze minen zijn opgenomen. Na verloop van tijd wordt verwacht dat deze kosten een groter deel van het inkomen van miners zullen vormen.

Halvings zijn ingebouwd in het Bitcoin-protocol en vinden automatisch ongeveer elke vier jaar plaats. Hierdoor is het uitgifteschema van Bitcoin voorspelbaar en transparant.

De tabel toont de aankomende halvings, inclusief de geschatte datum, het bloknummer waarop ze plaatsvinden, de nieuwe blokbeloning en het percentage van de totale bitcoinvoorraad dat dan gemijnd zal zijn.


| Gebeurtenis | Datum | Blok | Beloning | Gemijnd |
| --- | --- | --- | --- | --- |
| 5e Halving | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| 6e Halving | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| 7e Halving | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Naarmate er meer bitcoin worden gemijnd, blijft de circulerende voorraad toenemen totdat het maximum van 21.000.000 bitcoins is bereikt, wat rond het jaar 2140 wordt verwacht. Omdat er na verloop van tijd minder nieuwe bitcoins worden gecreëerd, kan de prijs van Bitcoin stijgen als de vraag toeneemt. Dit stimuleert ook miners om het netwerk te blijven beveiligen door hun rekenkracht bij te dragen.

#### Wat is een geldige blokhash in Bitcoin?

In Bitcoin strijden miners om een speciale code te vinden, genaamd een **blokhash**. Deze code identificeert een blok met transacties en maakt het mogelijk om het toe te voegen aan de blockchain.

Elk blok bevat informatie over recente transacties en bevat ook de hash van het vorige blok. Dit verbindt elk blok met elkaar, waardoor er een keten ontstaat van het allereerste blok (het Genesis-blok) tot het meest recente blok.

Een hash werkt als een **digitale vingerafdruk** voor de gegevens in het blok. Als er iets in het blok wordt gewijzigd, verandert de vingerafdruk ook. Dit maakt het eenvoudig voor iedereen om te controleren dat de transactiegeschiedenis van de blockchain niet is aangepast en helpt het netwerk veilig te houden.


> **Callout**
>
> Satoshi Nakamoto, de bedenker van Bitcoin, heeft het Genesis-blok gemijnd, waarmee in totaal 50 bitcoin werden vrijgegeven.


#### De race om een blok te minen

Miners strijden om een geldige blokhash te vinden. De eerste miner die er een vindt, mag het nieuwe blok aan de blockchain toevoegen en ontvangt een bitcoinbeloning.

Om geldig te zijn, moet de hash van het blok lager zijn dan een getal dat door het netwerk is vastgesteld, de zogenaamde moeilijkheidsdoelstelling. Omdat hashes willekeurig zijn, moeten miners steeds verschillende invoer proberen totdat ze er een vinden die werkt.

Als er te veel miners meedoen, zouden blokken te snel worden gevonden. Als er te weinig miners zijn, zou het te lang duren om blokken te vinden. Om het systeem soepel te laten verlopen, past Bitcoin de moeilijkheidsgraad automatisch aan elke 2.016 blokken (ongeveer elke twee weken).

Deze aanpassing zorgt ervoor dat er gemiddeld ongeveer elke 10 minuten een nieuw blok aan de blockchain wordt toegevoegd.


> **Definition – Definitie van moeilijkheidsgraad**
>
> De **moeilijkheidsgraad** bij het minen van Bitcoin geeft aan hoe moeilijk het is om een geldige blokhash te vinden. Het netwerk past deze moeilijkheidsgraad elke 2.016 blokken aan (ongeveer elke twee weken), zodat er ongeveer elke 10 minuten een nieuw blok aan de blockchain wordt toegevoegd. Hoe hoger de moeilijkheidsgraad, hoe moeilijker het is voor miners om een geldig blok te vinden.



> **Info**
>
> Door een geldige blokhash te vinden, bewijst een miner dat hij het vereiste werk heeft verricht om een nieuw blok aan de blockchain toe te voegen. Dit proces heet Proof of Work (PoW). Het is het beveiligingsmechanisme waarmee Bitcoin transacties kan bevestigen en nieuwe blokken aan de blockchain kan toevoegen. De miner die als eerste de geldige hash vindt, verdient een beloning in bitcoin, bestaande uit de blokbeloning en de transactiekosten van de transacties in dat blok.


Proof of Work (PoW) helpt Bitcoin veilig te houden door het extreem duur te maken voor iemand om te proberen te valsspelen of het netwerk over te nemen. Het is veel winstgevender om de regels te volgen.

Miners vervullen vier hoofdrollen:

1. **Transacties verzamelen**: Miners kiezen transacties die naar het netwerk zijn verzonden en plaatsen deze in een kandidaatblok.
1. **Proof of Work uitvoeren**: Miners strijden om een moeilijke wiskundige puzzel op te lossen door een geldige blokhash te vinden.
1. **Het blok uitzenden**: De eerste miner die een geldige oplossing vindt, deelt het nieuwe blok met het netwerk.
1. **Verdien beloningen**: Als het blok geldig is, wordt het toegevoegd aan de blockchain en ontvangt de miner nieuw gecreëerde bitcoin plus transactiekosten.

Veel miners over de hele wereld proberen tegelijkertijd het volgende blok te maken. Wanneer één miner een geldige oplossing vindt, controleert het netwerk het blok. Als alles klopt, wordt het toegevoegd aan de blockchain. Andere concurrerende blokken worden verworpen. Dit proces houdt het netwerk in overeenstemming en voorkomt dubbele uitgaven.

* Miners zijn computers die helpen om het grootboek van Bitcoin te onderhouden en bij te werken.
* Ze verzamelen transacties en groeperen deze in een blok. Vervolgens halen ze de gegevens van het blok door een hash-algoritme om een unieke code te maken, een zogenaamde hash.
* Miners herhalen dit proces vele malen, op zoek naar een hash die voldoet aan de regels van Bitcoin. De eerste miner die een geldige hash vindt, krijgt nieuw gecreëerde bitcoin als beloning en hun blok wordt toegevoegd aan de blockchain.
* De hash van elk blok verbindt het ook met het vorige blok. Als iemand zou proberen een eerdere transactie te wijzigen, zouden de hashes niet meer overeenkomen en zou het netwerk de gewijzigde keten afwijzen. Dit is wat het grootboek van Bitcoin veilig houdt.
