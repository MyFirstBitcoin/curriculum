# 9.1 Bitcoin-knooppunten en miners

Wat is een Bitcoin-node?  
Bitcoin-nodes klinken misschien technisch, maar het is simpelweg software die een kopie van de Bitcoin-blockchain op een computer bewaart. De blockchain is een gedeeld register van alle Bitcoin-transacties.

Wanneer je je eigen node draait, verifieer je Bitcoin-transacties zelf in plaats van op iemand anders te vertrouwen. Dit geeft je meer onafhankelijkheid en draagt ertoe bij dat het Bitcoin-netwerk gedecentraliseerd blijft.

Je kunt een Bitcoin-node zien als een digitale verkeersagent met een aantal belangrijke taken.

1. Het bewaart een kopie van de blockchain, oftewel de geschiedenis van alle Bitcoin-transacties.
1. Knooppunten staan in verbinding met andere knooppunten over de hele wereld en wisselen informatie uit. Een voorbeeld hiervan is de lijst met nieuwe transacties die wachten op bevestiging, ook wel de mempool genoemd.
1. Knooppunten controleren of elke transactie voldoet aan de regels van Bitcoin. Als een transactie ongeldig is, wijst het knooppunt deze af.

Knooppunten helpen ook nieuwe knooppunten om zich bij het netwerk aan te sluiten door de blockchain met hen te delen. Elk nieuw knooppunt controleert echter nog steeds zelfstandig alle regels.

Iedereen kan een node draaien door software zoals Bitcoin Core te installeren en de blockchain te downloaden. Zodra de node is ingesteld, blijft deze ongeveer elke 10 minuten nieuwe blokken ontvangen en controleert deze voordat ze aan zijn kopie van de blockchain worden toegevoegd.

Door een node te draaien draag je bij aan een veiliger en meer gedecentraliseerd Bitcoin-netwerk, omdat meer mensen het systeem onafhankelijk van elkaar verifiëren.

#### Wat is een Bitcoin-miner?

> Het doel van mining is niet het creëren van nieuwe bitcoins; dat is het stimuleringssysteem. Mining is het mechanisme waarmee de beveiliging van Bitcoin gedecentraliseerd wordt.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Mijnwerkers verzamelen onbevestigde transacties, vormen daaruit een blok en gebruiken energie om een sleutel te vinden waarmee het blok wordt toegevoegd en beveiligd.


Miners strijden om het volgende blok met transacties aan de blockchain toe te voegen. Hiervoor moeten ze een speciaal getal vinden waarmee een geldige blokhash kan worden gegenereerd. Je kunt het vergelijken met het zoeken naar de juiste sleutel uit miljarden mogelijkheden. De eerste miner die de juiste hash vindt, wint de race en verdient het recht om zijn blok aan de blockchain toe te voegen.

Wanneer een miner een geldige hash vindt, deelt hij zijn blok met het netwerk. Andere miners controleren snel of de oplossing correct is. Als dat het geval is, wordt het blok aan de blockchain toegevoegd, wat bijdraagt aan de beveiliging van het openbare grootboek van Bitcoin.

Mijnwerkers verdienen bitcoin op twee manieren:

* **Blokbeloningen:** Er worden nieuwe bitcoins gecreëerd en toegekend aan de miner die met succes een blok aan de blockchain toevoegt.
* **Transactiekosten:** Wanneer mensen bitcoin versturen, voegen ze een kleine vergoeding toe. De miner die het blok toevoegt, ontvangt de vergoedingen van de transacties die in dat blok zijn opgenomen.

#### Bitcoin-halveringen


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> De beloning voor miners voor het voltooien van één blok wordt elke 210.000 blokken gehalveerd, wat neerkomt op ongeveer eens in de vier jaar.


Bitcoin heeft een vast maximumaanbod van 21.000.000 bitcoin, maar deze zijn niet allemaal meteen bij de start van Bitcoin in omloop gebracht. In plaats daarvan worden er geleidelijk nieuwe bitcoin in omloop gebracht via **mijnbouw**.

Wanneer miners erin slagen een nieuw blok met transacties aan het Bitcoin-netwerk toe te voegen, ontvangen ze een **blokbeloning** in bitcoin. In de beginperiode van Bitcoin bedroeg deze beloning 50 bitcoin per blok. Deze beloning stimuleerde mensen om rekenkracht en elektriciteit in te zetten om het netwerk te beveiligen.

Om de 210.000 blokken (ongeveer om de 4 jaar) wordt de blokbeloning gehalveerd. Dit wordt de **halvering**. Door de halvering wordt de uitgifte van nieuwe bitcoins vertraagd en wordt ervoor gezorgd dat het totale aanbod nooit hoger zal zijn dan 21 miljoen. Hierdoor wordt bitcoin in de loop van de tijd steeds schaarser.


> **Definition – Circulerend aanbod**
>
> **Circulerend aanbod** verwijst naar de totale beschikbare hoeveelheid van een valuta. Bij Bitcoin is de totale hoeveelheid in omloop het aantal munten dat is gemined en op een bepaald moment in omloop is.



<!-- micrographic: bitcoin-supply-schedule -->



> **Definition – Schema voor de uitgifte van bitcoins**
>
> De **Schema voor de uitgifte van bitcoins** is het vooraf vastgestelde en openbare plan voor het in omloop brengen van nieuwe bitcoins, dat bedoeld is om de schaarste van Bitcoin op de lange termijn te handhaven.


Na elke halvering wordt de bitcoin-beloning die miners ontvangen voor het toevoegen van een blok gehalveerd. Hierdoor neemt de snelheid waarmee nieuwe bitcoins worden gecreëerd af.

Miners verdienen nog steeds transactiekosten aan de transacties die zijn opgenomen in het blok dat zij minen. Na verloop van tijd zullen deze kosten naar verwachting een groter deel van de inkomsten van miners gaan uitmaken.

Halvings zijn ingebouwd in het Bitcoin-protocol en vinden ongeveer om de vier jaar automatisch plaats. Hierdoor is het aanbodschema van Bitcoin voorspelbaar en transparant.

De tabel toont de komende halveringen, inclusief de geschatte datum, het bloknummer waarop ze plaatsvinden, de nieuwe blokbeloning en het percentage van de totale bitcoinvoorraad dat dan gemined zal zijn.


| Evenement | Datum | Blok | Beloning | Gewonnen |
| --- | --- | --- | --- | --- |
| 5e halvering | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| 6e halvering | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| 7e halvering | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Naarmate er meer bitcoins worden gemined, blijft het aanbod in omloop toenemen totdat het maximale aanbod van 21.000.000 bitcoins is bereikt, wat naar verwachting rond het jaar 2140 zal gebeuren. Omdat er in de loop van de tijd steeds minder nieuwe bitcoins worden gecreëerd, kan de prijs van Bitcoin stijgen als de vraag toeneemt. Dit stimuleert miners ook om het netwerk te blijven beveiligen door hun rekenkracht in te zetten.

#### Wat is een geldige blokhash in Bitcoin?

Mijnwerkers strijden om een speciale code te vinden die een **blokhash**. Deze code identificeert een reeks transacties en zorgt ervoor dat deze aan de blockchain kan worden toegevoegd.

Elk blok bevat informatie over recente transacties en bevat tevens de hash van het voorgaande blok. Hierdoor zijn alle blokken met elkaar verbonden, waardoor een keten ontstaat die loopt van het allereerste blok (het Genesis-blok) tot het meest recente blok.

Een hash werkt als een **digitale vingerafdruk** voor de gegevens in het blok. Als er informatie in het blok zou worden gewijzigd, zou ook de vingerafdruk veranderen. Hierdoor kan iedereen eenvoudig controleren of de transactiegeschiedenis van de blockchain niet is gewijzigd, wat bijdraagt aan de veiligheid van het netwerk.


> **Callout**
>
> Satoshi Nakamoto, de bedenker van Bitcoin, heeft het Genesis-blok gemined, waardoor in totaal 50 bitcoin vrijgekomen zijn.


#### De race om een blok te minen

Miners strijden om een geldige blokhash te vinden. De eerste miner die er een vindt, mag het nieuwe blok aan de blockchain toevoegen en ontvangt een beloning in bitcoins.

Om geldig te zijn, moet de hash van het blok lager zijn dan een door het netwerk vastgesteld getal, de zogenaamde moeilijkheidsdoelstelling. Omdat hashes willekeurig zijn, moeten miners verschillende invoergegevens blijven proberen totdat ze er een vinden die werkt.

Als er te veel miners met elkaar concurreren, zouden blokken te snel worden gevonden. Als er te weinig miners meedoen, zou het te lang duren om blokken te vinden. Om het systeem soepel te laten draaien, past Bitcoin de moeilijkheidsgraad automatisch aan om de 2.016 blokken (ongeveer om de twee weken).

Deze aanpassing zorgt ervoor dat er gemiddeld ongeveer elke 10 minuten een nieuw blok aan de blockchain wordt toegevoegd.


> **Definition – Definitie van moeilijkheidsgraad**
>
> De **moeilijkheidsgraad** Bij het minen van Bitcoin wordt gemeten hoe moeilijk het is om een geldige blokhash te vinden. Het netwerk past deze moeilijkheidsgraad om de 2.016 blokken (ongeveer elke twee weken) aan, zodat er ongeveer elke 10 minuten nieuwe blokken aan de blockchain worden toegevoegd. Hoe hoger de moeilijkheidsgraad, hoe moeilijker het voor miners is om een geldig blok te vinden.


Door een geldige blokhash te vinden, bewijst een miner dat hij het werk heeft verricht dat nodig is om een nieuw blok aan de blockchain toe te voegen. Dit proces wordt **Proof of Work** (PoW). Dit is het beveiligingsmechanisme waarmee Bitcoin transacties kan bevestigen en nieuwe blokken aan de blockchain kan toevoegen. De miner die als eerste de geldige hash vindt, ontvangt een beloning in bitcoin, bestaande uit de blokbeloning en de transactiekosten van de transacties die in dat blok zijn opgenomen.

Proof of Work (PoW) draagt bij aan de veiligheid van Bitcoin door het voor iedereen extreem duur te maken om te proberen vals te spelen of de controle over het netwerk over te nemen. Het is daarentegen veel winstgevender om zich aan de regels te houden.

Mijnwerkers vervullen vier belangrijke rollen:

1. **Transacties verzamelen**: Miners selecteren transacties die naar het netwerk zijn verzonden en voegen deze toe aan een kandidaatblok.
1. **Voer een Proof of Work uit**: Miners strijden om een moeilijke wiskundige puzzel op te lossen door een geldige blokhash te vinden.
1. **Het blok uitzenden**: De eerste miner die een geldige oplossing vindt, deelt het nieuwe blok met het netwerk.
1. **Verdien beloningen**: Als het blok geldig is, wordt het aan de blockchain toegevoegd en ontvangt de miner nieuw gecreëerde bitcoin plus transactiekosten.

Wereldwijd proberen veel miners tegelijkertijd het volgende blok te genereren. Zodra een miner een geldige oplossing vindt, controleert het netwerk het blok. Als alles in orde is, wordt het aan de blockchain toegevoegd. Andere concurrerende blokken worden afgewezen. Dit proces zorgt ervoor dat het netwerk op één lijn blijft en voorkomt dubbele uitgaven.

* Miners zijn computers die helpen bij het onderhouden en bijwerken van het grootboek van Bitcoin.
* Ze verzamelen transacties en bundelen deze in een blok. Vervolgens verwerken ze de gegevens van het blok via een hash-algoritme om een unieke code te genereren, een zogenaamde hash.
* Miners herhalen dit proces vele malen, op zoek naar een hash die voldoet aan de regels van Bitcoin. De eerste miner die een geldige hash vindt, ontvangt nieuw gecreëerde bitcoins als beloning, en zijn blok wordt aan de blockchain toegevoegd.
* De hash van elk blok koppelt het ook aan het voorgaande blok. Als iemand zou proberen een eerdere transactie te wijzigen, zouden de hashes niet meer met elkaar overeenkomen en zou het netwerk de gewijzigde keten afwijzen. Dit is wat het grootboek van Bitcoin veilig houdt.
