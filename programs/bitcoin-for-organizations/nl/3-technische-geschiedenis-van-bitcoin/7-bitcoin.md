# 3.7 Bitcoin

Na vele jaren en mislukte pogingen waren de Cypherpunks grotendeels hun interesse in het idee van een digitale, permissieloze munt verloren, toen Adam Back een e-mail ontving met een link naar een concept-whitepaper getiteld ‘elektronisch geld zonder derde partij’ van een anoniem persoon die zichzelf Satoshi Nakamoto noemde.

Om tot nu toe samen te vatten, hebben we in ieder geval de volgende ideeën:

* Cryptografische handtekeningen die een bepaald niveau van privacy en anonimiteit konden bieden
* Het concept van een niet-gedekte valuta (B-Money)
* Voorstellen (maar geen middelen) om de uitgifte van nieuwe valuta te beperken
* Digitale munten waarvan het eigendom werd toegekend via publieke sleutels (B-Money) en die konden worden verplaatst door te ondertekenen en opnieuw toe te wijzen op basis van het adres van de ontvanger (RPOW en Hashcash)
* Alle nodes onderhouden een kopie van een volledig gedistribueerd grootboek (B-Money) (destijds als onpraktisch afgedaan)
* Tijdstempelprotocol – met behulp van Merkle-boom hashing om een wiskundig bewijsbare chronologie van gebeurtenissen te bieden die moeilijk te vervalsen is als alle gebruikers dezelfde gegevens bijhouden
* Proof of work om echte wereldinspanning aan het systeem te koppelen (maar waarbij de hash zelf als valuta werd gebruikt)
* Volledig gedecentraliseerde netwerken waarin alle peers gelijk zijn en vrij kunnen komen en gaan uit het netwerk (BitTorrent)
* Het concept om nieuwe hashes aan eerdere hashes te koppelen (Bit Gold en tijdstempeling)

Wat op dat moment nog ontbrak, was onder andere:

* Een werkbare oplossing voor het ‘Byzantijnse generaalsprobleem’
* Een methode om de hoeveelheid geld in omloop te beperken ondanks voortdurende hardwareverbeteringen
* Een incentiveschema voor mensen om deel te nemen (kip-en-ei-probleem)

Het andere grote verschil tussen recente pogingen en Bitcoin was dat Satoshi al enige tijd aan de code werkte in de ware ‘Cypherpunks schrijven code’-geest voordat hij het aankondigde op de mailinglijsten, in tegenstelling tot Bit Gold en B-Money die meer conceptueel waren.

Wat was de innovatie die Bitcoin onderscheidde van eerdere pogingen tot elektronisch geld?

Proof of work zou worden gebruikt als consensusmechanisme en als manier om veiligheid en onveranderlijkheid te bieden: In plaats van de hash als vorm van geld te gebruiken, zou deze worden gebruikt door een nieuw conceptueel proces genaamd mining, waarbij een node een set transacties zou bundelen, een willekeurig getal zou toevoegen en vervolgens hashing zou toepassen op het ‘blok’ met data. Een geldig blok dat aan de hashvereiste voldeed, zou vervolgens aan het netwerk worden geadverteerd. Deze blokken zouden aan elkaar worden gekoppeld door de hash van het vorige blok in elk, en de langste blockchain zou worden gebruikt in het geval van een tiebreaker waarbij verschillende nodes verschillende blokken tegelijkertijd zouden valideren en adverteren, wat kettingsplitsingen veroorzaakt. Proof of work werd de gedistribueerde tiebreaker om het Byzantijnse generaalsprobleem op te lossen.

Deze miners kregen ook een stimulans om de benodigde CPU te leveren voor het uitvoeren van de proof-of-work door nieuwe bitcoin toegewezen te krijgen voor elk blok. Het aantal Bitcoin dat ze ontvangen is ook geprogrammeerd om ongeveer elke 4 jaar te dalen totdat alle Bitcoin is gecreëerd, waardoor er een harde limiet ontstaat op het totale aantal Bitcoin dat ooit in omloop zal zijn van 21 miljoen.

Het meest originele idee was de manier waarop hij het probleem oploste van hoeveel geld er wordt gecreëerd naarmate hardware verbetert en er meer rekenkracht op het netwerk kan worden toegepast. De tijdstempels van een vast aantal blokken (2016) zouden worden gemiddeld, en als ze te snel worden aangemaakt, zou de hash die nodig is om een nieuw blok te maken moeilijker worden, en als het te langzaam gaat, zou het makkelijker worden. Dit was ingebouwd in het gedecentraliseerde protocol dat alle nodes draaien, dus elke miner die dit negeert, zou energie verspillen aan het minen van een blok zonder voordeel, omdat het door de rest van het netwerk zou worden afgewezen. Deze aanpassing zorgt ervoor dat de creatie van nieuwe blokken op het geplande uitgifteschema blijft en biedt incentives voor miners om zich ‘aan de regels te houden’.

####   
Samenvatting

Veel van de puzzelstukjes die nodig zijn om een gedecentraliseerd peer-to-peer elektronisch geldsysteem te bouwen op basis van solide geldprincipes, waren al aanwezig voordat Satoshi zijn whitepaper uitbracht en kort daarna de eerste versie van de code.

> De aard van Bitcoin is zodanig dat zodra versie 0.1 werd uitgebracht, het kernontwerp voor de rest van zijn bestaan in steen gebeiteld was  
_Satoshi Nakamoto_

Hoewel er veel ideeën voor verbeteringen (BIPs) zijn voorgesteld en aangenomen, werkt Bitcoin sinds 2009 op de achtergrond volgens het protocol dat in de eerste release is ontworpen en met nauwelijks enige verstoring. Alle verbeteringen zijn doorgevoerd met behoud van achterwaartse compatibiliteit met alle eerdere versies.



##### Notities

1. Voor een uitleg van het Byzantijnse generaalsprobleem - zie [https://nl.wikipedia.org/wiki/Byzantijnse_generaal](https://en.wikipedia.org/wiki/Byzantine_fault)
