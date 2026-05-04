# 3.2 Publieke-sleutelcryptografie en protocollen

Het internet van vandaag, en de meeste moderne computersystemen, zijn afhankelijk van cryptografie, een methode om informatie te verhullen zodat alleen de ontvanger van de informatie deze kan ontcijferen. De fundamenten van de cryptografie die wordt gebruikt om Bitcoin te beveiligen, zijn terug te voeren tot de jaren 70.

Het eerste probleem dat opgelost moet worden is: hoe stuur je een gedeeld geheim over een onbeveiligd medium.

Dit werd voor het eerst onderzocht door Whitfield Diffie en Martin Hellman.

Het probleem: de twee partijen – meestal aangeduid als Alice en Bob – willen geheime informatie delen via een netwerk waar anderen mogelijk meeluisteren. Om dit te bereiken, hebben ze het Diffie-Hellman-sleuteluitwisselingsproces gecreëerd.

Dit gedeelde geheim kan vervolgens worden gebruikt als uitgangswaarde om talloze symmetrische sleutels te creëren om berichten te versleutelen en te ontsleutelen die ze naar elkaar sturen, zonder de sleutel zelf openbaar te maken.

Omdat de privésleutel nooit gedeeld hoeft te worden, en aan beide kanten verschillende sleutels worden gebruikt om te versleutelen en te ontsleutelen, wordt dit een asymmetrisch encryptie-algoritme genoemd.

Toepassingen:

* Alice ondertekent een bericht met Bobs publieke sleutel – hij is de enige die het kan ontsleutelen met zijn privésleutel
* Alice ondertekent een bericht met haar privésleutel – door te ontsleutelen met haar publieke sleutel kan iedereen verifiëren dat het bericht door Alice is verstuurd, zonder haar privésleutel te kennen
* Door deze twee benaderingen te combineren met twee lagen van encryptie, kan een bericht versleuteld worden verzonden zodat alleen Bob het kan ontsleutelen, en kan hij vervolgens verifiëren dat de afzender daadwerkelijk Alice was.

Hoewel hij niet als auteur op het artikel stond, was Ralph Merkle van groot belang bij het helpen oplossen van wat tot dan toe als een onoplosbare puzzel werd beschouwd – hoe privécommunicatie tot stand te brengen of te herstellen via een open en mogelijk vijandig netwerk.

Deze aanpak is op zichzelf vatbaar voor een brute-force aanval, waarbij een aanvaller de gedeelde getallen kan nemen en uiteindelijk een gedeelde sleutel kan reconstrueren, mits voldoende tijd en middelen, dus het is op zichzelf niet de volledige oplossing.

##### Protocollen voor Public Key Cryptosystemen

Naast zijn bijdrage aan het hierboven beschreven Diffie-Hellman public-key systeem,**Ralph Merkle** bleef jarenlang bijdragen aan dit vakgebied en was van groot belang bij de ontwikkeling van enkele belangrijke componenten die door Bitcoin worden gebruikt.

Een cryptografische hashfunctie is een wiskundig algoritme dat invoer van elke grootte neemt en complexe berekeningen uitvoert om een hashwaarde in bits terug te geven, die meestal wordt weergegeven als een alfanumerieke uitvoer van vaste lengte in hexadecimale notatie.

* Invoer kan elke grootte hebben
* De uitvoer is altijd van vaste lengte en deterministisch (dezelfde invoer levert elke keer dezelfde hash op)
* Het is eenvoudig te verifiëren, maar buitengewoon moeilijk om het proces om te keren om de invoer te bepalen
* Een kleine wijziging van de data verandert de uitvoer volledig

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/16a0db97ba457e83790f227e2ca0948f19118a25-515x331.svg)

Hashing is een integraal onderdeel van het Bitcoin-protocol. SHA-256, gebruikt in Bitcoin, is ontwikkeld door de NSA en is een voorbeeld van een cryptografisch hash-algoritme.

* Elk blok in de keten wordt gehasht zodat data niet kan worden gewijzigd – dit waarborgt de integriteit van het gedistribueerde grootboek.
* De gegenereerde hash moet voldoen aan de ‘Proof of work’-criteria om als een geldig blok te worden beschouwd.
* Merkle-bomen – door gebruik te maken van vertakkingen en hashes van hashes, kunnen hashbomen de verificatie van grote datasets mogelijk maken met minimale opslag.
* Op hashes gebaseerde handtekeningen en sleutels kunnen worden gebruikt voor wallets, adressen en autorisatie van transacties.

Gedecentraliseerde verificatie van blockchain-toestanden en append-only grootboekmodellen die bestand zijn tegen aanpassing, worden mogelijk gemaakt door eenrichtings-hashing. Hashfuncties bieden de betrouwbare, deterministische methode om gebeurtenissen op openbare grootboeken zoals Bitcoin te verifiëren zonder een gecentraliseerd vertrouwensmodel.

Van deze nieuwe mogelijkheden op het gebied van cryptografie werd door de bedenkers verwacht dat ze een nieuwe golf van innovatie zouden inluiden.

##### Elliptische kromme cryptografie

Een van deze latere innovaties kwam in de vorm van elliptische kromme cryptografie.

Elliptische kromme cryptografie werd in 1985 geïntroduceerd door twee wetenschappers, N. Koblitz en V. Miller. Zij stelden voor om punten te gebruiken die worden gedefinieerd door elliptische krommen in plaats van eindige priemvelden, zodat de aanname van het Discrete Logaritme probleem blijft gelden, zoals gebruikelijk is in het standaard Diffie-Hellman sleuteluitwisselingsprotocol. De details van hoe dit werkt vallen buiten de scope van deze sectie, maar op hoofdlijnen is een elliptische kromme de verzameling punten die voldoen aan een specifieke wiskundige vergelijking.

De vergelijking voor een elliptische kromme ziet er ongeveer zo uit:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Dit heeft enkele nuttige eigenschappen:

* Horizontale symmetrie. Elk punt op de kromme kan worden gespiegeld over de x-as en blijft op dezelfde kromme.
* elke niet-verticale lijn zal de kromme op maximaal drie plaatsen snijden.
* Compacte sleutellengtes zijn essentieel voor efficiënte opslag en overdracht van publieke sleutels in de blockchain.

Deze eigenschappen kunnen worden gebruikt om sleutelpaaren te maken op een vergelijkbare manier als bij het Diffie-Hellman-algoritme. Bitcoin gebruikt ECDSA, wat staat voor Elliptic Curve Digital Signature Algorithm. Dit is een proces dat een elliptische kromme en een eindig veld gebruikt om data te 'ondertekenen' op een manier waarop derden de authenticiteit van de handtekening kunnen verifiëren, terwijl de ondertekenaar het exclusieve vermogen behoudt om de handtekening te maken. Bij bitcoin is de data die wordt ondertekend de transactie die het eigendom overdraagt.

Het ‘eindige’ deel is vergelijkbaar met de ‘mod’-benadering bij Diffie-Hellman, waarbij de uitkomst van de vergelijking wordt gedeeld en de rest wordt gebruikt om ervoor te zorgen dat deze binnen een bepaald bereik van getallen past.
