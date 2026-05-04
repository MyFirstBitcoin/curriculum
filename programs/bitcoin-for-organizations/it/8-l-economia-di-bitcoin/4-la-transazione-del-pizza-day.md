# 8.4 La transazione del Pizza Day

Finora, questo modulo si è concentrato sull'utilizzo della natura aperta del registro di Bitcoin per compilare metriche utili dai dati aggregati delle transazioni. Tuttavia, è possibile utilizzare i dati del registro e i block explorer per esaminare transazioni reali e tracciare il movimento dei fondi all'interno della rete.

Ogni anno, il 22 maggio, la comunità Bitcoin celebra Laszlo Hanyecz, che è diventato la prima persona di cui si ha notizia ad aver usato bitcoin per acquistare beni fisici. Il 18 maggio 2010, Hanyecz annunciò su un forum di Bitcointalk.org che stava cercando una pizza ed era disposto a pagare in BTC. Offrì 10.000 BTC a chiunque fosse disposto a concludere la transazione. Aspettò diversi giorni, finché uno studente di 19 anni, Giovanni Sturdivant, accettò e inviò due pizze grandi.

La **Pizza Day** può essere visualizzata da chiunque e ha il seguente ID di transazione:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Inserendo questo ID di transazione su [mempool.space](https://mempool.space) si ottiene quanto segue:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Data e ora della transazione: 22 maggio 2010

Commissione di rete della transazione: 99.000.000 sats (all'epoca equivaleva a meno di 1 centesimo di euro. A maggio 2025, corrisponde a €87.500,00)

Altezza del blocco: 57.043

Numero di conferme: 838.645 (questo è il numero di blocchi aggiunti al registro dopo questa transazione)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Numero di input della transazione: 131

Numero di output della transazione: 1

Cliccando sulla chiave pubblica di output (che termina con `XaxFyQ`) che sappiamo essere stata di proprietà di Giovanni Sturdivant, che ha ricevuto 10.000 BTC per due pizze, si scopre quanto segue:

Questo indirizzo attualmente ha un saldo di 0,00257879 BTC e sembra che sia stato coinvolto in 14 transazioni, l'ultima delle quali risale al 13 dicembre 2024.



#### 8.4.1 Attività: Discussione di gruppo

1. Descrivi i benefici (ad esempio, audit, responsabilità) o i rischi (ad esempio, problemi di privacy) per individui o aziende che utilizzano un sistema di transazioni così trasparente e aperto.
1. In che modo questo tipo di trasparenza finanziaria potrebbe influenzare settori come la beneficenza, gli appalti pubblici, le rimesse o le forze dell'ordine?
1. I sistemi bancari tradizionali dovrebbero offrire un livello di visibilità simile? Saranno costretti a farlo dal mercato?
