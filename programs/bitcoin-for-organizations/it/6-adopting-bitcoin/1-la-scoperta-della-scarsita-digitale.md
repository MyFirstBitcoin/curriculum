# 6.1 La scoperta della scarsità digitale

> Con Bitcoin, è stato scoperto un nuovo tipo di bene… una sorta di bene digitale, generato dai computer e in parte creato per i computer. L’umanità ha una storia di invenzioni significative. Nei libri di storia che saranno scritti in futuro, Bitcoin sarà elencato come una di queste.  
_Prof. Dr. Philipp Sander_



#### 6.1.0 La scarsità in economia

Nell’ambito dell’economia, è ben compreso che la scarsità è un principio chiave che determina il valore. Beni e servizi che registrano una domanda significativa diventano più preziosi se l’offerta è limitata al punto che la domanda non può essere facilmente soddisfatta. Inoltre, la scarsità alimenta una maggiore competizione ed è un motore per la scoperta dei prezzi nel mercato. In un mercato di libera, equa e aperta concorrenza, i prezzi dovrebbero stabilizzarsi nel punto in cui domanda e offerta si incontrano.

Le risorse che registrano una domanda significativa possono essere considerate più preziose se sono finite o più difficili da acquisire. Questo può stimolare una domanda ancora maggiore per quella risorsa, poiché i partecipanti al mercato competono per assicurarsi l’accesso. Questa dinamica si osserva con le risorse naturali come i metalli preziosi, il petrolio o le cosiddette ‘soft commodities’ come i prodotti alimentari. La scarsità, quindi, è alla base delle decisioni economiche, dell’allocazione delle risorse e del costo opportunità. In un mondo di risorse illimitate, tutto sarebbe ugualmente accessibile e di valore molto basso. Al contrario, la scarsità conferisce valore e promuove scambi, investimenti e innovazione, poiché costringe le società a gestire efficacemente le risorse limitate.



#### 6.1.1 La sfida della scarsità digitale

La sfida della scarsità digitale risiede nella facilità con cui le informazioni digitali possono essere copiate e distribuite. Le informazioni digitali sono intrinsecamente più difficili da proteggere rispetto a quelle fisiche perché, a differenza dei beni fisici - alcuni dei

quali possiedono naturalmente scarsità a causa di vincoli materiali - gli oggetti digitali come file musicali, documenti o immagini possono essere duplicati all’infinito a costo praticamente nullo.

Tradizionalmente, la replicabilità dei dati digitali ha significato che questi beni non potevano avere un valore economico simile a quelli fisici perché mancavano di qualsiasi forma di scarsità applicabile. Per il denaro digitale, questo è particolarmente problematico e viene definito come il problema della ‘doppia spesa’, in cui una singola unità digitale (ad esempio un token o una valuta) potrebbe essere copiata e spesa più volte, svalutandola. Se è possibile spendere due volte una valuta, questa perde valore perché diventa indistinguibile da fondi contraffatti o fraudolenti.

Tradizionalmente, le istituzioni finanziarie centralizzate come le banche mitigano questo rischio mantenendo un registro che verifica ogni transazione e detrae i saldi di conseguenza, assicurando che una volta speso il denaro, non possa essere riutilizzato dallo stesso titolare del conto. Tuttavia, questo approccio richiede un’autorità centrale di fiducia o un ‘oracolo’ per gestire e verificare le transazioni, il che comporta dipendenza e un unico punto di controllo. Avere un oracolo centralizzato delle informazioni rende i beni digitali vulnerabili a manipolazioni e censura.

Per un sistema decentralizzato e a fiducia minimizzata come Bitcoin, dove non esiste un’autorità centrale che supervisiona le transazioni, prevenire la doppia spesa è una sfida monumentale. Senza un meccanismo che garantisca l’unicità di ogni transazione, Bitcoin sarebbe vulnerabile agli abusi, rendendolo impraticabile come riserva di valore e mezzo di scambio affidabile. Bitcoin risolve il problema della doppia spesa attraverso un registro decentralizzato, in cui le transazioni sono confermate simultaneamente da migliaia di partecipanti alla rete. Questo meccanismo permette a Bitcoin di mantenere un registro immutabile di ogni transazione, assicurando che ogni moneta possa essere spesa solo una volta.

Questa soluzione genera scarsità digitale senza fare affidamento su un controllo centrale. Bitcoin introduce la prima soluzione di successo alla scarsità digitale, aprendo la strada a un ecosistema di beni digitali scarsi e a fiducia minimizzata in un modo che prima si riteneva impossibile.



#### 6.1.2 Far rispettare la scarsità digitale con Bitcoin

> Proponiamo una soluzione al problema della doppia spesa utilizzando un server di marcatura temporale distribuito peer-to-peer per generare una prova computazionale dell’ordine cronologico delle transazioni. Il sistema è sicuro finché i nodi onesti controllano collettivamente più potenza di calcolo rispetto a qualsiasi gruppo cooperante di nodi attaccanti.  
_Satoshi Nakamoto_

Satoshi Nakamoto ha creato Bitcoin come soluzione ingegneristica ai problemi associati al denaro fiat. Tuttavia, quella soluzione richiedeva che Satoshi trovasse un modo per far rispettare una scarsità digitale assoluta. Per raggiungere questo obiettivo, Satoshi ha sviluppato un protocollo di comunicazione open-source che funziona su una rete decentralizzata di computer o nodi. Ognuno di questi nodi possiede una copia localmente verificabile di un registro immutabile, la cosiddetta blockchain o timechain. Il protocollo Bitcoin definisce le regole e la rete decentralizzata verifica indipendentemente le transazioni, aderendo alle stesse regole senza richiedere un’autorità centrale.

La scarsità di Bitcoin contribuisce al suo ruolo di riserva di valore. Proprio come l’oro, Bitcoin è prezioso non solo per la sua offerta limitata, ma anche per lo sforzo richiesto per ‘minare’ o produrre nuove monete. Il mining di Bitcoin (il processo che mantiene il registro e emette nuove monete) è un processo costoso e ad alta intensità energetica che rispecchia l’estrazione fisica di minerali dalla terra. Questa ‘prova di lavoro’ digitale impone un vincolo di produzione che allinea Bitcoin ai beni tangibili, conferendogli proprietà di durabilità e verificabilità che i beni digitali tradizionali non hanno. La difficoltà incorporata e il tasso decrescente di emissione di nuove monete attraverso i periodici ‘halving’ creano una struttura economica in cui l’offerta di Bitcoin diventa sempre più scarsa nel tempo, aumentando il suo fascino come riserva di valore a lungo termine.

##### Come viene fatta rispettare la scarsità digitale?

La soluzione di Bitcoin al problema della doppia spesa risiede nell’uso di un registro decentralizzato e pubblicamente consultabile. Il registro di Bitcoin può essere visto come un database immutabile che registra ogni transazione in una catena sequenziale di lotti con marcatura temporale, chiamati blocchi. Ogni blocco è rigorosamente cronologico e contiene transazioni che sono state verificate e accettate dai partecipanti della rete. Ogni blocco è collegato al precedente, creando un registro permanente distribuito su migliaia di nodi in tutto il mondo. Archiviando e condividendo questo registro su una rete decentralizzata, Bitcoin elimina la necessità di un’autorità centrale per confermare le transazioni. Quando avviene una transazione Bitcoin, i nodi della rete la validano in modo indipendente, assicurando che ciascuna venga spesa solo una volta. Questo registro condiviso rende anche estremamente difficile per gli attaccanti violare la rete o alterare le transazioni passate, poiché qualsiasi modifica richiederebbe l’approvazione della maggioranza dei partecipanti alla rete.

Il meccanismo di Proof-of-Work (PoW) di Bitcoin rafforza ulteriormente la protezione contro la doppia spesa richiedendo ai miner di risolvere un problema crittografico per avere il permesso di validare nuove transazioni e creare un nuovo blocco. Questo processo, noto come mining, richiede potenza computazionale e aggiunge un livello di difficoltà e costo alla modifica del registro. Ogni blocco aggiunto al registro deve contenere un collegamento crittografico al blocco precedente, il che solidifica l’integrità della catena e impedisce manomissioni.

Il ruolo di un nodo è quello di conservare la copia più aggiornata del registro, che contiene la storia completa delle transazioni. I nodi mantengono i miner ‘onesti’ poiché verificano che non sia avvenuta alcuna doppia spesa e, cosa importante, che tutte le monete siano state create in conformità con il programma di emissione di Bitcoin. Qualsiasi utente di Bitcoin può eseguire un nodo e verificare la proprietà delle proprie monete senza dover affidarsi a terzi. Non c’è bisogno di autorità per risolvere le controversie in Bitcoin perché qualsiasi transazione inclusa in un blocco è oggettivamente valida.

##### Come potrebbe un attaccante controllare la rete Bitcoin?

Se un attaccante volesse alterare una transazione passata per riuscire in un attacco di doppia spesa, dovrebbe rifare la Proof-of-Work per quel blocco e per tutti i blocchi successivi, competendo contro la potenza computazionale combinata dell’intera rete. Questo meccanismo di sicurezza garantisce che, se qualcuno tentasse una doppia spesa, dovrebbe controllare oltre il 50% della potenza di mining della rete per avere successo. Questo è noto come attacco del 51%.

Nei primi anni di Bitcoin, quando era possibile per singoli partecipanti creare o minare nuovi blocchi utilizzando hardware informatico generalmente disponibile, era almeno teoricamente possibile impiegare abbastanza potenza di calcolo per riuscire in un attacco del 51%. Oggi, la potenza di calcolo combinata della rete Proof-of-Work supera i 700 ExaHash/s. Questo significa che, in aggregato, i computer di mining stanno calcolando più di 700 quintilioni di hash (calcoli crittografici) ogni secondo. Siamo arrivati a un punto in cui l’enorme costo e la coordinazione necessari per riscrivere il registro e riuscire in un attacco del 51% rendono la doppia spesa impraticabile nella realtà.

##### Conferme e riorganizzazioni

Un ulteriore livello di protezione (che a volte viene trascurato) deriva dal processo di conferma delle transazioni di Bitcoin. Quando una transazione viene trasmessa per la prima volta, è considerata non confermata e raccolta nel ‘mempool’ mentre attende di essere inclusa in un blocco e validata dai miner. Una volta che una transazione viene aggiunta a un blocco, è considerata ‘confermata’. Ogni blocco aggiunto successivamente viene conteggiato come un’ulteriore conferma per la transazione. Sebbene una transazione sia considerata ufficiale dopo una sola conferma, non è considerata definitiva finché non vengono aggiunte ulteriori conferme.

Per la massima sicurezza, gli utenti di Bitcoin spesso attendono più conferme (tipicamente sei), poiché ogni blocco aggiuntivo alla blockchain rafforza ulteriormente la transazione, riducendo drasticamente la probabilità di un tentativo di doppia spesa riuscito. Questo processo di conferma stabilisce una finestra temporale durante la quale le transazioni vengono finalizzate.

##### Perché aspettare sei conferme?

Gli utenti di Bitcoin attendono ulteriori conferme perché è possibile che il blocco più recente delle transazioni venga rimosso dalla catena dei blocchi, se non fa più parte della catena più lunga. È importante notare che il mining è una competizione tra grandi pool di potenza di calcolo. Pertanto, è possibile che due miner concorrenti trovino una soluzione crittografica valida e blocchi separati vengano aggiunti alla catena quasi contemporaneamente. Se ciò accade, la catena viene essenzialmente divisa. I miner continueranno a tentare di aggiungere blocchi a ciascun ramo della catena. Tuttavia, una volta che il blocco successivo viene minato, la catena più lunga1 (definita come la catena che ha la maggiore prova di lavoro investita) è quella che prevale e il blocco sulla catena più corta viene ‘orfanato’ e diventa invalido. Tutte le transazioni nel blocco orfano vengono restituite al mempool per essere incluse in un successivo blocco valido. Questo processo si chiama riorganizzazione o semplicemente ‘reorg’.

Un malintenzionato, tentando una doppia spesa, deve ottenere il controllo della rete abbastanza a lungo da ‘riorganizzare’ la catena. Come abbiamo visto sopra, ottenere il controllo totale richiede una quantità enorme di potenza di calcolo, ma cosa succede se una grande operazione di mining - che ipoteticamente controlla poco più di un terzo di tutta la potenza di calcolo della rete - tenta una doppia spesa delle monete?

Vediamo un esempio:

Supponiamo, ad esempio, che la potenza di calcolo totale della rete Bitcoin sia di 550 ExaHash/s. Rogue Inc, che controlla 200 ExaHash/s, effettua un grande acquisto immobiliare e intende pagare in Bitcoin. Tuttavia, Rogue pianifica anche di tentare una doppia spesa degli stessi coin. Il venditore comunica a Rogue che attenderà sei conferme prima di consegnare i titoli di proprietà. Per portare a termine un attacco di doppia spesa, Rogue deve costruire in segreto un ramo alternativo della catena, minando una catena più lunga che contenga la transazione di doppia spesa. Una volta che il venditore ha visto sei conferme contenenti la propria transazione e ha consegnato il bene, Rogue deve quindi pubblicare tutti i blocchi che ha minato nel nuovo ramo, rendendolo così la catena più lunga. Quanto è possibile tutto ciò?

In qualsiasi momento, la probabilità che Rogue mini il prossimo blocco è 200/550 = 0,36. Anche se Rogue è il pool di mining più grande, la probabilità che i miner onesti trovino il prossimo blocco è 1 - 0,36 = 0,64. I blocchi dovrebbero essere minati molto più velocemente sulla catena onesta. Ma supponiamo che Rogue sia fortunata, mini un blocco e lo tenga segreto. Poi tenta di minarne un altro su questo ramo segreto. Tuttavia, la catena onesta mina un blocco e prende il vantaggio minandone un altro, prima che Rogue mini il suo secondo blocco.

A questo punto Rogue si arrende. Perché?


| Blocchi da recuperare | 1% | 10% | 36% (Rogue) | 51% |
| --- | --- | --- | --- | --- |
| 1 | 0,010101 | 0,111111 | 0,562500 | 1,0 |
| 2 | 0,010102 | 0,012346 | 0,316406 | 1,0 |
| 3 | 1,0e-06 | 0,001372 | 0,177919 | 1,0 |
| 4 | 1,0e-08 | 0,000152 | 0,100113 | 1,0 |
| 5 | 1,0e-10 | 0,000017 | 0,056314 | 1,0 |
| 6 | 1,0e-12 | 1,9e-06 | 0,031676 | 1,0 |


**Fonte**: Basato su una tabella in Grokking Bitcoin di Kalle Rosenbaum

Rogue si rende conto di non avere abbastanza hash rate per riuscire nella doppia spesa, nonostante controlli il 36% dell'hash rate di Bitcoin. Per avere successo dovrebbe minare altri quattro blocchi per superare la catena onesta. Nonostante la sua enorme potenza di calcolo e il controllo del 36% della rete, le probabilità di successo di Rogue sono solo 0,100113.


> **Info – Entra in gioco la teoria dei giochi**
>
> Le probabilità di successo di Rogue sono pessime, ma peggiorano ulteriormente. Per ogni minuto in cui continua a tentare, Rogue consuma una quantità enorme di elettricità. Tutto ciò sarà stato vano. Inoltre, per ogni blocco che non mina onestamente, Rogue rinuncia alla ricompensa del blocco, attualmente di 3,125 coin per blocco, con un valore attuale superiore a 300.000 €.
>
> La ragione principale del fallimento di Rogue è che il venditore dell'immobile ha richiesto sei conferme. Più conferme sono necessarie, più è difficile per i miner disonesti costruire catene alternative di blocchi. Infatti, per una transazione molto grande, un venditore può richiedere ancora più conferme. Ad esempio, dieci conferme (che dovrebbero richiedere circa 100 minuti) ridurrebbero le probabilità di successo di Rogue a solo 0,003.
>
> In questo modo, la teoria dei giochi applicata al mining garantisce che tutti siano incentivati ad agire onestamente e a non sprecare risorse di calcolo o rinunciare alle ricompense dei blocchi. Inoltre, è nell'interesse di tutti i miner che la rete Bitcoin sia sicura e affidabile. Questo assicura che il loro enorme investimento in potenza di calcolo sia protetto. Se la rete venisse attaccata con successo, il valore di mercato dei coin crollerebbe drasticamente poiché la fiducia nella rete verrebbe meno.




#### 6.1.3 La centralizzazione del mining è una minaccia?

Come si vede nella tabella sopra, la centralizzazione del mining può rappresentare una potenziale minaccia alla protezione contro la doppia spesa di Bitcoin, poiché aumenta la probabilità di un attacco del 51% - uno scenario in cui un singolo miner o un gruppo di miner controlla oltre la metà della potenza computazionale della rete. Se ciò dovesse accadere, l'entità controllante potrebbe teoricamente modificare le transazioni recenti o tentare una doppia spesa riscrivendo il registro, permettendole di spendere gli stessi coin più di una volta.

Una situazione del genere mina l'integrità della rete Bitcoin, concedendo un'influenza sproporzionata sulla validazione delle transazioni a pochi attori. Tuttavia, sebbene teoricamente possibile, eseguire un attacco del 51% sarebbe comunque estremamente complesso e costoso, richiedendo immense risorse computazionali, elettricità e coordinamento, che probabilmente supererebbero i potenziali benefici di tentare una doppia spesa.

Esistono delle salvaguardie che aiutano a limitare i rischi della centralizzazione del mining. I mining pool, ad esempio, permettono ai miner più piccoli di unire le risorse e condividere le ricompense dei blocchi, riducendo il dominio di una singola entità. Sebbene questo sia un modo utile per i piccoli miner di partecipare alla rete, esiste il rischio che l'entità che controlla il pool possa comportarsi in modo scorretto e tentare di attaccare la rete. Tuttavia, la trasparenza del registro di Bitcoin significa anche che qualsiasi concentrazione di potere di mining è visibile, avvisando la comunità dei potenziali rischi e permettendo contromisure. I miner sono ben consapevoli che qualsiasi attacco alla rete Bitcoin rischia di danneggiare seriamente la sua proposta di valore, perciò è molto semplice per i piccoli miner cambiare pool per evitare che la loro potenza di calcolo venga usata in modo illecito. Sebbene il rischio non sia nullo, la natura aperta e distribuita dell'ecosistema di Bitcoin, unita all'alto costo di un attacco, rende la centralizzazione del mining più una minaccia teorica che imminente, poiché mantenere tale controllo per periodi prolungati sarebbe finanziariamente insostenibile per qualsiasi attaccante.



#### 6.1.4 L'impatto più ampio della scarsità digitale

Bitcoin ha trasformato il modo in cui pensiamo alla scarsità nel mondo digitale. Poiché i beni digitali - come software, file musicali, e-book e contenuti online - possiedono caratteristiche che li distinguono dai beni fisici, possono essere riprodotti a costi trascurabili e condivisi istantaneamente. A differenza degli oggetti fisici, che sono vincolati da limiti materiali come i costi di produzione e le limitazioni di stoccaggio, i beni digitali esistono come dati che possono essere duplicati all'infinito senza alcun degrado della qualità. Questo significa che, mentre i beni fisici sono intrinsecamente scarsi a causa di questi vincoli materiali, i beni digitali sono stati tradizionalmente abbondanti, privi di meccanismi integrati per limitare l'offerta.

È importante notare che i beni digitali sono non rivali. Questo significa che il consumo di un bene digitale da parte di una persona non ne diminuisce la disponibilità per gli altri. Ad esempio, quando una canzone viene scaricata, può essere copiata e distribuita un numero illimitato di volte senza perdere utilità. Storicamente, questa abbondanza rappresenta una sfida per la creazione di valore, poiché il modello economico tradizionale di domanda e offerta viene distorto quando l'offerta è, almeno teoricamente, illimitata. In risposta a ciò, la gestione dei diritti digitali (DRM) e altre misure di scarsità artificiale hanno cercato di limitare l'accesso. Tuttavia, questi meccanismi possono essere aggirati e delegano la fiducia ad autorità centralizzate. L'innovazione di Bitcoin risiede nel modo in cui affronta questo problema in modo nativo, rendendolo il primo asset digitale a incorporare la scarsità tramite una tecnologia decentralizzata senza affidarsi a queste limitazioni tradizionali.

Bitcoin svolge un ruolo trasformativo nell'instaurare la scarsità digitale introducendo un protocollo che impone un'offerta finita. Un limite di 21 milioni di monete è codificato nel protocollo e questo limite non può essere modificato senza il consenso della rete, cioè di tutti i migliaia di partecipanti sparsi in tutto il mondo che gestiscono i nodi Bitcoin. In questo modo, Bitcoin ha creato un asset che imita la natura finita delle materie prime fisiche, come l'oro, pur esistendo interamente nel mondo digitale. Il limite massimo di offerta è fondamentale per la proposta di valore di Bitcoin ed è sostenuto da una combinazione di crittografia, meccanismi di consenso e codice open-source trasparente. Questo garantisce che tutti i partecipanti della rete rispettino le stesse regole, oltre a essere motivati dal principale incentivo economico di assicurare che l'offerta di monete sia assolutamente e dimostrabilmente finita.

Risolvendo il problema della doppia spesa, Bitcoin previene l'inflazione o la duplicazione dell'asset, una sfida che ha afflitto i precedenti esperimenti di denaro digitale. All'interno di Bitcoin, nessuna singola autorità controlla l'offerta, rendendolo immune alla manipolazione centrale tipica del sistema monetario fiat, come la stampa arbitraria di valuta o la svalutazione. Questa innovazione permette a Bitcoin di fungere da riserva di valore e copertura contro l'inflazione, consentendogli di occupare una posizione unica simile all'“oro digitale” - una risorsa digitale scarsa con valore verificabile.



#### 6.1.5 Conclusione

In conclusione, si sta diffondendo la consapevolezza che l'innovazione di Bitcoin nella scarsità digitale ha ridefinito il concetto di denaro. Tuttavia, a volte si trascura il fatto che Bitcoin ha anche trasformato il panorama digitale risolvendo il problema di lunga data della creazione di scarsità in un mondo digitale intrinsecamente abbondante. Bitcoin ha effettivamente introdotto una nuova categoria di asset digitali che rispecchiano le qualità delle materie prime fisiche.

Questa svolta dimostra che un sistema decentralizzato può stabilire scarsità, immutabilità e valore indipendentemente da qualsiasi autorità centrale. Inoltre, potrebbe avere applicazioni oltre il denaro, poiché ha ispirato un intero campo di ricerca e sviluppo attorno a questa tecnologia.

Guardando al futuro, il modello di scarsità digitale di Bitcoin sta plasmando il futuro del denaro e della conservazione del valore. Poiché le preoccupazioni sull'inflazione e le domande sulla gestione della valuta fiat diventano sempre più riconosciute, l'offerta fissa di Bitcoin lo rende sempre più attraente come copertura contro l'instabilità finanziaria tradizionale.

In definitiva, la scoperta della scarsità digitale da parte di Bitcoin potrebbe segnare l'inizio di un cambiamento di paradigma, in cui gli asset digitali con scarsità riconosciuta e fiducia verificabile ottengono riconoscimento come componenti di valore dell'economia moderna, stabilendo una base per il futuro della finanza decentralizzata e della proprietà digitale. Questo ha implicazioni significative per il campo dell'economia: Bitcoin ha fornito il modello di come scarsità e valore possano esistere in forma digitale.

> Oltre alla scarsità digitale, Bitcoin è anche il primo esempio di scarsità assoluta, l'unica merce liquida (digitale o fisica) con una quantità fissa che non può essere aumentata in alcun modo concepibile. Fino all'invenzione di Bitcoin, la scarsità era sempre relativa, mai assoluta.  
_Saifedean Ammous_



###### Note

1. La catena più lunga viene accettata dai nodi Bitcoin come la versione più valida del registro ed è definita come la catena che ha richiesto il maggior sforzo (o la maggiore prova di lavoro) per essere costruita. Maggiori informazioni qui: [https://learnmeabitcoin.com/technical/blockchain/longest-chain/](https://learnmeabitcoin.com/technical/blockchain/longest-chain/)
