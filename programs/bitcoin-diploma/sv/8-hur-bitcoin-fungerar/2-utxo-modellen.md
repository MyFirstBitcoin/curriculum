# 8.2 UTXO-modellen

##### Vad är UTXO:er?

Låt dig inte skrämmas av det konstiga namnet. Du kan tänka på UTXO:er som bitar av bitcoin, liknande sedlar och mynt i din plånbok. Till exempel, om du betalar för en vara som kostar 60 kr med en 100-kronorssedel, får du 40 kr i växel. Bitcoin fungerar på ett liknande sätt.

Alla bitcoin du äger består av olika UTXO:er. När du skickar bitcoin använder din plånbok en eller flera av dessa delar för att genomföra betalningen.

Om den del du spenderar är större än beloppet du skickar, kommer det återstående värdet tillbaka till dig som växel i form av en ny UTXO. Samtidigt får mottagaren en ny UTXO som representerar de bitcoin du skickade.

Din plånboks saldo är helt enkelt det totala värdet av alla UTXO:er du kontrollerar.


> **Callout – Integritet**
>
> Du bör inte låta andra känna till dina UTXO:er, eftersom om någon känner till dem kan de spåra dina transaktioner och till slut veta hur mycket pengar du äger.


###### Exempel

1. Anna vill skicka 5 BTC till Erik.
1. Hennes plånbok använder två av hennes UTXO:er som tillsammans är värda 6 BTC.
1. Transaktionen skickar **5 BTC till Erik**, vilket skapar en ny UTXO i Eriks plånbok.
1. De återstående **0,99 BTC går tillbaka till Anna som växel**, efter att ha betalat en **0,01 BTC transaktionsavgift**.
1. När transaktionen är bekräftad läggs den till i Bitcoins huvudbok och de UTXO:er som användes av Anna markeras som spenderade, så de inte kan användas igen.

###### Resurser


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
