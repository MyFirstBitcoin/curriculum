# 8 - Come funziona Bitcoin

Durata: 90 minuti

Idea centrale: La sicurezza di Bitcoin si basa su idee tecniche semplici ma potenti come chiavi, firme, hashing e UTXO, che permettono la proprietà e la verifica senza un'autorità centrale.

#### Obiettivi di apprendimento

Al termine di questa lezione, gli studenti dovrebbero essere in grado di:

* Spiegare come le chiavi pubbliche e private aiutano a proteggere la proprietà e le transazioni di Bitcoin.
* Descrivere cos'è una firma digitale e come dimostra che una transazione è stata autorizzata dal legittimo proprietario.
* Spiegare, in termini semplici, cosa significano crittografia, cifratura e decifratura nel contesto di Bitcoin.
* Definire l'hashing e descrivere perché le funzioni hash sono importanti per la sicurezza e l'integrità dei dati di Bitcoin.
* Identificare le proprietà di base di una funzione hash, come l'output a lunghezza fissa, il comportamento unidirezionale e la sensibilità a piccoli cambiamenti dell'input.
* Spiegare il modello UTXO e come i bitcoin vengono spesi, ricevuti e restituiti come resto tramite gli output delle transazioni.
* Descrivere come i nodi aiutano a prevenire la doppia spesa controllando se un output è già stato speso.

#### Strumenti e risorse

##### Materiali visivi

* Capitolo 8 - Come funziona Bitcoin

##### Libreria di supporto

* Scheda di riferimento del vocabolario — Capitolo 8 — Termini: crittografia, hash, UTXO, firma digitale, chiave privata/pubblica, merkle tree, blockchain
* Librerie di idee sbagliate — Capitolo 8 — Affronta: "la seed phrase persa può essere recuperata", "chiave privata = password", "la blockchain è anonima"
* Spiegazioni tecniche e approfondimenti — Funzioni hash, chiavi pubbliche/private, modello UTXO, sicurezza Proof of Work

#### Attività

* Transazioni in azione
* Esplorare il Mempool

#### Didattica online

* Usa una lavagna digitale e disegna ogni concetto dal vivo invece di affidarti solo alla spiegazione verbale.
* Insegna un'idea tecnica alla volta e fermati spesso per domande di verifica.
* Usa materiali visivi per chiavi, firme, hash e UTXO così gli studenti possono seguire la struttura.
* Mantieni l'obiettivo concettuale ed evita di andare troppo a fondo nella matematica o nel gergo tecnico.

#### Preparazione

* Prepara e plastifica i diagrammi: coppie di chiavi pubblica/privata, firme digitali, modello UTXO, hashing (funzione unidirezionale).
* Salva nei preferiti un esploratore blockchain e un calcolatore di hash SHA-256; seleziona 2-3 transazioni reali di Bitcoin da analizzare passo dopo passo.
* Prepara appunti sulla lavagna per spiegare input, output e come le transazioni vengono confermate sulla blockchain.

#### Procedura

Questa lezione offre agli studenti una prima panoramica del lato tecnico di Bitcoin senza presupporre conoscenze tecniche pregresse. La guida ora segue la stessa struttura compressa del Diploma, con la crittografia raggruppata sotto un'intestazione e gli UTXO sotto un'altra.

##### 8.0 Introduzione, 8 minuti

Inizia impostando le aspettative:

* Cosa rende Bitcoin sicuro se non c'è una banca centrale che lo controlla?
* Come può la rete sapere se una persona possiede davvero i bitcoin che sta cercando di inviare?
* Cosa succede realmente dietro le quinte quando qualcuno effettua una transazione Bitcoin?

Chiarisci che questo capitolo si concentra sulle basi tecniche di Bitcoin, in particolare chiavi, firme, hashing e UTXO. Rassicura anche gli studenti che non è necessario diventare ingegneri per comprendere la logica essenziale. Il capitolo stesso sottolinea questo punto confrontando Bitcoin a Internet: molte persone lo usano ogni giorno senza comprenderne ogni livello sottostante.

##### 8.1 Sicurezza tramite crittografia, 57 minuti

**Bitcoin come registro distribuito su molti computer**

Inizia con la semplice descrizione del capitolo sulla rete Bitcoin:

* Bitcoin è un registro di transazioni
* quel registro è conservato su molti computer chiamati nodi
* il registro è pubblico e pseudonimo
* mostra indirizzi e cronologia delle transazioni, non dettagli di identità personale

Questa sezione aiuta gli studenti a collegarsi a ciò che già sanno dai capitoli precedenti. Bitcoin non si basa su conti nascosti all'interno di una banca. Si basa su un registro condiviso che molti partecipanti possono verificare. è particolarmente utile qui perché mostra utenti, wallet e la rete Bitcoin più ampia collegati al registro pubblico.

**Chiavi pubbliche e private**

Ora passa alla crittografia.

Spiega che ogni utente Bitcoin ha:

* una chiave privata, che deve rimanere segreta
* una chiave pubblica, che può essere condivisa

Chiarisci il loro scopo in termini semplici:

* la chiave privata dimostra il controllo e autorizza la spesa
* la chiave pubblica aiuta gli altri a verificare che la transazione sia stata autorizzata correttamente

Un punto di insegnamento importante del capitolo è che Bitcoin utilizza la crittografia a chiave pubblica/privata, non il modello più vecchio in cui due persone devono prima condividere la stessa chiave segreta. Questo è importante perché permette una verifica sicura senza costringere gli utenti a rivelare il segreto che protegge i loro fondi.

Puoi spiegarlo così:

* la chiave privata è come la prova segreta che il bitcoin ti appartiene
* la chiave pubblica è parte di ciò che permette alla rete di verificare la tua autorizzazione
* chi controlla la chiave privata controlla la possibilità di spendere il bitcoin

Fai attenzione qui a non complicare troppo il linguaggio della crittografia. Il punto più importante per gli studenti è la proprietà e l'autorizzazione.

**Firme digitali e autorizzazione delle transazioni**

Ora spiega cosa succede quando qualcuno invia bitcoin.

Usa la sequenza del capitolo:

* un utente crea una transazione
* il mittente genera una firma digitale usando la propria chiave privata
* la transazione viene trasmessa alla rete
* i nodi verificano che la firma sia valida
* una volta verificata e confermata, la proprietà viene trasferita sul registro

Chiarisci che una firma digitale non è la stessa cosa che digitare un nome. È una prova crittografica che il vero proprietario ha autorizzato la transazione. Questo è uno dei meccanismi fondamentali che permette a Bitcoin di funzionare senza un'autorità centrale che approva manualmente le transazioni. Il diagramma è utile perché mostra visivamente la firma e la verifica, oltre al percorso della transazione dal mittente alla validazione della rete.

Una buona frase per la classe è:

Le transazioni Bitcoin non vengono approvate perché lo dice una banca. Vengono accettate perché la rete può verificare una prova crittografica valida.

**Hashing e funzioni unidirezionali**

Ora spiega l'hashing.

Inizia in modo semplice:

* una funzione prende un input e produce un output
* una funzione unidirezionale è facile da eseguire in una direzione, ma praticamente impossibile da invertire
* una funzione di hash prende dati di qualsiasi dimensione e li trasforma in un output di lunghezza fissa chiamato hash

Usa una delle analogie del capitolo, quella che ti sembra più chiara per il tuo pubblico:

* l'analogia del frullato per le funzioni unidirezionali
* l'analogia dell'impronta digitale per gli hash
* l'analogia dello spartito musicale per controllare se qualcosa è cambiato

L'analogia dell'impronta digitale è probabilmente la più chiara per la maggior parte delle classi:

* un hash è come un'impronta digitale digitale per i dati
* se l'input cambia anche solo un po', l'hash cambia completamente
* questo aiuta i computer a controllare l'integrità e a rilevare le manomissioni

Poi spiega perché l'hashing è importante in Bitcoin:

* le transazioni vengono hashate
* la rete usa gli hash per aiutare a verificare l'integrità
* se una transazione viene modificata, l'hash cambia
* questo aiuta a proteggere il registro da manipolazioni non rilevate

Le immagini alle pagine 7-10 sono molto utili qui. Il capitolo mostra sia l'idea dell'output a lunghezza fissa sia il principio del "piccolo cambiamento, risultato completamente diverso", che è uno dei concetti più importanti che gli studenti devono comprendere.

**Proprietà di base delle funzioni di hash**

Passa brevemente in rassegna le proprietà evidenziate nel capitolo, senza renderle troppo accademiche:

* Deterministica: lo stesso input dà sempre lo stesso output
* Unidirezionale / resistenza alla pre-immagine: non puoi realisticamente invertire il processo
* Sensibile ai cambiamenti: anche una piccola modifica dell'input crea un output molto diverso
* Resistente alle collisioni: è estremamente difficile trovare due input diversi con lo stesso output
* Veloce da verificare: la funzione è efficiente da eseguire e controllare

Non è necessario che gli studenti memorizzino ogni termine, ma dovrebbero capire il concetto generale: l'hashing dà a Bitcoin un modo affidabile per identificare i dati e rilevare i cambiamenti.

##### 8.2 Il modello UTXO, 25 minuti

**Il Modello UTXO**

Ora passiamo alla seconda parte principale del capitolo: gli UTXO, ovvero gli Output di Transazione Non Spesi.

Spiegalo in termini semplici usando l'analogia con il contante del capitolo:

* bitcoin non viene tracciato solo come il saldo di un conto bancario
* invece, è composto da pezzi spendibili chiamati UTXO
* quando spendi bitcoin, usi uno o più UTXO esistenti come input
* nuovi UTXO vengono poi creati come output

Usa l'esempio del capitolo:

* se hai un UTXO da 10 BTC
* e invii 6 BTC
* un nuovo UTXO da 6 BTC va al destinatario
* un nuovo UTXO di resto torna a te
* una piccola parte viene pagata come commissione ai miner

Questo aiuta gli studenti a vedere che Bitcoin funziona più come spendere contanti e ricevere il resto che come sottrarre numeri da una semplice riga di conto. I diagrammi sono particolarmente efficaci qui perché mostrano visivamente un UTXO che viene suddiviso in output per il destinatario, output di resto e commissione.

Rendi espliciti due punti chiave:

* il saldo del tuo wallet è la somma dei tuoi UTXO
* quando spendi, i vecchi UTXO vengono consumati e ne vengono creati di nuovi

**Prevenire la Doppia Spesa**

Concludi il contenuto spiegando una delle implicazioni più importanti del modello UTXO.

Se qualcuno prova a spendere lo stesso output due volte, i nodi rifiutano il secondo tentativo perché mantengono il registro e possono verificare se quell'UTXO è già stato speso. È così che Bitcoin previene la doppia spesa senza bisogno di una società centrale di pagamenti che gestisca i registri. L'esempio è molto utile qui perché mostra Giovanni che combina UTXO, invia fondi a Luca, riceve il resto e fa sì che la transazione confermata aggiorni il registro su tutti i nodi.

Un modo chiaro per dirlo in classe è:

Bitcoin previene la doppia spesa perché la rete tiene traccia di quali output rimangono non spesi e quali sono già stati utilizzati.

###### Riepilogo e Verifica della Comprensione

Concludi con alcune domande rapide:

* Qual è la differenza tra una chiave pubblica e una chiave privata?
* Cosa dimostra una firma digitale?
* Perché l'hashing è utile in Bitcoin?
* Cosa succede se una transazione viene modificata dopo essere stata sottoposta ad hash?
* Cos'è un UTXO in termini semplici?
* Come fa la rete a impedire che qualcuno spenda due volte lo stesso bitcoin?

#### Note per l'Educatore

Questo capitolo contiene un linguaggio più tecnico rispetto ai precedenti, quindi dai priorità alla chiarezza, alle analogie e alla ripetizione.

L'obiettivo non è trasformare gli studenti in sviluppatori. L'obiettivo è aiutarli a capire perché la sicurezza di Bitcoin funziona.

I punti più importanti da privilegiare, se il tempo è poco, sono:

* chiave privata vs chiave pubblica
* firme digitali
* cosa fa l'hashing
* UTXO come pezzi spendibili di bitcoin
* come viene prevenuta la doppia spesa

I visual più utili in questo capitolo sono:

* il diagramma utente-wallet-rete
* il visual della firma digitale
* gli esempi di hashing e i diagrammi dell'output a lunghezza fissa alle pagine 7-10
* i diagrammi UTXO alle pagine 10-12

##### Cosa Significa un Buon Risultato

* È importante trattare la crittografia come una base e non come un mistero, usare molti visual, evitare matematica avanzata, collegarsi ai capitoli precedenti e verificare la comprensione con applicazioni come "Se qualcuno cambia una transazione, cosa si rompe?"
* Gli educatori dovrebbero essere pazienti con gli studenti che fanno fatica, pensare in modo visivo e disegnare tutto, essere onesti su ciò che gli studenti non devono capire, essere disposti a dire "Non lo so ma ecco come potremmo scoprirlo" e rimanere incoraggianti per tutto il tempo.
* Gli studenti capiscono perché Bitcoin non può essere hackerato perché è protetto dalla matematica, rispettano il design elegante del sistema, si sentono a proprio agio con la complessità sapendo che non serve ogni dettaglio, acquisiscono fiducia nel fare domande senza giudizio e riconoscono di aver fatto un salto di livello nella comprensione di qualcosa che la maggior parte delle persone non conosce.
* Gli Obiettivi di Apprendimento sono raggiunti se gli studenti sanno spiegare le basi della crittografia come le funzioni unidirezionali e le firme digitali senza matematica avanzata, comprendono il modello UTXO mostrando che possiedi monete e non conti, riconoscono l'hashing come fondamento della sicurezza di Bitcoin, comprendono l'anatomia di una transazione inclusi firme e conferme, spiegano perché Bitcoin è immutabile e pongono domande critiche su potenziali attacchi o vulnerabilità.

##### Gestione del Tempo

Se il tempo è poco, dai la priorità a:

* Chiave privata vs chiave pubblica
* Firme digitali
* Cosa fa l'hashing
* UTXO come porzioni spendibili di bitcoin
* Come viene impedita la doppia spesa

Se sei in anticipo, approfondisci:

* Diagramma utente-wallet-rete e modello visivo di sicurezza
* Firma digitale: processo crittografico dettagliato (visuale)
* Alberi di Merkle e sicurezza della catena
* Vettori di attacco avanzati e perché falliscono

##### Se gli studenti fanno fatica

* La crittografia sembra minacciosa → "La usi ogni giorno; My First Bitcoin la usa allo stesso modo."
* Hashing come concetto → Analogia dell'impronta digitale; unico, non puoi cambiare senza cambiare anche l'hash.
* Firme digitali → "Dimostra l'autorizzazione senza rivelare la password."
