# 8.1 Securitate prin criptografie

> Ceea ce ne oferă Bitcoin este o promisiune fermă: programul va rula exact așa cum este specificat.  
_Andreas M. Antonopoulos_

#### Criptografie cu chei publice/private


> **Definition – Definiția criptografiei**
>
> **Criptografie** este practica de a transforma informația într-un secret pe care doar persoanele potrivite îl pot citi.


* **Criptare** este procesul de a transforma informația într-o formă codificată, astfel încât doar cineva cu cheia corectă să o poată citi.
* **Decriptare** este procesul de a transforma acea informație codificată înapoi într-o formă lizibilă.

În criptografia tradițională, două persoane care doresc să comunice în mod privat trebuie mai întâi să împartă aceeași cheie secretă, similar cu o parolă comună. O persoană folosește această cheie pentru a cripta mesajul înainte de a-l trimite, iar cealaltă persoană folosește aceeași cheie pentru a decripta și a citi mesajul.

Problema cu acest sistem este că ambele persoane trebuie să dețină deja cheia secretă. Dacă altcineva obține acces la acea cheie, poate citi orice mesaj interceptat.

Bitcoin rezolvă această problemă folosind o abordare diferită numită criptografie cu chei publice, unde utilizatorii nu trebuie să împartă chei secrete în avans.

Criptografia cu chei publice/private rezolvă problema împărtășirii secretelor. În loc să împartă o parolă, fiecare persoană are două chei: o cheie publică și o cheie privată.

* **cheia publică** poate fi împărtășită cu oricine.
* **cheia privată** trebuie să fie întotdeauna păstrată secretă.

Dacă Ion vrea să trimită ceva către Andrei, poate folosi cheia publică a lui Andrei. Doar Andrei o poate debloca folosind cheia sa privată. Chiar dacă cineva interceptează mesajul, nu îl poate citi sau folosi fără cheia privată.

În Bitcoin, acest sistem este folosit pentru a crea semnături digitale. O semnătură digitală dovedește că deținătorul unei chei private a aprobat o tranzacție, similar cu semnarea numelui pe un document. Acesta este motivul pentru care tranzacțiile Bitcoin sunt sigure și verificabile fără a avea încredere într-o terță parte.

Tranzacțiile Bitcoin implică transferul proprietății bitcoin de la o adresă la alta.

Criptarea este folosită pentru a asigura că doar adevăratul deținător al bitcoinului are autoritatea de a trimite banii către altcineva. Astfel, proprietatea lor este protejată împotriva actorilor rău intenționați.

Ca măsură suplimentară de protecție, fiecare tranzacție Bitcoin primește automat o SEMNĂTURĂ digitală UNICĂ. Această semnătură digitală unică este alimentată de o tehnologie rezistentă la manipulare care ajută rețeaua să verifice că adevăratul proprietar al bitcoinului, și nu altcineva, i-a trimis.


> **Info**
>
> Fiecare utilizator are două chei: o **cheie privată**, care este **păstrată secretă**, și o **cheie publică** care poate fi **împărtășită cu alții**. **Cheia privată** servește ca o formă de identificare și dovadă a proprietății, confirmând: „Această adresă îmi aparține și am control asupra ei.”


###### Cum funcționează o tranzacție Bitcoin

1. **Crearea tranzacției**: Un utilizator inițiază o tranzacție Bitcoin specificând detalii precum adresa destinatarului și suma de bitcoin care va fi trimisă.
1. **Generarea semnăturii digitale**: Expeditorul generează o **semnătură digitală** unică folosind **cheia sa privată**. Această semnătură este un cod unic care verifică autenticitatea tranzacției.
1. **Transmiterea tranzacției**: Tranzacția semnată este transmisă către rețeaua Bitcoin, indicând intenția de a transfera proprietatea bitcoinului de la expeditor la destinatar.
1. **Verificarea în rețea**: Nodurile din rețeaua Bitcoin primesc tranzacția și folosesc **cheia publică** pentru a verifica autenticitatea semnăturii tranzacției. În același timp, ei folosesc **cheia publică** pentru a verifica **semnătura digitală**.
1. **Confirmarea pe rețeaua Bitcoin**: Dacă verificarea are succes, tranzacția va fi adăugată în registru, care servește drept o evidență sigură și transparentă a tuturor tranzacțiilor. Odată confirmată, proprietatea bitcoinului este transferată oficial de la expeditor la destinatar.


> **Callout – Rezumat**
>
> Semnătura digitală **semnătura digitală**, creată cu **cheia privată** a expeditorului, dovedește că tranzacția a fost autorizată de proprietarul bitcoinului. Rețeaua Bitcoin poate apoi să verifice această dovadă și să înregistreze tranzacția.


#### Explicație despre Hashing

Vă rugăm să nu vă lăsați intimidați de termenii tehnici și conceptele matematice care urmează. Înțelegem că nu toată lumea este pasionată de matematică, dar s-ar putea să vă surprindeți și să vedeți că chiar și cele mai complexe idei pot fi înțelese cu puțin efort.


> **Definition – Definiția unei funcții**
>
> O **funcție** este ca o mașină care primește niște informații și le transformă în ceva nou. Informația pe care o dai funcției este **inputul**. Noua informație creată de funcție este **outputul**. Funcțiile ajută calculatoarele să îndeplinească sarcini și să rezolve probleme.


##### Ce este o funcție?

O funcție este un set de instrucțiuni care primește un input și produce un output. Poți să o vezi ca pe o rețetă: urmezi pașii cu anumite ingrediente și obții întotdeauna un rezultat previzibil.

În Bitcoin, funcțiile sunt folosite pentru a procesa și verifica tranzacțiile. Când cineva trimite bitcoin, funcțiile criptografice ajută la verificarea validității tranzacției, confirmă că expeditorul are suficiente fonduri și actualizează soldurile în registrul Bitcoin. Odată verificată și adăugată într-un bloc, tranzacția devine parte din evidența permanentă pe blockchain.

##### Ce este o funcție unidirecțională?

O funcție unidirecțională este un tip special de funcție care este ușor de calculat într-o direcție, dar extrem de dificil de inversat. De exemplu, să amesteci ingredientele într-un smoothie este ușor, dar nu poți separa smoothie-ul înapoi în ingredientele originale.

Securitatea Bitcoin se bazează pe funcții unidirecționale. Acestea sunt folosite în criptografia cu chei publice și private, permițând oamenilor să partajeze o cheie publică păstrând cheia privată secretă. Chiar dacă cheia publică este vizibilă, este imposibil să deduci cheia privată din ea. Acesta este motivul pentru care tranzacțiile Bitcoin sunt sigure.

##### Ce este o funcție hash?

O **funcție hash** este ca o mașină de coduri secrete. Primește un mesaj și îl transformă într-un cod.

###### Cum funcționează hashing-ul în tranzacțiile Bitcoin

În Bitcoin, fiecare tranzacție este transformată într-un hash înainte de a fi adăugată pe blockchain. Un hash este o amprentă digitală unică a tranzacției. Dacă cineva încearcă să schimbe chiar și o mică parte din tranzacție, hash-ul se va schimba complet. Acest lucru face ca rețeaua să detecteze ușor orice tentativă de modificare.

###### Rolul hashing-ului în securitatea Bitcoin

Hashing-ul ajută la protejarea rețelei Bitcoin, făcând tranzacțiile ușor de verificat și imposibil de modificat în tăcere. Deoarece fiecare tranzacție are propriul hash unic, rețeaua poate detecta rapid dacă ceva a fost modificat.

O funcție hash primește date și le convertește într-un șir fix de cifre și litere numit hash. Același input va produce întotdeauna același hash, dar chiar și o mică schimbare în input va genera un rezultat complet diferit. Această proprietate permite calculatoarelor să verifice dacă datele nu au fost modificate.


> **Definition – Definiția hashing-ului**
>
> **Hashing-ul** este ca și cum ai crea o amprentă pentru date digitale. Este procesul de a lua un mesaj digital și de a-l transforma într-un cod de lungime fixă, care servește drept identificator unic. Așa cum o amprentă poate identifica o persoană, un hash poate identifica un mesaj digital.


Rezultatul **outputul**, sau hash-ul, are întotdeauna aceeași lungime, indiferent cât de lungă era informația originală. Bitcoin folosește câteva tipuri specifice de funcții hash numite **SHA-256** și **RIPEMD160**.

Câteva exemple sunt mai jos:

* Hash-ul SHA256 al șirului **salut lume**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Hash-ul SHA256 al șirului **salut lume.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Observă că o mică schimbare în intrare modifică complet ieșirea, în comparație cu prima.
* Hash-ul SHA256 al fișierului iso descărcabil **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Această intrare este un fișier uriaș, totuși ieșirea are aceeași lungime fixă

Poți să te gândești la hashing ca la o partitură muzicală care surprinde esența unei piese. Așa cum o partitură este o reprezentare unică a unei melodii, o valoare hash este o reprezentare unică a unor date.

Comparând partitura unei piese cu interpretarea reală, un muzician poate determina dacă interpretarea este corectă. În mod similar, comparând valoarea hash a datelor primite cu valoarea hash originală, poți verifica dacă datele au fost modificate în timpul transmiterii.

Așa cum o mică abatere într-o interpretare muzicală poate face ca piesa să sune diferit, chiar și cea mai mică schimbare a datelor originale va duce la o valoare hash diferită. Acest lucru face ca hashing-ul să fie un instrument puternic pentru a asigura integritatea și autenticitatea unei tranzacții Bitcoin.

Procesul de codificare a **cheii publice** prin hashing este folosit pentru a îmbunătăți securitatea informațiilor, transformându-le într-un format de lungime fixă, ilizibil. Bitcoin folosește algoritmii SHA-256 și RIPEMD160 pentru a genera adrese publice. Rezultatul servește ca un identificator unic pentru **cheia publică** și ajută la asigurarea integrității și securității tranzacțiilor stocate în registru. Prin criptarea informațiilor în acest mod, devine mai dificil pentru persoanele neautorizate să acceseze și să modifice datele.

##### Proprietățile unei funcții hash

* **Deterministă**: Aceleași ingrediente produc întotdeauna același smoothie. La fel, aceleași date vor produce întotdeauna același hash.
* **Rezistență la pre-imagine**: Dacă ai doar smoothie-ul, nu poți afla exact ce fructe au fost folosite. În mod similar, dacă ai doar un hash, nu poți determina datele originale.
* **Efect de avalanșă**: Schimbarea chiar și a unei părți mici din ingrediente creează un smoothie complet diferit. În hashing, o schimbare foarte mică a datelor produce un hash complet diferit.
* **Rezistență la coliziune**: Este extrem de dificil să găsești două seturi diferite de ingrediente care să producă exact același smoothie. La fel, este extrem de puțin probabil ca două seturi diferite de date să producă același hash.
* **Rapid de verificat**: Prepararea smoothie-ului este rapidă și este ușor de verificat că rezultatul este un smoothie. Funcțiile hash sunt rapide de calculat și oricine poate verifica ușor rezultatul.

#### Activitate: Generează un hash SHA 256

https://tools.keycdn.com/sha256-online-generator

Ești curios cum funcționează hashing-ul? Scanează codul QR pentru a genera instantaneu un hash SHA256 din orice cuvânt, propoziție sau intrare dorești. Funcțiile hash sunt ca amprentele digitale: sunt unidirecționale, adică odată ce ceva a fost hash-uit, nu poate fi inversat. Încearcă și vezi cu ochii tăi!
