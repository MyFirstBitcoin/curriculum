# 2.7 Bitcoin non è veramente decentralizzato

> La complessità delle criptovalute nasce dai tentativi di decentralizzazione: distribuendo il potere e la governance all'interno del sistema, teoricamente non c'è bisogno di intermediari fidati come le istituzioni finanziarie. Questa era la premessa del white paper iniziale di Bitcoin, che offriva una soluzione crittografica pensata per consentire pagamenti senza coinvolgere alcuna istituzione finanziaria o altro intermediario fidato. Tuttavia, Bitcoin è diventato centralizzato molto rapidamente e ora dipende da un piccolo gruppo di sviluppatori software e mining pool per funzionare  
_Fondo Monetario Internazionale_

Come mostra la citazione sopra tratta da un post abbastanza recente del Fondo Monetario Internazionale, l'industria finanziaria tradizionale continua a sostenere che Bitcoin non sia decentralizzato, oltre a confondere Bitcoin con altri crypto asset.

##### Introduzione

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/4d318ee0b65d453094dc7d88369875066f60494a-161x167.svg)

La decentralizzazione è un aspetto fondamentale di Bitcoin. La capacità di mantenere le regole del protocollo, come la scarsità e la distribuzione, senza un'autorità centrale garantisce che possa agire come denaro senza permessi per una società globale.

Come ha osservato Satoshi nella sua corrispondenza online, servizi decentralizzati come BitTorrent riuscivano a 'resistere' ai tentativi di repressione da parte dei governi, rispetto ai servizi con proprietari identificati e server centralizzati. Era chiaramente preoccupato per il rischio potenziale che i governi o altri interessi potessero chiudere o influenzare negativamente Bitcoin.

In questo contesto, ci interessa la decentralizzazione di:

* Lo sviluppo e la gestione del codice che esegue il protocollo; chi può cambiare le regole?
* La funzione di mining che crea nuovi blocchi secondo le regole e valida contro la doppia spesa
* I nodi che validano le transazioni per verificarne la validità e mantengono una copia della blockchain

##### Sviluppatori

Bitcoin è un protocollo open-source che chiunque è libero di consultare, scaricare, copiare o proporre modifiche. È disponibile in una libreria su GitHub, il cui codice sorgente è stato lanciato originariamente nel 2009 da Satoshi Nakamoto. Chiunque è libero di scaricare il codice ed eseguire un nodo, la maggior parte dei quali utilizza il software originale Bitcoin Core, che è stato aggiornato nel tempo.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Fonte: https://river.com/learn/what-is-bitcoin-core/_

Lo sviluppo di Bitcoin Core segue le migliori pratiche dello sviluppo open source. In qualsiasi momento, può esserci un numero qualsiasi di sviluppatori che scrivono o revisionano modifiche al codice. Devono ascoltare le preoccupazioni degli operatori dei nodi e dei miner, così come della base utenti, prima di apportare qualsiasi modifica critica al codice, che verrà revisionata e approvata come mostrato nel diagramma di flusso sopra prima di essere integrata nel codice.

Le regole di Bitcoin sono quindi codificate in questo software Bitcoin Core, che gira su ogni nodo. Chiunque può proporre una modifica alle regole – le regole sono codice, ma non sono _solo_ codice, sono _concordate_ regole. Se cambiate unilateralmente, il nuovo codice non fa più parte del consenso e non è più parte di Bitcoin. Cambiare qualcosa in Bitcoin e rimanere nel consenso è complicato. Le modifiche proposte al codice rientrano in una di tre categorie:

* All'interno delle regole esistenti: Aggiornamenti minori come errori di ortografia, interfaccia utente migliorata o gestione dei dati possono rientrare in questa categoria e sono relativamente semplici da approvare.
* Aggiunta di una nuova regola che impone restrizioni alle regole – come la riduzione della dimensione del blocco. Questo è chiamato 'soft fork'. I nodi che scelgono di non implementare la modifica e restano sulla vecchia versione potranno comunque partecipare alla rete.
* Aggiunta di una nuova regola che rompe le regole attuali, ad esempio un aumento della dimensione del blocco. I nodi che non aggiornano il codice considereranno un blocco creato con dimensione maggiore come non valido. Questo è chiamato 'hard fork' e crea una divisione della catena tra i nodi che eseguono il codice originale e quelli che eseguono il nuovo codice, generando una nuova moneta. Questo è già successo in passato, ma non ha mai portato a un successo duraturo per la nuova moneta, poiché la maggior parte dei nodi ha deciso di mantenere il codice originale.

Pertanto, una singola parte o un gruppo di persone non può cambiare unilateralmente il codice di Bitcoin senza ottenere un consenso, altrimenti rischia una divisione della catena e la creazione di una nuova moneta con un diverso insieme di regole.

##### Mining

La funzione di mining valida le transazioni come qualsiasi altro nodo della rete, ma poi consuma l'energia necessaria per creare un nuovo blocco che rispetti le regole di consenso del codice. Il successo permette al miner di ottenere le ricompense sotto forma di commissioni di transazione e premi in Bitcoin (al momento della scrittura 3,125 monete per blocco).

Il mining viene normalmente effettuato tramite 'pool' di mining, dove le persone uniscono la potenza di calcolo o hash rate per aumentare le probabilità di minare un blocco e condividere le ricompense. Esiste il rischio che uno o più di questi pool possano unirsi per raggiungere una dominanza del 51% nel mining e, di fatto, sovvertire il protocollo di validazione della rete a proprio favore per effettuare una doppia spesa delle monete. Questo richiederebbe una quantità enorme di risorse a costi elevatissimi, e i singoli miner possono facilmente cambiare pool in qualsiasi momento. Un attacco del genere probabilmente farebbe anche crollare il valore di bitcoin, poiché sarebbe evidente che l'integrità della rete è stata compromessa. L'attaccante dovrebbe quindi convertire rapidamente i bitcoin ottenuti in valuta fiat prima che il valore si eroda. Questo renderebbe ancora più difficile sostenere un attacco a lungo termine, e quindi è più redditizio per un miner o un operatore di pool rispettare le regole e cercare di minare blocchi validi.

Anche la distribuzione geografica della funzione di mining è importante per evitare che, ad esempio, i governi prendano il controllo della capacità di mining o la blocchino. Ad esempio, un recente divieto di mining da parte della Cina ha dimostrato la capacità di Bitcoin di adattarsi e sopravvivere a tali interventi governativi, adattandosi e riprendendosi rapidamente dalla conseguente perdita di potenza di calcolo.

##### Nodi

A differenza del mining, che richiede un investimento finanziario significativo per competere efficacemente nella corsa a minare nuovi blocchi, o dello sviluppo del codice che richiede competenze di programmazione, eseguire un nodo è qualcosa che chiunque sia interessato a contribuire alla decentralizzazione di Bitcoin può fare.

I nodi eseguono il software Bitcoin Core e fanno rispettare le regole incluse nel codice per assicurarsi che i miner non imbrogliino, ad esempio assegnandosi una ricompensa per blocco superiore a quella consentita. Fanno anche rispettare il limite massimo di 21 milioni di monete, fondamentale per mantenere la scarsità di Bitcoin. Perché un governo o un attore malevolo possa fermare Bitcoin, dovrebbe distruggere ogni singola copia della blockchain, attualmente in esecuzione su migliaia di nodi distribuiti in tutto il mondo, un compito quasi impossibile.

##### Persone

Un altro aspetto della potenziale centralizzazione sono le persone. Ogni altro 'alt-coin' ha un leader – qualcuno che potrebbe essere costretto a sostenere cambiamenti non nell'interesse di Bitcoin. Satoshi Nakamoto è rimasto abbastanza a lungo da assicurarsi che Bitcoin fosse sulla strada del successo prima di sparire per sempre, lasciandolo nelle mani di altri per migliorare e adattare il software.

E i possessori di grandi quantità di Bitcoin? I primi investitori, che hanno mantenuto le loro monete senza perderle, saranno ora estremamente ricchi. È importante notare che questo può essere vero, ma non dà loro più influenza sul sistema rispetto a chiunque altro, a differenza delle monete 'proof of stake' dove i primi adottanti, già ricchi di quella moneta, ottengono vantaggi nelle decisioni e nella distribuzione delle future monete. Questo ha portato o porterà inevitabilmente alla centralizzazione nel tempo.

##### Conclusione

Quali sono le potenziali minacce che la decentralizzazione può cercare di mitigare?

* Governi che chiudono o vietano Bitcoin
* Modifiche indesiderate al codice che favoriscono un insieme di interessi in Bitcoin, ad esempio aumentando la ricompensa per blocco
* Coercizione del protocollo da parte di governi o attori malevoli per influenzare la direzione del protocollo
* Possibilità che un pool di miner prenda il controllo della rete e 'doppia-spenda' Bitcoin – un attacco del 51%

Come possiamo vedere, la combinazione di nodi, sviluppatori di codice e miner, oltre all'utilizzo del meccanismo di 'proof of work', decentralizza Bitcoin a un livello sufficiente da rendere queste potenziali minacce non particolarmente preoccupanti. La comunità dovrà continuare a monitorare la situazione per garantire che rimanga così.
