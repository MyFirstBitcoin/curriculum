# 9.1 Nodi e Minatori Bitcoin

I nodi Bitcoin possono sembrare tecnici, ma sono semplicemente dei software che mantengono una copia della blockchain di Bitcoin su un computer. La blockchain è un registro condiviso di tutte le transazioni Bitcoin.

Quando gestisci un tuo nodo, verifichi personalmente le transazioni Bitcoin invece di affidarti a qualcun altro. Questo ti dà maggiore indipendenza e aiuta a mantenere la rete Bitcoin decentralizzata.

Puoi pensare a un nodo Bitcoin come a un vigile digitale con alcuni compiti importanti.

1. Mantiene una copia della blockchain, che è la storia di tutte le transazioni Bitcoin.
1. I nodi si collegano con altri nodi in tutto il mondo e condividono informazioni. Un esempio è l'elenco delle nuove transazioni in attesa di conferma, chiamato mempool.
1. I nodi controllano che ogni transazione rispetti le regole di Bitcoin. Se una transazione non è valida, il nodo la rifiuta.

I nodi aiutano anche i nuovi nodi a unirsi alla rete condividendo con loro la blockchain. Tuttavia, ogni nuovo nodo verifica comunque tutte le regole in modo indipendente.

Chiunque può gestire un nodo installando un software come Bitcoin Core e scaricando la blockchain. Una volta configurato, il nodo continua a ricevere nuovi blocchi circa ogni 10 minuti e li verifica prima di aggiungerli alla propria copia della blockchain.

Gestire un nodo aiuta a rendere la rete Bitcoin più sicura e decentralizzata, perché più persone verificano il sistema in modo indipendente.

#### Che cos'è un nodo Bitcoin?

> Lo scopo del mining non è la creazione di nuovi bitcoin; quello è il sistema di incentivi. Il mining è il meccanismo attraverso cui la sicurezza di Bitcoin è decentralizzata.  
_Andreas M. Antonopoulos_


> **Callout**
>
> I miner raccolgono le transazioni non confermate, formano un blocco e utilizzano energia per trovare una chiave che aggiunge e protegge il blocco.


I miner competono per aggiungere il prossimo blocco di transazioni alla blockchain. Per farlo, devono trovare un numero speciale che crea un hash di blocco valido. Puoi immaginarlo come cercare la chiave giusta tra miliardi di possibilità. Il primo miner che trova l'hash corretto vince la gara e ottiene il diritto di aggiungere il proprio blocco alla blockchain.

Quando un miner trova un hash valido, condivide il proprio blocco con la rete. Gli altri miner verificano rapidamente che la soluzione sia corretta. Se lo è, il blocco viene aggiunto alla blockchain, contribuendo a mantenere sicuro il registro pubblico di Bitcoin.

I miner guadagnano bitcoin in due modi:

* **Ricompense di blocco:** Nuovi bitcoin vengono creati e assegnati al miner che aggiunge con successo un blocco alla blockchain.
* **Commissioni di transazione:** Quando le persone inviano bitcoin, includono una piccola commissione. Il miner che aggiunge il blocco riceve le commissioni delle transazioni incluse in quel blocco.

#### Halving di Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Le ricompense dei miner per il completamento di un blocco si dimezzano ogni 210.000 blocchi, circa ogni quattro anni.


Bitcoin ha una fornitura massima fissa di 21.000.000 bitcoin, ma non tutti sono stati creati quando Bitcoin è stato lanciato. Invece, nuovi bitcoin vengono introdotti gradualmente in circolazione tramite **il mining**.

Quando i miner aggiungono con successo un nuovo blocco di transazioni alla rete Bitcoin, ricevono una **ricompensa di blocco** in bitcoin. Nei primi tempi di Bitcoin, questa ricompensa era di 50 bitcoin per blocco. Questa ricompensa incoraggiava le persone a utilizzare potenza di calcolo ed elettricità per aiutare a proteggere la rete.

Circa ogni 210.000 blocchi (all'incirca ogni 4 anni), la ricompensa di blocco viene dimezzata. Questo evento si chiama **halving**. L'halving rallenta la creazione di nuovi bitcoin e aiuta a garantire che la fornitura totale non superi mai i 21 milioni. Nel tempo, questo rende i bitcoin sempre più scarsi.


> **Definition – Offerta circolante**
>
> **L'offerta circolante** si riferisce alla quantità totale disponibile di una valuta. Nel caso di Bitcoin, l'offerta circolante totale è il numero di monete che sono state minate e sono in circolazione in un dato momento.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/ee94ebc906c46f44226a0e366a3991b1b3a0ae29-292x200.svg)


> **Definition – Programma di emissione di Bitcoin**
>
> Il **programma di emissione di Bitcoin** è il piano prestabilito e pubblico per l'immissione di nuovi bitcoin in circolazione, progettato per mantenere la scarsità di Bitcoin nel tempo.


Dopo ogni evento di halving, la ricompensa in bitcoin che i miner ricevono per l'aggiunta di un blocco viene dimezzata. Questo riduce la velocità con cui vengono creati nuovi bitcoin.

I miner continuano comunque a guadagnare le commissioni delle transazioni incluse nel blocco che minano. Nel tempo, si prevede che queste commissioni diventino una parte sempre più importante delle entrate dei miner.

I halving sono integrati nel protocollo di Bitcoin e avvengono automaticamente circa ogni quattro anni. Per questo motivo, il programma di emissione di Bitcoin è prevedibile e trasparente.

La tabella mostra i prossimi halving, includendo la data approssimativa, il numero del blocco in cui avvengono, la nuova ricompensa per blocco e la percentuale della fornitura totale di bitcoin che sarà stata minata.


| Evento | Data | Blocco | Ricompensa | Minato |
| --- | --- | --- | --- | --- |
| 5° Halving | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| 6° Halving | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| 7° Halving | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Man mano che vengono minati più bitcoin, la fornitura circolante continua ad aumentare fino a raggiungere il massimo di 21.000.000 di bitcoin, previsto intorno all'anno 2140. Poiché nel tempo vengono creati sempre meno nuovi bitcoin, se la domanda aumenta, il prezzo di Bitcoin può salire. Questo incentiva anche i miner a continuare a proteggere la rete contribuendo con la loro potenza di calcolo.

#### Cos'è un hash di blocco valido in Bitcoin?

In Bitcoin, i miner competono per trovare un codice speciale chiamato **hash di blocco**. Questo codice identifica un blocco di transazioni e permette che venga aggiunto alla blockchain.

Ogni blocco contiene informazioni sulle transazioni recenti e include anche l'hash del blocco precedente. Questo collega ogni blocco all'altro, formando una catena dal primissimo blocco (il Blocco Genesis) fino al più recente.

Un hash funziona come un **impronta digitale** per i dati nel blocco. Se qualsiasi informazione nel blocco venisse modificata, anche l'impronta digitale cambierebbe. Questo rende facile per chiunque verificare che la cronologia delle transazioni della blockchain non sia stata alterata e aiuta a mantenere sicura la rete.


> **Callout**
>
> Satoshi Nakamoto, il creatore di Bitcoin, ha minato il Blocco Genesis, che ha sbloccato un totale di 50 bitcoin.


#### La corsa per minare un blocco

I miner competono per trovare un hash di blocco valido. Il primo miner che ne trova uno può aggiungere il nuovo blocco alla blockchain e ricevere una ricompensa in bitcoin.

Per essere valido, l'hash del blocco deve essere inferiore a un numero stabilito dalla rete chiamato target di difficoltà. Poiché gli hash sono casuali, i miner devono continuare a provare diversi input finché non ne trovano uno che funziona.

Se troppi miner competessero, i blocchi verrebbero trovati troppo velocemente. Se invece partecipassero troppo pochi miner, ci vorrebbe troppo tempo per trovare i blocchi. Per mantenere il sistema efficiente, Bitcoin regola automaticamente la difficoltà ogni 2.016 blocchi (circa ogni due settimane).

Questa regolazione assicura che, in media, venga aggiunto un nuovo blocco alla blockchain circa ogni 10 minuti.


> **Definition – Definizione di livello di difficoltà**
>
> Il **livello di difficoltà** nel mining di Bitcoin misura quanto sia difficile trovare un hash di blocco valido. La rete regola questa difficoltà ogni 2.016 blocchi (circa ogni due settimane) in modo che i nuovi blocchi vengano aggiunti alla blockchain circa ogni 10 minuti. Più alta è la difficoltà, più è difficile per i miner trovare un blocco valido.


Trovando un hash di blocco valido, un miner dimostra di aver svolto il lavoro necessario per aggiungere un nuovo blocco alla blockchain. Questo processo si chiama **Proof of Work** (PoW). È il meccanismo di sicurezza che permette a Bitcoin di confermare le transazioni e aggiungere nuovi blocchi alla blockchain. Il miner che trova per primo l'hash valido guadagna una ricompensa in bitcoin, che include la ricompensa per il blocco e le commissioni di transazione delle transazioni incluse in quel blocco.

La Proof of Work (PoW) aiuta a mantenere sicuro Bitcoin rendendo estremamente costoso per chiunque tentare di imbrogliare o prendere il controllo della rete. Invece, è molto più conveniente seguire le regole.

I miner svolgono quattro ruoli principali:

1. **Raccogliere le transazioni**: I miner scelgono le transazioni che sono state inviate alla rete e le inseriscono in un blocco candidato.
1. **Eseguire la Proof of Work**: I miner competono per risolvere un difficile puzzle matematico trovando un hash di blocco valido.
1. **Trasmetti il blocco**: Il primo miner che trova una soluzione valida condivide il nuovo blocco con la rete.
1. **Ottieni ricompense**: Se il blocco è valido, viene aggiunto alla blockchain e il miner riceve nuovi bitcoin creati più le commissioni di transazione.

Molti miner in tutto il mondo cercano di creare il prossimo blocco contemporaneamente. Quando un miner trova una soluzione valida, la rete controlla il blocco. Se tutto è corretto, viene aggiunto alla blockchain. Gli altri blocchi in competizione vengono scartati. Questo processo mantiene la rete in accordo e previene la doppia spesa.

* I miner sono computer che aiutano a mantenere e aggiornare il registro di Bitcoin.
* Raccolgono le transazioni e le raggruppano in un blocco. Poi elaborano i dati del blocco tramite un algoritmo di hashing per creare un codice unico chiamato hash.
* I miner ripetono questo processo molte volte, cercando un hash che rispetti le regole di Bitcoin. Il primo miner che trova un hash valido riceve nuovi bitcoin come ricompensa e il suo blocco viene aggiunto alla blockchain.
* L'hash di ogni blocco lo collega anche al blocco precedente. Se qualcuno provasse a modificare una transazione passata, gli hash non corrisponderebbero più e la rete rifiuterebbe la catena alterata. Questo è ciò che mantiene sicuro il registro di Bitcoin.
