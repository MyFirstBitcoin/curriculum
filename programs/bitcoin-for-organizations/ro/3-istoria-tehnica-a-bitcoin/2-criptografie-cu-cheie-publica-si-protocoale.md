# 3.2 Criptografie cu cheie publică și protocoale

Internetul de astăzi și majoritatea sistemelor informatice moderne se bazează pe criptografie, o metodă de ascundere a informațiilor astfel încât doar destinatarul să le poată decoda. Fundamentele criptografiei folosite pentru securizarea Bitcoin pot fi urmărite până în anii '70.

Prima problemă de rezolvat este – cum să trimiți un secret comun printr-un mediu nesecurizat.

Aceasta a fost analizată pentru prima dată de Whitfield Diffie și Martin Hellman.

Problema: cele două părți – de obicei denumite Alice și Bogdan – doresc să partajeze informații secrete printr-o rețea unde alții pot asculta. Pentru a realiza acest lucru, au creat procesul de schimb de chei Diffie-Hellman.

Acest secret comun poate fi apoi folosit ca valoare de bază pentru a crea numeroase chei simetrice pentru criptarea și decriptarea mesajelor pe care și le trimit reciproc, fără a partaja cheia în mod deschis.

Deoarece cheia privată nu trebuie niciodată partajată, iar chei diferite sunt folosite la fiecare capăt pentru criptare și decriptare, aceasta este denumită algoritm de criptare asimetrică.

Cazuri de utilizare:

* Alice semnează un mesaj cu cheia publică a lui Bogdan – care este singura persoană care îl poate decripta folosind cheia sa privată
* Alice semnează un mesaj cu cheia ei privată – decriptând cu cheia ei publică, oricine poate verifica că mesajul a fost trimis de Alice, fără a-i cunoaște cheia privată
* Combinând aceste două abordări cu două straturi de criptare, un mesaj poate fi trimis criptat astfel încât doar Bogdan să îl poată decripta, iar el poate apoi verifica dacă expeditorul a fost într-adevăr Alice

Deși nu este menționat pe lucrare, Ralph Merkle a fost esențial în ajutarea la rezolvarea a ceea ce până atunci era considerat un puzzle de nerezolvat – cum să stabilești sau să restabilești comunicarea privată printr-o rețea deschisă și potențial ostilă.

Această abordare, de una singură, este vulnerabilă la un atac de tip brute force, unde un atacator poate lua numerele partajate și poate recrea o cheie comună în cele din urmă, dacă are suficient timp și resurse, deci nu este răspunsul complet de una singură.

##### Protocoale pentru Criptosisteme cu Cheie Publică

Pe lângă contribuția la sistemul cu cheie publică Diffie-Hellman descris mai sus, **Ralph Merkle** a continuat să contribuie în acest domeniu mulți ani și a fost esențial în dezvoltarea unor componente cheie folosite de Bitcoin.

O funcție hash criptografică este un algoritm matematic care primește intrări de orice dimensiune și procesează calcule complexe pentru a returna o valoare hash în biți, care este de obicei reprezentată printr-o ieșire alfanumerică de lungime fixă folosind formatul hexazecimal.

* Intrările pot avea orice dimensiune
* Ieșirea este întotdeauna de lungime fixă și deterministă (aceeași intrare generează același hash de fiecare dată)
* Este ușor de verificat, dar extrem de dificil de inversat procesul pentru a determina intrarea
* O modificare minoră a datelor schimbă complet ieșirea

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/809de0cfec42c56327cc8916f5acf4eb88e3554a-515x331.svg)

Hash-ul este o parte integrantă a protocolului Bitcoin. SHA-256, folosit în Bitcoin, a fost creat de NSA și este un exemplu de algoritm de hash criptografic.

* Fiecare bloc din lanț este hash-uit astfel încât datele să nu poată fi schimbate – asigurând integritatea registrului distribuit
* Hash-ul generat trebuie să îndeplinească criteriile de ‘Dovadă a muncii’ pentru a fi considerat un bloc valid
* Arborii Merkle – folosind ramificări și hash-uri de hash-uri, arborii hash permit verificarea unor seturi mari de date cu stocare minimă
* Semnăturile și cheile bazate pe hash pot fi folosite pentru portofele, adrese și autorizarea tranzacțiilor

Verificarea distribuită a stărilor blockchain-ului și modelele de registru doar-adăugare, rezistente la revizuire, sunt posibile datorită hash-ului unidirecțional. Funcțiile hash oferă metoda fiabilă și deterministă de a verifica evenimentele pe registre publice precum Bitcoin, în absența unui model centralizat de încredere.

Aceste noi capabilități din domeniul criptografiei erau așteptate de către creatorii lor să aducă un nou val de inovație în acest domeniu.

##### Criptografie cu curbe eliptice

Una dintre aceste inovații ulterioare a venit sub forma criptografiei cu curbe eliptice.

Criptografia cu curbe eliptice a fost introdusă în 1985 de doi oameni de știință, N. Koblitz și V. Miller. Ei au propus ideea de a folosi puncte definite de curbe eliptice în locul câmpurilor prime finite astfel încât să se păstreze ipoteza problemei logaritmului discret, așa cum este folosită în mod obișnuit în protocolul standard de schimb de chei Diffie-Hellman. Detaliile despre cum funcționează acest lucru depășesc scopul acestei secțiuni, dar la nivel general, o curbă eliptică este setul de puncte care satisfac o anumită ecuație matematică.

Ecuația pentru o curbă eliptică arată cam așa:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Aceasta are câteva proprietăți utile:

* Simetrie orizontală. Orice punct de pe curbă poate fi reflectat peste axa x și va rămâne pe aceeași curbă.
* orice linie non-verticală va intersecta curba în cel mult trei puncte.
* Dimensiunile compacte ale cheilor sunt esențiale pentru stocarea și transmiterea eficientă a cheilor publice în blockchain.

Aceste proprietăți pot fi folosite pentru a crea perechi de chei într-un mod similar cu algoritmul Diffie-Hellman. Bitcoin folosește ECDSA, care este prescurtarea de la Elliptic Curve Digital Signature Algorithm. Este un proces care folosește o curbă eliptică și un câmp finit pentru a „semna” date astfel încât terții să poată verifica autenticitatea semnăturii, în timp ce semnatarul păstrează capacitatea exclusivă de a crea semnătura. În cazul bitcoin, datele care sunt semnate sunt tranzacțiile care transferă proprietatea.

Partea ‘finită’ este similară cu abordarea ‘mod’ din Diffie-Hellman, unde rezultatul ecuației este împărțit și restul este folosit pentru a se asigura că se încadrează într-un interval de numere.
