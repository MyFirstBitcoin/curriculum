# 2.3 Bitcoin è troppo lento per essere una moneta globale

> I visionari vedono un futuro di lavoratori in telelavoro, biblioteche interattive e aule multimediali. Parlano di assemblee cittadine elettroniche e comunità virtuali... La verità è che nessun database online sostituirà il tuo quotidiano, nessun CD-ROM potrà prendere il posto di un insegnante competente e nessuna rete informatica cambierà il modo in cui funziona il governo.  
_Clifford Stroll_

Diciassette anni dopo, Newsweek cessò la pubblicazione cartacea e divenne disponibile esclusivamente online. Immagina di essere vivo nel 1974, quando fu creato per la prima volta il Transmission Control Protocol (TCP).

Nessuno aveva previsto lo smartphone, con tutte le sue app, che tieni in mano. Nessuno aveva immaginato il sistema di navigazione satellitare nella tua auto.

Internet non è emersa tutta in una volta, ma piuttosto gradualmente come un'evoluzione di protocolli e livelli. Queste evoluzioni si sono basate su TCP, ma principalmente non lo hanno cambiato.

> Quindi, mentre guardo alla transizione verso le piattaforme di comunicazione del futuro, vedo che la bellezza dei protocolli Internet sta nella separazione dei livelli tra servizio e tecnologia.  
_Michael K Powell_



##### Confronta l'evoluzione di Bitcoin con quella di Internet

TCP era necessario ma non sufficiente per la nascita di tutto il resto su Internet. L'evoluzione di Bitcoin sembra seguire un percorso simile. I sistemi aperti sembrano essere più resilienti e di successo quando vengono sviluppati a livelli, anche se può passare molto tempo tra la posa dei primi mattoni e l'adozione diffusa. Le soluzioni tutto-in-uno non sembrano essere efficaci nei sistemi aperti quanto quelle costruite a livelli su protocolli. Così come nessuno ha dovuto ricostruire Internet perché i film non potevano essere trasmessi in streaming usando TCP, probabilmente sarà lo stesso con Bitcoin.

Esistono già diversi protocolli di livello 2 sopra Bitcoin, e ci sono molte applicazioni che si basano su questi protocolli di livello 2 (vedi la sezione 201.4 per maggiori dettagli su questi).

Invece di concentrarti su ciò che bitcoin e la rete Bitcoin non possono fare oggi, pensa a ciò che già si può fare oggi e confrontalo con ciò che era possibile dieci anni fa. Fai questo esercizio con Internet dal 1985 al 1995, poi guarda quanto più veloce è diventata Internet nei successivi 30 anni e le applicazioni che sono diventate possibili. Usa questa intuizione per proiettare Bitcoin nel futuro e immagina come potrebbe essere tra soli altri 10 anni, o 30 se la tua immaginazione arriva così lontano.



##### Confronta Bitcoin con il sistema monetario globale esistente

L'affermazione centrale che Bitcoin sia troppo lento per essere una moneta globale è probabilmente vera se dovessimo limitarci al livello base di Bitcoin. È anche vero che il livello base dei nostri sistemi monetari attuali è troppo lento per essere una moneta globale, se una restrizione simile significasse che non esistesse alcuna infrastruttura di pagamento costruita sopra di esso da banche private e servizi di pagamento come Visa e Mastercard. Il nostro sistema attuale è costruito a livelli, quindi potremmo aspettarci che il futuro sia simile. Alcuni compromessi di progettazione, come tra fiducia, velocità e costo, possono essere trasferiti tra sistemi che offrono le stesse soluzioni, anche se sono costruiti per muovere diversi tipi di valore.

Alcuni degli attuali layer 2 su Bitcoin affrontano direttamente il problema della velocità, ad esempio Liquid e Lightning Network (vedi la sezione 201.4 per maggiori dettagli). Liquid è più veloce ed economico della blockchain di Bitcoin, e Lightning Network è ancora più veloce ed economico di Liquid. Una proliferazione di layer 2, ciascuno con compromessi diversi, è da aspettarsi ed è salutare.

Probabilmente ci saranno altri layer 2 e 3 e un'esplosione di applicazioni che li utilizzeranno, proprio come è successo con l'evoluzione di Internet.



##### Motivazione

Quando viene sollevata questa critica, vale la pena considerare se il critico abbia altre motivazioni. Ad esempio, hanno un nuovo o diverso progetto blockchain? Questo potrebbe essere analogo a cercare di vendere un Transmission Control Protocol migliore.

Il Trilemma della Scalabilità, o della Blockchain, è stato sollevato per la prima volta da Vitalik Buterin nel 2017. Sostiene che c'è sempre un compromesso nella progettazione di una blockchain tra le proprietà di Decentralizzazione, Sicurezza e Scalabilità. Chiunque sollevi la critica che Bitcoin sia troppo lento e che abbia una soluzione più veloce in una blockchain di livello 1, sta sacrificando parte della sicurezza o della decentralizzazione per ottenerla. Sebbene un tale compromesso possa avere senso per una blockchain progettata per altri usi, l'ordine di priorità per una moneta globale deve essere:


> **Note**
>
> * **Decentralizzazione**
>   * Rende possibile eliminare le parti fidate
> * **Sicurezza**
>   * Impedisce agli attori malintenzionati di manomettere le transazioni o il registro
> * **Scalabilità**
>   * Permette al sistema di scalare economicamente in termini di utenti e velocità


Le prime due caratteristiche creano l'ambiente per emissione senza creatori, pagamenti senza intermediari e custodia senza gestori.

Bitcoin fa il giusto compromesso tra le tre caratteristiche di progettazione della blockchain, dato che il suo caso d'uso mirato è quello di moneta globale, e mitiga i compromessi di scalabilità e velocità utilizzando i livelli.

> Satoshi ha scoperto come proteggere l'integrità del denaro digitale senza parti fidate: non servono creatori, intermediari o gestori.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
