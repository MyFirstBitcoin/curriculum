# 7.1 Het Lightning Network

Het Lightning Network is een betalingssysteem waarmee gebruikers snel en goedkoop bitcoin kunnen verzenden en ontvangen. Het werkt door een gedeelde portemonnee in te stellen waarin beide partijen een deel van hun bitcoin opslaan. Vervolgens kunnen ze onbeperkt transacties met elkaar uitvoeren zonder dat elke transactie op de hoofdblockchain hoeft te worden vastgelegd. Hierdoor hoeven ze niet elke afzonderlijke transactie te verifiëren en in een blok op te nemen, wat het proces zowel snel als kosteneffectief maakt. Door de lagere kosten kan het Lightning Network worden gebruikt voor kleine betalingen die on-chain niet altijd haalbaar zijn. Zodra de partijen besluiten hun samenwerking te beëindigen, wordt alleen het eindsaldo op de blockchain vastgelegd.

Stel je eens voor dat je een dag in een café werkt. Omdat je van plan bent om een tijdje te blijven, open je een rekening en betaal je vooraf in plaats van per bestelling te betalen. Aan het einde van de dag nemen jij en de eigenaar de rekening door om de afrekening te regelen. Als je storting hoger is dan wat je hebt uitgegeven, krijg je het verschil terug; als je meer hebt uitgegeven, betaal je het resterende bedrag.

Dit systeem kan worden uitgebreid naar meer deelnemers. Stel bijvoorbeeld dat je tijdens een van je bezoekjes aan het café een vriend meeneemt die de barman niet kent en voor wie hij dus geen rekening kan openen. Je biedt je vrienden je bestaande rekening aan om hun uitgaven te dekken, en spreekt af dat ze je privé terugbetalen. Stel je nu eens voor dat duizenden mensen tegelijkertijd hetzelfde doen, waardoor anderen bestaande rekeningen kunnen gebruiken om met nog meer mensen in contact te komen — dat bewijst dat het Lightning Network werkt!

Met Lightning kun je betalingen doen aan iedereen op het netwerk, niet alleen aan de persoon met wie je een directe verbinding hebt — mits er een route tussen beide partijen kan worden gevonden. Je betaling kan zich een weg banen door het netwerk totdat deze zijn bestemming bereikt, zelfs als je geen directe verbinding hebt met de ontvanger.

Laten we eens kijken naar het verschil tussen on-chain- en off-chain-transacties.

##### Transacties op de blockchain

Dit zijn transacties die rechtstreeks op de Bitcoin-blockchain plaatsvinden. Het duurt ongeveer 10 minuten voordat ze zijn bevestigd, en de kosten zijn afhankelijk van de omvang van de transactie in virtuele bytes. Ze zijn veiliger maar trager, omdat ze de consensus van het netwerk vereisen.

##### Transacties via het Lightning Network

Deze transacties vinden plaats op een apart netwerk dat bovenop de Bitcoin-blockchain is gebouwd. Ze worden sneller afgewikkeld en tegen lagere kosten. Ze worden vaak gebruikt wanneer factoren als de snelheid en de kosten van transacties belangrijker zijn. In vergelijking met on-chain-transacties zijn ze minder veilig.


|  | Bitcoin-netwerk | Lightning Network |
| --- | --- | --- |
| Definitie | Een gedecentraliseerd digitaal netwerk dat cryptografie gebruikt om financiële transacties te beveiligen. | Een betalingsprotocol op het tweede niveau dat bovenop de Bitcoin-blockchain draait en snellere en goedkopere transacties mogelijk maakt. |
| Voordelen | Gedecentraliseerd en veilig. Geen terugboekingen of fraude. Kan pseudoniem worden gebruikt. Wereldwijd geaccepteerd. | Snellere en goedkopere transacties. Betere schaalbaarheid. Off-chain-transacties zorgen niet voor overbelasting van de blockchain. |
| Nadelen | Trage verwerkingstijden. Hoge kosten voor bepaalde soorten transacties. Ingewikkeld voor beginners. | Vereist mogelijk vertrouwen in de kanaalbeheerders. Er is een on-chain-transactie nodig om kanalen te openen en te sluiten. |
