# 5.1 L’impatto di Bitcoin sui leader IT

> Ogni persona informata deve conoscere Bitcoin perché potrebbe essere uno degli sviluppi più importanti al mondo.  
_Leon Luow_



#### 5.1.0 Introduzione

I responsabili IT hanno delle responsabilità verso l’azienda, utilizzando la tecnologia sia per guidare l’innovazione e la competitività delle loro imprese, sia per trovare modi per migliorare l’efficienza interna e ridurre i costi.

Ci sono diversi rischi comuni e idee sbagliate su Bitcoin che è utile comprendere e su cui fornire indicazioni:

* Spesso viene visto come parte di una più ampia industria ‘crypto’ e di soluzioni basate su una delle innovazioni chiave utilizzate, la blockchain.
* Si percepisce che ‘sprechi energia’ per far funzionare la rete.
* Esiste un rischio per gli utenti del Cloud Pubblico che l’ambiente possa essere violato e utilizzato per ‘minare’ Bitcoin o altre criptovalute da parte di un attore malevolo, portando a una bolletta molto elevata e inaspettata, oltre a impatti sulle prestazioni delle applicazioni aziendali.
* C’è una mancanza di conoscenza della tecnologia dietro Bitcoin.

Dal lato positivo, Bitcoin potrebbe portare benefici a qualsiasi azienda:

* Essere aggiunto al tesoro come asset, sia minato direttamente che acquistato sul mercato aperto.
* Utilizzare risorse altrimenti inattive per minare Bitcoin per l’azienda.
* Fornire una giustificazione per investimenti in soluzioni di IA che richiedono risorse di calcolo ad alte prestazioni simili.
* Aggiungere un metodo di pagamento alternativo per l’acquisto di servizi o prodotti aziendali.
* Ridurre le commissioni globali sulle transazioni in valuta estera.
* Fornire un ulteriore beneficio ai dipendenti tramite incentivi basati su pagamenti Lightning.
* Costruire nuove fonti di reddito per l’azienda basate su Bitcoin.

Qualsiasi responsabile IT deve prendersi il tempo per comprendere Bitcoin, il potenziale impatto e i rischi associati, così come i possibili benefici, per poter fornire guida e leadership all’azienda.

> Bitcoin è un risultato crittografico straordinario. La capacità di creare qualcosa che non può essere duplicato nel mondo digitale ha un valore enorme. Molte persone costruiranno aziende su questa base.  
_Eric Schmidt_



#### 5.1.1 Rischi e idee sbagliate su Bitcoin

##### Bitcoin come parte di una più ampia industria ‘crypto’.

Bitcoin è stato il primo tentativo riuscito di creare un asset digitale finito e ha dato origine a un’intera industria di ‘alt-coin’ che cercano di utilizzare parte della tecnologia sottostante per ‘migliorare’ Bitcoin o per costruire soluzioni che rispondano ad altre potenziali opportunità di mercato.

I fornitori di cloud pubblico hanno creato piattaforme blockchain per permettere alle aziende di costruire queste soluzioni, tuttavia l’interesse verso queste tende a crescere e diminuire in base all’hype del settore; infatti Microsoft ha interrotto il suo servizio blockchain nel 2021.

* Fino al 2017, Bitcoin rappresentava fino al 95% della capitalizzazione totale del mercato crypto.
* La prima ondata di ICO ‘alternative’ ha visto la sua dominanza scendere al minimo storico del 37,6%.
* Poiché queste non sono riuscite a portare reali benefici aziendali e hanno iniziato a svanire, la dominanza di Bitcoin ha ricominciato a salire.
* Nel 2021, con l’aumento del prezzo di Bitcoin, è apparsa sul mercato una nuova ondata di soluzioni alternative basate su NFT che ha nuovamente spinto verso il basso la dominanza di Bitcoin.
* Dopo che anche questo hype non ha portato benefici reali, la dominanza di Bitcoin ha ricominciato a salire.
* Quando e se Bitcoin entrerà in un altro mercato rialzista, è possibile che emerga una nuova ondata di ‘alt-coin’ per capitalizzare su una nuova tendenza, ma probabilmente farà la stessa fine.

Se l’azienda si rivolge al responsabile IT con l’ultimo ‘oggetto luccicante’ promosso per una particolare applicazione della blockchain, o come alternativa a Bitcoin, è importante tenere a mente questa tendenza e chiedersi:

* Qual è lo scopo della blockchain?
* È davvero necessaria o desiderabile una blockchain, considerando i suoi limiti prestazionali rispetto a un database relazionale centralizzato?
* Chi può cambiare il protocollo e quale impatto ha sulla soluzione?
* Quali compromessi sono stati fatti in termini di sicurezza o decentralizzazione per ottenere le prestazioni dichiarate?
* Quale beneficio può offrire che non possa essere fornito utilizzando Bitcoin e i protocolli associati, come Lightning?

##### Le implicazioni dell’esecuzione di Bitcoin

A seconda del settore in cui opera l’azienda, potrebbero esserci benefici potenziali dall’attività di mining di Bitcoin, tipicamente dove il calore generato può essere utilizzato in modo utile. Tuttavia, spesso ci sono resistenze dovute alla percezione che Bitcoin sia dannoso per l’ambiente, sprechi energia o abbia pochi benefici.

Come responsabile IT, comprendere questa dinamica e se ci siano potenziali benefici per l’azienda è necessario per fornire una guida efficace. La posizione generale è stata che Bitcoin non sia ‘buono per l’ambiente’ e ‘sprechi energia’. Tuttavia, questo sta cambiando rapidamente, vengono pubblicati rapporti più positivi e si prevede che questa narrazione cambi verso una in cui il mining di Bitcoin possa essere visto come positivo per l’ambiente e la transizione verso fonti di energia rinnovabile. Questo è un tema su cui molte aziende si concentrano nelle loro iniziative ESG.

##### Comprendere i potenziali rischi del mining di crypto

Ci sono stati esempi in passato in cui l’ambiente cloud pubblico gestito da un’azienda è stato preso di mira da hacker, che possono molto rapidamente abilitare risorse di calcolo aggiuntive per minare crypto. Più risorse vengono abilitate con il profilo di prestazioni più elevato (e costoso), maggiori sono le possibilità che l’hacker abbia di minare Bitcoin o altre crypto. Questo è chiamato ‘Crypto-Jacking’ - secondo AWS:

‘Questo è un tipo di crimine informatico che comporta l’uso non autorizzato di dispositivi (edge computer, smartphone, tablet o anche server) per minare criptovalute. Con l’aumento dei prezzi delle criptovalute e l’uso di dispositivi edge sempre più potenti con capacità GPU per casi d’uso di Machine Learning all’edge, cresce la minaccia che i cryptojacker sfruttino vulnerabilità di sicurezza su questi dispositivi. Quando ciò accade, le risorse edge vengono usate per minare criptovalute, con conseguente aumento dell’uso di CPU/GPU, degrado delle prestazioni delle applicazioni edge e aumento dei tempi di elaborazione delle inferenze ML all’edge.’

È quindi fondamentale che qualsiasi utilizzo di risorse cloud pubbliche sia progettato correttamente seguendo le best practice. Queste sono tipicamente descritte in una qualche forma di Cloud Adoption Framework, che fornisce raccomandazioni su sicurezza, prestazioni, monitoraggio, resilienza e operazioni. Il responsabile IT dovrebbe assicurarsi che queste vengano seguite e che sia abilitato un qualche tipo di monitoraggio in tempo reale per identificare e mitigare tali attacchi prima che vengano generate bollette elevate.

##### Mancanza di conoscenza della tecnologia utilizzata da Bitcoin

Ci sono molte idee sbagliate sulla tecnologia dietro Bitcoin, che portano a domande su se possa essere hackerato, sull’energia utilizzata o se verrà superato da una nuova versione come spesso accade con la tecnologia. Come responsabile tecnico, avere una comprensione della tecnologia sottostante sarebbe utile per posizionare correttamente Bitcoin internamente e mitigare queste preoccupazioni.



#### 5.1.2 Dal lato positivo.

##### Bitcoin come asset di tesoreria

Ci sono potenziali benefici finanziari per un’azienda che inserisce Bitcoin a bilancio come asset di tesoreria.

* Riserva di valore e copertura contro l’inflazione
* Fiducia calante nelle valute fiat come riserva di valore
* Rischio controparte nel settore bancario
* Vantaggio del primo arrivato per le aziende che aggiungono Bitcoin al proprio tesoro

Sebbene le implicazioni finanziarie di questa operazione dal punto di vista contabile non siano di competenza del responsabile IT, comprendere come potrebbe funzionare e come i Bitcoin possano essere acquistati, conservati e protetti lo è.

Esistono servizi disponibili sul mercato che aiutano ad acquistare, custodire e offrire servizi di prestito contro gli asset conservati. Se questo diventa un argomento di discussione all'interno dell'azienda, come dovrebbe essere, il responsabile IT può aiutare a valutare eventuali aziende terze che offrono questi servizi. La due diligence per garantire che i servizi offerti soddisfino le necessarie esigenze di sicurezza, trasparenza e funzionalità aiuterà a selezionare un partner affidabile.

##### Vantaggi del mining di Bitcoin

Si prevede che l'utilizzo dei datacenter crescerà solo in futuro, e una grande percentuale dei costi per la gestione di un datacenter deriva dalla dissipazione del calore generato. Questo è particolarmente vero per applicazioni che utilizzano il calcolo ad alte prestazioni, come l'IA/ML e il mining di Bitcoin.

Aziende di diversi settori in tutto il mondo hanno identificato come questo aumento della produzione di calore possa diventare un beneficio netto per l'azienda invece che un costo, utilizzando il calore generato per:

* Piscine/SPA
* Centri acquatici
* Coltivazione di fiori/ortaggi in serre
* Riscaldamento dei locali aziendali e dei sistemi di acqua calda

Questo può essere realizzato collaborando con una società di mining di Bitcoin che utilizza le strutture aziendali per minare Bitcoin a scopo di lucro e fornisce il calore per l'uso generale, oppure

l'azienda potrebbe svolgere questa funzione direttamente per accumulare un tesoro di Bitcoin. Questo approccio può anche aiutare un'azienda con eventuali iniziative ESG.

Un metodo più indiretto per ottenere alcuni di questi benefici può essere quello di spostare i requisiti di calcolo verso datacenter che adottano questo approccio e offrono spazio rack o infrastruttura come parte di un servizio gestito, trasferendo parte di questi risparmi sui costi all'azienda.

Come responsabile IT, rimanere aggiornato su questo ambito ti aiuterà a fornire indicazioni all'azienda nell'adozione di soluzioni che potrebbero essere utili al business.

##### Bitcoin e IA

Si prevede che l'uso di IA e ML crescerà notevolmente nei prossimi anni. L'intersezione tra Bitcoin e Intelligenza Artificiale sta guidando una nuova era di innovazione digitale, evidenziata in particolare dall'integrazione dell'IA con il Lightning Network di Bitcoin. Questa unione è destinata a rivoluzionare aspetti di internet, dai micropagamenti agli agenti economici online guidati dall'IA.

* Il fine tuning dei modelli di IA è una fase essenziale nello sviluppo dell'IA: i micropagamenti tramite Lightning possono permettere a persone in tutto il mondo di essere pagate per ogni compito in Bitcoin, incentivando la partecipazione.
* In scenari in cui entità di IA effettuano transazioni per servizi, la rete Lightning è uno strumento indispensabile per attività economiche guidate dall'IA dove la velocità è fondamentale.
* Una volta sviluppato il sistema di IA, i micropagamenti potrebbero facilitare un modello pay-per-use più equo, in cui gli utenti pagano solo per le risorse di IA effettivamente utilizzate.

Per qualsiasi azienda che stia valutando l'uso dell'IA, sia come servizio da acquistare sia nello sviluppo di una propria soluzione di IA, è importante comprendere come Bitcoin e Lightning si integrino e aggiungano valore a qualsiasi soluzione.

Fonte: [https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/](https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/)

##### Nuove opzioni di pagamento al dettaglio

Qualsiasi azienda che accetta pagamenti per servizi, sia direttamente nei punti vendita sia online, potrebbe beneficiare dell'accettazione di pagamenti in Bitcoin nei seguenti modi:

* Aumento dell'affluenza e crescita del business rivolgendosi ai clienti Bitcoin
* Commissioni di pagamento basse o nulle
* Regolamento istantaneo
* Nessun chargeback

Dal punto di vista contabile, ci sono diversi modi per gestire i Bitcoin ricevuti: mantenerli come parte del tesoro aziendale, convertirli direttamente in valuta fiat, o una combinazione secondo quanto concordato. A seconda dell'azienda, potrebbero esserci alcune implicazioni tecniche per raggiungere questo obiettivo, come nuovi terminali POS o l'integrazione con una soluzione software per i pagamenti online, di cui il responsabile IT deve comprendere le implicazioni tecniche se viene concordato come obiettivo aziendale.

##### Riduzione delle commissioni di trasferimento FX globali

Per le aziende che trasferiscono grandi somme di denaro a livello globale, i costi e la complessità di queste operazioni possono spesso essere una sfida. Nuove soluzioni basate su Bitcoin vengono offerte sul mercato per ridurre questi costi e fornire regolamenti più rapidi e immediati. Adottare questi servizi potrebbe essere vantaggioso per l'azienda, e avere una comprensione di questo mercato, dei servizi offerti e collaborare con il team contabile per implementare la soluzione migliore richiede un livello di conoscenza tecnica che il responsabile IT può fornire.

##### Benefici per i dipendenti

La maggior parte delle aziende sta valutando come offrire benefici e incentivi ai propri dipendenti per migliorare il reclutamento e la fidelizzazione. Recentemente, diversi atleti professionisti e politici di alto profilo hanno annunciato di ricevere tutto o parte dello stipendio in Bitcoin. La possibilità di pagare una parte dello stipendio in Bitcoin sarà importante per i datori di lavoro quando diventerà un elemento decisivo nelle assunzioni chiave, o quando membri fondamentali del team inizieranno a richiedere questa opzione o a cercare datori di lavoro che la offrono altrove.

* Integrare l'opzione di una retribuzione totale o parziale in Bitcoin offre a un'organizzazione un vantaggio competitivo per anticipare i tempi. Le soluzioni di payroll in Bitcoin rendono semplice l'integrazione di questo processo.
* Aziende come MicroStrategy stanno valutando modi per incentivare le prestazioni o persino la partecipazione alle riunioni con micropagamenti basati su Lightning.

Anche se la decisione di implementare tali benefici per i dipendenti non spetta direttamente al responsabile IT, fornire una comprensione del perché ciò possa essere vantaggioso, delle soluzioni disponibili per realizzarlo e delle implicazioni tecniche dell'implementazione può invece rientrare nelle sue competenze. I direttori IT che propongono proattivamente idee ai colleghi possono dimostrare il loro valore strategico più ampio per l'azienda.

##### Nuove opportunità di mercato

Come affermato nella citazione di Google, molte aziende cercheranno di costruire nuove fonti di reddito basate sull'ecosistema Bitcoin in crescita. Questo potrebbe aprire nuovi mercati da considerare per l'azienda, che il responsabile IT può essere determinante nel valutare per quanto riguarda idoneità, sfide tecniche e potenziali opportunità.



#### 5.1.3 Riepilogo

Si prevede che Bitcoin continuerà il suo percorso di adozione, diventando sempre più importante per le aziende nel tempo, influenzando sia le strategie aziendali che tecniche e le iniziative in diversi ambiti. In qualità di responsabile tecnico dell'azienda, il responsabile IT trarrà beneficio dall'anticipare questi sviluppi, fornendo indicazioni all'azienda e assicurandosi che ottenga il massimo beneficio dall'implementazione di soluzioni Bitcoin in tutta l'organizzazione.
