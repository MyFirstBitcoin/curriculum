# 8.1 Beveiliging door cryptografie

> Wat Bitcoin ons geeft, is een harde belofte: het programma zal precies uitvoeren zoals gespecificeerd.  
_Andreas M. Antonopoulos_

#### Openbare/Privé Sleutel Cryptografie


> **Definition – Definitie van Cryptografie**
>
> **Cryptografie** is de praktijk van het omzetten van informatie in een geheim dat alleen de juiste mensen kunnen lezen.


* **Versleuteling** is het proces waarbij informatie wordt omgezet in een gecodeerde vorm, zodat alleen iemand met de juiste sleutel het kan lezen.
* **Ontsleuteling** is het proces waarbij die gecodeerde informatie weer leesbaar wordt gemaakt.

In traditionele cryptografie moeten twee mensen die privé willen communiceren eerst dezelfde geheime sleutel delen, vergelijkbaar met een gedeeld wachtwoord. De ene persoon gebruikt deze sleutel om het bericht te versleutelen voordat het wordt verzonden, en de andere persoon gebruikt dezelfde sleutel om het te ontsleutelen en te lezen.

Het probleem met dit systeem is dat beide personen de geheime sleutel al moeten delen. Als iemand anders toegang krijgt tot die sleutel, kan diegene alle onderschepte berichten lezen.

Bitcoin lost dit probleem op met een andere aanpak, genaamd openbare-sleutelcryptografie, waarbij gebruikers niet vooraf geheime sleutels hoeven te delen.

Openbare/prive sleutelcryptografie lost het probleem van het delen van geheimen op. In plaats van een wachtwoord te delen, heeft elke persoon twee sleutels: een openbare sleutel en een privé sleutel.

* De **openbare sleutel** kan met iedereen gedeeld worden.
* De **privé sleutel** moet altijd geheim blijven.

Als Jan iets naar Arel wil sturen, kan hij de openbare sleutel van Arel gebruiken. Alleen Arel kan het ontgrendelen met zijn privé sleutel. Zelfs als iemand het bericht onderschept, kan diegene het niet lezen of gebruiken zonder de privé sleutel.

In Bitcoin wordt dit systeem gebruikt om digitale handtekeningen te maken. Een digitale handtekening bewijst dat de eigenaar van een privé sleutel een transactie heeft goedgekeurd, vergelijkbaar met het ondertekenen van je naam op een document. Dit maakt het mogelijk dat Bitcoin-transacties veilig en verifieerbaar zijn zonder een derde partij te hoeven vertrouwen.

Bitcoin-transacties gaan over het overdragen van eigendom van bitcoin van het ene adres naar het andere.

Versleuteling wordt gebruikt om ervoor te zorgen dat alleen de echte eigenaar van de bitcoin het recht heeft om zijn geld naar iemand anders te sturen. Het zorgt ervoor dat hun eigendom beschermd is tegen kwaadwillenden.

Als extra beschermingsmaatregel krijgt elke Bitcoin-transactie automatisch een UNIEKE digitale handtekening. Deze unieke digitale handtekening wordt mogelijk gemaakt door technologie die niet te manipuleren is en helpt het netwerk te verifiëren dat de echte eigenaar van de bitcoin, en niet iemand anders, deze heeft verzonden.


> **Info**
>
> Elke gebruiker heeft twee sleutels: een **privé sleutel**, die **geheim wordt gehouden**, en een **openbare sleutel** die kan worden **gedeeld met anderen**. De **privé sleutel** dient als een vorm van identificatie en bewijs van eigendom, waarmee wordt bevestigd: “Dit adres behoort mij toe en ik heb er controle over.”


###### Hoe een Bitcoin-transactie werkt

1. **De transactie aanmaken**: Een gebruiker start een Bitcoin-transactie door details op te geven zoals het adres van de ontvanger en het aantal te verzenden bitcoin.
1. **Digitale handtekening genereren**: De verzender genereert een unieke **digitale handtekening** met behulp van zijn **privé sleutel**. Deze handtekening is een unieke code die de echtheid van de transactie bevestigt.
1. **De transactie uitzenden**: De ondertekende transactie wordt uitgezonden naar het Bitcoin-netwerk, waarmee de intentie wordt aangegeven om het eigendom van bitcoin van de verzender naar de ontvanger over te dragen.
1. **Verificatie op het netwerk**: Nodes op het Bitcoin-netwerk ontvangen de transactie en gebruiken de openbare sleutel van de ontvanger **openbare sleutel** om de echtheid van de handtekening van de transactie te verifiëren. Tegelijkertijd gebruiken ze de openbare sleutel van de verzender **openbare sleutel** om de **digitale handtekening**.
1. **Bevestiging op het Bitcoin-netwerk**: Als de verificatie slaagt, wordt de transactie toegevoegd aan het grootboek, dat dient als een veilig en transparant overzicht van alle transacties. Zodra de transactie is bevestigd, wordt het eigendom van de bitcoin officieel overgedragen van de verzender naar de ontvanger.


> **Callout – Samenvatting**
>
> De **digitale handtekening**, aangemaakt met de **privésleutel** van de verzender, bewijst dat de transactie is goedgekeurd door de eigenaar van de bitcoin. Het Bitcoin-netwerk kan dit bewijs vervolgens verifiëren en de transactie vastleggen.


#### Uitleg over hashen

Laat je niet afschrikken door de technische termen en wiskundige concepten die volgen. We begrijpen dat niet iedereen dol is op wiskunde, maar misschien verras je jezelf en zie je dat zelfs de meest complexe ideeën te begrijpen zijn met een beetje moeite.


> **Definition – Definitie van een functie**
>
> Een **functie** is als een machine die informatie neemt en er iets nieuws van maakt. De informatie die je aan de functie geeft, is de **input**. De nieuwe informatie die de functie creëert, is de **output**. Functies helpen computers taken uit te voeren en problemen op te lossen.


##### Wat is een functie?

Een functie is een reeks instructies die een input neemt en een output oplevert. Je kunt het vergelijken met een recept: je volgt de stappen met bepaalde ingrediënten en je krijgt altijd een voorspelbaar resultaat.

In Bitcoin worden functies gebruikt om transacties te verwerken en te verifiëren. Wanneer iemand bitcoin verstuurt, helpen cryptografische functies om te controleren of de transactie geldig is, of de verzender genoeg saldo heeft, en om de saldi op het Bitcoin-grootboek bij te werken. Zodra de transactie is geverifieerd en aan een blok is toegevoegd, wordt deze onderdeel van het permanente register op de blockchain.

##### Wat is een eenrichtingsfunctie?

Een eenrichtingsfunctie is een speciaal soort functie die gemakkelijk in één richting te berekenen is, maar extreem moeilijk om om te keren. Bijvoorbeeld: ingrediënten tot een smoothie blenden is eenvoudig, maar je kunt de smoothie niet meer terugbrengen naar de oorspronkelijke ingrediënten.

De veiligheid van Bitcoin is gebaseerd op eenrichtingsfuncties. Ze worden gebruikt in openbare en privésleutelcryptografie, waardoor mensen een openbare sleutel kunnen delen terwijl hun privésleutel geheim blijft. Ook al is de openbare sleutel zichtbaar, het is onmogelijk om daaruit de privésleutel af te leiden. Dit maakt Bitcoin-transacties veilig.

##### Wat is een hashfunctie?

Een **hashfunctie** is als een geheime codemachine. Het neemt een bericht en verandert het in een code.

###### Hoe hashing werkt bij Bitcoin-transacties

Bij Bitcoin wordt elke transactie omgezet in een hash voordat deze aan de blockchain wordt toegevoegd. Een hash is een unieke digitale vingerafdruk van de transactie. Als iemand ook maar een klein deel van de transactie probeert te veranderen, verandert de hash volledig. Hierdoor kan het netwerk gemakkelijk knoeien detecteren.

###### De rol van hashing in Bitcoin-beveiliging

Hashing helpt het Bitcoin-netwerk te beschermen door transacties eenvoudig te verifiëren en onmogelijk stilletjes aan te passen. Omdat elke transactie een unieke hash heeft, kan het netwerk snel zien of er iets is veranderd.

Een hashfunctie neemt gegevens en zet deze om in een vaste reeks cijfers en letters, een zogenaamde hash. Dezelfde input levert altijd dezelfde hash op, maar zelfs een kleine wijziging in de input zorgt voor een totaal ander resultaat. Dankzij deze eigenschap kunnen computers controleren of gegevens niet zijn veranderd.


> **Definition – Definitie van hashing**
>
> **Hashing** is als het maken van een vingerafdruk voor digitale gegevens. Het is het proces waarbij een digitaal bericht wordt omgezet in een code van vaste lengte, die dient als unieke identificatie. Net zoals een vingerafdruk een persoon kan identificeren, kan een hash een digitaal bericht identificeren.


De **output**, of hash, is altijd even lang, ongeacht hoe lang de oorspronkelijke informatie was. Bitcoin gebruikt een paar specifieke soorten hashfuncties, genaamd **SHA-256** en **RIPEMD160**.

Hieronder volgen een paar voorbeelden:

* SHA256-hash van de string **hallo wereld**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256-hash van de string **hallo wereld.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Let op dat een kleine wijziging in de invoer de uitvoer volledig verandert in vergelijking met de eerste
* SHA256-hash van het downloadbare iso-bestand **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Deze invoer is een enorm bestand, maar de uitvoer heeft nog steeds dezelfde vaste lengte

Je kunt hashing ook zien als een muziekpartituur die de essentie van een muziekstuk vastlegt. Net zoals een partituur een unieke weergave is van een melodie, is een hashwaarde een unieke weergave van gegevens.

Door de partituur van een muziekstuk te vergelijken met de daadwerkelijke uitvoering, kan een muzikant bepalen of de uitvoering correct is. Op dezelfde manier kun je door de hashwaarde van ontvangen gegevens te vergelijken met de originele hashwaarde bepalen of de gegevens tijdens de overdracht zijn gewijzigd.

Net zoals een kleine afwijking in een muzikale uitvoering ervoor kan zorgen dat het anders klinkt, zal zelfs de kleinste wijziging in de originele gegevens resulteren in een andere hashwaarde. Dit maakt hashing tot een krachtig hulpmiddel om de integriteit en authenticiteit van een Bitcoin-transactie te waarborgen.

Het proces van het coderen van de **publieke sleutel** via hashing wordt gebruikt om de veiligheid van informatie te verbeteren door deze om te zetten in een vaste, onleesbare lengte. Bitcoin gebruikt de SHA-256- en RIPEMD160-algoritmen om publieke adressen te genereren. De resulterende uitvoer dient als een unieke identificatie voor de **publieke sleutel** en helpt om de integriteit en veiligheid van transacties die in het grootboek zijn opgeslagen te waarborgen. Door de informatie op deze manier te versleutelen, wordt het moeilijker voor onbevoegden om toegang te krijgen tot de gegevens en deze te manipuleren.

##### Eigenschappen van een hashfunctie

* **Deterministisch**: Dezelfde ingrediënten leveren altijd dezelfde smoothie op. Op dezelfde manier levert dezelfde data altijd dezelfde hash op.
* **Pre-image weerstand**: Als je alleen de smoothie hebt, kun je niet achterhalen welke exacte vruchten zijn gebruikt. Op dezelfde manier kun je met alleen een hash niet de originele gegevens bepalen.
* **Avalanche-effect**: Zelfs een kleine verandering in de ingrediënten zorgt voor een totaal andere smoothie. Bij hashing zorgt een heel kleine wijziging in de data voor een compleet andere hash.
* **Botsingsbestendigheid**: Het is extreem moeilijk om twee verschillende sets ingrediënten te vinden die exact dezelfde smoothie opleveren. Op dezelfde manier is het uiterst onwaarschijnlijk dat twee verschillende gegevens dezelfde hash opleveren.
* **Snel te verifiëren**: Het maken van de smoothie gaat snel, en het is eenvoudig te controleren dat het resultaat een smoothie is. Hashfuncties zijn snel te berekenen en voor iedereen makkelijk te controleren.

#### Activiteit: Genereer SHA 256 Hash

https://tools.keycdn.com/sha256-online-generator

Benieuwd hoe hashing werkt? Scan de QR-code om direct een SHA256-hash te genereren van elk woord, elke zin of invoer die je kiest. Hashfuncties zijn als digitale vingerafdrukken: ze zijn eenrichtingsverkeer, wat betekent dat zodra iets gehasht is, het niet meer teruggedraaid kan worden. Probeer het zelf en ontdek het!
