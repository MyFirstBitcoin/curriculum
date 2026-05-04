# 8.2 Metriche per l’analisi del registro

Poiché la trasparenza di Bitcoin è diversa dai sistemi finanziari tradizionali — dove gran parte dei flussi monetari avviene dietro le porte chiuse delle istituzioni — si sviluppa un ricco campo di analisi on-chain, in cui i dati a livello di rete diventano una lente per comprendere il comportamento degli utenti, i flussi monetari e le tendenze di lungo periodo. Queste metriche possono aiutare a rispondere a domande specifiche, come quanto attivamente viene utilizzata la rete, se le monete vengono accumulate o vendute, e se la rete sta diventando più sicura.

Comprendere queste metriche è utile non solo per gli utenti di Bitcoin, ma anche per ricercatori o responsabili politici che cercano di ottenere informazioni su questo sistema finanziario unico per trasparenza.

Questa sezione contiene alcune delle metriche più comunemente utilizzate per analizzare l’attività di Bitcoin, raggruppate in sottocategorie. Non si tratta di un elenco esaustivo. Visita [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) per un elenco più completo e relative descrizioni.



#### 8.2.1 Metriche sugli indirizzi

Le metriche sugli indirizzi sono utili da monitorare nel tempo poiché indicano il livello di attività sulla rete Bitcoin. Ad esempio, man mano che Bitcoin viene adottato, il numero di indirizzi attivi aumenta. Possiamo approfondire ulteriormente analizzando il numero di indirizzi che detengono una quantità minima specificata di Bitcoin, ad esempio 0,1 BTC, in un determinato periodo di tempo, come un anno. Sebbene ciò fornisca una visione dell’adozione di Bitcoin nel tempo, è una misura imperfetta poiché un individuo può possedere più indirizzi Bitcoin. Al contrario, exchange o ETF possono apparire come entità singole pur detenendo fondi per un gran numero di persone.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Indirizzi che detengono Bitcoin > X BTC per anno. Fonte: Bitcoin Magazine Pro._

Confrontando gli indirizzi con il prezzo di mercato attuale di BTC è possibile vedere la percentuale complessiva di indirizzi Bitcoin in profitto. Questo ci permette di monitorare il sentiment di mercato, poiché possiamo vedere quale proporzione del mercato sta mantenendo BTC in profitto o in perdita.

Ad esempio, il **Percentuale di profitto non realizzato** nel grafico qui sotto mostra la proporzione di tutti gli indirizzi del registro con un profitto non realizzato misurato in dollari statunitensi. Nota che, poiché il grafico qui sotto è stato preso vicino al massimo storico di Bitcoin, la percentuale di indirizzi che mostra un profitto non realizzato è vicina al cento per cento. Possiamo anche vedere che periodi prolungati di Percentuale di profitto non realizzato al di sotto di una deviazione standard dalla media sono insoliti. Pertanto, una discesa sotto questa linea può suggerire un buon punto di ingresso per gli acquirenti.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Percentuale di profitto non realizzato. Fonte: checkonchain.com_



#### 8.2.2 Indicatori on-chain

Gli indicatori on-chain sono utili perché offrono una visione del comportamento della rete, oltre a ciò che possono mostrare solo il prezzo e le metriche sugli indirizzi. Aiutano gli analisti a comprendere le azioni e il sentiment dei diversi tipi di partecipanti, come i detentori di lungo periodo rispetto ai trader di breve periodo, monitorando come le monete vengono detenute, spostate o valutate nel tempo. Questi indicatori sfruttano la natura trasparente del registro per rivelare dinamiche di mercato nascoste come accumulo, distribuzione o anche la convinzione degli investitori. Questo li rende particolarmente utili per identificare tendenze strutturali, valutare se il mercato è surriscaldato o sottovalutato e anticipare i punti di svolta in un ciclo di mercato.

Ad esempio, esaminando il valore delle detenzioni di BTC da quando sono state transate l’ultima volta, possiamo dedurre se il mercato è in difficoltà (come potrebbe accadere durante un minimo importante del ciclo). Questa metrica è nota come **Prezzo Realizzato** e ci fornisce un ‘costo medio di acquisto’ di tutti i BTC in circolazione. Se il prezzo di mercato scende sotto il Prezzo Realizzato, questo mostra che in aggregato la maggior parte degli indirizzi sta registrando una perdita teorica.

Raggruppando ulteriormente i dati del registro in fasce di età, possiamo mostrare come la quantità di BTC si sposta tra indirizzi nel tempo, creando schemi ondulati in un grafico noti come **Onde HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Onde HODL di Bitcoin. Fonte: Bitcoin Magazine Pro._

Le onde HODL mostrano cosa stanno facendo i detentori di BTC a lungo, medio e breve termine. Ad esempio, nel grafico sopra, i detentori di breve termine sono mostrati in rosso e arancione e possiamo vedere picchi di attività quando questo gruppo si affretta ad acquistare vicino ai massimi di mercato. All’altro estremo, possiamo vedere che i detentori di lunghissimo termine (in viola e blu) stanno aumentando costantemente la loro quota complessiva della rete, indicando una forte convinzione tra questi gruppi. Il grafico non è perfetto poiché alcune monete possono passare da vecchi a nuovi indirizzi sotto il controllo dello stesso utente. Tuttavia, offre una visione interessante della convinzione dei detentori di lungo periodo.

Un altro modo per esaminare il ‘denaro intelligente’ dei detentori di lungo periodo è analizzare i **Coin Days Destroyed** (CDD). Il concetto di ‘Coin Days’ è un multiplo del numero di BTC moltiplicato per i giorni trascorsi dall’ultimo movimento delle monete. Ad esempio, 5 BTC che non si muovono da 100 giorni hanno accumulato 500 coin days e 10 BTC che non si muovono da 10 giorni hanno accumulato 100 coin days. In questo modo, diamo un peso maggiore alle monete detenute più a lungo. Quando queste monete vengono spostate, quei coin days vengono ‘distrutti’. Questo indicatore mostra aumenti nei CDD in momenti di movimenti di prezzo significativi, offrendo agli analisti un modo per distinguere l’attività di mercato di routine da cambiamenti significativi nel sentiment dei detentori di lungo periodo.

Un’altra metrica che può aiutare a identificare se il mercato sta sottovalutando o sopravvalutando BTC è il rapporto tra valore di mercato e valore realizzato, ovvero il **MVRV**. Si calcola semplicemente come il rapporto tra il valore di mercato (numero di BTC in circolazione moltiplicato per il prezzo di mercato) diviso per il valore realizzato (la somma di tutti i BTC dall’ultimo movimento). Un MVRV elevato suggerisce che più monete sono in profitto (spesso visto vicino ai massimi di mercato) e un MVRV basso indica che molte monete sono detenute in perdita (visto vicino ai minimi di mercato).



#### 8.2.3 Metriche del mining

Le metriche del mining sono utili per comprendere la sicurezza, gli incentivi economici e la salute complessiva della rete Bitcoin. Metriche come hashrate, ricavi dei miner, difficoltà e rapporto delle commissioni rivelano quanta potenza computazionale sta proteggendo la blockchain e quanto bene i miner vengono ricompensati per le loro attività.

L’**Hashrate** della rete Bitcoin è forse l’indicatore più comunemente citato della salute della rete e della forza della sicurezza. Poiché il processo di mining protegge la rete e conferma che le transazioni sul registro sono valide, maggiore è la potenza di calcolo (o di hashing), più difficile sarà per un attore malevolo sopraffare e attaccare la rete.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate di Bitcoin. Fonte: Bitcoin Magazine Pro._

Il grafico sopra mostra che, a maggio 2025, la potenza di calcolo totale della rete è di circa 900 TeraHash/s (900 trilioni di calcoli crittografici ‘hash’ al secondo). Se l’hashrate è in aumento, significa che la rete sta diventando più sicura, il che è rassicurante per gli utenti.

Il Puell Multiple (ideato da David Puell) osserva il ciclo di mercato dal punto di vista dei miner e dei loro ricavi. La metrica si calcola dividendo l’emissione giornaliera di BTC (in USD) per la media mobile a 365 giorni del valore dell’emissione giornaliera. La metrica aiuta a identificare periodi di stress o sollievo per i miner. Storicamente, un valore superiore a 3 ha preceduto un calo del valore di mercato di BTC, poiché indica che i miner sono altamente redditizi. Un valore inferiore a 0,5 indica stress e storicamente ha segnalato i minimi di mercato per il valore di BTC.
