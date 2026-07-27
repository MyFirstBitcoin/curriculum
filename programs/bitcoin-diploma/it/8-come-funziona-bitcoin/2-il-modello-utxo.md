# 8.2 Il modello UTXO

##### Cosa sono gli UTXO?

Non lasciarti intimidire dal nome strano. Puoi pensare agli UTXO come a dei pezzi di bitcoin, simili alle banconote e alle monete nel tuo portafoglio. Ad esempio, se paghi un oggetto da 6 € con una banconota da 10 €, ricevi 4 € di resto. Bitcoin funziona in modo simile.

Tutti i bitcoin che possiedi sono composti da diversi UTXO. Quando invii bitcoin, il tuo portafoglio utilizza uno o più di questi pezzi per effettuare il pagamento.

Se il pezzo che spendi è più grande dell'importo che invii, il valore rimanente ti torna come resto sotto forma di un nuovo UTXO. Allo stesso tempo, il destinatario riceve un nuovo UTXO che rappresenta i bitcoin che hai inviato.

Il saldo del tuo portafoglio è semplicemente il valore totale di tutti gli UTXO che controlli.


> **Callout – Privacy**
>
> Non dovresti rendere noti i tuoi UTXO agli altri perché, se qualcuno li conosce, può tracciare le tue transazioni e alla fine sapere quanti soldi possiedi.


###### Esempio

1. Giovanni vuole inviare 5 BTC a Luca.
1. Il suo portafoglio utilizza due dei suoi UTXO che insieme valgono 6 BTC.
1. La transazione invia **5 BTC a Luca**, creando un nuovo UTXO nel portafoglio di Luca.
1. Il resto di **0,99 BTC torna a Giovanni come resto**, dopo aver pagato una **commissione di transazione di 0,01 BTC**.
1. Una volta che la transazione è confermata, viene aggiunta al registro di Bitcoin e gli UTXO utilizzati da Giovanni vengono segnati come spesi, quindi non possono essere usati di nuovo.

###### Risorse


[▶ Guarda “How Bitcoin Works under the Hood”](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
