# 6.4 Ricevere e inviare transazioni

Una transazione Bitcoin è un trasferimento di proprietà di bitcoin a un nuovo proprietario. Nota che non sono le monete vere e proprie a essere trasferite, ma la proprietà di esse: in altre parole, il diritto di spenderle. Ogni volta che una transazione viene accettata in un blocco, tutti i nodi della rete aggiornano la loro copia locale del registro pubblico per riflettere il cambiamento di proprietà. Sotto questo aspetto, una transazione Bitcoin è più simile a una transazione immobiliare (o di altra proprietà) che a una transazione in contanti.

Per "inviare" bitcoin, il mittente firma un messaggio con la propria chiave privata, segnalando alla rete che il legittimo proprietario dei bitcoin ha trasferito la proprietà al destinatario.

Ora i bitcoin saranno collegati all'indirizzo del destinatario, dandogli la proprietà dei bitcoin, così che solo il nuovo proprietario potrà spenderli utilizzando la propria chiave privata.

Le nuove transazioni Bitcoin vengono avviate da wallet in tutto il mondo, ma non esiste un processore di pagamento centrale. Invece, i miner competono per registrare le transazioni nel registro.

Supponiamo che Giovanni debba 0,5 BTC a Eliana ed è pronto a restituirglieli. Entrambi hanno dei wallet digitali.

1. Eliana condivide il suo indirizzo con Giovanni.
1. Giovanni utilizza il software del suo wallet per creare la transazione, che include l'indirizzo di Eliana, l'importo da trasferire (0,5 BTC) e una commissione per il miner. Commissioni più alte rendono più probabile che un miner includa la transazione nel prossimo blocco.
1. Dopo aver firmato la transazione, questa viene trasmessa alla rete, dove viene verificata dai nodi. Essi controllano se Giovanni ha fondi sufficienti ed è il legittimo proprietario delle monete che intende spendere. Se non lo è, la transazione viene immediatamente rifiutata.
1. Una volta che la transazione è stata verificata, i miner scelgono se aggiungerla al prossimo blocco, di solito in base alla commissione selezionata. Quando la transazione viene inclusa in un blocco, viene aggiunta alla blockchain e i fondi vengono trasferiti all'indirizzo di Eliana.
1. La proprietà è stata trasferita a Eliana. Ora può usare la sua chiave privata per spendere i fondi.

_È importante notare che una volta completata la transazione, non può essere annullata._


> **Note – Come funziona una transazione Bitcoin**
>
> 1. Qualcuno richiede una transazione
> 1. La transazione viene trasmessa ai computer P2P (nodi)
> 1. I miner verificano la transazione
> 1. Le transazioni vengono combinate per formare un blocco di dati
> 1. Il nuovo blocco viene aggiunto alla blockchain esistente
> 1. La transazione è completa



> **Note – Ricevere transazioni Bitcoin**
>
> Per ricevere bitcoin, dovrai fornire al mittente un indirizzo pubblico Bitcoin. Si tratta di una stringa unica di lettere e numeri che rappresenta il tuo wallet e viene utilizzata per identificarlo sulla rete Bitcoin.
>
> Puoi trovare il tuo indirizzo pubblico aprendo il tuo wallet Bitcoin e cercando un'opzione per “Ricevere” o “Deposita” bitcoin.
>
> Puoi quindi condividere il tuo indirizzo Bitcoin in diversi modi:
>
> 1. **Copia e incolla l'indirizzo**: Puoi copiare l'indirizzo selezionandolo e premendo "Copia", quindi incollarlo in una email o in un messaggio.
> 1. **Condividi un link al tuo wallet Bitcoin**: Alcuni wallet Bitcoin ti permettono di creare un link al tuo wallet che puoi condividere con il mittente. Potrà quindi cliccare sul link per accedere al tuo wallet e inviarti bitcoin.
> 1. **Condividi un codice QR**: Se il mittente ha uno smartphone con un'app wallet Bitcoin installata, può scansionare il codice QR per ottenere il tuo indirizzo Bitcoin.


Una volta che il mittente ha il tuo indirizzo, può inviarti bitcoin inserendo il tuo indirizzo e l'importo che desidera inviare. I bitcoin vengono quindi inviati dal suo wallet al tuo.

La transazione viene confermata dalla rete Bitcoin e di solito richiede circa 10 minuti. Per maggiore sicurezza, si consiglia di attendere due conferme, che richiedono circa 20 minuti.


> **Note – Inviare transazioni Bitcoin**
>
> Per inviare bitcoin, ti serviranno alcune cose: un wallet Bitcoin, l'indirizzo pubblico del destinatario e l'importo di bitcoin che vuoi inviare.
>
> 1. Apri il tuo wallet Bitcoin.
> 1. Vai al pulsante “Invia” e incolla l'indirizzo del destinatario nel campo "A". In alternativa, puoi anche scansionare il codice QR se il destinatario ne fornisce uno.
> 1. Inserisci l'importo di bitcoin che vuoi inviare nel campo “Importo”.
> 1. Controlla attentamente l'indirizzo del destinatario e l'importo da inviare. Ricorda che le transazioni sono irreversibili!
> 1. Prima di cliccare su “Conferma e Invia”, ti consigliamo di ricontrollare ancora una volta i dettagli della transazione per assicurarti di inviare la quantità corretta di bitcoin all'indirizzo giusto.
> 1. Trasmetti la transazione e attendi che la rete confermi la transazione.
>
> Ora sai come valutare, selezionare e configurare un wallet Bitcoin self-custodial. L'invio e la ricezione di bitcoin sulla rete Bitcoin sono chiamati transazioni “on-chain”. Questo perché le transazioni avvengono sulla rete principale di Bitcoin e vengono registrate nella blockchain.
>
> Le transazioni on-chain sono il modo più sicuro per effettuare transazioni con bitcoin grazie alla verifica decentralizzata fornita dalla rete.
>
> Tuttavia, le transazioni on-chain sono più lente e possono essere significativamente più costose rispetto ad altre opzioni (di cui parleremo nel Modulo 7) a causa della commissione per i miner.


#### Attività: Le transazioni in pratica

https://qr.myfirstbitcoin.org/transactions.pdf

**Questo è un esercizio cooperativo che semplifica i ruoli di base delle persone coinvolte in una transazione Bitcoin.**

###### Punti chiave

1. Ci sono quattro tipi di partecipanti in ogni transazione bitcoin: il mittente, il destinatario, i miner e gli operatori dei nodi.
1. Il mittente deve approvare (firmare crittograficamente) l'**importo di bitcoin** da inviare E l'**indirizzo specifico** a cui inviare.
1. Il destinatario deve fornire un **indirizzo valido** al mittente E verificare che la transazione sia stata confermata con successo sulla blockchain.
1. I miner si assicurano che tutti i criteri siano validi prima di aggiungere le transazioni ai blocchi futuri.
1. Gli operatori dei nodi verificano che i blocchi minati siano validi prima di aggiornare la loro versione della blockchain (il registro).

###### Suggerimento per lo studente

Ruota tra tutti e quattro i ruoli per sperimentare cosa fa ciascun partecipante.
