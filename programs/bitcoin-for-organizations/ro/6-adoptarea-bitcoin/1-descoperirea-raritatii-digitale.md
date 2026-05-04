# 6.1 Descoperirea rarității digitale

> Odată cu Bitcoin, a fost descoperit un nou tip de marfă... un fel de marfă digitală, generată de computere și parțial creată pentru computere. Omenirea are o istorie a invențiilor semnificative. În cărțile de istorie care vor fi scrise în viitor, Bitcoin va fi menționat ca una dintre acestea.  
_Prof. Dr. Philipp Sander_



#### 6.1.0 Raritatea în economie

În domeniul economiei, este bine înțeles că raritatea este un principiu cheie care determină valoarea. Bunurile și serviciile care se confruntă cu o cerere semnificativă devin mai valoroase dacă oferta este limitată în așa măsură încât cererea nu poate fi satisfăcută cu ușurință. Mai mult, raritatea alimentează competiția crescută și este un factor determinant al descoperirii prețului pe piață. Într-o piață cu concurență liberă, corectă și deschisă, prețurile ar trebui să se stabilească la punctul în care oferta și cererea se întâlnesc.

Resursele care se bucură de o cerere semnificativă pot fi considerate mai valoroase dacă sunt finite sau mai greu de obținut. Acest lucru poate stimula o cerere crescută pentru acea resursă, pe măsură ce participanții la piață concurează pentru a-și asigura accesul la ea. Această dinamică poate fi observată la resursele naturale precum metalele prețioase, petrolul sau așa-numitele „mărfuri moi” precum produsele alimentare. Raritatea, așadar, stă la baza deciziilor economice, alocării resurselor și costului de oportunitate. Într-o lume cu resurse nelimitate, totul ar fi la fel de accesibil și de foarte mică valoare. Prin contrast, raritatea conferă valoare și promovează comerțul, investițiile și inovația, deoarece obligă societățile să gestioneze eficient resursele limitate.



#### 6.1.1 Provocarea rarității digitale

Provocarea legată de raritatea digitală constă în ușurința cu care informația digitală poate fi copiată și distribuită. Informația digitală este, prin natura sa, mai dificil de securizat decât informația fizică deoarece, spre deosebire de bunurile fizice - unele dintre

care posedă în mod natural raritate datorită constrângerilor materiale - elementele digitale precum fișierele muzicale, documentele sau imaginile pot fi duplicate la infinit, practic fără niciun cost.

În mod tradițional, replicabilitatea datelor digitale a însemnat că aceste active nu puteau avea o valoare economică similară cu cele fizice, deoarece le lipsea orice formă de raritate aplicabilă. Pentru banii digitali, aceasta este o problemă deosebit de gravă și este caracterizată ca problema „dublului cheltuielii”, unde o singură unitate digitală (de exemplu, un token sau o monedă) poate fi copiată și cheltuită de mai multe ori, devalorizând-o astfel. Dacă este posibilă dublarea cheltuielii unei monede, aceasta îi scade valoarea, făcând-o de nedistins de fondurile contrafăcute sau frauduloase.

În mod tradițional, instituțiile financiare centralizate precum băncile atenuează acest risc prin menținerea unui registru care verifică fiecare tranzacție și deduce soldurile în consecință, asigurându-se că, odată ce banii sunt cheltuiți, nu pot fi reutilizați de același titular de cont. Totuși, această abordare necesită o autoritate centrală de încredere sau un „oracol” care să gestioneze și să verifice tranzacțiile, ceea ce impune dependență și un punct unic de control. Existența unui oracol centralizat de informații lasă activele digitale vulnerabile la manipulare și cenzură.

Pentru un sistem descentralizat, cu încredere minimizată, precum Bitcoin, unde nu există o autoritate centrală care să supravegheze tranzacțiile, prevenirea dublului cheltuieli este o provocare monumentală. Fără un mecanism care să asigure unicitatea fiecărei tranzacții, Bitcoin ar fi vulnerabil la exploatare, făcându-l nepractic ca depozit de valoare și mijloc de schimb de încredere. Bitcoin rezolvă problema dublului cheltuieli printr-un registru descentralizat, unde tranzacțiile sunt confirmate simultan de mii de participanți ai rețelei. Acest mecanism permite Bitcoin să mențină o evidență imuabilă a fiecărei tranzacții, asigurând că fiecare monedă poate fi cheltuită o singură dată.

Această soluție generează raritate digitală fără a se baza pe control centralizat. Bitcoin introduce prima soluție de succes pentru raritatea digitală, deschizând calea pentru un ecosistem de active digitale rare, cu încredere minimizată, într-un mod considerat anterior imposibil.



#### 6.1.2 Impunerea rarității digitale cu Bitcoin

> Propunem o soluție la problema dublului cheltuieli folosind un server de timestamp distribuit peer-to-peer pentru a genera dovada computațională a ordinii cronologice a tranzacțiilor. Sistemul este sigur atâta timp cât nodurile oneste controlează colectiv mai multă putere de procesare decât orice grup cooperant de noduri atacatoare.  
_Satoshi Nakamoto_

Satoshi Nakamoto a creat Bitcoin ca o soluție inginerească la problemele asociate cu banii fiat. Totuși, această soluție a necesitat ca Satoshi să descopere o modalitate de a impune o raritate digitală absolută. Pentru a realiza acest lucru, Satoshi a dezvoltat un protocol de comunicare open-source care rulează pe o rețea descentralizată de computere sau noduri. Fiecare dintre aceste noduri deține o copie locală, verificabilă, a unui registru imuabil, așa-numitul blockchain sau timechain. Protocolul Bitcoin definește regulile, iar rețeaua descentralizată verifică independent tranzacțiile, respectând aceleași reguli fără a necesita o autoritate centrală.

Raritatea Bitcoin contribuie la rolul său de depozit de valoare. La fel ca aurul, Bitcoin este valoros nu doar datorită ofertei sale limitate, ci și datorită efortului necesar pentru a „mina” sau produce noi monede. Minatul de Bitcoin (procesul care menține registrul și emite noi monede) este un proces costisitor, intensiv energetic, care reflectă acțiunea fizică de extragere a mineralelor din pământ. Acest „proof-of-work” digital impune o constrângere de producție care aliniază Bitcoin cu mărfurile tangibile, conferindu-i proprietăți de durabilitate și verificabilitate pe care bunurile digitale tradiționale nu le au. Dificultatea încorporată și rata descrescătoare de emitere a noilor monede prin „înjumătățiri” periodice creează o structură economică în care oferta de Bitcoin devine din ce în ce mai rară în timp, crescându-i atractivitatea ca depozit de valoare pe termen lung.

##### Cum este impusă raritatea digitală?

Soluția Bitcoin la problema dublului cheltuieli constă în utilizarea unui registru descentralizat și public. Registrul Bitcoin poate fi privit ca o bază de date imuabilă care înregistrează fiecare tranzacție într-un lanț secvențial de loturi cu marcaj temporal, numite blocuri. Fiecare bloc este strict cronologic și conține tranzacții care au fost verificate și acceptate de participanții rețelei. Fiecare bloc este conectat la cel anterior, creând o evidență permanentă care este distribuită pe mii de noduri la nivel mondial. Prin stocarea și partajarea acestui registru pe o rețea descentralizată, Bitcoin elimină necesitatea unei autorități centrale pentru confirmarea tranzacțiilor. Când are loc o tranzacție Bitcoin, nodurile din rețea o validează independent, asigurând că fiecare monedă este cheltuită o singură dată. Acest registru partajat face, de asemenea, extrem de dificil pentru atacatori să pirateze rețeaua sau să modifice tranzacțiile trecute, deoarece orice schimbare ar necesita aprobarea majorității participanților la rețea.

Mecanismul Proof-of-Work (PoW) al Bitcoin întărește și mai mult protecția împotriva dublului cheltuieli, deoarece minerii trebuie să rezolve o problemă criptografică pentru a primi permisiunea de a valida noi tranzacții și de a crea un nou bloc. Acest proces, cunoscut sub numele de minare, necesită putere de calcul și adaugă un nivel de dificultate și cost modificării registrului. Fiecare bloc adăugat la registru trebuie să conțină o legătură criptografică cu blocul anterior, ceea ce consolidează integritatea lanțului și previne manipularea.

Rolul unui nod este de a stoca cea mai actuală copie a registrului, care conține istoricul complet al tranzacțiilor. Nodurile îi mențin pe mineri „onești”, deoarece verifică faptul că nu a avut loc nicio dublă cheltuială și, important, că toate monedele au fost create în conformitate cu programul de emisie al Bitcoin. Orice utilizator de Bitcoin poate rula un nod și își poate verifica deținerea monedelor fără a avea nevoie să aibă încredere într-o terță parte. Nu este nevoie de autorități pentru a rezolva dispute în Bitcoin, deoarece orice tranzacție inclusă într-un bloc este obiectiv validă.

##### Cum ar putea un atacator să controleze rețeaua Bitcoin?

Dacă un atacator ar dori să modifice o tranzacție trecută pentru a reuși un atac de dublă cheltuială, ar trebui să refacă Proof-of-Work pentru acel bloc și pentru fiecare bloc ulterior, concurând cu puterea de calcul combinată a întregii rețele. Acest mecanism de securitate asigură că, dacă cineva ar încerca o dublă cheltuială, ar trebui să controleze peste 50% din puterea de minare a rețelei pentru a reuși. Acest lucru este cunoscut sub numele de atac de 51%.

În primii ani ai Bitcoin, când era posibil ca participanți individuali să creeze sau să mineze noi blocuri folosind hardware de calcul obișnuit, era cel puțin teoretic posibil să se folosească suficientă putere de calcul pentru a reuși un atac de 51%. Astăzi, puterea de calcul combinată a rețelei Proof-of-Work depășește 700 ExaHash/s. Aceasta înseamnă că, în total, computerele de minare calculează peste 700 de cvintilioane de hash-uri (operațiuni criptografice) pe secundă. Am ajuns la un punct în care costul imens și coordonarea necesară pentru a rescrie registrul și a reuși un atac de 51% fac dublarea cheltuielii imposibilă în practică.

##### Confirmări și reorganizări

Un alt strat de protecție (care uneori este trecut cu vederea) provine din procesul de confirmare a tranzacțiilor în Bitcoin. Când o tranzacție este transmisă pentru prima dată, este considerată neconfirmată și colectată în „mempool” în timp ce așteaptă să fie inclusă într-un bloc și validată de mineri. Odată ce o tranzacție este adăugată într-un bloc, este considerată „confirmată”. Fiecare bloc adăugat după aceea este considerat o confirmare suplimentară pentru tranzacție. Deși o tranzacție este considerată oficială după o singură confirmare, nu este considerată finală până când nu sunt adăugate confirmări suplimentare.

Pentru securitate deplină, utilizatorii Bitcoin așteaptă adesea mai multe confirmări (de obicei șase), deoarece fiecare bloc suplimentar adăugat la blockchain securizează și mai mult tranzacția, reducând dramatic probabilitatea unei încercări de dublă cheltuială reușite. Acest proces de confirmare stabilește o fereastră de timp în care tranzacțiile sunt finalizate.

##### De ce să aștepți șase confirmări?

Utilizatorii Bitcoin așteaptă confirmări suplimentare deoarece este posibil ca cel mai recent bloc de tranzacții să fie eliminat din lanțul de blocuri, dacă nu mai face parte din cel mai lung lanț. Este important de menționat că minatul este o competiție între foarte mari grupuri de putere de calcul. Prin urmare, este posibil ca doi mineri concurenți să găsească o soluție criptografică validă și blocuri separate să fie adăugate la lanț aproape simultan. Dacă se întâmplă acest lucru, lanțul este practic împărțit. Minerii vor continua să încerce să adauge blocuri la fiecare ramură a lanțului. Totuși, odată ce următorul bloc este minat, cel mai lung lanț1 (definit ca lanțul care are cea mai mare dovadă de lucru investită în el) este cel care prevalează, iar blocul de pe lanțul mai scurt este „orfanizat” și devine invalid. Toate tranzacțiile din blocul orfanizat sunt returnate în mempool pentru a fi incluse într-un bloc valid ulterior. Acest proces se numește reorganizare sau, simplu, „reorg”.

Un actor rău intenționat, care încearcă o dublă cheltuială, trebuie să preia controlul rețelei suficient de mult timp pentru a „reorganiza” lanțul. După cum am văzut mai sus, obținerea controlului total necesită o cantitate enormă de putere de calcul, dar ce se întâmplă dacă o operațiune de minare de mari dimensiuni - care controlează ipotetic puțin peste o treime din toată puterea de calcul a rețelei - încearcă o dublă cheltuială a monedelor?

Să parcurgem un exemplu:

Să presupunem, de exemplu, că puterea totală de minare a rețelei Bitcoin este de 550 ExaHash/s. Rogue Inc, care controlează 200 ExaHash/s, face o achiziție imobiliară mare și intenționează să plătească în Bitcoin. Totuși, Rogue plănuiește și să încerce o dublă cheltuire a acelorași monede. Vânzătorul îi spune lui Rogue că va aștepta șase confirmări înainte de a preda actele de proprietate. Pentru a reuși un atac de dublă cheltuire, Rogue trebuie să construiască în secret o ramură alternativă în lanț, minând un lanț mai lung care să conțină tranzacția de dublă cheltuire. Odată ce vânzătorul a văzut șase confirmări care includ tranzacția sa și a predat activul, Rogue trebuie apoi să publice toate blocurile minate pe noua ramură, făcând-o astfel cel mai lung lanț. Cât de posibil este acest lucru?

În orice moment, probabilitatea ca Rogue să mineze următorul bloc este 200/550 = 0,36. Chiar dacă Rogue este cel mai mare pool de minare, probabilitatea ca minerii onești să găsească următorul bloc este 1 - 0,36 = 0,64. Blocurile ar trebui să fie minate mult mai rapid pe lanțul onest. Dar să presupunem că Rogue are noroc, minează un bloc și îl ține secret. Apoi încearcă să mineze încă unul pe această ramură secretă. Totuși, lanțul onest minează apoi un bloc și trece în față minând încă unul, înainte ca Rogue să mineze al doilea său bloc.

Rogue renunță atunci. De ce?


| Blocuri de recuperat | 1% | 10% | 36% (Rogue) | 51% |
| --- | --- | --- | --- | --- |
| 1 | 0,010101 | 0,111111 | 0,562500 | 1,0 |
| 2 | 0,010102 | 0,012346 | 0,316406 | 1,0 |
| 3 | 1,0e-06 | 0,001372 | 0,177919 | 1,0 |
| 4 | 1,0e-08 | 0,000152 | 0,100113 | 1,0 |
| 5 | 1,0e-10 | 0,000017 | 0,056314 | 1,0 |
| 6 | 1,0e-12 | 1,9e-06 | 0,031676 | 1,0 |


**Sursă**: Bazat pe un tabel din Grokking Bitcoin de Kalle Rosenbaum

Rogue își dă seama că nu are suficientă putere de hash pentru a realiza dublă cheltuire, deși controlează 36% din puterea de hash a Bitcoin. Pentru a reuși, trebuie să mineze încă patru blocuri pentru a depăși lanțul onest. În ciuda puterii sale de calcul vaste și a controlului a 36% din rețea, șansele de succes ale lui Rogue sunt doar 0,100113.


> **Info – Teoria jocurilor intră în acțiune**
>
> Șansele de succes ale lui Rogue sunt foarte mici, dar devine și mai rău. Pentru fiecare minut în care continuă să încerce, Rogue consumă o cantitate enormă de electricitate. Tot acest efort va fi în zadar. Mai mult, pentru fiecare bloc pe care nu îl minează onest, Rogue pierde recompensa de bloc, care este în prezent de 3,125 monede pe bloc, evaluate la peste 300.000 € în prezent.
>
> Motivul principal al eșecului lui Rogue a fost că vânzătorul imobilului a cerut șase confirmări. Cu cât sunt necesare mai multe confirmări, cu atât este mai greu pentru minerii necinstiți să construiască lanțuri alternative de blocuri. De fapt, pentru o tranzacție foarte mare, un vânzător poate cere mai multe confirmări. De exemplu, zece confirmări (care ar trebui să dureze aproximativ 100 de minute) ar reduce șansele de succes ale lui Rogue la doar 0,003.
>
> În acest fel, teoria jocurilor din jurul minării asigură că toți sunt stimulați să acționeze onest și să nu irosească resurse de calcul sau să piardă recompensele de bloc. Mai mult, este în interesul tuturor minerilor ca rețeaua Bitcoin să fie sigură și de încredere. Acest lucru asigură protejarea investiției lor uriașe în putere de calcul. Dacă rețeaua este atacată cu succes, valoarea de piață a monedelor va scădea dramatic, deoarece încrederea în rețea va fi diminuată.




#### 6.1.3 Este centralizarea minării o amenințare?

După cum se vede în tabelul de mai sus, centralizarea minării poate reprezenta o amenințare potențială pentru protecția împotriva dublei cheltuiri a Bitcoin, deoarece crește probabilitatea unui atac de 51% - un scenariu în care un singur miner sau un grup de mineri controlează peste jumătate din puterea computațională a rețelei. Dacă acest lucru s-ar întâmpla, entitatea care controlează ar putea, teoretic, să modifice tranzacțiile recente sau să încerce o dublă cheltuire rescriind registrul, permițându-i să cheltuiască aceleași monede de mai multe ori.

O astfel de situație subminează integritatea rețelei Bitcoin, oferind o influență disproporționată asupra validării tranzacțiilor unui număr mic de actori. Totuși, deși este posibil teoretic, executarea unui atac de 51% ar fi totuși extrem de complexă și costisitoare, necesitând resurse computaționale, electricitate și coordonare imense, ceea ce ar depăși probabil beneficiile potențiale ale încercării unei duble cheltuiri.

Există măsuri de protecție care ajută la limitarea riscurilor centralizării minării. Pool-urile de minare, de exemplu, permit minerilor mai mici să își combine resursele și să împartă recompensele de bloc, reducând dominația oricărei entități individuale. Deși aceasta este o modalitate utilă pentru micii mineri de a participa la rețea, există riscul ca entitatea care controlează pool-ul să se comporte necorespunzător și să încerce să atace rețeaua. Totuși, transparența registrului Bitcoin înseamnă și că orice concentrare a puterii de minare este vizibilă, alertând comunitatea asupra riscurilor potențiale și permițând măsuri de contracarare. Minerii sunt foarte conștienți că orice atac asupra rețelei Bitcoin riscă să îi afecteze grav valoarea, astfel încât este foarte ușor pentru micii mineri să treacă la un nou pool pentru a evita ca puterea lor de minare să fie folosită în mod rău intenționat. Deși riscul nu este zero, natura deschisă și distribuită a ecosistemului Bitcoin, combinată cu costul ridicat al unui atac, face ca centralizarea minării să fie mai degrabă o amenințare teoretică decât una iminentă, deoarece menținerea unui astfel de control pentru perioade îndelungate ar fi neviabilă financiar pentru orice atacator.



#### 6.1.4 Impactul mai larg al rarității digitale

Bitcoin a transformat modul în care gândim despre raritate în domeniul digital. Deoarece bunurile digitale – precum software-ul, fișierele muzicale, cărțile electronice și conținutul online – au caracteristici care le diferențiază de bunurile fizice, ele pot fi reproduse la costuri neglijabile și distribuite instantaneu. Spre deosebire de obiectele fizice, care sunt limitate de constrângeri materiale precum costurile de producție și limitările de stocare, bunurile digitale există ca date ce pot fi copiate la infinit fără degradarea calității. Aceasta înseamnă că, în timp ce bunurile fizice sunt în mod inerent rare din cauza acestor constrângeri materiale, bunurile digitale au fost în mod tradițional abundente, lipsindu-le orice mecanism încorporat de limitare a ofertei.

Este important de menționat că bunurile digitale sunt non-rivale. Asta înseamnă că utilizarea unui bun digital de către o persoană nu diminuează disponibilitatea acelui bun pentru ceilalți. De exemplu, atunci când o melodie este descărcată, ea poate fi copiată și distribuită de un număr nelimitat de ori fără a-și pierde utilitatea. Istoric, această abundență a reprezentat o provocare pentru crearea de valoare, deoarece modelul economic tradițional al cererii și ofertei devine distorsionat atunci când oferta este, cel puțin teoretic, nelimitată. Ca răspuns la aceasta, managementul drepturilor digitale (DRM) și alte măsuri artificiale de creare a rarității au încercat să restricționeze accesul. Totuși, aceste mecanisme pot fi ocolite și transferă încrederea către autorități centralizate. Inovația adusă de Bitcoin constă în modul în care abordează această problemă în mod nativ, fiind primul activ digital care încorporează raritatea prin tehnologie descentralizată, fără a se baza pe aceste limitări tradiționale.

Bitcoin joacă un rol transformator în stabilirea rarității digitale prin introducerea unui protocol care impune o ofertă finită. O limită de 21 de milioane de monede este codificată în protocol și această limită nu poate fi schimbată fără consensul rețelei, adică al tuturor miilor de participanți răspândiți la nivel global care rulează noduri Bitcoin. În acest fel, Bitcoin a creat un activ care imită natura finită a mărfurilor fizice, precum aurul, existând în același timp exclusiv în domeniul digital. Plafonul de ofertă este fundamental pentru valoarea Bitcoin și este susținut de o combinație de criptografie, mecanisme de consens și cod open-source transparent. Acest lucru asigură că toți participanții din rețea respectă aceleași reguli, fiind motivați de stimulentul economic cheie de a garanta că oferta de monede este absolut și demonstrabil finită.

Prin rezolvarea problemei dublei cheltuieli, Bitcoin previne inflația sau duplicarea activului, o provocare care a afectat experimentele anterioare cu bani digitali. În cadrul Bitcoin, nicio autoritate unică nu controlează oferta, ceea ce îl face imun la manipularea centralizată de tipul celei întâlnite în sistemul monetar fiat, precum tipărirea arbitrară de monedă sau devalorizarea. Această inovație permite Bitcoin să servească drept depozit de valoare și protecție împotriva inflației, permițându-i să ocupe o poziție unică asemănătoare cu „aurul digital” – o resursă digitală rară cu valoare verificabilă.



#### 6.1.5 Concluzie

În concluzie, devine tot mai larg înțeles faptul că inovația Bitcoin privind raritatea digitală a redefinit conceptul de bani. Totuși, uneori se trece cu vederea faptul că Bitcoin a transformat și peisajul digital prin rezolvarea problemei de lungă durată a creării rarității într-o lume digitală inerent abundentă. Bitcoin a introdus efectiv o nouă categorie de activ digital care reflectă calitățile mărfurilor fizice.

Această descoperire demonstrează că un sistem descentralizat poate stabili raritate, imuabilitate și valoare independent de orice autoritate centrală. Mai mult, ar putea avea utilizări dincolo de bani, deoarece a inspirat un întreg domeniu de cercetare și dezvoltare în jurul acestei tehnologii.

Privind spre viitor, modelul Bitcoin de raritate digitală modelează viitorul banilor și al stocării valorii. Pe măsură ce preocupările legate de inflație și întrebările privind gestionarea monedei fiat devin tot mai recunoscute, oferta fixă a Bitcoin îl face din ce în ce mai atractiv ca protecție împotriva instabilității financiare tradiționale.

În cele din urmă, descoperirea de către Bitcoin a rarității digitale ar putea marca începutul unei schimbări de paradigmă, în care activele digitale cu raritate recunoscută și încredere verificabilă câștigă recunoaștere ca elemente valoroase ale economiei moderne, stabilind o fundație pentru viitorul finanțelor descentralizate și al proprietății digitale. Acest lucru are implicații semnificative pentru domeniul economic – Bitcoin a oferit modelul pentru modul în care raritatea și valoarea pot exista într-o formă digitală.

> Dincolo de raritatea digitală, Bitcoin este și primul exemplu de raritate absolută, singura marfă lichidă (digitală sau fizică) cu o cantitate fixă stabilită care nu poate fi crescută în mod conceput. Până la inventarea Bitcoin, raritatea a fost întotdeauna relativă, niciodată absolută.  
_Saifedean Ammous_



###### Note

1. Cel mai lung lanț este acceptat de nodurile Bitcoin ca fiind cea mai validă versiune a registrului și este definit ca lanțul care a necesitat cel mai mare efort (sau cea mai mare dovadă de lucru) pentru a fi construit. Mai multe informații aici: [https://learnmeabitcoin.com/technical/blockchain/longest-chain/](https://learnmeabitcoin.com/technical/blockchain/longest-chain/)
