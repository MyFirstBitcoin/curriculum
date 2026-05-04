# 3.2 Crittografia a chiave pubblica e protocolli

Internet oggi, e la maggior parte dei sistemi informatici moderni, si basano sulla crittografia, un metodo per oscurare le informazioni in modo che solo il destinatario possa decodificarle. Le basi della crittografia utilizzata per proteggere Bitcoin risalgono agli anni '70.

Il primo problema da risolvere è: come inviare un segreto condiviso su un mezzo non sicuro.

Questo fu affrontato per la prima volta da Whitfield Diffie e Martin Hellman.

Il problema: le due parti – solitamente chiamate Alice e Giovanni – vogliono condividere informazioni segrete attraverso una rete dove altri potrebbero ascoltare. Per raggiungere questo obiettivo, crearono il processo di scambio di chiavi Diffie-Hellman.

Questo segreto condiviso può poi essere utilizzato come valore iniziale per creare numerose chiavi simmetriche per criptare e decriptare messaggi da inviarsi reciprocamente senza condividere la chiave stessa in chiaro.

Poiché la chiave privata non deve mai essere condivisa, e chiavi diverse vengono usate alle due estremità per criptare e decriptare, questo viene definito algoritmo di crittografia asimmetrica.

Casi d'uso:

* Alice firma un messaggio con la chiave pubblica di Giovanni – che è l'unica persona che può decriptarlo usando la sua chiave privata
* Alice firma un messaggio con la sua chiave privata – decriptando con la sua chiave pubblica chiunque può verificare che il messaggio sia stato inviato da Alice, senza conoscere la sua chiave privata
* Combinando questi due approcci con due livelli di crittografia, un messaggio può essere inviato criptato in modo che solo Giovanni possa decriptarlo, e lui può poi verificare che il mittente sia effettivamente Alice

Anche se non accreditato nell'articolo, Ralph Merkle fu determinante nell'aiutare a risolvere quello che fino ad allora era considerato un enigma irrisolvibile: come stabilire o ristabilire una comunicazione privata su una rete aperta e potenzialmente ostile.

Questo approccio da solo è vulnerabile a un attacco brute force, dove un attaccante può prendere i numeri condivisi e ricreare una chiave condivisa, dato abbastanza tempo e risorse, quindi non è la soluzione completa da solo.

##### Protocolli per i sistemi crittografici a chiave pubblica

Oltre a contribuire al sistema a chiave pubblica Diffie-Hellman descritto sopra, **Ralph Merkle** continuò a contribuire in questo campo per molti anni, ed è stato fondamentale nello sviluppo di alcuni componenti chiave utilizzati da Bitcoin.

Una funzione di hash crittografica è un algoritmo matematico che prende input di qualsiasi dimensione ed esegue calcoli complessi per restituire un valore hash in bit, che di solito viene rappresentato da un output alfanumerico a lunghezza fissa in formato esadecimale.

* Gli input possono essere di qualsiasi dimensione
* L'output è sempre di lunghezza fissa e deterministico (lo stesso input genera sempre lo stesso hash)
* È facile da verificare ma estremamente difficile invertire il processo per determinare l'input
* Una minima modifica dei dati altera completamente gli output

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/bf388380f380552db5ffb893a8a91c8cf84e85d8-515x331.svg)

L'hashing è una parte integrante del protocollo Bitcoin. SHA-256, utilizzato in Bitcoin, è stato creato dalla NSA ed è un esempio di algoritmo di hashing crittografico.

* Ogni blocco nella catena viene hashato in modo che i dati non possano essere modificati – garantendo l'integrità del registro distribuito
* L'hash generato deve soddisfare i criteri di 'Proof of work' per essere considerato un blocco valido
* Alberi di Merkle – utilizzando ramificazioni e hash di hash, gli alberi hash permettono la verifica di grandi insiemi di dati con uno spazio di archiviazione minimo
* Firme e chiavi basate su hash possono essere utilizzate per wallet, indirizzi e autorizzazione delle transazioni

La verifica distribuita degli stati della blockchain e i modelli di registro append-only resistenti alle revisioni sono resi possibili dall'hashing unidirezionale. Le funzioni hash forniscono un metodo affidabile e deterministico per verificare eventi su registri pubblici come Bitcoin in assenza di un modello di fiducia centralizzato.

Queste nuove capacità nel campo della crittografia erano viste dai loro creatori come l'inizio di una nuova ondata di innovazione in questo settore.

##### Crittografia a curve ellittiche

Una di queste innovazioni successive si presentò sotto forma della crittografia a curve ellittiche.

La crittografia a curve ellittiche fu introdotta nel 1985 da due scienziati, N. Koblitz e V. Miller. Proposero l'idea di utilizzare punti definiti da curve ellittiche invece dei campi primi finiti, in modo che valga l'assunzione del problema del logaritmo discreto, come comunemente usato nel protocollo standard di scambio di chiavi Diffie-Hellman. I dettagli di come funziona sono oltre lo scopo di questa sezione, ma a grandi linee, una curva ellittica è l'insieme dei punti che soddisfano una specifica equazione matematica.

L'equazione per una curva ellittica appare più o meno così:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Questo ha alcune proprietà utili:

* Simmetria orizzontale. Qualsiasi punto sulla curva può essere riflesso sull'asse x e rimane sulla stessa curva.
* qualsiasi retta non verticale interseca la curva al massimo in tre punti.
* Dimensioni compatte delle chiavi sono essenziali per l'archiviazione e la trasmissione efficiente delle chiavi pubbliche nella blockchain.

Queste proprietà possono essere utilizzate per creare coppie di chiavi in modo simile all'algoritmo Diffie-Hellman. Bitcoin utilizza ECDSA, che sta per Elliptic Curve Digital Signature Algorithm. È un processo che utilizza una curva ellittica e un campo finito per 'firmare' dati in modo che terze parti possano verificare l'autenticità della firma mentre il firmatario mantiene la capacità esclusiva di creare la firma. Con bitcoin, i dati che vengono firmati sono la transazione che trasferisce la proprietà.

La parte 'finita' è simile all'approccio 'mod' con Diffie-Hellman, dove il risultato dell'equazione viene diviso e il resto viene utilizzato per assicurare che rientri in un intervallo di numeri.
