# 8.2 Het UTXO-model

##### Wat zijn UTXO's?

Laat je niet afschrikken door de vreemde naam. Je kunt UTXO’s zien als stukjes bitcoin, net als de biljetten en munten in je portemonnee. Als je bijvoorbeeld een artikel van $6 betaalt met een biljet van $10, krijg je $4 wisselgeld terug. Bitcoin werkt op een vergelijkbare manier.

Alle bitcoin die je bezit, bestaat uit verschillende UTXO’s. Wanneer je bitcoin verstuurt, gebruikt je wallet een of meer van deze eenheden om de betaling uit te voeren.

Als het bedrag dat je uitgeeft hoger is dan het bedrag dat je verstuurt, krijg je het resterende bedrag als wisselgeld terug in de vorm van een nieuwe UTXO. Tegelijkertijd ontvangt de ontvanger een nieuwe UTXO die de door jou verstuurde bitcoin vertegenwoordigt.

Het saldo van je portemonnee is simpelweg de totale waarde van alle UTXO’s waarover je beschikt.


> **Callout – Privacy**
>
> Je moet je UTXO’s niet aan anderen bekendmaken, want als iemand ze kent, kan diegene je transacties volgen en uiteindelijk te weten komen hoeveel geld je bezit.


###### Voorbeeld

1. Alice wil Bob 5 BTC sturen.
1. Haar portemonnee gebruikt twee van haar UTXO’s die samen 6 BTC waard zijn.
1. De transactie verzendt **5 BTC naar Bob**, waardoor er een nieuwe UTXO in de portemonnee van Bob wordt aangemaakt.
1. De overige **0,99 BTC wordt als wisselgeld aan Alice teruggegeven**, na betaling van een **0,01 BTC transactiekosten**.
1. Zodra de transactie is bevestigd, wordt deze toegevoegd aan het grootboek van Bitcoin en worden de door Alice gebruikte UTXO’s gemarkeerd als ‘uitgegeven’, zodat ze niet opnieuw kunnen worden gebruikt.

###### Bronnen


[▶ Bekijk ‘Hoe Bitcoin onder de motorkap werkt’](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
