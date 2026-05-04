# 8.1 Sicurezza tramite crittografia

> Quello che Bitcoin ci offre è una promessa ferrea: il programma verrà eseguito esattamente come specificato.  
_Andreas M. Antonopoulos_

#### Crittografia a chiave pubblica/privata


> **Definition – Definizione di crittografia**
>
> **Crittografia** è la pratica di trasformare le informazioni in un segreto che solo le persone giuste possono leggere.


* **Cifratura** è il processo di trasformazione delle informazioni in una forma codificata, così che solo chi possiede la chiave corretta possa leggerle.
* **Decifratura** è il processo di trasformazione di quelle informazioni codificate di nuovo in qualcosa di leggibile.

Nella crittografia tradizionale, due persone che vogliono comunicare in modo privato devono prima condividere la stessa chiave segreta, simile a una password condivisa. Una persona usa questa chiave per cifrare il messaggio prima di inviarlo, e l'altra persona usa la stessa chiave per decifrarlo e leggerlo.

Il problema di questo sistema è che entrambe le persone devono già condividere la chiave segreta. Se qualcun altro ottiene accesso a quella chiave, può leggere qualsiasi messaggio intercettato.

Bitcoin risolve questo problema utilizzando un approccio diverso chiamato crittografia a chiave pubblica, in cui gli utenti non devono condividere chiavi segrete in anticipo.

La crittografia a chiave pubblica/privata risolve il problema della condivisione dei segreti. Invece di condividere una password, ogni persona ha due chiavi: una chiave pubblica e una chiave privata.

* La **chiave pubblica** può essere condivisa con chiunque.
* La **chiave privata** deve sempre essere mantenuta segreta.

Se Giovanni vuole inviare qualcosa ad Arel, può usare la chiave pubblica di Arel. Solo Arel può sbloccarlo usando la sua chiave privata. Anche se qualcuno intercetta il messaggio, non può leggerlo o usarlo senza la chiave privata.

In Bitcoin, questo sistema viene utilizzato per creare firme digitali. Una firma digitale dimostra che il proprietario di una chiave privata ha approvato una transazione, simile a firmare il proprio nome su un documento. Questo è ciò che permette alle transazioni Bitcoin di essere sicure e verificabili senza dover fidarsi di una terza parte.

Le transazioni Bitcoin comportano il trasferimento della proprietà dei bitcoin da un indirizzo a un altro.

La cifratura viene utilizzata per garantire che solo il vero possessore dei bitcoin abbia l'autorità di inviare il proprio denaro a qualcun altro. Garantisce che la loro proprietà sia protetta da attori malintenzionati.

Come ulteriore misura di protezione, ogni transazione Bitcoin riceve automaticamente una firma digitale UNICA. Questa firma digitale unica è alimentata da una tecnologia a prova di manomissione che aiuta la rete a verificare che il vero proprietario dei bitcoin, e non qualcun altro, li abbia inviati.


> **Info**
>
> Ogni utente ha due chiavi: una **chiave privata**, che viene **mantenuta segreta**, e una **chiave pubblica** che può essere **condivisa con altri**. La **chiave privata** serve come forma di identificazione e prova di proprietà, confermando: “Questo indirizzo appartiene a me e ne ho il controllo.”


###### Come funziona una transazione Bitcoin

1. **Creazione della transazione**: Un utente avvia una transazione Bitcoin specificando dettagli come l'indirizzo del destinatario e la quantità di bitcoin da inviare.
1. **Generazione della firma digitale**: Il mittente genera una **firma digitale** unica utilizzando la propria **chiave privata**. Questa firma è un codice unico che verifica l'autenticità della transazione.
1. **Trasmissione della transazione**: La transazione firmata viene trasmessa alla rete Bitcoin, indicando l'intenzione di trasferire la proprietà dei bitcoin dal mittente al destinatario.
1. **Verifica sulla rete**: I nodi della rete Bitcoin ricevono la transazione e utilizzano la **chiave pubblica** per verificare l'autenticità della firma della transazione. Allo stesso tempo, utilizzano la **chiave pubblica** per verificare la **firma digitale**.
1. **Conferma sulla rete Bitcoin**: Se la verifica ha successo, la transazione verrà aggiunta al registro, che funge da archivio sicuro e trasparente di tutte le transazioni. Una volta confermata, la proprietà dei bitcoin viene ufficialmente trasferita dal mittente al destinatario.


> **Callout – Riepilogo**
>
> La **firma digitale**, creata con la **chiave privata** del mittente, dimostra che la transazione è stata autorizzata dal proprietario dei bitcoin. La rete Bitcoin può quindi verificare questa prova e registrare la transazione.


#### Spiegazione dell'hashing

Non lasciarti intimidire dai termini tecnici e dai concetti matematici che seguono. Sappiamo che non tutti amano la matematica, ma potresti sorprenderti e scoprire che anche le idee più complesse possono essere comprese con un po' di impegno.


> **Definition – Definizione di funzione**
>
> Una **funzione** è come una macchina che prende delle informazioni e le trasforma in qualcos'altro. Le informazioni che dai alla funzione sono l'**input**. Le nuove informazioni che la funzione crea sono l'**output**. Le funzioni aiutano i computer a svolgere compiti e risolvere problemi.


##### Cos'è una funzione?

Una funzione è un insieme di istruzioni che prende un input e produce un output. Puoi pensarla come una ricetta: segui i passaggi con determinati ingredienti e ottieni sempre un risultato prevedibile.

In Bitcoin, le funzioni vengono utilizzate per elaborare e verificare le transazioni. Quando qualcuno invia bitcoin, le funzioni crittografiche aiutano a controllare che la transazione sia valida, a confermare che il mittente abbia fondi sufficienti e ad aggiornare i saldi sul registro di Bitcoin. Una volta verificata e aggiunta a un blocco, la transazione diventa parte del registro permanente sulla blockchain.

##### Cos'è una funzione unidirezionale?

Una funzione unidirezionale è un tipo speciale di funzione che è facile da calcolare in una direzione ma estremamente difficile da invertire. Ad esempio, frullare degli ingredienti per fare un frullato è facile, ma non puoi separare il frullato negli ingredienti originali.

La sicurezza di Bitcoin si basa sulle funzioni unidirezionali. Sono utilizzate nella crittografia a chiave pubblica e privata, permettendo alle persone di condividere una chiave pubblica mantenendo segreta la chiave privata. Anche se la chiave pubblica è visibile, è impossibile ricavare la chiave privata da essa. Questo è ciò che rende sicure le transazioni Bitcoin.

##### Cos'è una funzione di hash?

Una **funzione di hash** è come una macchina per codici segreti. Prende un messaggio e lo trasforma in un codice.

###### Come funziona l'hashing nelle transazioni Bitcoin

In Bitcoin, ogni transazione viene trasformata in un hash prima di essere aggiunta alla blockchain. Un hash è un'impronta digitale unica della transazione. Se qualcuno prova a cambiare anche solo una piccola parte della transazione, l'hash cambierà completamente. Questo rende facile per la rete rilevare eventuali manomissioni.

###### Il ruolo dell'hashing nella sicurezza di Bitcoin

L'hashing aiuta a proteggere la rete Bitcoin rendendo le transazioni facili da verificare e impossibili da modificare di nascosto. Poiché ogni transazione ha il suo hash unico, la rete può rilevare rapidamente se qualcosa è stato alterato.

Una funzione di hash prende dei dati e li converte in una stringa fissa di numeri e lettere chiamata hash. Lo stesso input produrrà sempre lo stesso hash, ma anche un piccolo cambiamento nell'input creerà un risultato completamente diverso. Questa proprietà permette ai computer di verificare che i dati non siano stati modificati.


> **Definition – Definizione di hashing**
>
> **L'hashing** è come creare un'impronta digitale per i dati digitali. È il processo di prendere un messaggio digitale e trasformarlo in un codice di lunghezza fissa, che funge da identificatore unico. Proprio come un'impronta digitale può identificare una persona, un hash può identificare un messaggio digitale.


L'**output**, o hash, ha sempre la stessa lunghezza, indipendentemente da quanto fosse lunga l'informazione originale. Bitcoin utilizza alcuni tipi specifici di funzioni di hash chiamate **SHA-256** e **RIPEMD160**.

Ecco alcuni esempi:

* Hash SHA256 della stringa **ciao mondo**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Hash SHA256 della stringa **ciao mondo.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Nota che una piccola modifica nell'input cambia completamente l'output rispetto al primo
* Hash SHA256 del file iso scaricabile **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Questo input è un file enorme, eppure l'output ha ancora la stessa lunghezza fissa

Puoi anche pensare all'hashing come a uno spartito musicale che cattura l'essenza di un brano. Proprio come uno spartito è una rappresentazione unica di una melodia, un valore hash è una rappresentazione unica di un dato.

Confrontando lo spartito di un brano musicale con l'esecuzione reale, un musicista può determinare se l'esecuzione è accurata. Allo stesso modo, confrontando il valore hash dei dati ricevuti con il valore hash originale, si può determinare se i dati sono stati alterati durante la trasmissione.

Così come una piccola deviazione in un'esecuzione musicale può farla suonare diversa, anche il minimo cambiamento ai dati originali produrrà un valore hash differente. Questo rende l'hashing uno strumento potente per garantire l'integrità e l'autenticità di una transazione Bitcoin.

Il processo di codifica della **chiave pubblica** tramite hashing viene utilizzato per migliorare la sicurezza delle informazioni convertendole in un formato illeggibile a lunghezza fissa. Bitcoin utilizza gli algoritmi SHA-256 e RIPEMD160 per produrre indirizzi pubblici. L'output risultante funge da identificatore unico per la **chiave pubblica** e aiuta a garantire l'integrità e la sicurezza delle transazioni memorizzate nel registro. Crittografando le informazioni in questo modo, diventa più difficile per persone non autorizzate accedere e manipolare i dati.

##### Proprietà di una funzione di hashing

* **Deterministica**: Gli stessi ingredienti producono sempre lo stesso frullato. Allo stesso modo, gli stessi dati produrranno sempre lo stesso hash.
* **Resistenza alla pre-immagine**: Se hai solo il frullato, non puoi capire esattamente quali frutti sono stati usati. Allo stesso modo, se hai solo un hash, non puoi determinare i dati originali.
* **Effetto valanga**: Cambiare anche solo una piccola parte degli ingredienti crea un frullato completamente diverso. Nell'hashing, una piccolissima modifica ai dati produce un hash completamente diverso.
* **Resistenza alle collisioni**: È estremamente difficile trovare due insiemi diversi di ingredienti che producano esattamente lo stesso frullato. Allo stesso modo, è estremamente improbabile che due dati diversi producano lo stesso hash.
* **Veloce da verificare**: Preparare il frullato è rapido, ed è facile verificare che il risultato sia un frullato. Le funzioni hash sono veloci da calcolare e facili da verificare per chiunque.

#### Attività: Genera hash SHA 256

https://tools.keycdn.com/sha256-online-generator

Curioso di sapere come funziona l'hashing? Scansiona il codice QR per generare istantaneamente un hash SHA256 da qualsiasi parola, frase o input che scegli. Le funzioni hash sono come impronte digitali digitali: sono a senso unico, cioè una volta che qualcosa è stato hashato, non può essere invertito. Prova tu stesso!
