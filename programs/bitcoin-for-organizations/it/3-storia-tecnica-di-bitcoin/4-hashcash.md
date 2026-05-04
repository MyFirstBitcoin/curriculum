# 3.4 Hashcash

Hashcash è stato creato da Adam Back, un altro dei primi innovatori in questo campo. Adam aveva un forte interesse per i mercati liberi e la privacy su internet, e si imbatté nella mailing list dei Cypherpunk, alla quale si iscrisse diventando un partecipante attivo.

Era molto interessato al denaro digitale e fece alcune proposte su come il gruppo potesse eventualmente collaborare più strettamente su DigiCash con Chaum, ma queste non portarono a nulla. Poi rivolse la sua attenzione a un altro problema emergente: lo spam via email. Lui e gli altri Cypherpunk volevano trovare una soluzione al problema dello spam, dove per gli spammer era banale creare e inviare migliaia di email che intasavano le reti. La sua soluzione innovativa si basava sull'hashing: la capacità, tramite la crittografia, di trasformare qualsiasi dato in una stringa unica e casuale di una lunghezza specifica, per creare l'equivalente di un 'francobollo' digitale che doveva essere aggiunto all'email affinché fosse considerata valida e trasmessa attraverso la rete. Un costo trascurabile per una email autentica, ma proibitivo per uno spammer.

La principale innovazione introdotta da Hashcash fu quella di collegare risorse del mondo reale – la potenza computazionale – a una rete digitale. Fino a quel momento, le risorse digitali potevano essere replicate senza limiti, ma il numero di 'hashcash' creati era limitato da quanta energia le persone erano disposte a investire.

Anche se la soluzione soddisfaceva alcuni dei criteri che Adam riteneva necessari in un sistema di denaro digitale – era anonima, resiliente e trustless – ogni hashcash non era riutilizzabile e non era veramente scarso. Suggerì altri modi in cui questi problemi potevano essere affrontati utilizzando terze parti esterne.

##### BitGold

Nick Szabo sviluppò il concetto di Hashcash e della proof of work per proporre una soluzione alternativa, che descrisse in una mailing list un anno dopo la pubblicazione di Hashcash, nel 1998.

Pur avvicinandosi a una soluzione, questa proposta presentava ancora diverse sfide.

* Chi gestirebbe il Registro della proprietà degli hash e come potrebbe essere considerato affidabile?
* L'hashing generalmente sarebbe diventato più economico nel tempo, una sfida anche per HashCash.

Poiché gli hash collegati sarebbero stati marcati temporalmente, propose una sorta di tracciamento storico della difficoltà dell'hashing nel tempo; un hash precedente avrebbe richiesto più costi di elaborazione rispetto a uno successivo, dato che i costi sarebbero diminuiti. Sfortunatamente, ciò significava che gli hash non sarebbero stati 'fungibili', cioè di valore uguale, considerato un attributo chiave del denaro digitale. Per aiutare a risolvere questo problema, Nick suggerì una sorta di 'free banking' che operasse sopra BitGold e potesse aggregare diversi gruppi di hash valutati allo stesso modo.

##### B-Money

Poco dopo la proposta di Bit Gold, Wei Dai propose una soluzione simile. Aveva già sviluppato diversi altri strumenti per i Cypherpunk e aveva idee proprie sul denaro digitale.

La sua proposta somigliava a Bit Gold in quanto utilizzava firme digitali per trasferire denaro, e i registri delle transazioni sarebbero stati conservati su un libro mastro, contenente chiavi pubbliche e la quantità di unità di valuta attribuite a ciascuna. Come per Bit-Gold, le terze parti fidate erano considerate punti deboli per la sicurezza, e si riteneva che un sistema di denaro elettronico non dovesse dipendere da un'unica entità per tracciare i saldi, le transazioni o per prevenire la doppia spesa.

Wei Dai propose diverse soluzioni a questi problemi, una delle quali era che, invece di un'entità centrale che mantenesse il libro mastro, TUTTI i nodi ne avrebbero mantenuto una copia. Se tutti gli utenti controllavano il proprio libro mastro e la validità di ogni transazione, finché tutti i nodi rimanevano aggiornati, i libri mastri sarebbero rimasti sincronizzati in tutta la rete. Questo sistema altamente distribuito sarebbe stato difficile da corrompere.

Wei Dai riconobbe che ciò non risolveva il problema dei generali bizantini (1), poiché i nodi potevano facilmente perdere la sincronizzazione o semplicemente mentire. Suggerì metodi alternativi come avere un sottoinsieme di server 'fidati' che mantenessero il libro mastro e creare incentivi economici per mantenere questi server onesti.

Per la politica monetaria, propose di ancorare il potere d'acquisto di B-Money a una sorta di indice dei prezzi al consumo esterno. Voleva che la stessa quantità di B-Money potesse acquistare una quota uguale dell'indice nel tempo, fornendo una certa stabilità dei prezzi. Quindi, chiunque poteva generare nuove unità di valuta fornendo un hash valido, ma la difficoltà di generare un hash poteva cambiare nel tempo in base ai costi della CPU e all'indice dei prezzi, così che ogni unità sarebbe stata 'immutabile'.
