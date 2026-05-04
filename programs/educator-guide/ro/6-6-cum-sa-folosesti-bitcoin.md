# 6 - Cum să folosești Bitcoin

Durată: 90 de minute

Idee principală: Folosirea Bitcoin pe lanț îi învață pe studenți cum funcționează în practică proprietatea, auto-custodia și verificarea, transformând teoria în acțiune financiară directă.

#### Obiective de învățare

La finalul acestei lecții, studenții ar trebui să poată:

* Să identifice modalități comune de a obține și schimba bitcoin, inclusiv metode peer-to-peer și prin platforme centralizate.
* Să explice diferența dintre portofelele auto-custodiale și cele custodiale și de ce auto-custodia este importantă în Bitcoin.
* Să descrie scopul cheilor private, adreselor publice, frazelor seed și interfețelor portofelului.
* Să compare diferite tipuri de portofele și să evalueze compromisurile lor în funcție de securitate, comoditate, confidențialitate și control.
* Să configureze un portofel Bitcoin pe mobil și să explice procesul de recuperare de bază.
* Să demonstreze cum se primește și se trimite o tranzacție bitcoin pe lanț.

Să aplice principiul „Nu te încrede, verifică” la alegerea portofelului, tranzacții și utilizarea mai largă a Bitcoin.

#### Instrumente & Resurse

##### Materiale vizuale

* Capitolul 6 - Cum să folosești Bitcoin

##### Bibliotecă de suport

* Card de referință vocabular — Capitolul 6 — Termeni: portofel, cheie privată, adresă publică, frază seed, custodial, auto-custodial, UTXO, taxă de tranzacție
* Tabele comparative & fișe de referință — Comparație tipuri de portofele (custodial, mobil, hardware, hârtie)
* Explicații tehnice & detalii aprofundate — Chei publice/private, model UTXO, confirmarea tranzacțiilor
* Aprofundare securitate cheie privată — Fraze seed, derivare chei, metode de backup, vectori de atac
* Ghidul anatomiei unei tranzacții — Exemplu pas cu pas despre cum funcționează o tranzacție Bitcoin
* Listă de verificare pentru cele mai bune practici de securitate — Înainte de a începe, crearea portofelului, primire, trimitere, prevenirea phishing-ului

#### Activități

* Tranzacții în acțiune
* Cursa Lightning Relay
* Explorarea Mempool-ului

#### Predare online

* Clarifică de la început dacă studenții urmăresc o demonstrație sau își configurează singuri portofelul.
* Folosește capturi de ecran mari și lizibile pentru fiecare pas de configurare a portofelului.
* Pauzează după fiecare pas și cere studenților să confirme în chat că au înțeles înainte de a continua.
* Oferă un avertisment direct înainte de secțiunea despre fraza seed și amintește-le studenților să nu partajeze niciodată informații sensibile online.

#### Pregătire

* Descarcă și testează o aplicație de portofel mobil (Blue Wallet sau Muun); pregătește capturi de ecran cu pașii cheie de configurare.
* Pregătește un ghid de configurare a portofelului (descărcare → creare → backup seed → primire) pentru referință.
* Asigură-te că rețeaua/WiFi funcționează; ai pregătită o adresă demo și un cod QR de arătat.

#### Procedură

Această lecție trece de la teorie la practică directă. Acum se potrivește direct cu structura Diplomei astfel încât achiziția, portofelele, configurarea, tranzacțiile și verificarea apar sub aceleași titluri principale ca în ghidul pentru studenți. Suportul suplimentar pentru predare rămâne inclus în acele secțiuni.

##### 6.0 Introducere, 8 minute

Începe prin a conecta acest capitol cu cel anterior:

* Dacă Bitcoin este bani, cum îl obțin și folosesc oamenii de fapt?
* Ce înseamnă să controlezi cu adevărat bitcoin-ul tău?
* De ce este diferită folosirea Bitcoin față de o aplicație bancară?

Clarifică faptul că acest capitol este despre utilizarea practică. Studenții nu mai învață doar ce este Bitcoin, ci învață cum să interacționeze direct cu el.

##### 6.1 Achiziționarea și schimbul de Bitcoin, 12 minute

Explică faptul că oamenii pot obține bitcoin în diferite moduri, inclusiv:

* să fie plătiți în bitcoin
* minarea de bitcoin
* schimbarea fiat-ului cu bitcoin în persoană
* schimbarea fiat-ului cu bitcoin online

Apoi concentrează-te pe cele două rute principale de achiziție acoperite în capitol:

* peer-to-peer, în persoană
* peer-to-peer, online
* exchange-uri centralizate

Fă compromisurile clare.

Pentru P2P în persoană, subliniază schimbul direct fără bancă sau intermediar, dar menționează și riscurile practice ale întâlnirii cu persoane pentru tranzacții cu numerar.

Pentru P2P online, explică escrow-ul în termeni simpli, ca o modalitate de a reduce riscul de contrapartidă, permițând totodată schimbul direct între persoane.

Pentru exchange-urile centralizate, clarifică faptul că sunt convenabile, dar necesită ca utilizatorii să aibă încredere într-o companie, să furnizeze adesea informații personale și să lase fondurile sub controlul unei terțe părți până la retragere. Acesta este un moment bun pentru a sublinia că de multe ori comoditatea vine cu compromisuri în ceea ce privește confidențialitatea și suveranitatea.

##### 6.2 O Introducere în Portofelele Bitcoin, 35 de minute

**Ce este de fapt un portofel Bitcoin**

Clarifică de la început o neînțelegere comună: bitcoin-ul nu este stocat în aplicația portofel ca banii fizici într-o geantă.  
Bitcoin-ul există pe registrul menținut de rețea. Ceea ce controlează utilizatorul este abilitatea de a-l cheltui prin cheile private.

Apoi explică cele două lucruri la care oamenii se referă adesea prin „portofel”:

* sistemul de chei private, din care sunt generate adresele
* aplicația sau interfața folosită pentru a interacționa cu rețeaua

Folosește analogia cu emailul din capitol, dacă este de ajutor:

* adresă publică = ca o adresă de email pe care o poți împărtăși
* cheie privată = ca o parolă pe care trebuie să o protejezi

Fii foarte clar aici: cine controlează cheile private controlează bitcoin-ul. Acesta este conceptul de bază pe care studenții trebuie să îl înțeleagă.

**Portofele cu autocustodie vs portofele custodiale**

Aceasta este una dintre cele mai importante părți ale capitolului.

Explică clar distincția:

* Portofel cu autocustodie: utilizatorul controlează cheile private
* Portofel custodial: o terță parte controlează cheile private în numele utilizatorului

Apoi prezintă compromisurile:

Autocustodie

* control total asupra fondurilor
* fără proces de aprobare
* protecție împotriva confiscării arbitrare
* responsabilitate mai mare
* nu există recuperare ușoară dacă fraza seed este pierdută

Custodial

* recuperare și suport mai ușor
* mai simplu pentru începători
* mai expus la blocarea contului, hack-uri și controlul unei terțe părți
* utilizatorul nu deține cu adevărat bitcoin-ul

Acesta este momentul potrivit pentru a sublinia expresia:

"Nu sunt cheile tale, nu sunt monedele tale."

Studenții ar trebui să plece din această secțiune înțelegând nu doar sloganul, ci și ce înseamnă el în practică.

**Tipuri diferite de portofele și cum să alegi unul**

Prezintă tipurile de portofele acoperite în capitol:

* portofel online
* portofel mobil
* portofel desktop
* portofel hardware
* portofel pe hârtie

Nu trata niciunul ca fiind perfect. În schimb, explică faptul că fiecare implică compromisuri între:

* securitate
* confidențialitate
* comoditate
* compatibilitate
* comisioane
* control
* reputație

De asemenea, clarifică faptul că recomandăm să se acorde atenție dacă software-ul portofelului este open-source, deoarece instrumentele open-source pot fi revizuite, auditate și continuate de către comunitate. Acest lucru se leagă direct de principiul verificării în Bitcoin.

##### 6.3 Configurarea unui portofel Bitcoin pe mobil, 10 minute

Ghidează elevii prin procesul de bază prezentat în capitol:

* descarcă portofelul
* creează un portofel nou
* generează și notează fraza de recuperare
* confirmă fraza de recuperare
* adaugă securitate suplimentară dacă este disponibilă
* deschide portofelul și găsește funcția de primire

Fă avertismentul despre fraza seed foarte explicit:

* dacă fraza seed este pierdută, accesul la fonduri poate fi pierdut
* dacă altcineva obține fraza seed, poate lua fondurile

Dacă elevii fac acest exercițiu practic, educatorul ar trebui să facă pauză la fiecare pas și să verifice că toată lumea înțelege ce face. Dacă lecția este mai conceptuală, această secțiune poate fi explicată ca o prezentare, nu efectuată live. Opțiunea de recuperare prezentată în capitol este utilă și pentru a explica faptul că portofelele pot fi restaurate dacă fraza seed a fost salvată corect.

##### 6.4 Primirea și trimiterea tranzacțiilor, 17 minute

**Primirea și trimiterea tranzacțiilor on-chain**

Explică acum cum funcționează tranzacțiile on-chain.

Pentru a primi bitcoin:

* deschide portofelul
* apasă pe primește sau depune
* copiază adresa, distribuie linkul sau arată codul QR

Pentru a trimite bitcoin:

* deschide portofelul
* lipește sau scanează adresa destinatarului
* introdu suma
* verifică toate detaliile de două ori
* transmite tranzacția
* așteaptă confirmarea

Fă aceste puncte cheie foarte clare:

* tranzacția transferă proprietatea, nu monede fizice
* tranzacțiile sunt ireversibile
* nodurile verifică validitatea
* minerii includ tranzacțiile în blocuri
* taxele influențează prioritatea confirmării
* tranzacțiile on-chain sunt în general sigure, dar mai lente și adesea mai scumpe decât tranzacțiile Lightning

Diagrama fluxului tranzacției din capitol este deosebit de utilă aici, deoarece îi ajută pe elevi să vizualizeze drumul de la cererea din portofel până la confirmarea în rețea.

**Tranzacții în acțiune și exercițiu pe roluri**

Folosește structura exercițiului cooperativ din capitol pentru a consolida înțelegerea. Explică cele patru roluri implicate:

* expeditor
* destinatar
* miner
* operator de nod

O abordare simplă la clasă este să atribuiți roluri și să parcurgeți o tranzacție pas cu pas. Acest lucru îi ajută pe elevi să vadă că o tranzacție Bitcoin nu este magie, ci un proces coordonat care implică aprobare, verificare, includere într-un bloc și actualizarea registrului.

Scopul aici nu este profunzimea tehnică. Este să-i ajutăm pe elevi să înțeleagă cine face ce într-o tranzacție și de ce contează verificarea.

##### 6.5 Nu te încrede, verifică, 8 minute

Explică că acest lucru se aplică la:

* portofele
* schimburi
* aplicații
* detalii ale tranzacției
* afirmații despre „profituri ușoare”
* proiecte care pretind că sunt ca Bitcoin

Explică clar că Bitcoin necesită ca utilizatorii să gândească critic, să verifice ceea ce folosesc și să evite încrederea oarbă. De asemenea, explică de ce instrumentele open-source sunt importante în acest context: ele fac posibilă verificarea independentă.

###### Încheiere și verificarea înțelegerii

Încheie cu câteva întrebări rapide:

* Care este diferența dintre un portofel custodial și unul self-custodial?
* De ce este atât de importantă fraza seed?
* Ce se întâmplă când trimiți o tranzacție on-chain?
* De ce tranzacțiile on-chain sunt mai lente decât unele alte plăți cu Bitcoin?
* Ce înseamnă practic „Nu te încrede, verifică”?

#### Note pentru educator

Acest capitol este foarte practic, așa că prioritizează claritatea, siguranța și repetiția.

Elevii nu trebuie să stăpânească fiecare tip de portofel într-o singură lecție. Obiectivele principale sunt:

* înțelegerea elementelor de bază ale portofelului
* înțelegerea self-custody
* învățarea fluxului de bază al unei tranzacții
* adoptarea unei mentalități responsabile de verificare

Fii deosebit de atent când discuți despre frazele seed și configurarea portofelului. Elevii trebuie să plece înțelegând că acestea nu sunt detalii minore, ci baza deținerii Bitcoin.

Cele mai utile materiale vizuale și activități din acest capitol sunt:

* comparația între self-custodial și custodial
* tabelul cu compromisurile fiecărui tip de portofel
* exercițiul pas cu pas de configurare a portofelului
* diagrama fluxului unei tranzacții
* activitatea de tranzacționare pe roluri

##### Cum arată binele

* Este important ca elevii să configureze efectiv un portofel sau să urmărească o demonstrație atentă, să pună fraza seed în centrul atenției cu „Aceste 12 cuvinte SUNT Bitcoin-ul tău”, să testeze scenarii precum „Ce se întâmplă dacă îți pierzi telefonul?” și să exerseze recunoașterea tentativelor de phishing.
* Educatorii ar trebui să fie ghizi practici care au făcut acest lucru înainte, să fie conștienți de securitate fără a fi paranoici și să fie sinceri despre dificultatea și efortul de învățare necesar.
* Elevii simt că au învățat o abilitate reală pe care o pot folosi, înțeleg că fraza seed este reală și importantă, nu doar abstractă, se simt capabili să dețină propriul Bitcoin și înțeleg că descentralizarea presupune responsabilitate personală.
* Rezultatele învățării ar trebui atinse dacă elevii pot configura un portofel și pot înțelege diferența dintre cheile publice și private, pot explica compromisurile între portofelele custodial și self-custodial, pot explica cum funcționează o tranzacție, inclusiv inputuri, outputuri și comisioane, pot demonstra conștientizare privind securitatea, inclusiv protejarea frazei seed, și pot pune întrebări critice despre proprietate și control.

##### Gestionarea timpului

Dacă timpul este scurt, prioritizează:

* Înțelegerea elementelor de bază ale portofelului
* Înțelegerea self-custody
* Învățarea fluxului de bază al unei tranzacții
* Adoptarea unei mentalități responsabile de verificare

Dacă ai timp în plus, acordă atenție:

* Tabelul de comparație între self-custodial și custodial
* Tabelul cu compromisurile fiecărui tip de portofel
* Exercițiu pas cu pas de configurare a portofelului cu demonstrație live
* Diagrama fluxului unei tranzacții cu calcule de comisioane
* Practici avansate de securitate și considerații despre portofele hardware

##### Dacă elevii întâmpină dificultăți

* Frazele seed ca „reale” → „Această frază ESTE bitcoin-ul tău; nu există serviciu clienți.”
* Chei publice vs. private → Analogie cu emailul (adresă vs. parolă).
* De ce este greu → „Tu îl controlezi; tu ești responsabil.” Recunoaște compromisurile.
