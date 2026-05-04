# 3.7 Bitcoin

Dopo molti anni e tentativi falliti, i Cypherpunk avevano per lo più iniziato a perdere interesse nell’idea di una valuta digitale senza permessi, quando Adam Back ricevette un’email con un link a una bozza di white paper intitolata ‘electronic cash without a third party’ da una persona anonima che si faceva chiamare Satoshi Nakamoto.

Per ricapitolare a questo punto, abbiamo almeno le seguenti idee:

* Firme crittografiche che potevano fornire un certo livello di privacy e anonimato
* Concetto di una valuta non garantita (B-Money)
* Proposte (ma non mezzi) per limitare l’emissione di nuova valuta
* Monete digitali la cui proprietà era attribuita tramite chiavi pubbliche (B-Money) e potevano essere trasferite firmando e riassegnate in base all’indirizzo del destinatario (RPOW e Hashcash)
* Tutti i nodi mantengono una copia di un registro totalmente distribuito (B-Money) (all’epoca scartato come impraticabile)
* Protocollo di marcatura temporale – utilizzo dell’hashing ad albero di Merkle per fornire una cronologia degli eventi matematicamente dimostrabile e difficile da falsificare se tutti gli utenti mantengono gli stessi registri
* Proof of work per collegare uno sforzo reale al sistema (ma utilizzando l’hash stesso come valuta)
* Reti totalmente decentralizzate in cui tutti i peer sono uguali e possono entrare e uscire dalla rete (BitTorrent)
* Concetto di collegare nuovi hash ai precedenti (Bit Gold e marcatura temporale)

Quello che mancava in quel momento includeva:

* Una soluzione praticabile al problema dei ‘generali bizantini’
* Un metodo per limitare la quantità di denaro in circolazione nonostante i continui miglioramenti hardware
* Schema di incentivi per far partecipare le persone (problema dell’uovo e della gallina)

L’altra grande differenza tra i tentativi recenti e Bitcoin era che Satoshi aveva lavorato sul codice per un po’ di tempo nel vero spirito originale dei ‘Cypherpunk scrivono codice’ prima di annunciarlo sulle mailing list, a differenza di Bit Gold e B-Money che erano più concettuali.

Qual è stata l’innovazione che ha distinto Bitcoin dai precedenti tentativi di denaro elettronico?

La proof of work sarebbe stata utilizzata come meccanismo di consenso e come modo per fornire sicurezza e immutabilità: invece di usare l’hash come forma di denaro, sarebbe stato utilizzato da un nuovo processo concettuale chiamato mining, in cui un nodo raggruppava un insieme di transazioni, aggiungeva un numero casuale e poi applicava l’hashing al ‘blocco’ di dati. Un blocco valido che soddisfaceva il requisito dell’hash sarebbe stato poi pubblicizzato alla rete. Questi blocchi sarebbero stati collegati tra loro utilizzando l’hash del blocco precedente in ciascuno, e la blockchain più lunga sarebbe stata utilizzata in caso di spareggio, quando nodi diversi avrebbero validato e pubblicizzato blocchi diversi contemporaneamente creando divisioni nella catena. La proof of work è diventata il meccanismo distribuito di spareggio per risolvere il problema dei generali bizantini.

Questi miner ricevevano anche un incentivo a fornire la potenza di calcolo necessaria per eseguire la proof-of-work, venendo assegnati nuovi bitcoin per ogni blocco. La quantità di Bitcoin assegnata è anche programmata per diminuire circa ogni 4 anni fino a quando tutti i Bitcoin saranno stati creati, creando un limite massimo al totale di Bitcoin che sarà mai in circolazione, fissato a 21 milioni.

L’idea più originale fu il modo in cui risolse il problema di quanta moneta viene creata man mano che l’hardware migliora e si può applicare più potenza alla rete. I timestamp di un numero fisso di blocchi (2016) sarebbero stati mediati, e se venivano creati troppo rapidamente, l’hash necessario per creare un nuovo blocco sarebbe stato reso più difficile, se troppo lentamente sarebbe stato reso più facile. Questo era integrato nel protocollo decentralizzato che tutti i nodi eseguono, quindi qualsiasi miner che lo ignorasse avrebbe sprecato energia per minare un blocco senza alcun beneficio, poiché sarebbe stato rifiutato dal resto della rete. Questo aggiustamento garantisce che la creazione di nuovi blocchi rimanga secondo il programma previsto di emissione e fornisce incentivi ai miner per ‘seguire le regole’.

####   
Riepilogo

Molti dei pezzi del puzzle necessari per costruire un sistema di denaro elettronico peer to peer decentralizzato basato su principi di moneta solida erano già presenti prima che Satoshi pubblicasse il suo whitepaper e poco dopo il rilascio iniziale del codice.

> La natura di Bitcoin è tale che una volta rilasciata la versione 0.1, il design di base è stato fissato per tutta la sua esistenza  
_Satoshi Nakamoto_

Sebbene molte idee di miglioramento (BIP) siano state proposte e adottate, Bitcoin ha continuato a funzionare in background dal 2009 seguendo il protocollo progettato nella versione iniziale e con pochissime interruzioni. Tutti i miglioramenti sono stati fatti mantenendo la compatibilità retroattiva con tutte le versioni precedenti.



##### Note

1. Per una spiegazione del problema dei Generali Bizantini - vedi [https://it.wikipedia.org/wiki/Problema_dei_generali_bizantini](https://en.wikipedia.org/wiki/Byzantine_fault)
