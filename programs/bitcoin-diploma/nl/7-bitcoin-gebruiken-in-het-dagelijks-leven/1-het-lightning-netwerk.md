# 7.1 Het Lightning-netwerk

Het Lightning Network is een betalingssysteem waarmee gebruikers snel en goedkoop bitcoin kunnen versturen en ontvangen. Het werkt door een gedeelde portemonnee op te zetten waarin beide partijen een deel van hun bitcoin plaatsen. Vervolgens kunnen ze onbeperkt transacties met elkaar doen zonder dat elke transactie op de hoofd-blockchain hoeft te worden vastgelegd. Zo omzeilen ze de noodzaak om elke afzonderlijke transactie te verifiëren en in een blok op te nemen, wat het proces zowel snel als kosteneffectief maakt. Door de lagere kosten kan het Lightning Network worden gebruikt voor kleine betalingen die op de blockchain niet altijd haalbaar zijn. Zodra de partijen besluiten hun samenwerking te beëindigen, wordt alleen het eindsaldo op de blockchain vastgelegd.

Stel je een dag voor waarop je in een café werkt. Je bent van plan om een tijdje te blijven, dus je opent een rekening en betaalt vooraf in plaats van bij elke bestelling apart af te rekenen. Aan het einde van de dag bekijken jij en de eigenaar samen de rekening om de balans op te maken. Als je aanbetaling hoger is dan wat je hebt uitgegeven, krijg je het verschil terug; als je meer hebt uitgegeven, betaal je het resterende bedrag bij.

Dit systeem kan opgeschaald worden naar meer deelnemers. Stel bijvoorbeeld dat je tijdens een van je bezoeken aan het café een vriend meeneemt die de barman niet kent en voor wie geen rekening kan worden geopend. Je biedt je vriend aan om jouw bestaande rekening te gebruiken voor zijn uitgaven, en spreekt af dat hij jou privé terugbetaalt. Stel je nu voor dat duizenden mensen dit tegelijkertijd doen, waardoor anderen bestaande rekeningen kunnen gebruiken om met nog meer mensen te verbinden — zo werkt het Lightning Network!

Met Lightning kun je betalingen doen aan iedereen op het netwerk, niet alleen aan degene met wie je direct een rekening deelt — zolang er maar een route tussen beide partijen gevonden kan worden. Je betaling kan via het netwerk zijn weg vinden tot aan de ontvanger, zelfs als je niet direct een open kanaal met die persoon hebt.

Laten we eens kijken naar het verschil tussen on-chain en off-chain transacties.

##### On-chain transacties

Dit zijn transacties die direct op de Bitcoin-blockchain plaatsvinden. Ze nemen ongeveer 10 minuten om bevestigd te worden, en de kosten hangen af van de grootte van de transactie in virtuele bytes. Ze zijn veiliger maar langzamer, omdat ze het netwerkbrede consensus vereisen.

##### Lightning Network-transacties

Deze transacties vinden plaats op een apart netwerk dat bovenop de Bitcoin-blockchain is gebouwd. Ze worden sneller en met lagere kosten afgehandeld. Ze worden vaak gebruikt wanneer snelheid en kosten belangrijker zijn dan andere overwegingen. In vergelijking met on-chain transacties zijn ze minder veilig.


|  | Bitcoin-netwerk | Lightning Network |
| --- | --- | --- |
| Definitie | Een gedecentraliseerd digitaal netwerk dat cryptografie gebruikt om financiële transacties te beveiligen. | Een betalingsprotocol als tweede laag dat bovenop de Bitcoin-blockchain werkt en snellere en goedkopere transacties mogelijk maakt. |
| Voordelen | Gedecentraliseerd en veilig. Geen terugboekingen of fraude. Kan pseudoniem worden gebruikt. Wereldwijde acceptatie. | Snellere en goedkopere transacties. Grotere schaalbaarheid. Off-chain transacties verstoppen de blockchain niet. |
| Nadelen | Langzame transactietijden. Hoge kosten voor bepaalde soorten transacties. Complex voor beginners. | Kan vertrouwen vereisen in de kanaalbeheerders. Vereist een on-chain transactie om kanalen te openen en te sluiten. |
