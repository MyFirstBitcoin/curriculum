# 2.4 Non c’è innovazione in Bitcoin.

> La creazione di mille foreste è racchiusa in una sola ghianda.   
_Ralph Waldo Emerson_

I critici spesso cercano di sostenere che Bitcoin sia una tecnologia "vecchia" o "morta" perché non modifica il protocollo del livello base con la stessa frequenza delle blockchain concorrenti. Questa affermazione ignora sia le ragioni per cui i cambiamenti a Bitcoin vengono adottati lentamente, sia la quantità di innovazione che avviene per scalare la rete sui livelli superiori, come il Lightning Network. Ignora anche il fatto che molte delle nostre tecnologie più flessibili e durature non si evolvono rapidamente a livello di base.

Ad esempio, non c'è innovazione nemmeno nel Transmission Control Protocol (TCP), che è alla base di Internet. Il TCP è stato creato per la prima volta nel 1974. L'ultima volta che il TCP è stato aggiornato è stato nel 1982. Fa ciò che deve fare. Non è perfetto, e ci sono dibattiti sul fatto che sia necessario aggiornare IPv4 per supportare gli sviluppi futuri di Internet. Tuttavia, affermare che non ci sia stata innovazione su Internet dal 1982 sarebbe un'affermazione notevole. Tutta questa innovazione è avvenuta 'su' TCP, piuttosto che 'in' esso.

La stragrande maggioranza dell'innovazione che sta avvenendo non è 'in' Bitcoin ma 'su' Bitcoin. Un giorno probabilmente non ci sarà più innovazione 'in' Bitcoin, e questo dovrebbe essere un obiettivo e non una critica, poiché sarà il riflesso di quanto sia diventato fondamentale nel sostenere l'economia globale fornendo le basi per una moneta solida globale, neutrale e senza permessi. Una moneta solida sia dal punto di vista economico, grazie all'offerta fissa e a un registro immutabile, sia dal punto di vista tecnologico, poiché non cambia e ciò che è in funzione ha avuto anni di operatività ininterrotta. Bitcoin ha già raggiunto il 100% di operatività negli ultimi 10 anni.

Tuttavia, sarebbe preoccupante se non ci fosse innovazione 'su' Bitcoin. Diamo un'occhiata a quanto è successo negli ultimi 10 anni:



#### 'In' Bitcoin

Segregated Witness (SegWit) è stato implementato nel 2017 per proteggere contro la malleabilità delle transazioni e aumentare la capacità dei blocchi. SegWit è stato anche un prerequisito necessario affinché Lightning e alcune sidechain potessero funzionare in modo efficiente.

Taproot è stato implementato nel 2021 per consentire il raggruppamento e la validazione di più firme tramite l'incorporazione delle firme Schnorr, introducendo un linguaggio di scripting per permettere funzionalità più complesse e aumentando la privacy e la resistenza alla censura delle transazioni.



#### 'Su' Bitcoin

##### Liquid Sidechain

La sidechain Liquid è stata implementata nel 2018. Liquid, come altre sidechain, è un registro blockchain separato che è collegato alla blockchain principale di Bitcoin, secondo un insieme di regole predefinite. Queste regole sono abbastanza flessibili da permettere alla catena Liquid di svilupparsi e incorporare miglioramenti di design e scalabilità nel tempo. Tuttavia, il collegamento alla blockchain di Bitcoin garantisce che il limite totale di 21 milioni di bitcoin sia coerente su entrambe le catene.

L'asset in Liquid, L-BTC, è ancorato in modo bidirezionale al bitcoin sulla catena principale. Ci sono compromessi in termini di costo, velocità, privacy e sicurezza che rendono L-BTC ideale per alcune applicazioni. Costo, velocità e privacy sono tutti migliorati con L-BTC, a scapito di dover riporre una certa fiducia nelle organizzazioni che compongono la Liquid Federation, che insieme controllano un processo multisig 11 su 15 per ancorare e disancorare L-BTC a bitcoin e viceversa.

##### Lightning Network

Il Lightning Network è stato implementato nel 2018. Lightning è progettato come una rete di pagamenti peer to peer sotto forma di un grafo di nodi collegati tramite canali; non è una blockchain. Il bitcoin viene bloccato da un gestore di nodi sulla blockchain principale per renderlo disponibile all'uso su Lightning Network, garantendo così che venga utilizzato solo bitcoin 'reale'. I nodi possono quindi aprire canali di liquidità tramite smart contract multisig tra di loro. I pagamenti trovano percorsi attraverso la rete dalla fonte alla destinazione, ottimizzando i costi in base al requisito che esista sufficiente liquidità nella giusta direzione tra ogni nodo del percorso. Il Lightning Network migliora notevolmente costi, velocità e privacy a fronte di una perdita di sicurezza (o di un aumento della fiducia richiesta) e di una maggiore complessità. Tuttavia, è pensato per pagamenti quotidiani ad alto volume e basso valore, quindi questo è considerato un compromesso molto ragionevole per i suoi milioni di transazioni giornaliere (fonte: River, 2023).

##### Chaumian eCash Mints

I Fedimint possono essere considerati come una rete Lightning limitata a una comunità. Sono progettati per sfruttare la fiducia intrinseca che esiste all'interno di alcune comunità (ad esempio famiglie, villaggi, gruppi di amici) in cambio di una semplificazione della complessità e di un aumento della privacy per gli utenti. Sono protocolli modulari e open source per custodire e transare bitcoin in un contesto comunitario. Sono interoperabili con lo stesso Lightning Network.

**Cashu** è un token al portatore che può essere conservato su un dispositivo come un telefono cellulare; il design mira a riprodurre i vantaggi del denaro contante fisico ma in forma digitale. Cashu è un esempio di Chaumian eCash costruito su Bitcoin e aumenta la privacy e la resistenza alla censura, riducendo la complessità in cambio della fiducia nella mint eCash utilizzata. Le mint Cashu emettono token eCash, che rappresentano bitcoin, che possono essere spesi dagli utenti senza rivelare la loro identità. Cashu è interoperabile con il Lightning Network.

È probabile che in futuro vengano costruite molte altre applicazioni di secondo livello, con molte applicazioni di terzo livello a loro volta costruite sopra ciascuna di esse.

Come esempio dell'incredibile numero di applicazioni costruite sopra Lightning, ecco un estratto da un rapporto di ricerca sul Lightning Network di River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
