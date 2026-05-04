# 7.1 La Lightning Network

Il Lightning Network è un sistema di pagamento che permette agli utenti di inviare e ricevere bitcoin in modo rapido ed economico. Funziona creando un portafoglio condiviso dove entrambe le parti depositano una parte dei loro bitcoin. In questo modo, possono effettuare un numero illimitato di transazioni tra di loro senza dover registrare ognuna sulla blockchain principale. Così facendo, si evita la necessità di verificare e includere ogni singola transazione in un blocco, rendendo il processo sia veloce che conveniente. Le commissioni più basse permettono di utilizzare il Lightning Network anche per piccoli pagamenti che non sono sempre convenienti sulla blockchain. Quando le parti decidono di terminare la loro collaborazione, solo il saldo finale viene registrato sulla blockchain.

Immagina una giornata di lavoro in un bar. Decidendo di fermarti a lungo, apri un conto e paghi in anticipo invece di pagare ogni singolo ordine. Alla fine della giornata, tu e il proprietario controllate il conto per saldare il totale. Se il tuo deposito è superiore a quanto hai speso, ricevi indietro la differenza; se hai speso di più, paghi quello che ancora devi.

Questo sistema può essere ampliato per includere più partecipanti. Ad esempio, in una delle tue visite al bar, porti un amico che il barista non conosce e a cui non può aprire un conto. Offri al tuo amico di usare il tuo conto per coprire le sue spese, e vi accordate che ti rimborserà in privato. Ora immagina migliaia di persone che fanno la stessa cosa contemporaneamente, permettendo ad altri di usare conti già aperti per collegarsi con ancora più persone — ecco come funziona il Lightning Network!

Con Lightning, puoi effettuare pagamenti a chiunque sulla rete, non solo alla persona con cui hai un conto diretto — a patto che esista un percorso tra le due parti. Il tuo pagamento può attraversare la rete fino a raggiungere la destinazione, anche se non hai un canale aperto direttamente con il destinatario.

Vediamo la differenza tra transazioni on-chain e off-chain.

##### Transazioni On-Chain

Queste sono transazioni che avvengono direttamente sulla blockchain di Bitcoin. Richiedono circa 10 minuti per essere confermate e le commissioni dipendono dalla dimensione della transazione in byte virtuali. Sono più sicure ma più lente, poiché richiedono il consenso della rete.

##### Transazioni Lightning Network

Queste transazioni avvengono su una rete separata costruita sopra la blockchain di Bitcoin. Si regolano più velocemente e con commissioni più basse. Sono comunemente usate quando la velocità e il costo delle transazioni sono più importanti. Rispetto alle transazioni on-chain, sono meno sicure.


|  | Rete Bitcoin | Lightning Network |
| --- | --- | --- |
| Definizione | Una rete digitale decentralizzata che utilizza la crittografia per proteggere le transazioni finanziarie. | Un protocollo di pagamento di secondo livello che opera sopra la blockchain di Bitcoin, permettendo transazioni più veloci ed economiche. |
| Vantaggi | Decentralizzata e sicura. Nessun rischio di chargeback o frode. Può essere usata in modo pseudonimo. Accettazione globale. | Transazioni più veloci ed economiche. Maggiore scalabilità. Le transazioni off-chain non congestionano la blockchain. |
| Svantaggi | Tempi di transazione lenti. Commissioni elevate per alcuni tipi di transazioni. Complessa per i principianti. | Può richiedere fiducia negli operatori dei canali. Richiede una transazione on-chain per aprire e chiudere i canali. |
