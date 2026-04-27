# 8.2 Het UTXO-model

##### Wat zijn UTXO's?

Laat je niet afschrikken door de vreemde naam. Je kunt UTXO's zien als stukjes bitcoin, vergelijkbaar met de biljetten en munten in je portemonnee. Stel, je betaalt een artikel van €6 met een biljet van €10, dan krijg je €4 terug als wisselgeld. Bitcoin werkt op een vergelijkbare manier.

Alle bitcoin die je bezit bestaat uit verschillende UTXO's. Wanneer je bitcoin verstuurt, gebruikt je portemonnee een of meer van deze stukjes om de betaling te doen.

Als het stukje dat je uitgeeft groter is dan het bedrag dat je verstuurt, komt de resterende waarde als wisselgeld terug naar jou in de vorm van een nieuwe UTXO. Tegelijkertijd ontvangt de ontvanger een nieuwe UTXO die de door jou verstuurde bitcoin vertegenwoordigt.

Het saldo van je portemonnee is simpelweg de totale waarde van alle UTXO's die jij beheert.


> **Callout – Privacy**
>
> Je moet anderen niet op de hoogte brengen van jouw UTXO's, want als iemand ze kent, kan diegene je transacties volgen en uiteindelijk weten hoeveel geld je bezit.


###### Voorbeeld

1. Anna wil 5 BTC naar Bas sturen.
1. Haar portemonnee gebruikt twee van haar UTXO's die samen 6 BTC waard zijn.
1. De transactie stuurt **5 BTC naar Bas**, waarmee een nieuwe UTXO in Bas' portemonnee wordt aangemaakt.
1. De resterende **0,99 BTC komt als wisselgeld terug naar Anna**, na het betalen van een **0,01 BTC transactiekost**.
1. Zodra de transactie is bevestigd, wordt deze toegevoegd aan het grootboek van Bitcoin en worden de door Anna gebruikte UTXO's als uitgegeven gemarkeerd, zodat ze niet opnieuw gebruikt kunnen worden.

###### Bronnen


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
