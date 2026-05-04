# 8 - Cum funcționează Bitcoin

Durată: 90 de minute

Ideea de bază: Securitatea Bitcoin se bazează pe concepte tehnice simple, dar puternice, precum cheile, semnăturile, funcțiile hash și UTXO-urile, care permit deținerea și verificarea fără o autoritate centrală.

#### Obiective de învățare

La finalul acestei lecții, elevii ar trebui să poată:

* Să explice cum cheile publice și private ajută la securizarea deținerii și tranzacțiilor cu Bitcoin.
* Să descrie ce este o semnătură digitală și cum dovedește că o tranzacție a fost autorizată de adevăratul proprietar.
* Să explice, pe înțelesul tuturor, ce înseamnă criptografie, criptare și decriptare în contextul Bitcoin.
* Să definească hashing-ul și să descrie de ce funcțiile hash sunt importante pentru securitatea și integritatea datelor în Bitcoin.
* Să identifice proprietățile de bază ale unei funcții hash, precum ieșirea de lungime fixă, comportamentul unidirecțional și sensibilitatea la modificări mici ale intrării.
* Să explice modelul UTXO și cum bitcoin-ul este cheltuit, primit și returnat ca rest prin ieșirile tranzacțiilor.
* Să descrie cum nodurile ajută la prevenirea dublei cheltuiri verificând dacă o ieșire a fost deja cheltuită.

#### Instrumente & Resurse

##### Materiale vizuale

* Capitolul 8 - Cum funcționează Bitcoin

##### Bibliotecă de suport

* Card de referință vocabular — Capitolul 8 — Termeni: criptografie, hash, UTXO, semnătură digitală, cheie privată/publică, arbore merkle, blockchain
* Biblioteci de concepții greșite — Capitolul 8 — Adresează: „fraza seed pierdută poate fi recuperată”, „cheia privată = parolă”, „blockchain-ul este anonim”
* Explicații tehnice & detalii aprofundate — Funcții hash, chei publice/private, model UTXO, securitatea Proof of Work

#### Activități

* Tranzacții în acțiune
* Explorarea Mempool-ului

#### Predare online

* Folosește o tablă digitală și desenează fiecare concept în timp real, nu te baza doar pe explicații verbale.
* Predă o idee tehnică pe rând și fă pauze dese pentru întrebări de verificare.
* Folosește materiale vizuale pentru chei, semnături, hash-uri și UTXO-uri, astfel încât elevii să poată urmări structura.
* Păstrează scopul conceptual și evită să intri prea adânc în matematică sau jargon.

#### Pregătire

* Pregătește și laminează diagrame: perechi de chei publice/private, semnături digitale, model UTXO, hashing (funcție unidirecțională).
* Salvează în favorite un explorator de blockchain și un calculator SHA-256 hash; selectează 2-3 tranzacții reale Bitcoin pentru a le parcurge pas cu pas.
* Pregătește notițe pe tablă pentru a explica intrările, ieșirile și modul în care tranzacțiile sunt confirmate pe blockchain.

#### Procedură

Această lecție oferă elevilor o primă privire asupra părții tehnice a Bitcoin, fără a presupune cunoștințe tehnice anterioare. Ghidul urmează acum aceeași structură comprimată ca Diploma, cu criptografia grupată sub un titlu și UTXO-urile sub altul.

##### 8.0 Introducere, 8 minute

Începe prin a stabili așteptările:

* Ce face Bitcoin sigur dacă nu există o bancă centrală care să-l controleze?
* Cum poate rețeaua să știe dacă o persoană chiar deține bitcoin-ul pe care încearcă să-l trimită?
* Ce se întâmplă de fapt în spate atunci când cineva face o tranzacție Bitcoin?

Clarifică faptul că acest capitol se concentrează pe fundamentele tehnice de bază ale Bitcoin, în special cheile, semnăturile, hashing-ul și UTXO-urile. De asemenea, liniștește elevii că nu trebuie să devină ingineri pentru a înțelege logica esențială. Capitolul însuși subliniază acest lucru comparând Bitcoin cu internetul: mulți oameni îl folosesc zilnic fără să înțeleagă fiecare strat de dedesubt.

##### 8.1 Securitate prin criptografie, 57 minute

**Bitcoin ca registru stocat pe mai multe calculatoare**

Începe cu prezentarea simplă a capitolului despre rețeaua Bitcoin:

* Bitcoin este o evidență a tranzacțiilor
* această evidență este stocată pe multe calculatoare numite noduri
* registrul este public și pseudonim
* arată adresele și istoricul tranzacțiilor, nu detalii despre identitatea personală

Această secțiune îi ajută pe elevi să facă legătura cu ceea ce știu deja din capitolele anterioare. Bitcoin nu se bazează pe conturi ascunse într-o bancă. Se bazează pe un registru partajat pe care mulți participanți îl pot verifica. este deosebit de util aici pentru că arată utilizatorii, portofelele și rețeaua Bitcoin conectate la registrul public.

**Chei publice și private**

Acum treci la criptografie.

Explică faptul că fiecare utilizator Bitcoin are:

* o cheie privată, care trebuie să rămână secretă
* o cheie publică, care poate fi împărtășită

Clarifică scopul lor în termeni simpli:

* cheia privată dovedește controlul și autorizează cheltuirea
* cheia publică îi ajută pe ceilalți să verifice că tranzacția a fost autorizată corect

Un punct forte de predare din acest capitol este că Bitcoin folosește criptografie cu chei publice/chei private, nu modelul mai vechi în care două persoane trebuie mai întâi să împărtășească aceeași cheie secretă. Acest lucru contează pentru că permite verificarea sigură fără a forța utilizatorii să dezvăluie secretul care le protejează fondurile.

Poți explica astfel:

* cheia privată este ca dovada secretă că bitcoinul îți aparține
* cheia publică face parte din ceea ce permite rețelei să verifice autorizarea ta
* oricine controlează cheia privată controlează posibilitatea de a cheltui bitcoinul

Ai grijă să nu complici prea mult limbajul criptografic. Cel mai important punct pentru elevi este proprietatea și autorizarea.

**Semnături digitale și autorizarea tranzacțiilor**

Acum explică ce se întâmplă când cineva trimite bitcoin.

Folosește secvența din capitol:

* un utilizator creează o tranzacție
* expeditorul generează o semnătură digitală folosind cheia sa privată
* tranzacția este transmisă în rețea
* nodurile verifică dacă semnătura este validă
* după verificare și confirmare, proprietatea este transferată în registru

Fă clar că o semnătură digitală nu este același lucru cu a scrie un nume. Este dovada criptografică că adevăratul proprietar a autorizat tranzacția. Acesta este unul dintre mecanismele de bază care permit Bitcoin să funcționeze fără o autoritate centrală care să aprobe manual tranzacțiile. Diagrama este utilă pentru că arată vizual semnarea și verificarea, precum și traseul tranzacției de la expeditor la validarea în rețea.

O propoziție bună pentru clasă este:

Tranzacțiile Bitcoin nu sunt aprobate pentru că o bancă spune așa. Ele sunt acceptate pentru că rețeaua poate verifica dovada criptografică validă.

**Hashing și funcții unidirecționale**

Apoi, explică hashing-ul.

Începe simplu:

* o funcție primește o intrare și produce o ieșire
* o funcție unidirecțională este ușor de rulat într-o direcție, dar practic imposibil de inversat
* o funcție hash primește date de orice dimensiune și le transformă într-o ieșire de lungime fixă numită hash

Folosește una dintre analogiile din capitol, pe cea care ți se pare cea mai clară pentru audiență:

* analogia smoothie pentru funcțiile unidirecționale
* analogia amprentei pentru hash-uri
* analogia partiturii muzicale pentru verificarea dacă ceva s-a schimbat

Probabil că analogia amprentei este cea mai clară pentru majoritatea claselor:

* un hash este ca o amprentă digitală pentru date
* dacă intrarea se schimbă chiar și puțin, hash-ul se schimbă complet
* acest lucru ajută calculatoarele să verifice integritatea și să detecteze modificările neautorizate

Apoi explică de ce hashing-ul contează în Bitcoin:

* tranzacțiile sunt hash-uite
* rețeaua folosește hash-uri pentru a ajuta la verificarea integrității
* dacă o tranzacție este modificată, hash-ul se schimbă
* acest lucru ajută la protejarea registrului împotriva manipulării nedetectate

Vizualele de la paginile 7 la 10 sunt foarte utile aici. Capitolul arată atât ideea de ieșire de lungime fixă, cât și principiul „schimbare mică, rezultat complet diferit”, care este unul dintre cele mai importante concepte pe care elevii trebuie să le înțeleagă.

**Proprietăți de bază ale funcțiilor hash**

Parcurge pe scurt proprietățile evidențiate în capitol, fără a le face să pară prea academice:

* Determinist: aceeași intrare dă aceeași ieșire de fiecare dată
* Unidirecțională / rezistență la pre-imagine: nu poți inversa procesul în mod realist
* Sensibil la schimbare: chiar și o mică modificare a intrării creează o ieșire foarte diferită
* Rezistență la coliziune: este extrem de dificil să găsești două intrări diferite cu aceeași ieșire
* Rapid de verificat: funcția este eficientă de rulat și verificat

Nu este nevoie ca elevii să memoreze fiecare termen, dar ar trebui să înțeleagă ideea generală: hashing-ul oferă Bitcoin o modalitate fiabilă de a identifica datele și de a detecta schimbările.

##### 8.2 Modelul UTXO, 25 de minute

**Modelul UTXO**

Acum treci la a doua parte majoră a capitolului: UTXO-uri, sau Output-uri de Tranzacție Nespese.

Explică-l în termeni simpli folosind analogia cu banii cash din capitol:

* bitcoin nu este urmărit doar ca un sold de cont bancar
* în schimb, este format din bucăți cheltuibile numite UTXO-uri
* când cheltui bitcoin, folosești unul sau mai multe UTXO-uri existente ca input-uri
* apoi se creează noi UTXO-uri ca output-uri

Folosește exemplul din capitol:

* dacă ai un UTXO de 10 BTC
* și trimiți 6 BTC
* un nou UTXO de 6 BTC ajunge la destinatar
* un nou UTXO de rest se întoarce la tine
* o mică parte se plătește ca taxă pentru mineri

Acest lucru îi ajută pe elevi să vadă că Bitcoin funcționează mai degrabă ca atunci când cheltuiești bani cash și primești rest, decât ca o simplă scădere dintr-un sold de cont. Diagramele sunt deosebit de utile aici pentru că arată vizual cum un UTXO este împărțit în output pentru destinatar, output de rest și taxă.

Fă două puncte cheie explicite:

* soldul portofelului tău este suma UTXO-urilor tale
* când cheltui, UTXO-urile vechi sunt consumate și se creează unele noi

**Prevenirea dublei cheltuieli**

Încheie conținutul explicând una dintre cele mai importante implicații ale modelului UTXO.

Dacă cineva încearcă să cheltuiască același output de două ori, nodurile resping a doua încercare pentru că ele mențin registrul și pot verifica dacă acel UTXO a fost deja cheltuit. Așa previne Bitcoin dubla cheltuire fără a avea nevoie de o companie centralizată de plăți care să gestioneze evidența. Exemplul este foarte util aici pentru că parcurge pașii în care Alice combină UTXO-uri, trimite fonduri către Bogdan, primește rest și are tranzacția confirmată care actualizează registrul pe toate nodurile.

O modalitate clară de a spune asta la clasă este:

Bitcoin previne dubla cheltuire pentru că rețeaua ține evidența output-urilor care rămân necheltuite și a celor care au fost deja folosite.

###### Încheiere și verificare a înțelegerii

Încheie cu câteva întrebări rapide:

* Care este diferența dintre o cheie publică și o cheie privată?
* Ce dovedește o semnătură digitală?
* De ce este util hashing-ul în Bitcoin?
* Ce se întâmplă dacă o tranzacție este modificată după ce a fost hash-uită?
* Ce este un UTXO în termeni simpli?
* Cum oprește rețeaua pe cineva să cheltuiască același bitcoin de două ori?

#### Note pentru educator

Acest capitol conține un limbaj mai tehnic decât cele anterioare, așa că prioritizează claritatea, analogiile și repetiția.

Scopul nu este să transformi elevii în dezvoltatori. Scopul este să îi ajuți să înțeleagă de ce funcționează securitatea Bitcoin.

Cele mai importante puncte de prioritizat, dacă timpul este scurt, sunt:

* cheie privată vs cheie publică
* semnături digitale
* ce face hashing-ul
* UTXO-urile ca bucăți cheltuibile de bitcoin
* cum este prevenită dubla cheltuire

Cele mai utile vizualuri din acest capitol sunt:

* diagrama utilizator-portofel-rețea
* vizualul semnăturii digitale
* exemplele de hashing și diagramele cu output de lungime fixă de la paginile 7 la 10
* diagramele UTXO de la paginile 10 la 12

##### Cum arată binele

* Este important să tratezi criptografia ca o fundație, nu ca un mister, să folosești multe vizualuri, să eviți matematica avansată, să faci legătura cu capitolele anterioare și să testezi înțelegerea cu aplicații de tipul „Dacă cineva modifică o tranzacție, ce se strică?”
* Educatorii ar trebui să fie răbdători cu elevii care întâmpină dificultăți, să gândească vizual și să deseneze totul, să fie sinceri despre ce nu trebuie să înțeleagă elevii, să fie dispuși să spună „Nu știu, dar iată cum am putea afla” și să rămână încurajatori pe tot parcursul.
* Elevii înțeleg de ce Bitcoin nu poate fi spart pentru că este protejat de matematică, respectă designul elegant al sistemului, se simt confortabil cu complexitatea știind că nu trebuie să știe fiecare detaliu, capătă încredere să pună întrebări fără să fie judecați și recunosc că au avansat în înțelegerea a ceva ce majoritatea oamenilor nu cunosc.
* Rezultatele de învățare ar trebui să fie atinse dacă elevii pot explica elementele de bază ale criptografiei precum funcțiile unidirecționale și semnăturile digitale fără matematică avansată, să înțeleagă modelul UTXO arătând că deții monede, nu conturi, să recunoască hashing-ul ca fundație a securității Bitcoin, să înțeleagă anatomia unei tranzacții inclusiv semnăturile și confirmările, să explice de ce Bitcoin este imuabil și să pună întrebări critice despre potențiale atacuri sau vulnerabilități.

##### Gestionarea timpului

Dacă timpul este scurt, prioritizează:

* Cheie privată vs cheie publică
* Semnături digitale
* Ce face hashing-ul
* UTXO-urile ca bucăți de bitcoin ce pot fi cheltuite
* Cum este prevenită dubla cheltuire

Dacă ești înainte, acordă timp pentru:

* Diagrama utilizator-portofel-rețea și modelul vizual de securitate
* Semnătura digitală vizual: proces criptografic detaliat
* Arbori Merkle și securitatea lanțului
* Vectori de atac avansați și de ce eșuează

##### Dacă studenții întâmpină dificultăți

* Criptografia pare amenințătoare → „O folosești zilnic; My First Bitcoin o folosește la fel.”
* Hashing ca concept → Analogia cu amprenta; unică, nu poți schimba fără să se schimbe hash-ul.
* Semnături digitale → „Dovedește autorizarea fără să dezvăluie parola.”
