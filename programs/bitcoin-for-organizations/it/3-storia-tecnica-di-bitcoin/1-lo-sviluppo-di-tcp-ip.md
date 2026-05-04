# 3.1 Lo sviluppo di TCP/IP

La maggior parte di noi conosce i protocolli TCP/IP utilizzati oggi come fondamento di Internet. Le loro origini risalgono alla fine degli anni '70, quando gli scienziati esploravano progetti alternativi ad Arpanet – una rete ancora più antica concepita dal Dipartimento della Difesa degli Stati Uniti per consentire la condivisione delle risorse tra computer remoti. TCP/IP divenne lo standard di protocollo per Arpanet nel 1983, il che portò a renderlo il modello di rete dominante entro la fine degli anni '90 e la base per Internet su cui oggi funziona Bitcoin.


| Modello OSI | TCP/IP |
| --- | --- |
| Applicazione | Applicazione |
| Presentazione | Applicazione |
| Sessione | Applicazione |
| Trasporto | Trasporto |
| Rete | Rete |
| Collegamento dati | Collegamento dati |
| Fisico | Fisico |


Contemporaneamente allo sviluppo del modello TCP/IP, veniva sviluppato un quadro simile ma più completo dall'Organizzazione Internazionale per la Standardizzazione (ISO) e dall'industria delle telecomunicazioni (CCITT). Il processo per sviluppare nuovi protocolli o suggerire modifiche era lento e macchinoso rispetto all'approccio più decentralizzato utilizzato per sviluppare TCP/IP, portando così al predominio di quest'ultimo approccio oggi.

##### Richiesta di Modifica

Qualsiasi sviluppo suggerito ai protocolli esistenti o idee per nuovi protocolli può essere proposto nel modello TCP/IP tramite una **Richiesta di Modifica** (RFC). Queste passano attraverso un processo di approvazione, gestito dall'Internet Engineering Task Force (IETF), e diventano open source una volta approvate per permettere a chiunque di implementarle e adottarle. Alcuni esempi degni di nota:

* 1969 RFC 1 Documentava come i pacchetti sarebbero stati inviati nell'Arpanet
* 1981 RFC791 definiva il protocollo Internet V4 – ancora oggi ampiamente adottato
* 1982 RFC 821 Simple Mail Transfer Protocol
* 1987 Domain Name System – come i nomi di dominio vengono risolti in indirizzi IP
* 1999 RFC 2616 Hypertext Transfer Protocol – essenziale per la navigazione web


> **Callout**
>
> La **Bitcoin Improvement Proposal** (BIP) segue un approccio simile alle RFC, ma concentrandosi esclusivamente sui miglioramenti a Bitcoin stesso piuttosto che sullo sviluppo di nuovi o alternativi protocolli. Anche Bitcoin prende spunto da questo modello a strati, e vedrai protocolli aggiuntivi descritti come layer due o tre.


Allo stesso modo in cui gli strati di base del modello TCP/IP sono cambiati relativamente poco negli ultimi decenni, con l'innovazione che avviene negli strati superiori, anche il layer base di Bitcoin si prevede che cambi molto lentamente a questo punto, con soluzioni di scalabilità come Lightning e Liquid che operano sopra di esso.

Un buon esempio di come i protocolli di base diventino difficili da modificare nel tempo è IPv6. L'esaurimento previsto dello spazio degli indirizzi in IPv4 ha creato la necessità di un nuovo protocollo. Il primo standard in bozza è stato creato nel 1998, ma ratificato come standard Internet solo nel 2017. Sebbene abbia risolto molti problemi di IPv4 e sia molto più a prova di futuro, la sua adozione nel settore è ancora molto lenta. Nel frattempo, molti nuovi protocolli sono stati definiti negli strati superiori per abilitare multimedia, email, ecc.

##### I mattoni fondamentali utilizzati da Bitcoin

Questa separazione dei problemi di interconnettività permette ai protocolli di essere sviluppati indipendentemente dagli strati sopra e sotto. Invece di dover reinventare soluzioni per ogni strato, Bitcoin come rete può fare affidamento sulle capacità sottostanti della rete fornite dagli strati fisico e di collegamento dati.


| Livello | TCP/IP Originale |
| --- | --- |
| Applicazione | Utilizza il Domain Name System (DNS) per identificare i nodi vicini. La porta 8333 segnala il protocollo Bitcoin. |
| Trasporto | UDP per comunicazioni FIBRE tra miner per bassa latenza. TCP per comunicazioni P2P tra nodi. |
| Trasporto | Instradamento TOR: consente anonimato e privacy. Protocollo di broadcast: instrada il traffico attraverso la rete. |
| Collegamento | Funziona su qualsiasi mezzo (ad es., Ethernet, Wi-Fi, ecc.) |
| Fisico | Trasmissione fisica tramite wireless, Ethernet o altre interfacce hardware. |


##### Bitcoin è un protocollo neutrale per trasferire valore come HTTPS è un protocollo per trasferire informazioni

* **HTTPS**: Siti web sicuri
* **SMTP**: Invia email
* **FTP**: Trasferisci file
* **DNS**: Gestisci nomi di dominio
* **BTC**: Conserva e trasferisci valore

Bitcoin permette di trasferire valore in modo affidabile e senza la necessità di una terza parte tra persone o dispositivi attraverso Internet. Si prevede che questo sbloccherà un valore enorme.
