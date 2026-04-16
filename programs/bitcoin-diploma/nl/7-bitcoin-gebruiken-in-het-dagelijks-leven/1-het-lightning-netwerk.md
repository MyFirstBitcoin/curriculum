# 7.1 Het Lightning-netwerk

Het Lightning Network is een betalingssysteem waarmee gebruikers snel en goedkoop bitcoin kunnen verzenden en ontvangen. Het werkt door een gedeelde portemonnee op te zetten waarin beide partijen een deel van hun bitcoin opslaan. Vervolgens kunnen ze onbeperkt transacties met elkaar uitvoeren zonder dat elke transactie op de hoofd-blockchain hoeft te worden vastgelegd. Op deze manier omzeilen ze de noodzaak om elke afzonderlijke transactie te verifiëren en in een blok op te nemen, wat het proces zowel snel als kosteneffectief maakt. De lagere kosten betekenen dat het Lightning Network gebruikt kan worden voor kleine betalingen die op de blockchain zelf niet altijd haalbaar zijn. Zodra de partijen besluiten hun samenwerking te beëindigen, wordt alleen het eindsaldo op de blockchain geregistreerd.

Stel je een dag werken in een café voor. Je bent van plan een tijdje te blijven, dus je opent een rekening en betaalt vooraf in plaats van bij elke bestelling apart te betalen. Aan het einde van de dag bekijken jij en de eigenaar samen de rekening om de eindafrekening te maken. Als je aanbetaling hoger is dan wat je hebt uitgegeven, krijg je het verschil terug; als je meer hebt uitgegeven, betaal je het resterende bedrag.

Dit systeem kan opgeschaald worden om meer deelnemers te omvatten. Bijvoorbeeld: tijdens een van je bezoeken aan het café neem je een vriend mee die de barman niet kent en voor wie geen rekening geopend kan worden. Jij biedt je vriend aan om jouw bestaande rekening te gebruiken voor hun uitgaven, en spreekt af dat zij jou privé terugbetalen. Stel je nu voor dat duizenden mensen dit tegelijkertijd doen, waardoor anderen bestaande rekeningen kunnen gebruiken om met nog meer mensen te verbinden — zo werkt het Lightning Network!

Met Lightning kun je betalingen doen aan iedereen op het netwerk, niet alleen aan de persoon met wie je direct een rekening deelt — zolang er maar een route tussen beide partijen gevonden kan worden. Je betaling kan door het netwerk navigeren totdat deze de bestemming bereikt, zelfs als je geen open kanaal hebt met de ontvanger.

Laten we eens kijken naar het verschil tussen on-chain en off-chain transacties.

##### On-chain transacties

Dit zijn transacties die direct op de Bitcoin-blockchain plaatsvinden. Ze nemen ongeveer 10 minuten om te bevestigen, en de kosten hangen af van de grootte van de transactie in virtuele bytes. Ze zijn veiliger maar trager, omdat ze het consensus van het netwerk vereisen.

##### Lightning Network-transacties

Deze transacties vinden plaats op een apart netwerk dat bovenop de Bitcoin-blockchain is gebouwd. Ze worden sneller en met lagere kosten afgehandeld. Ze worden vaak gebruikt wanneer factoren als snelheid en kosten van transacties belangrijker zijn. In vergelijking met on-chain transacties zijn ze minder veilig.


|  | Bitcoin-netwerk | Lightning-netwerk |
| --- | --- | --- |
| Definitie | Een gedecentraliseerd digitaal netwerk dat cryptografie gebruikt om financiële transacties te beveiligen. | Een betalingsprotocol als tweede laag dat bovenop de Bitcoin-blockchain werkt en snellere en goedkopere transacties mogelijk maakt. |
| Voordelen | Gedecentraliseerd en veilig. Geen terugboekingen of fraude. Kan pseudoniem gebruikt worden. Wereldwijde acceptatie. | Snellere en goedkopere transacties. Grotere schaalbaarheid. Off-chain transacties verstoppen de blockchain niet. |
| Nadelen | Trage transactietijden. Hoge kosten voor bepaalde soorten transacties. Complex voor beginners. | Kan vertrouwen vereisen in de kanaalbeheerders. Vereist een on-chain transactie om kanalen te openen en te sluiten. |
