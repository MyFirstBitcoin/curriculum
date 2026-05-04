# 9 - Come funziona il mining di Bitcoin

Durata: 90 minuti

Idea centrale: Il mining di Bitcoin e la validazione dei nodi lavorano insieme per proteggere la rete, confermare le transazioni e far rispettare le regole del sistema tramite la Proof of Work.

#### Obiettivi di apprendimento

Al termine di questa lezione, gli studenti dovrebbero essere in grado di:

* Spiegare la differenza tra il ruolo dei nodi Bitcoin e quello dei miner di Bitcoin.
* Descrivere come i nodi validano le transazioni, condividono informazioni e aiutano a far rispettare le regole di Bitcoin.
* Spiegare cosa fanno i miner, inclusa la selezione delle transazioni, la costruzione di blocchi candidati e la competizione per trovare un hash di blocco valido.
* Definire la mempool e spiegare perché funziona come una sala d'attesa per le transazioni non confermate.
* Descrivere come le commissioni di transazione influenzano la selezione da parte dei miner e la velocità di conferma.
* Spiegare la Proof of Work come il meccanismo che protegge Bitcoin rendendo costosi gli attacchi.
* Descrivere come l'aggiustamento della difficoltà aiuta a mantenere un tempo medio di blocco di circa 10 minuti.
* Ripercorrere l'intero ciclo di vita di una transazione Bitcoin, dalla creazione e firma fino alla conferma in un blocco.

#### Strumenti e risorse

##### Supporti visivi

* Capitolo 9 - Come funziona il mining di Bitcoin?

##### Libreria di supporto

* Scheda di riferimento del vocabolario — Capitolo 9 — Termini: mining, Proof of Work, puzzle hash, aggiustamento della difficoltà, ricompensa del blocco, mempool, attacco del 51%
* Librerie di idee sbagliate — Capitolo 9 — Affronta: "i miner creano Bitcoin dal nulla", "i miner controllano Bitcoin", "più mining = meno sicurezza"
* Tabelle di confronto e schede di riferimento — Economia del mining: ricavi, costi, allineamento degli incentivi; aggiustamento della difficoltà
* Spiegazioni tecniche e approfondimenti — Sicurezza della Proof of Work; perché attaccare è costoso; soglia del 51%

#### Attività

* Esplorare la mempool
* Transazioni in azione

#### Didattica online

* Usa un diagramma chiaro del flusso di una transazione, dalla firma nel wallet fino alla conferma.
* Mantieni nodi e miner separati visivamente sullo schermo per tutta la lezione.
* Usa mempool.space o uno screenshot di esso per mostrare le transazioni non confermate e la pressione delle commissioni.
* Fermati dopo ogni fase del processo di mining e poni una breve domanda di comprensione.

#### Preparazione

* Prepara un diagramma del processo di mining (mempool → selezione delle transazioni → creazione del blocco → aggiustamento della difficoltà) da mostrare.
* Salva tra i preferiti mempool.space o la pagina mining di blockchain.com; prepara screenshot delle statistiche attuali del mining e degli aggiustamenti della difficoltà.
* Crea una spiegazione visiva della Proof of Work come meccanismo di sicurezza; mostra l'aggiustamento della difficoltà negli ultimi 3-6 mesi.

#### Procedura

Questa lezione esamina più da vicino come le transazioni Bitcoin si muovono attraverso la rete e diventano parte della blockchain. Ora segue direttamente la struttura del Diploma, così le sezioni principali sono allineate con la guida per gli studenti, pur mantenendo la spiegazione più completa per l'educatore all'interno di ogni sezione.

##### 9.0 Introduzione, 8 minuti

Inizia collegando questo capitolo al precedente:

* Se un utente firma una transazione con una chiave privata, cosa succede dopo?
* Chi controlla se quella transazione è valida?
* Come viene aggiunta alla blockchain?
* Perché Bitcoin ha bisogno sia dei nodi che dei miner?

Chiarisci che questo capitolo spiega come la rete processa le transazioni nella pratica e come il mining protegge il sistema senza un'autorità centrale.

##### 9.1 Nodi e miner di Bitcoin, 47 minuti

**Nodi e miner, ruoli diversi**

Inizia separando chiaramente i due ruoli.

Nodi Bitcoin:

* mantengono una copia della blockchain
* verificano se le transazioni rispettano le regole
* condividono informazioni con altri nodi
* aiutano wallet e altri software ad accedere ai dati della blockchain
* possono rifiutare transazioni o blocchi non validi

Il capitolo descrive i nodi come guardiani della validazione, e amplia questa idea con l'analogia del "vigile digitale". Questo è utile perché mostra i nodi come controllori e coordinatori, non come sovrani. Il diagramma rafforza anche il concetto che molti nodi mantengono copie del registro in tutto il mondo.

I miner di Bitcoin:

* raccolgono transazioni valide
* assemblano blocchi candidati
* competono per trovare un hash di blocco valido
* trasmettono i blocchi validi quando vincono
* ricevono la ricompensa del blocco e le commissioni di transazione

Un punto chiave del capitolo è che lo scopo del mining non è semplicemente creare nuovi bitcoin, ma decentralizzare la sicurezza di Bitcoin. I nuovi bitcoin sono l'incentivo, mentre il processo di mining stesso è il meccanismo di sicurezza.

**Cosa Fanno Realmente i Nodi**

Approfondisci la sezione sui nodi con l'elenco delle funzioni dei nodi presentato nel capitolo:

* Guardiani della validazione: controllano che le transazioni e i blocchi rispettino le regole
* Nodo di comunicazione: si collegano tra loro e condividono i dati delle transazioni
* Controllore di qualità: rifiutano le informazioni non valide
* Informatori della blockchain: forniscono dati ad altri software come i wallet
* Accoglienza dei nuovi nodi: aiutano i nuovi nodi a ottenere la blockchain, mentre ogni nuovo nodo verifica comunque i dati in modo indipendente

Questo è un buon momento per sottolineare che gestire un nodo offre all'utente maggiore indipendenza. Invece di dipendere completamente da servizi esterni per conoscere lo stato della rete, possono verificarlo autonomamente. lo spiega chiaramente, incluso il riferimento a Bitcoin Core come una delle implementazioni che gli utenti possono eseguire.

**Cosa Fanno Realmente i Miner**

Ora spiega il mining in modo più accurato.

I miner:

* raccolgono transazioni verificate ma non ancora confermate
* le raggruppano in un blocco candidato
* eseguono ripetutamente l'hash dei dati del blocco cercando un hash valido
* trasmettono il blocco vincente alla rete
* ottengono ricompense se il blocco viene accettato

Usa l'analogia del capitolo della "montagna di chiavi" se può essere utile. Offre agli studenti un'immagine concreta della corsa al mining. L'idea principale non è che i miner risolvano un problema matematico utile nel senso comune, ma che dimostrino di aver speso energia e potenza di calcolo reali per mettere in sicurezza il sistema.

Questo è anche il momento giusto per spiegare le ricompense dei miner:

* ricompensa del blocco: nuovi bitcoin emessi
* commissioni di transazione: commissioni associate alle transazioni che gli utenti vogliono confermare

Chiarisci che i miner di solito danno priorità alle transazioni con commissioni più alte, perché queste aumentano la loro ricompensa. Il capitolo spiega anche i "halving" qui, quindi puoi notare brevemente che la ricompensa del blocco diminuisce ogni 210.000 blocchi, circa ogni quattro anni, secondo il programma pubblico di emissione di Bitcoin. Le pagine 5 e 6 includono il programma di emissione e la tabella dei prossimi halving, che possono aiutare a rafforzare la prevedibilità dell'emissione di Bitcoin.

**Hash di Blocco Valido, Proof of Work e Regolazione della Difficoltà**

Questa sezione è il cuore del capitolo.

Spiega che i miner stanno cercando un hash di blocco valido, cioè un hash che soddisfi il target della rete. Il capitolo spiega questo come la ricerca di un numero inferiore al target fissato dalla rete.

Poi spiega chiaramente la Proof of Work:

* i miner devono eseguire ripetuti calcoli computazionali
* il primo che trova un hash valido dimostra di aver fatto quel lavoro
* questo rende costoso riscrivere o attaccare il registro
* i nodi poi verificano il blocco prima di accettarlo

Una frase efficace per l'insegnamento è:

La Proof of Work protegge Bitcoin rendendo costosa la disonestà e facile la verifica.

Spiega anche la regolazione della difficoltà:

* la rete regola la difficoltà del mining ogni 2.016 blocchi
* questo avviene circa ogni due settimane
* l'obiettivo è mantenere il tempo medio di creazione dei blocchi vicino ai 10 minuti
* se più potenza di calcolo si unisce alla rete, la difficoltà aumenta
* se c'è meno potenza di calcolo, la difficoltà diminuisce

Le pagine 7 e 8 spiegano questo processo e mostrano come target più difficili richiedano più lavoro. Questo aiuta gli studenti a capire che il tempo di Bitcoin non è controllato da un'autorità centrale ma da regole di protocollo che rispondono automaticamente alle condizioni della rete.

##### 9.2 Cos'è la Mempool?, 15 minuti

Ora passa alla mempool.

Spiega che la mempool è la sala d'attesa per le transazioni valide ma non ancora confermate. Quando un utente trasmette una transazione, i nodi la verificano per primi. Se è valida, la aggiungono alla loro mempool e la condividono con altri nodi. Poi i miner possono selezionare tra queste transazioni in attesa quando costruiscono un blocco. Le pagine 10 e 11 spiegano direttamente questo processo.

Punti importanti da sottolineare:

* la mempool non è la blockchain
* le transazioni lì sono ancora non confermate
* ogni nodo mantiene la propria mempool
* non esiste una singola mempool universale
* le transazioni con commissioni più alte hanno maggiori probabilità di essere selezionate prima

Il capitolo spiega anche i motivi comuni per cui una transazione può rimanere non confermata a lungo:

* commissione bassa
* congestione della rete
* tentativo di doppia spesa
* dati errati o incompleti
* transazione malformata

Se utile, menziona l’attività con mempool.space come modo pratico per visualizzare le transazioni non confermate e le commissioni. Chiarisci anche che mempool.space è solo un explorer, non la mempool stessa.

##### 9.3 Come funzionano le transazioni Bitcoin, 20 minuti

Ora riunisci tutto usando la sequenza passo-passo del capitolo.

Una versione chiara per la classe è:



1. Il mittente seleziona un UTXO e crea una transazione
1. Il mittente aggiunge l’indirizzo del destinatario e la commissione
1. Il mittente firma la transazione con la propria chiave privata
1. La transazione viene trasmessa alla rete
1. I nodi la verificano e la aggiungono alle loro mempool
1. I miner la selezionano per un blocco candidato
1. I miner competono tramite Proof of Work
1. Un miner trova un hash valido del blocco e trasmette il blocco
1. I nodi verificano il blocco e lo aggiungono alla blockchain
1. La transazione riceve conferme man mano che vengono aggiunti nuovi blocchi
1. Rendi esplicito il punto finale:
1. una volta che la transazione è inclusa in un blocco valido, è confermata
1. gli input spesi non sono più utilizzabili
1. il destinatario ora controlla i nuovi UTXO creati da quella transazione

Il diagramma riassuntivo è particolarmente utile qui perché collega visivamente l’intero processo dalla firma del wallet all’inclusione da parte del miner, fino alla validazione del nodo e alla distribuzione del blocco.

###### Conclusione e verifica della comprensione

Chiudi con alcune domande rapide:

* Qual è la differenza tra un nodo e un miner?
* Cos’è la mempool?
* Perché alcune transazioni vengono confermate più velocemente di altre?
* Cosa dimostra il Proof of Work?
* Perché Bitcoin regola la difficoltà di mining?
* Quali sono i passaggi principali tra l’invio di una transazione e la ricezione della conferma?

#### Note per l’educatore

Mantieni chiaro il filo conduttore della lezione: i nodi verificano, i miner competono, il Proof of Work protegge, e la mempool contiene le transazioni valide finché non vengono confermate.

Questo capitolo può sembrare tecnico, quindi usa spesso analogie e diagrammi.

Evita di far sembrare il mining come "creare bitcoin dal nulla." Sii preciso che la ricompensa è l’incentivo, mentre il processo di mining protegge la rete.

I punti più importanti da prioritizzare, se il tempo è poco, sono:



1. Ruoli di nodo e miner
1. Mempool come sala d’attesa
1. Proof of Work
1. Regolazione della difficoltà
1. Flusso della transazione dalla firma alla conferma

##### Cosa significa "buon risultato"

* È importante chiarire subito che Miner ≠ Nodo, mostrare il mining come attività economica con costi reali di hardware e di elettricità, usare la regolazione della difficoltà e il Proof of Work per spiegare il meccanismo di sicurezza, e verificare la comprensione con scenari su cambiamenti della rete.
* Gli educatori dovrebbero usare numeri reali per rendere concrete le discussioni, essere estremamente chiari e ripetitivi sulla distinzione tra Minatori e Nodi, essere realistici riguardo alle preoccupazioni di centralizzazione con i mining pool e rispettare la reale sofisticazione coinvolta.
* Gli studenti comprendono che il mining è svolto da persone intelligenti che fanno un lavoro complesso perché guadagnano Bitcoin, riconoscono che gli incentivi guidano comportamenti onesti perché i profitti dei minatori dipendono dal successo di Bitcoin, vedono il sistema autoregolarsi tramite l'aggiustamento automatico della difficoltà, capiscono che il mining è un vero business e non beneficenza, e apprezzano che la sicurezza di Bitcoin costa elettricità e denaro reali.
* Gli Obiettivi di Apprendimento sono raggiunti se gli studenti sanno distinguere i minatori che creano i blocchi dai nodi che li validano, comprendono il Proof of Work come meccanismo di sicurezza che rende gli attacchi esponenzialmente costosi, riconoscono che l'aggiustamento della difficoltà mantiene il tempo di blocco intorno ai 10 minuti, capiscono gli incentivi dei minatori tra ricompense di blocco e commissioni, spiegano perché un attacco del 51% non funziona, e vedono il mining come un'attività economica con costi e benefici reali.

##### Gestione del Tempo

Se il tempo è poco, dare priorità a:

* Ruoli di nodo vs minatore (la distinzione fondamentale)
* Mempool come sala d'attesa
* Meccanismo di Proof of Work
* Aggiustamento della difficoltà (sistema autoregolante)
* Flusso della transazione dalla firma alla conferma

Se si è in anticipo, soffermarsi su:

* Economia del mining e specifiche dell'hardware
* Dinamiche dei mining pool e preoccupazioni di centralizzazione
* Scenari di attacco del 51% e perché falliscono matematicamente
* Sicurezza a lungo termine tramite allineamento degli incentivi

##### Se gli studenti fanno fatica

* Minatori vs. nodi (confusione) → "I nodi validano, i minatori propongono; arbitri vs. giocatori."
* Proof of Work sprecone → "La sicurezza costosa previene gli attacchi; li rende inutili."
* Aggiustamento della difficoltà → "Più minatori = blocchi più veloci = la difficoltà aumenta; il sistema respira."
