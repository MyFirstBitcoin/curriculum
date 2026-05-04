# 6 - Come usare Bitcoin

Durata: 90 minuti

Idea centrale: Usare Bitcoin on-chain insegna agli studenti come funzionano in pratica la proprietà, l'auto-custodia e la verifica, trasformando la teoria in azione finanziaria diretta.

#### Obiettivi di apprendimento

Al termine di questa lezione, gli studenti dovrebbero essere in grado di:

* Identificare i modi comuni per acquisire e scambiare bitcoin, inclusi i metodi peer-to-peer e tramite exchange centralizzati.
* Spiegare la differenza tra wallet auto-custodiali e custodiali, e perché l'auto-custodia è importante in Bitcoin.
* Descrivere lo scopo delle chiavi private, degli indirizzi pubblici, delle seed phrase e delle interfacce dei wallet.
* Confrontare diversi tipi di wallet e valutarne i pro e i contro in base a sicurezza, comodità, privacy e controllo.
* Configurare un wallet Bitcoin mobile e spiegare il processo base di recupero.
* Dimostrare come ricevere e inviare una transazione bitcoin on-chain.

Applicare il principio "Non Fidarti, Verifica" nella scelta del wallet, nelle transazioni e nell'uso più ampio di Bitcoin.

#### Strumenti e risorse

##### Materiali visivi

* Capitolo 6 - Come usare Bitcoin

##### Libreria di supporto

* Scheda di riferimento del vocabolario — Capitolo 6 — Termini: wallet, chiave privata, indirizzo pubblico, seed phrase, custodiale, auto-custodiale, UTXO, commissione di transazione
* Tabelle di confronto e schede di riferimento — Confronto tra tipi di wallet (custodiale, mobile, hardware, cartaceo)
* Approfondimenti tecnici — Chiavi pubbliche/private, modello UTXO, conferma delle transazioni
* Approfondimento sulla sicurezza delle chiavi private — Seed phrase, derivazione delle chiavi, metodi di backup, vettori di attacco
* Guida all'anatomia di una transazione — Esempio passo-passo di come funziona una transazione Bitcoin
* Checklist delle migliori pratiche di sicurezza — Prima di iniziare, creazione del wallet, ricezione, invio, prevenzione del phishing

#### Attività

* Transazioni in azione
* Staffetta Lightning
* Esplorando il Mempool

#### Didattica online

* Chiarisci fin dall'inizio se gli studenti stanno guardando una dimostrazione o stanno configurando un wallet in prima persona.
* Usa screenshot grandi e leggibili per ogni passaggio della configurazione del wallet.
* Metti in pausa dopo ogni passaggio e chiedi agli studenti di confermare la comprensione in chat prima di proseguire.
* Dai un avvertimento diretto prima della sezione sulla seed phrase e ricorda agli studenti di non condividere mai informazioni sensibili online.

#### Preparazione

* Scarica e testa un'app di wallet mobile (Blue Wallet o Muun); prepara screenshot dei passaggi chiave della configurazione.
* Prepara una guida alla configurazione del wallet (download → creazione → backup della seed → ricezione) come riferimento.
* Assicurati che la rete/WiFi funzioni; tieni pronta un indirizzo demo e un codice QR da mostrare.

#### Procedura

Questa lezione passa dalla teoria alla pratica diretta. Ora corrisponde direttamente alla struttura del Diploma, così che acquisizione, wallet, configurazione, transazioni e verifica compaiano sotto gli stessi titoli principali della guida per studenti. Il supporto didattico extra rimane inserito all'interno di queste sezioni.

##### 6.0 Introduzione, 8 minuti

Inizia collegando questo capitolo al precedente:

* Se Bitcoin è denaro, come fanno le persone a ottenerlo e usarlo concretamente?
* Cosa significa davvero controllare i propri bitcoin?
* Perché usare Bitcoin è diverso dall'usare l'app di una banca?

Chiarisci che questo capitolo riguarda l'uso pratico. Gli studenti non stanno più solo imparando cosa sia Bitcoin, ma stanno imparando come interagirci direttamente.

##### 6.1 Acquisire e scambiare Bitcoin, 12 minuti

Spiega che le persone possono acquisire bitcoin in diversi modi, tra cui:

* ricevere un pagamento in bitcoin
* minare bitcoin
* scambiare euro contanti con bitcoin di persona
* scambiare euro per bitcoin online

Poi concentrati sulle due principali modalità di acquisizione trattate nel capitolo:

* peer-to-peer, di persona
* peer-to-peer, online
* exchange centralizzati

Rendi chiari i compromessi.

Per il P2P di persona, sottolinea lo scambio diretto senza una banca o un intermediario, ma menziona anche i rischi pratici di incontrare persone per scambi in contanti.

Per il P2P online, spiega l'escrow in termini semplici, come un modo per ridurre il rischio della controparte pur permettendo lo scambio diretto tra pari.

Per gli exchange centralizzati, chiarisci che sono comodi, ma richiedono agli utenti di fidarsi di una società, spesso di condividere informazioni personali e di lasciare i fondi sotto il controllo di terzi fino al prelievo. Questo è un buon momento per rafforzare che la comodità spesso comporta compromessi in termini di privacy e sovranità.

##### 6.2 Introduzione ai wallet Bitcoin, 35 minuti

**Cosa è realmente un wallet Bitcoin**

Chiarisci subito un malinteso comune: i bitcoin non sono conservati all'interno dell'app del wallet come il contante fisico in una borsa.  
I bitcoin esistono sul registro mantenuto dalla rete. Quello che l'utente controlla è la possibilità di spenderli tramite le chiavi private.

Poi spiega le due cose che spesso si intendono con "wallet":

* il sistema di chiavi private, da cui vengono generate le address
* l'app o l'interfaccia usata per interagire con la rete

Usa l'analogia dell'email del capitolo se utile:

* indirizzo pubblico = come un indirizzo email che puoi condividere
* chiave privata = come una password che devi proteggere

Sii molto chiaro qui: chi controlla le chiavi private controlla i bitcoin. Questo è il concetto fondamentale che gli studenti devono comprendere.

**Wallet self-custodial vs custodial**

Questa è una delle parti più importanti del capitolo.

Spiega chiaramente la distinzione:

* Wallet self-custodial: l'utente controlla le chiavi private
* Wallet custodial: una terza parte controlla le chiavi private per conto dell'utente

Poi illustra i compromessi:

Self-custodial

* pieno controllo sui fondi
* nessun processo di approvazione
* protezione contro confische arbitrarie
* maggiore responsabilità
* nessun recupero facile se si perde la seed phrase

Custodial

* recupero e supporto più semplici
* più semplice per i principianti
* più esposto a blocchi dell'account, hack e controllo di terzi
* l'utente non detiene realmente i bitcoin

Questo è il momento giusto per sottolineare la frase:

"Not your keys, not your coins."

Gli studenti dovrebbero uscire da questa sezione comprendendo non solo lo slogan, ma anche cosa significa realmente nella pratica.

**Tipi diversi di wallet e come sceglierne uno**

Presenta i tipi di wallet trattati nel capitolo:

* wallet online
* wallet mobile
* wallet desktop
* wallet hardware
* wallet cartaceo

Non trattarne uno come perfetto. Spiega invece che ognuno comporta compromessi tra:

* sicurezza
* privacy
* comodità
* compatibilità
* commissioni
* controllo
* reputazione

Chiarisci anche che consigliamo di prestare attenzione al fatto che il software del wallet sia open-source, perché gli strumenti open-source possono essere revisionati, controllati e portati avanti dalla comunità. Questo si collega direttamente al principio della verifica in Bitcoin.

##### 6.3 Configurare un wallet Bitcoin su cellulare, 10 minuti

Guida gli studenti attraverso il processo di base mostrato nel capitolo:

* scarica il wallet
* crea un nuovo wallet
* genera e scrivi la frase di recupero
* conferma la frase di recupero
* aggiungi sicurezza extra se disponibile
* apri il wallet e trova la funzione ricevi

Rendi molto esplicito l’avvertimento sulla seed phrase:

* se la seed phrase viene persa, si può perdere l’accesso ai fondi
* se qualcun altro ottiene la seed phrase, può prendere i fondi

Se gli studenti stanno facendo questa attività in pratica, l’educatore dovrebbe fermarsi a ogni passaggio e verificare che tutti abbiano capito cosa stanno facendo. Se la lezione è più concettuale, questa sezione può essere spiegata come una dimostrazione invece che eseguita dal vivo. L’opzione di recupero mostrata nel capitolo è anche utile per spiegare che i wallet possono essere ripristinati se la seed phrase è stata salvata correttamente.

##### 6.4 Ricevere e Inviare Transazioni, 17 minuti

**Ricevere e Inviare Transazioni On-chain**

Ora spiega come funzionano le transazioni on-chain.

Per ricevere bitcoin:

* apri il wallet
* tocca ricevi o deposita
* copia l’indirizzo, condividi il link o mostra il codice QR

Per inviare bitcoin:

* apri il wallet
* incolla o scansiona l’indirizzo del destinatario
* inserisci l’importo
* controlla tutti i dettagli
* trasmetti la transazione
* attendi la conferma

Rendi chiari questi punti chiave:

* la transazione trasferisce la proprietà, non monete fisiche
* le transazioni sono irreversibili
* i nodi verificano la validità
* i miner includono le transazioni nei blocchi
* le commissioni influenzano la priorità di conferma
* le transazioni on-chain sono generalmente sicure, ma più lente e spesso più costose rispetto alle transazioni Lightning

Il diagramma del flusso di transazione nel capitolo è particolarmente utile qui, perché aiuta gli studenti a visualizzare il percorso dalla richiesta del wallet alla conferma sulla rete.

**Transazioni in Azione ed Esercizio con Ruoli**

Usa la struttura dell’esercizio cooperativo dal capitolo per rafforzare la comprensione. Spiega i quattro ruoli coinvolti:

* mittente
* destinatario
* miner
* operatore di nodo

Un approccio semplice in classe è assegnare i ruoli e seguire una transazione passo dopo passo. Questo aiuta gli studenti a vedere che una transazione Bitcoin non è magia, ma un processo coordinato che coinvolge approvazione, verifica, inclusione in un blocco e aggiornamenti del registro.

L’obiettivo qui non è la profondità tecnica. È aiutare gli studenti a capire chi fa cosa in una transazione e perché la verifica è importante.

##### 6.5 Non Fidarti, Verifica, 8 minuti

Spiega che questo si applica a:

* wallet
* exchange
* app
* dettagli delle transazioni
* affermazioni su "guadagni facili"
* progetti che fingono di essere come Bitcoin

Chiarisci che Bitcoin richiede agli utenti di pensare in modo critico, verificare ciò che stanno usando ed evitare la fiducia cieca. Spiega anche perché gli strumenti open-source sono importanti in questo contesto: permettono la verifica indipendente.

###### Riepilogo e Verifica della Comprensione

Concludi con alcune domande rapide:

* Qual è la differenza tra un wallet custodial e uno self-custodial?
* Perché la seed phrase è così importante?
* Cosa succede quando invii una transazione on-chain?
* Perché le transazioni on-chain sono più lente rispetto ad alcuni altri pagamenti Bitcoin?
* Cosa significa "Non Fidarti, Verifica" nella pratica?

#### Note per l’Educatore

Questo capitolo è molto pratico, quindi dai priorità a chiarezza, sicurezza e ripetizione.

Gli studenti non devono padroneggiare ogni tipo di wallet in una sola lezione. Gli obiettivi principali sono:

* comprendere le basi dei wallet
* comprendere l’auto-custodia
* imparare il flusso base di una transazione
* adottare una mentalità di verifica responsabile

Sii particolarmente attento quando parli di seed phrase e configurazione del wallet. Gli studenti devono uscire dalla lezione capendo che questi non sono dettagli secondari, ma la base della proprietà di Bitcoin.

I materiali visivi e le attività più utili in questo capitolo sono:

* il confronto tra self-custodial e custodial
* la tabella dei compromessi tra i tipi di wallet
* l’esercizio guidato passo-passo di configurazione del wallet
* il diagramma del flusso di una transazione
* l’attività di transazione basata sui ruoli

##### Cosa Significa Fare Bene

* È importante che gli studenti configurino effettivamente un wallet o assistano a una demo attenta, rendano la seed phrase il fulcro con "Queste 12 parole SONO il tuo Bitcoin", testino scenari come "Cosa succede se perdi il telefono?" e pratichino il riconoscimento del phishing.
* Gli educatori dovrebbero essere guide pratiche che hanno già fatto questi passaggi, essere attenti alla sicurezza senza paranoia e onesti riguardo alla curva di difficoltà e all’apprendimento richiesto.
* Gli studenti sentono di aver imparato una vera abilità che possono usare, capiscono che la seed phrase è reale e importante e non solo astratta, si sentono capaci di detenere i propri Bitcoin e comprendono che la decentralizzazione richiede responsabilità personale.
* Gli Obiettivi di Apprendimento sono raggiunti se gli studenti sanno configurare un wallet e comprendono la differenza tra chiave pubblica e privata, conoscono i compromessi tra wallet custodial e self-custodial, sanno spiegare come funziona una transazione (inclusi input, output e commissioni), dimostrano consapevolezza della sicurezza (inclusa la protezione della seed phrase) e sanno porre domande critiche su proprietà e controllo.

##### Gestione del Tempo

Se il tempo è poco, dai priorità a:

* Comprendere le basi dei wallet
* Comprendere l’auto-custodia
* Imparare il flusso base di una transazione
* Adottare una mentalità di verifica responsabile

Se sei in anticipo, dedica tempo a:

* Tabella di confronto tra self-custodial e custodial
* Tabella dei compromessi tra i tipi di wallet
* Esercizio guidato passo-passo di configurazione del wallet con demo dal vivo
* Diagramma del flusso di una transazione con calcolo delle commissioni
* Pratiche di sicurezza avanzate e considerazioni sui wallet hardware

##### Se gli studenti hanno difficoltà

* Seed phrase come "reale" → "Questa frase È il tuo bitcoin; non esiste assistenza clienti."
* Chiavi pubbliche vs. private → Analogia con l’email (indirizzo vs. password).
* Perché è difficile → "Sei tu a controllarlo; sei tu il responsabile." Riconosci il compromesso.
