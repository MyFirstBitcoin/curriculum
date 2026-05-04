# 7 - Usa Bitcoin nella vita quotidiana

Durata: 90 minuti

Idea principale: Il Lightning Network rende Bitcoin più pratico per i pagamenti quotidiani, permettendo transazioni più veloci e meno costose, mantenendo Bitcoin come base.

#### Obiettivi di apprendimento

Al termine di questa lezione, gli studenti dovrebbero essere in grado di:

* Spiegare cos'è il Lightning Network e perché è stato costruito sopra Bitcoin.
* Confrontare le transazioni on-chain e Lightning in termini di velocità, costi e compromessi sulla sicurezza.
* Distinguere tra wallet Lightning custodial e self-custodial, e spiegare perché l'autocustodia è importante.
* Configurare un wallet Lightning e descrivere il ruolo della seed phrase nel recupero del wallet.
* Dimostrare come i pagamenti Lightning si muovono attraverso la rete, anche quando due utenti non condividono un canale diretto.
* Individuare modi concreti in cui Bitcoin può essere usato nella vita quotidiana tramite Lightning, inclusi caffè, spesa, pagamenti ai commercianti e acquisti locali.
* Spiegare come strumenti come BTCPay Server, BTCMap e le gift card aiutano ad espandere l'uso di Bitcoin nella pratica.
* Descrivere cos'è un'economia circolare Bitcoin e perché Lightning la rende più realizzabile.

#### Strumenti e risorse

##### Materiali visivi

* Capitolo 7 - Usare Bitcoin nella vita quotidiana

##### Libreria di supporto

* Scheda di riferimento del vocabolario — Termini: Lightning Network, canale di pagamento, instradamento, Layer 2, economia circolare, rimessa
* Esempi reali e libreria di casi di studio — El Salvador, economia circolare di Austin, storie di adozione di Lightning da parte dei commercianti
* Tabelle di confronto e schede di riferimento — Confronto On-Chain vs. Lightning; confronto di commissioni e velocità tra metodi di pagamento
* Lightning Network spiegato in modo semplice — Come funzionano i canali di pagamento senza gergo tecnico; instradamento; sicurezza; casi d'uso
* Scenari di pagamento passo-passo — Passaggi: invio a un amico, ricezione di un pagamento, rimesse, accettare come freelance
* Strumento di confronto commissioni e velocità — Quando usare Lightning vs. on-chain vs. banca (con esempi di costi)

#### Attività

* Staffetta Lightning

#### Didattica online

* Usa una slide di confronto affiancato per i pagamenti on-chain e Lightning.
* Inizia con un caso d'uso reale come il caffè o le rimesse, così gli studenti capiscono perché esiste Lightning.
* Usa un semplice diagramma di instradamento a tre persone per mantenere chiara la spiegazione della rete.
* Mantieni leggera la spiegazione della meccanica dei canali, a meno che la classe non abbia già una solida base.

#### Preparazione

* Scarica un wallet Lightning e prepara screenshot che mostrino affiancati la velocità delle transazioni on-chain (lenta) e Lightning (veloce).
* Ricerca 2-3 commercianti o comunità reali che usano Lightning; aggiungi BTCMap.org ai preferiti come riferimento.
* Prepara una tabella di confronto on-chain vs. Lightning (velocità, commissioni, sicurezza, casi d'uso) da distribuire.

#### Procedura

Questa lezione mostra agli studenti come Bitcoin diventa pratico per i pagamenti quotidiani grazie al Lightning Network. La guida ora segue direttamente la struttura del Diploma, così le sezioni principali su Lightning corrispondono alla guida per gli studenti, mentre confronti, strumenti per commercianti ed economia circolare rimangono nelle sezioni dedicate.

##### 7.0 Introduzione, 8 minuti

Inizia collegando questo capitolo al precedente:

* Se Bitcoin funziona on-chain, perché è stato necessario un altro livello?
* Cosa succede quando le persone vogliono fare molti piccoli pagamenti rapidamente?
* Che tipo di sistema di pagamento funzionerebbe meglio per caffè, spesa o pagare un amico?

Chiarisci che questo capitolo si concentra su Bitcoin per l'uso quotidiano, soprattutto quando velocità e basse commissioni sono importanti. Sottolinea che Lightning è costruito sopra Bitcoin, non è separato da esso.

##### 7.1 Il Lightning Network, 25 minuti

**Cos'è il Lightning Network**

Spiega che il Lightning Network è un sistema di pagamento costruito sopra Bitcoin che permette agli utenti di inviare e ricevere bitcoin in modo rapido ed economico. Funziona spostando molti piccoli pagamenti fuori dalla blockchain principale e registrando solo il risultato finale on-chain in un secondo momento.

Un modo utile per spiegarlo è con l'analogia del conto al bar del capitolo:

* invece di pagare ogni articolo uno per uno on-chain
* due persone aprono un canale
* aggiornano i saldi man mano che effettuano transazioni
* solo il saldo finale viene registrato sulla blockchain quando chiudono il canale

Questo rende Lightning più veloce ed economico per pagamenti piccoli e frequenti. Chiarisci anche che i pagamenti Lightning possono essere instradati attraverso la rete, quindi gli utenti non hanno bisogno di un canale diretto con ogni persona a cui pagano.

**On-chain vs Lightning**

Ora rendi il contrasto molto chiaro.

Transazioni on-chain

* avvengono direttamente sulla blockchain di Bitcoin
* sono generalmente più lente
* dipendono dall'inclusione e dalla conferma in un blocco
* tendono ad essere più sicure
* possono essere più costose a seconda delle commissioni

Transazioni Lightning

* avvengono su un secondo livello costruito sopra Bitcoin
* si regolano molto più velocemente
* di solito costano molto meno
* sono utili per pagamenti piccoli e frequenti
* comportano compromessi rispetto al regolamento on-chain

Mantieni il punto principale semplice: on-chain è più forte per il regolamento finale, Lightning è più forte per velocità e uso quotidiano a basso costo. Il confronto è particolarmente utile qui.

##### 7.2 Tipi diversi di wallet Lightning, 10 minuti

Spiega che un wallet Lightning svolge la stessa funzione di base di un wallet Bitcoin, ricevere e inviare bitcoin, ma è progettato per l'uso sulla rete Lightning. Poi illustra le principali distinzioni tra i wallet presentate nel capitolo:

* self-custodial: l'utente controlla le chiavi
* custodial: qualcun altro controlla le chiavi

Chiarisci il compromesso principale:

* i wallet custodial possono sembrare più facili e comodi
* ma l'utente dipende dal permesso e dal controllo di qualcun altro
* i wallet self-custodial danno più proprietà e sovranità

Rinforza anche la raccomandazione del capitolo di preferire wallet open-source, perché gli strumenti open-source possono essere revisionati, migliorati e verificati dalla comunità.

##### 7.3 Configurare un wallet Bitcoin Lightning, 10 minuti

Guida gli studenti attraverso il flusso di configurazione di base:

* scarica un wallet Lightning
* crea un nuovo wallet
* scrivi la frase di recupero
* conferma le parole nell'ordine corretto
* aggiungi sicurezza extra se il wallet lo permette
* inizia a usare il wallet

Sii particolarmente chiaro riguardo alla seed phrase:

* è ciò che permette all'utente di recuperare l'accesso
* se viene persa, si può perdere l'accesso ai fondi
* se un'altra persona la ottiene, può controllare i fondi

Questa sezione dovrebbe rafforzare fortemente la responsabilità e la gestione sicura, proprio come nel capitolo on-chain.

##### 7.4 Inviare e ricevere transazioni Lightning, 17 minuti

**Come funzionano in pratica le transazioni Lightning**

Usa l'esempio di Marzia, Giovanni ed Eva per spiegare il routing. Marzia non ha bisogno di un canale diretto con Eva. Il suo pagamento può passare attraverso Giovanni, che è connesso alla rete, e raggiungere comunque Eva in modo sicuro.

Rendi chiari questi punti:

* I pagamenti Lightning possono passare attraverso intermediari
* quegli intermediari aiutano a instradare i pagamenti
* il processo di routing non significa che gli utenti si affidano a una banca o a un processore di pagamenti centralizzato
* la rete utilizza la crittografia affinché il pagamento raggiunga il destinatario previsto

Questo aiuta gli studenti a capire che Lightning è comunque peer-to-peer, anche quando i pagamenti passano attraverso una struttura di rete più ampia. Se utile, sottolinea che il capitolo menziona anche che gli operatori di nodi possono guadagnare commissioni e aiutare a rafforzare la rete instradando i pagamenti.

**Finanziare i canali e usare Lightning ripetutamente**

Spiega meglio l'esempio di Mina:

* Mina sposta bitcoin dal suo wallet on-chain al suo wallet Lightning
* questo finanzia un canale di pagamento
* può quindi effettuare pagamenti ripetuti senza dover riaprire il processo ogni volta
* quando il canale si chiude, il saldo finale viene regolato di nuovo sulla blockchain

Rendi chiara una limitazione importante: i fondi bloccati in un canale attivo vengono utilizzati per Lightning e non sono liberamente disponibili per un uso separato sulla blockchain nello stesso momento. Questo aiuta gli studenti a capire che Lightning è potente, ma comporta una struttura di pagamento diversa.

##### 7.5 Comprare caffè e generi alimentari con Bitcoin, 20 minuti

**Casi d'uso quotidiani**

Passa dalla meccanica alla vita reale.

Spiega che Lightning è particolarmente utile per:

* comprare un caffè
* generi alimentari
* shopping
* pagare gli amici
* piccole transazioni quotidiane

L'esempio di Mina nel capitolo aiuta a mostrare perché Lightning è più adatto rispetto ai tradizionali sistemi di pagamento in molte situazioni: è veloce, ha commissioni basse, è senza confini ed è accessibile anche a chi potrebbe non avere un conto bancario. La tabella di confronto e il diagramma del processo di pagamento sono strumenti didattici efficaci qui, soprattutto per mostrare quanti intermediari esistono nei pagamenti con carta tradizionali.

**Strumenti per commercianti e spendere Bitcoin nel mondo reale**

Ora spiega come aziende e utenti possono rendere Lightning pratico nella vita di tutti i giorni.

Copri i tre principali strumenti o percorsi del capitolo:

BTCPay Server

* processore di pagamenti open-source
* permette ai commercianti di accettare bitcoin direttamente
* nessun intermediario che controlla i fondi
* utile per pagamenti aziendali online e di persona

BTCMap

* aiuta gli utenti a trovare commercianti e comunità che accettano bitcoin
* permette alle persone di cercare localmente
* può essere aggiornato dalla comunità

Carte regalo e voucher

* strumenti di transizione per spendere bitcoin dove l'accettazione diretta non esiste ancora
* aiutano a colmare il divario mentre l'adozione cresce

Questa sezione è importante perché mostra agli studenti che l'uso di Bitcoin non è solo teorico. Esistono già strumenti reali che le persone possono usare oggi.

**Economie circolari e Bitcoin come mezzo di scambio**

Concludi il contenuto principale spiegando che un'economia circolare è una comunità in cui i partecipanti cercano di comprare e vendere tra loro il più possibile. Applicato a Bitcoin, questo significa che commercianti, lavoratori e utenti scelgono di transare in bitcoin e si sostengono economicamente a vicenda.

Spiega perché Lightning è importante qui:

* i pagamenti sono quasi istantanei
* le commissioni sono basse
* i piccoli pagamenti diventano pratici
* il commercio locale diventa più facile da sostenere

Puoi menzionare che il capitolo fa riferimento a esempi come Arnhem e Bitcoin Beach, mostrando che le economie circolari non sono ipotetiche. Esistono già e continuano a crescere. La linea temporale visiva è particolarmente utile qui

###### Conclusione e verifica della comprensione

Concludi con alcune domande rapide:

* Perché è stata creata la Lightning Network?
* Qual è una differenza principale tra i pagamenti on-chain e quelli Lightning?
* Perché la self-custody è importante in un wallet Lightning?
* Come può qualcuno ricevere un pagamento Lightning senza avere un canale diretto con ogni persona?
* Cos'è un'economia circolare Bitcoin?

#### Note per l'educatore

Mantieni chiaro il filo conduttore principale: Bitcoin è il livello base, Lightning aiuta a rendere i pagamenti quotidiani più veloci ed economici.

Questo capitolo dovrebbe risultare pratico e concreto, non eccessivamente tecnico.

Dai priorità alla comprensione rispetto alla meccanica approfondita dei canali.

I punti più importanti da privilegiare, se il tempo è poco, sono:

* cos'è Lightning
* compromessi tra on-chain e Lightning
* custodia e configurazione del wallet
* pagamenti nel mondo reale
* economie circolari

Le immagini più utili in questo capitolo sono:

* il confronto tra on-chain e Lightning
* le distinzioni tra wallet
* l'esempio di instradamento con Marzia, Giovanni ed Eva
* la tabella comparativa e il grafico della capacità
* il diagramma dei pagamenti tradizionali
* la timeline dell'economia circolare

##### Cosa Significa Far Bene

* È importante partire dal problema "Bitcoin impiega 10 minuti e costa 2 €", spiegare Lightning come una corsia veloce sopra Bitcoin, usare esempi reali da commercianti e corridoi di rimesse, e creare alberi decisionali per quando usare on-chain rispetto a Lightning.
* Gli educatori dovrebbero essere pragmatici su ciò che Lightning risolve realmente, condividere storie dal campo dove Bitcoin viene utilizzato, essere chiari sui compromessi specifici e rimanere realistici sull'adozione pur essendo entusiasti delle possibilità.
* Gli studenti vedono Bitcoin funzionare davvero per pagamenti reali in luoghi reali, comprendono che velocità e costo sono importanti per i pagamenti, immaginano un'economia circolare dove Bitcoin resta locale, riconoscono che Lightning ≠ Bitcoin (strumenti diversi per scopi diversi) e diventano curiosi sui sistemi economici costruiti sui pagamenti in Bitcoin.
* Gli Obiettivi di Apprendimento sono raggiunti se gli studenti sanno spiegare la Lightning Network come un layer sopra Bitcoin, comprendono le basi dei canali di pagamento e dell'instradamento, vedono casi d'uso reali per i pagamenti Lightning, confrontano on-chain e Lightning in diversi scenari, comprendono il concetto di economia circolare e riconoscono i compromessi specifici di ogni approccio.

##### Gestione del Tempo

Se il tempo è poco, dare priorità a:

* Cos'è Lightning
* Compromessi tra on-chain e Lightning
* Pagamenti nel mondo reale
* Economie circolari

Se si è in anticipo, approfondire:

* Meccaniche dei canali di pagamento e instradamento
* Strumento di confronto tra commissioni e velocità
* Studi di caso sulle economie circolari di El Salvador e Austin
* Esempi pratici di scenari di pagamento Lightning

##### Se gli studenti fanno fatica

* Perché esiste Lightning → Confronta: 10 min/2 € vs. secondi/frazione di centesimo.
* Canali di pagamento → Analogia del conto al bar; si regola internamente e poi su Bitcoin.
* Perché è importante a livello globale → "E se non avessi una banca ma avessi Bitcoin?"
