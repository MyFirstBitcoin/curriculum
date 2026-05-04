# 2.4 Er vindt geen innovatie plaats in Bitcoin

> Het ontstaan van duizend bossen zit in één eikel.   
_Ralph Waldo Emerson_

Critici proberen vaak te beweren dat Bitcoin 'oude' of 'dode' technologie is omdat het basisprotocol niet zo vaak verandert als concurrerende blockchains. Deze bewering negeert zowel de redenen waarom veranderingen in Bitcoin langzaam worden doorgevoerd als de hoeveelheid innovatie die plaatsvindt om het netwerk op hogere lagen te schalen, zoals het Lightning Network. Ook wordt genegeerd dat veel van onze meest flexibele en duurzame technologieën zich ook niet snel ontwikkelen op de basislaag.

Er vindt bijvoorbeeld ook geen innovatie plaats in het Transmission Control Protocol (TCP), dat ten grondslag ligt aan het internet. TCP werd voor het eerst ontwikkeld in 1974. De laatste keer dat TCP werd bijgewerkt was in 1982. Het doet wat het moet doen. Het is niet perfect, en er zijn discussies over de vraag of we IPv4 moeten upgraden om toekomstige internetontwikkelingen te ondersteunen. Echter, beweren dat er sinds 1982 geen innovatie op het internet heeft plaatsgevonden, zou een opmerkelijke uitspraak zijn. Al deze innovatie heeft plaatsgevonden ‘op’ TCP, niet ‘in’ TCP.

De overgrote meerderheid van de innovatie vindt niet ‘in’ Bitcoin plaats, maar ‘op’ Bitcoin. Op een dag zal er waarschijnlijk geen innovatie meer ‘in’ Bitcoin zijn, en dat zou een doel moeten zijn en geen kritiek, omdat het een weerspiegeling zal zijn van hoe fundamenteel het is geworden in het ondersteunen van de wereldeconomie door de basis te bieden voor wereldwijd, neutraal en permissieloos gezond geld. Geld dat gezond is, zowel in economische zin doordat er een vaste voorraad is en een onveranderlijk grootboek, als in technologische zin omdat het niet verandert en wat draait al jaren onafgebroken werkt. Bitcoin heeft de afgelopen 10 jaar al 100% uptime bereikt.

Het zou echter zorgwekkend zijn als er geen innovatie ‘op’ Bitcoin plaatsvond. Laten we daar de afgelopen 10 jaar naar kijken:



#### 'In' Bitcoin

Segregated Witness (SegWit) werd in 2017 geïmplementeerd om te beschermen tegen aanpasbaarheid van transacties en om de blokcapaciteit te vergroten. SegWit was ook een noodzakelijke voorloper voor het efficiënt functioneren van lightning en sommige sidechains.

Taproot werd in 2021 geïmplementeerd om het groeperen en valideren van meerdere handtekeningen mogelijk te maken door Schnorr-handtekeningen te integreren, een scripttaal te introduceren voor meer complexe functionaliteit en de privacy en censuurbestendigheid van transacties te vergroten.



#### 'Op' Bitcoin

##### Liquid Sidechain

De Liquid sidechain werd in 2018 geïmplementeerd. Liquid, net als andere sidechains, is een afzonderlijk blockchain-grootboek dat volgens een vooraf gedefinieerde set regels is gekoppeld aan de hoofd-Bitcoin-blockchain. Deze regels zijn flexibel genoeg om de Liquid-keten in staat te stellen zich te ontwikkelen en ontwerp- en schaalbaarheidsverbeteringen in de loop van de tijd te integreren. De koppeling aan de Bitcoin-blockchain zorgt er echter voor dat het totale aanbod van 21 miljoen bitcoin consistent is over beide ketens.

Het activum in Liquid, L-BTC, is tweerichtings-gekoppeld aan bitcoin op de hoofdketen. Er zijn kosten-, snelheids-, privacy- en beveiligingsafwegingen die L-BTC ideaal maken voor bepaalde toepassingen. Kosten, snelheid en privacy zijn allemaal verbeterd met L-BTC, ten koste van enig vertrouwen in de organisaties die deel uitmaken van de Liquid Federation, die samen een 11 van 15 multisig-proces beheren om L-BTC in en uit te koppelen naar bitcoin en omgekeerd.

##### Lightning Network

Het Lightning Network werd in 2018 geïmplementeerd. Lightning is ontworpen als een peer-to-peer betalingsnetwerk in de vorm van een grafiek van knooppunten die via kanalen met elkaar verbonden zijn; het is geen blockchain. Bitcoin wordt door een node-operator op de hoofdblockchain vastgezet om het beschikbaar te maken voor gebruik op het Lightning Network, wat ervoor zorgt dat alleen ‘echte’ bitcoin wordt gebruikt. Knooppunten kunnen vervolgens liquiditeitskanalen openen via multisig smart contracts met elkaar. Betalingen vinden hun weg door het netwerk van bron naar bestemming, waarbij wordt geoptimaliseerd voor kosten en de vereiste dat er voldoende liquiditeit is in de juiste richting tussen elke stap in de route. Het Lightning Network verbetert kosten, snelheid en privacy enorm in ruil voor een verlies aan veiligheid (of toename van vereist vertrouwen) en toename van complexiteit. Het is echter bedoeld voor grote aantallen, kleine waarde dagelijkse betalingen, dus dit wordt beschouwd als een zeer redelijke afweging voor de miljoenen dagelijkse transacties (bron: River, 2023).

##### Chaumian eCash Mints

Fedimints kunnen worden gezien als een community-gebonden lightning network. Ze zijn ontworpen om het inherente vertrouwen dat binnen bepaalde gemeenschappen bestaat (bijv. families, dorpen, vriendengroepen) te benutten in ruil voor het vereenvoudigen van de complexiteit en het vergroten van de privacy voor gebruikers. Het zijn modulaire, open source protocollen om bitcoin te bewaren en te verhandelen in een gemeenschapscontext. Ze zijn interoperabel met het Lightning Network zelf.

**Cashu** is een toondertoken die kan worden opgeslagen op een apparaat zoals een mobiele telefoon; het ontwerp is gericht op het reproduceren van de voordelen van fysiek contant geld, maar dan in digitale vorm. Cashu is een voorbeeld van Chaumian eCash gebouwd op Bitcoin en verhoogt privacy en censuurbestendigheid en vermindert complexiteit in ruil voor het vertrouwen in de gebruikte eCash-mint. Cashu-mints geven eCash-tokens uit, die bitcoin vertegenwoordigen en door gebruikers kunnen worden uitgegeven zonder hun identiteit prijs te geven. Cashu is interoperabel met het Lightning Network.

Waarschijnlijk zullen er in de toekomst nog veel meer layer 2-toepassingen worden gebouwd, met daarbovenop weer veel layer 3-toepassingen.

Als voorbeeld van het ongelooflijke aantal toepassingen dat bovenop Lightning wordt gebouwd, volgt hier een fragment uit een Lightning Network Research Report van River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
