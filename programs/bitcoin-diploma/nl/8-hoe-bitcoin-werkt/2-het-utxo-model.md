# 8.2 Het UTXO-model

##### Wat zijn UTXO's?

Laat je niet afschrikken door de vreemde naam. Je kunt UTXO's zien als stukjes bitcoin, vergelijkbaar met de biljetten en munten in je portemonnee. Bijvoorbeeld, als je een artikel van €6 betaalt met een biljet van €10, krijg je €4 terug als wisselgeld. Bitcoin werkt op een vergelijkbare manier.

Alle bitcoin die je bezit, bestaat uit verschillende UTXO's. Wanneer je bitcoin verstuurt, gebruikt je wallet een of meer van deze stukjes om de betaling te doen.

Als het stukje dat je uitgeeft groter is dan het bedrag dat je verstuurt, komt de resterende waarde als wisselgeld terug naar jou in de vorm van een nieuwe UTXO. Tegelijkertijd ontvangt de ontvanger een nieuwe UTXO die de door jou verstuurde bitcoin vertegenwoordigt.

Het saldo van je wallet is simpelweg de totale waarde van alle UTXO's die je beheert.


> **Callout – Privacy**
>
> Het is belangrijk om te weten dat je anderen niet op de hoogte moet brengen van jouw UTXO's, want als iemand ze kent, kan diegene je transacties volgen en uiteindelijk weten hoeveel geld je bezit.


###### Voorbeeld

1. Alice wil 5 BTC naar Bob sturen.
1. Haar wallet gebruikt twee van haar UTXO's die samen 6 BTC waard zijn.
1. De transactie stuurt **5 BTC naar Bob**, waarmee een nieuwe UTXO in Bob's wallet wordt aangemaakt.
1. De resterende **0,99 BTC komt als wisselgeld terug naar Alice**, na het betalen van een **0,01 BTC transactiekosten**.
1. Zodra de transactie is bevestigd, wordt deze toegevoegd aan het grootboek van Bitcoin en worden de door Alice gebruikte UTXO's als uitgegeven gemarkeerd, zodat ze niet opnieuw kunnen worden gebruikt.

###### Bronnen


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
