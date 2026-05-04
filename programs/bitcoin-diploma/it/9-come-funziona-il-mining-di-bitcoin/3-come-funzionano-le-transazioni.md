# 9.3 Come funzionano le transazioni

Ora che hai compreso le chiavi pubbliche e private, così come i ruoli dei nodi e dei miner, ecco come funziona una transazione Bitcoin dall'inizio alla fine.

1. Adam vuole inviare bitcoin a Giovanni. Crea una transazione con l'indirizzo di Giovanni, l'importo da inviare e una commissione.
1. Adam firma la transazione con la sua chiave privata per dimostrare la proprietà.
1. Trasmette la transazione alla rete Bitcoin.
1. I nodi la ricevono e verificano che rispetti le regole, inclusa la verifica della firma e che Adam abbia abbastanza bitcoin.
1. Se valida, la transazione viene condivisa in tutta la rete e aggiunta al mempool, dove le transazioni in attesa aspettano.
1. I miner scelgono le transazioni dal mempool e le includono in un blocco che cercano di minare.
1. Quando un miner riesce a minare un blocco, questo viene condiviso con la rete e controllato dagli altri nodi.
1. Se valido, il blocco viene aggiunto alla blockchain. Giovanni riceve i bitcoin.
1. Man mano che vengono aggiunti altri blocchi, la transazione ottiene conferme, diventando più sicura.

Una volta inclusa in un blocco, la transazione è confermata. Adam non può più spendere quei bitcoin e Giovanni può spendere ciò che ha ricevuto in una nuova transazione.


> **Note**
>
> Transazione e commissione selezionate → Firmata dal wallet e inviata → Distribuita dai nodi → Il miner aggiunge la transazione al modello di blocco → Il miner vince la gara di Proof-of-Work → Il nuovo blocco viene validato → Il nuovo blocco viene distribuito dai nodi


###### Risorse


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
