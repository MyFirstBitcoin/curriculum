# 8.1 Beveiliging door middel van cryptografie

> Wat Bitcoin ons biedt, is een vaste belofte: het programma zal precies zo werken als is gespecificeerd.  
_Andreas M. Antonopoulos_

#### Cryptografie met openbare en privésleutels


> **Definition – Definitie van cryptografie**
>
> **Cryptografie** is de methode waarbij informatie wordt omgezet in een geheim dat alleen de juiste personen kunnen lezen.


* **Versleuteling** is het proces waarbij informatie in een gecodeerde vorm wordt omgezet, zodat alleen iemand met de juiste sleutel deze kan lezen.
* **Ontcijfering** is het proces waarbij die gecodeerde informatie weer wordt omgezet in iets leesbaars.

In de traditionele cryptografie moeten twee personen die vertrouwelijk met elkaar willen communiceren, eerst dezelfde geheime sleutel delen, vergelijkbaar met een gedeeld wachtwoord. De ene persoon gebruikt deze sleutel om het bericht te versleutelen voordat hij het verstuurt, en de andere persoon gebruikt dezelfde sleutel om het te ontsleutelen en te lezen.

Het probleem met dit systeem is dat beide personen de geheime sleutel al moeten delen. Als iemand anders toegang krijgt tot die sleutel, kan hij of zij alle onderschepte berichten lezen.

Bitcoin lost dit probleem op via een andere methode, namelijk cryptografie met openbare sleutels, waarbij gebruikers geen geheime sleutels van tevoren hoeven uit te wisselen.

Cryptografie met openbare en privésleutels biedt een oplossing voor het delen van geheime informatie. In plaats van een wachtwoord te delen, beschikt iedereen over twee sleutels: een openbare sleutel en een privésleutel.

* De **openbare sleutel** kan met iedereen worden gedeeld.
* De **privésleutel** moet altijd geheim worden gehouden.

Als John iets naar Arel wil sturen, kan hij de openbare sleutel van Arel gebruiken. Alleen Arel kan het bericht ontgrendelen met zijn privésleutel. Zelfs als iemand het bericht onderschept, kan hij het zonder de privésleutel niet lezen of gebruiken.

Bij Bitcoin wordt dit systeem gebruikt om digitale handtekeningen te maken. Een digitale handtekening bewijst dat de eigenaar van een privésleutel een transactie heeft goedgekeurd, net zoals je je naam op een document zet. Hierdoor zijn Bitcoin-transacties veilig en controleerbaar zonder dat je op een derde partij hoeft te vertrouwen.

Bij Bitcoin-transacties wordt het eigendom van bitcoins van het ene adres naar het andere overgedragen.

Versleuteling wordt gebruikt om ervoor te zorgen dat alleen de daadwerkelijke eigenaar van de bitcoin bevoegd is om zijn geld naar iemand anders over te maken. Het zorgt ervoor dat zijn eigendom wordt beschermd tegen kwaadwillende partijen.

Als extra beveiligingsmaatregel krijgt elke Bitcoin-transactie automatisch een UNIEKE digitale handtekening. Deze unieke digitale handtekening is gebaseerd op fraudebestendige technologie waarmee het netwerk kan controleren of de echte eigenaar van de bitcoins deze heeft verzonden, en niet iemand anders.


> **Dark**
>
> Elke gebruiker heeft twee sleutels: een **privésleutel**, wat **geheim gehouden**, en een **openbare sleutel** dat kan **met anderen gedeeld**. De **privésleutel** dient als identificatiemiddel en eigendomsbewijs, waarmee wordt bevestigd: „Dit adres is van mij en ik heb er zeggenschap over.”


###### Hoe een Bitcoin-transactie werkt

1. **De transactie aanmaken**: Een gebruiker start een Bitcoin-transactie door gegevens op te geven zoals het adres van de ontvanger en het bedrag aan bitcoin dat moet worden verzonden.
1. **Het genereren van digitale handtekeningen**: De afzender genereert een uniek **digitale handtekening** met behulp van hun **privésleutel**. Deze handtekening is een unieke code die de authenticiteit van de transactie bevestigt.
1. **Bekendmaking van de transactie**: De ondertekende transactie wordt naar het Bitcoin-netwerk verzonden, waarmee het voornemen wordt aangegeven om het eigendom van de bitcoins van de afzender naar de ontvanger over te dragen.
1. **Controle via het netwerk**: Knooppunten in het Bitcoin-netwerk ontvangen de transactie en gebruiken de **openbare sleutel** om de echtheid van de handtekening te controleren. van de transactie. Tegelijkertijd gebruiken ze de **openbare sleutel** om de **digitale handtekening**.
1. **Bevestiging op het Bitcoin-netwerk**: Als de verificatie succesvol verloopt, wordt de transactie toegevoegd aan het grootboek, dat fungeert als een veilig en transparant register van alle transacties. Zodra de transactie is bevestigd, wordt het eigendom van de bitcoin officieel overgedragen van de afzender naar de ontvanger.


> **Callout – Samenvatting**
>
> De **digitale handtekening**, gemaakt met de afzender’s **privésleutel**, bewijst dat de transactie door de eigenaar van de bitcoin is goedgekeurd. Het Bitcoin-netwerk kan dit bewijs vervolgens verifiëren en de transactie vastleggen.


#### Uitleg over hashing

Laat je alsjeblieft niet afschrikken door de technische termen en wiskundige begrippen die hierna volgen. We begrijpen dat niet iedereen dol is op wiskunde, maar misschien verras je jezelf wel en kom je erachter dat zelfs de meest ingewikkelde ideeën met een beetje inspanning te begrijpen zijn.


> **Definition – Definitie van een functie**
>
> A **functie** is als een machine die bepaalde informatie verwerkt en er iets nieuws van maakt. De informatie die je aan de functie doorgeeft, is de **invoer**. De nieuwe informatie die de functie genereert, is de **uitvoer**. Functies helpen computers bij het uitvoeren van taken en het oplossen van problemen.


##### Wat is een functie?

Een functie is een reeks instructies die een invoer ontvangt en een uitvoer oplevert. Je kunt het vergelijken met een recept: je volgt de stappen met bepaalde ingrediënten, en je krijgt altijd een voorspelbaar resultaat.

In Bitcoin worden functies gebruikt om transacties te verwerken en te verifiëren. Wanneer iemand bitcoin verstuurt, helpen cryptografische functies om te controleren of de transactie geldig is, te bevestigen dat de afzender over voldoende saldo beschikt en de saldi in het Bitcoin-grootboek bij te werken. Zodra de transactie is geverifieerd en aan een blok is toegevoegd, wordt deze onderdeel van het permanente register op de blockchain.

##### Wat is een eenrichtingsfunctie?

Een eenrichtingsfunctie is een speciaal soort functie die in één richting eenvoudig te berekenen is, maar uiterst moeilijk omgekeerd kan worden. Zo is het bijvoorbeeld eenvoudig om ingrediënten tot een smoothie te mixen, maar kun je de smoothie niet weer in de oorspronkelijke ingrediënten terugverdelen.

De beveiliging van Bitcoin is gebaseerd op eenrichtingsfuncties. Deze worden gebruikt bij cryptografie met openbare en privésleutels, waardoor mensen een openbare sleutel kunnen delen terwijl ze hun privésleutel geheim houden. Hoewel de openbare sleutel zichtbaar is, is het onmogelijk om daaruit de privésleutel af te leiden. Dit is wat Bitcoin-transacties veilig maakt.

##### Wat is een hashfunctie?

A **hashfunctie** is net een machine voor geheime codes. Hij neemt een bericht in en zet dat om in een code.

###### Hoe hashing werkt bij Bitcoin-transacties

Bij Bitcoin wordt elke transactie omgezet in een hash voordat deze aan de blockchain wordt toegevoegd. Een hash is een unieke digitale vingerafdruk van de transactie. Als iemand ook maar een klein deel van de transactie probeert te wijzigen, verandert de hash volledig. Hierdoor kan het netwerk manipulatie gemakkelijk opsporen.

###### De rol van hashing in de beveiliging van Bitcoin

Hashing draagt bij aan de beveiliging van het Bitcoin-netwerk doordat transacties hierdoor eenvoudig te verifiëren zijn en niet stiekem kunnen worden gewijzigd. Omdat elke transactie een eigen unieke hash heeft, kan het netwerk snel vaststellen of er iets is gewijzigd.

Een hashfunctie zet gegevens om in een vaste reeks cijfers en letters, een zogenaamde hash. Dezelfde invoer levert altijd dezelfde hash op, maar zelfs een minieme wijziging in de invoer leidt tot een totaal ander resultaat. Dankzij deze eigenschap kunnen computers controleren of gegevens niet zijn gewijzigd.


> **Definition – Definitie van hashing**
>
> **Hashing** is te vergelijken met het maken van een vingerafdruk voor digitale gegevens. Het is het proces waarbij een digitaal bericht wordt omgezet in een code van vaste lengte, die als unieke identificatiecode dient. Net zoals een vingerafdruk een persoon kan identificeren, kan een hash een digitaal bericht identificeren.


De **uitvoer**, of hash, heeft altijd dezelfde lengte, ongeacht hoe lang de oorspronkelijke informatie was. Bitcoin maakt gebruik van een aantal specifieke soorten hashfuncties, genaamd **SHA-256** en **RIPEMD160**.

Hieronder volgen enkele voorbeelden:

* SHA256-hash van de tekenreeks **hallo wereld**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256-hash van de tekenreeks **Hallo wereld.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Merk op dat een kleine wijziging in de invoer de uitvoer volledig verandert in vergelijking met de eerste
* SHA256-hash van het downloadbare ISO-bestand **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Deze invoer is een enorm bestand, maar de uitvoer heeft nog steeds dezelfde vaste lengte

Je kunt hashing ook zien als een partituur die de essentie van een muziekstuk weergeeft. Net zoals een partituur een unieke weergave van een melodie is, is een hashwaarde een unieke weergave van een stuk data.

Door de partituur van een muziekstuk te vergelijken met de daadwerkelijke uitvoering, kan een muzikant vaststellen of de uitvoering correct is. Op dezelfde manier kan men, door de hashwaarde van ontvangen gegevens te vergelijken met de oorspronkelijke hashwaarde, vaststellen of de gegevens tijdens de overdracht zijn gewijzigd.

Net zoals een kleine afwijking in een muzikale uitvoering ervoor kan zorgen dat deze anders klinkt, leidt zelfs de kleinste wijziging in de oorspronkelijke gegevens tot een andere hashwaarde. Dit maakt hashing een krachtig hulpmiddel om de integriteit en authenticiteit van een Bitcoin-transactie te waarborgen.

Het proces van het coderen van de **openbare sleutel** Hashing wordt gebruikt om de beveiliging van informatie te verbeteren door deze om te zetten in een onleesbaar formaat met een vaste lengte. Bitcoin maakt gebruik van de SHA-256- en RIPEMD160-algoritmen om openbare adressen te genereren. De resulterende output dient als een unieke identificatiecode voor de **openbare sleutel** en draagt bij aan het waarborgen van de integriteit en veiligheid van de transacties die in het grootboek zijn opgeslagen. Door de informatie op deze manier te versleutelen, wordt het voor onbevoegden moeilijker om toegang te krijgen tot de gegevens en deze te manipuleren.

##### Eigenschappen van een hashfunctie

* **Deterministisch**: Met dezelfde ingrediënten krijg je altijd dezelfde smoothie. Op dezelfde manier leveren dezelfde gegevens altijd dezelfde hash op.
* **Weerstand van het pre-beeld**: Als je alleen de smoothie hebt, kun je niet achterhalen welke vruchten er precies in zijn verwerkt. Op dezelfde manier kun je, als je alleen een hash hebt, de oorspronkelijke gegevens niet achterhalen.
* **Lawine-effect**: Als je zelfs maar een heel klein onderdeel van de ingrediënten verandert, krijg je een heel andere smoothie. Bij het hashen leidt een heel kleine wijziging in de gegevens tot een heel andere hash.
* **Botsbestendigheid**: Het is uiterst moeilijk om twee verschillende combinaties van ingrediënten te vinden die precies dezelfde smoothie opleveren. Op dezelfde manier is het uiterst onwaarschijnlijk dat twee verschillende gegevens dezelfde hash opleveren.
* **Snel te controleren**: Het maken van de smoothie gaat snel, en je kunt gemakkelijk controleren of het resultaat inderdaad een smoothie is. Hashfuncties zijn snel te berekenen en voor iedereen gemakkelijk te verifiëren.

#### Activiteit: SHA-256-hash genereren


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Ben je benieuwd hoe hashing werkt? Scan de QR-code om direct een SHA256-hash te genereren van elk woord, elke zin of elke invoer die je maar wilt. Hashfuncties zijn als digitale vingerafdrukken: ze werken eenrichtingsverkeer, wat betekent dat als iets eenmaal is gehasht, dit niet meer ongedaan kan worden gemaakt. Probeer het eens uit en ontdek het zelf!
