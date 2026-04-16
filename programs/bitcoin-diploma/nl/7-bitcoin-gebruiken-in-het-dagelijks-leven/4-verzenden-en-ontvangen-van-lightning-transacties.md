# 7.4 Verzenden en ontvangen van Lightning-transacties

Met een Lightning-wallet is het gebruik van Bitcoin snel, goedkoop en privé, waardoor transacties tussen twee mensen eenvoudig zijn. Je kunt snel bitcoin versturen en ontvangen voor alledaagse dingen zoals koffie kopen of winkelen.

Laten we een paar voorbeelden bekijken van het Lightning Network in de praktijk.

###### Voorbeeld 1

Zowel Marcia als Eve hebben 5 eenheden valuta. Marcia wil 2 eenheden naar Eve sturen. De betaling gaat via Jeff, die helpt de betaling door het Lightning Network te leiden. Nadat de betaling is voltooid, heeft Eve 7 eenheden en Marcia 3.

Jeff helpt de betaling te routeren, maar hij kan het geld niet stelen. Het Lightning Network gebruikt cryptografie om ervoor te zorgen dat alleen de bedoelde ontvanger de betaling kan ontvangen. Jeff helpt simpelweg de betaling door het netwerk te bewegen.

Dit laat een belangrijk voordeel van het Lightning Network zien: mensen kunnen snel betalingen versturen zonder tussenpersonen zoals banken te hoeven vertrouwen.

Node-operators zoals Jeff kunnen ook kleine vergoedingen verdienen voor het helpen routeren van betalingen. Door dit te doen, helpen ze het netwerk gedecentraliseerd en efficiënt te houden.

Vergeleken met gewone Bitcoin-transacties:

* **On-chain transacties** vinden direct plaats op de Bitcoin-blockchain. Ze zijn zeer veilig, maar kunnen trager en duurder zijn.
* **Lightning-transacties** vinden off-chain plaats en maken het mogelijk om betalingen veel sneller en tegen veel lagere kosten te versturen.

Hierdoor is Lightning handig voor kleine, dagelijkse betalingen, terwijl on-chain transacties vaak worden gebruikt voor grotere overboekingen of langdurige opslag.

###### Voorbeeld 2

Mina houdt van uit eten gaan en stopt vaak bij haar favoriete lokale café. Met zoveel verschillende betaalopties weet ze niet zeker welke de beste keuze is. Gelukkig heeft ze wat geleerd over Bitcoin en het Lightning Network. Na haar opties te hebben bekeken, beseft Mina dat betalen via Lightning de beste optie is.

Mina wil een koffie kopen, maar betalen met een gewone Bitcoin-transactie kan soms tijd kosten en hogere kosten met zich meebrengen. In plaats daarvan besluit ze het Lightning Network te gebruiken.

Het Lightning Network maakt het mogelijk om direct bitcoin te versturen met zeer lage kosten. Dit maakt het ideaal voor kleine, dagelijkse aankopen zoals koffie.

Om Lightning te gebruiken, downloadt Mina een Lightning-wallet op haar telefoon. Vervolgens stuurt ze wat bitcoin van haar gewone Bitcoin-wallet naar haar Lightning-wallet. Deze stap gebruikt een normale Bitcoin-transactie op de blockchain. Zodra het geld in haar Lightning-wallet staat, kan ze het op het Lightning Network gebruiken.

Nu kan Mina het café direct betalen via Lightning. De betaling vindt buiten de hoofd-Bitcoin-blockchain plaats, waardoor het veel sneller en goedkoper is dan een gewone on-chain transactie.


| Voordelen | Lightning Network | Traditioneel banksysteem |
| --- | --- | --- |
| Snelheid | Snel | Traag |
| Transparantie | Transparant | Ondoorzichtig |
| Beveiliging | Veilig | Kwetsbaar |
| Transactiekosten | Laag | Hoog |
| Financiële inclusie | Hoog | Beperkt |
| Schaalbaarheid | Hoog | Laag |
| Privacy | Hoog | Gemiddeld |
| Interoperabiliteit | Hoog | Laag |
| Wettelijke naleving | Gemiddeld | Hoog |
| Kosteneffectiviteit | Hoog | Gemiddeld |


Eenvoudig gezegd vinden on-chain transacties direct plaats op de Bitcoin-blockchain en kunnen ze meer tijd en kosten met zich meebrengen. Lightning-transacties vinden off-chain plaats, waardoor snelle en goedkope betalingen mogelijk zijn, terwijl je toch bitcoin gebruikt.


| Visa, Inc. | Bitcoin On-chain | Lightning Network |
| --- | --- | --- |
| Capaciteit van 65.000 transacties per seconde. | Capaciteit van 7 transacties per seconde. | Capaciteit van miljoenen transacties per seconde. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Dit is een kaart van het volledige Lightning Network. Dankzij duizenden Lightning-nodebeheerders kun je sats sturen naar elke gebruiker met een Bitcoin Lightning-wallet, waar ter wereld ze zich ook bevinden. De betaling komt binnen enkele seconden aan en kost slechts een paar cent.

**Probeer het zelf uit!**


---


#### Activiteit: Lightning Estafette

https://qr.myfirstbitcoin.org/lightning.pdf

**Dit is een praktische oefening waarbij studenten echte sats versturen en ontvangen via het Lightning Network.**

###### Belangrijke punten

1. Door een Lightning-wallet te gebruiken, krijg je meer vertrouwen in het ontvangen en versturen van echte sats.
1. Let op de eenheden. Sommige wallets laten gebruikers bitcoin OF sats versturen (1/100.000.000 van een bitcoin).
1. Lightning-betalingen kunnen soms vastlopen bij het routeren, vooral bij grotere betalingen. Hoewel dit mogelijk is, komt deze gebruikerservaring steeds minder vaak voor naarmate het netwerk volwassener wordt.

###### Studententip

Controleer bij je docent of/en hoe de huidige on-chain Bitcoin-transactiekosten invloed hebben op de specifieke Lightning-wallet die je gebruikt.
