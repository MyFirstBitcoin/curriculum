# 9 - Cum funcționează mineritul de Bitcoin

Durată: 90 de minute

Idee principală: Mineritul de Bitcoin și validarea de către noduri lucrează împreună pentru a securiza rețeaua, a confirma tranzacțiile și a impune regulile sistemului prin Proof of Work.

#### Obiective de învățare

La finalul acestei lecții, elevii ar trebui să poată:

* Explice diferența dintre rolul nodurilor Bitcoin și rolul minerilor Bitcoin.
* Descrie cum nodurile validează tranzacțiile, partajează informații și ajută la impunerea regulilor Bitcoin.
* Explice ce fac minerii, inclusiv selectarea tranzacțiilor, construirea blocurilor candidate și competiția pentru a găsi un hash valid al blocului.
* Definească mempool-ul și să explice de ce funcționează ca o sală de așteptare pentru tranzacțiile neconfirmate.
* Descrie cum taxele de tranzacție influențează selecția minerilor și viteza de confirmare.
* Explice Proof of Work ca mecanismul care securizează Bitcoin făcând atacurile costisitoare.
* Descrie cum ajustarea dificultății ajută la menținerea unui timp mediu de bloc de aproximativ 10 minute.
* Parcurgă întregul ciclu de viață al unei tranzacții Bitcoin, de la creare și semnare până la confirmarea într-un bloc.

#### Instrumente & Resurse

##### Materiale vizuale

* Capitolul 9 - Cum funcționează mineritul Bitcoin?

##### Bibliotecă de suport

* Card de referință vocabular — Capitolul 9 — Termeni: minerit, Proof of Work, puzzle hash, ajustarea dificultății, recompensă de bloc, mempool, atac de 51%
* Biblioteci de concepții greșite — Capitolul 9 — Abordează: „minerii creează Bitcoin din nimic”, „minerii controlează Bitcoin”, „mai mult minerit = mai puțină securitate”
* Tabele comparative & fișe de referință — Economia mineritului: venituri, costuri, alinierea stimulentelor; ajustarea dificultății
* Explicații tehnice & analize detaliate — Securitatea Proof of Work; de ce atacurile sunt costisitoare; pragul de 51%

#### Activități

* Explorarea mempool-ului
* Tranzacții în acțiune

#### Predare online

* Folosește o diagramă clară a fluxului unei tranzacții de la semnarea în portofel până la confirmare.
* Păstrează nodurile și minerii vizual separați pe ecran pe tot parcursul lecției.
* Folosește mempool.space sau o captură de ecran a acestuia pentru a arăta tranzacțiile neconfirmate și presiunea taxelor.
* Fă pauză după fiecare etapă a procesului de minerit și pune o întrebare scurtă de înțelegere.

#### Pregătire

* Pregătește o diagramă a procesului de minerit (mempool → selecția tranzacțiilor → crearea blocului → ajustarea dificultății) pentru afișare.
* Adaugă la favorite pagina mempool.space sau blockchain.com pentru minerit; pregătește capturi de ecran cu statisticile actuale de minerit și ajustările de dificultate.
* Creează o explicație vizuală a Proof of Work ca mecanism de securitate; arată ajustarea dificultății din ultimele 3-6 luni.

#### Procedură

Această lecție analizează mai atent modul în care tranzacțiile Bitcoin circulă prin rețea și devin parte din blockchain. Acum urmează direct structura Diplomei, astfel încât secțiunile principale să se alinieze cu ghidul pentru elevi, păstrând totodată explicațiile detaliate pentru educatori în fiecare secțiune.

##### 9.0 Introducere, 8 minute

Începe prin a conecta acest capitol cu cel anterior:

* Dacă un utilizator semnează o tranzacție cu o cheie privată, ce se întâmplă după aceea?
* Cine verifică dacă acea tranzacție este validă?
* Cum ajunge să fie adăugată în blockchain?
* De ce are nevoie Bitcoin atât de noduri, cât și de mineri?

Clarifică faptul că acest capitol explică modul în care rețeaua procesează tranzacțiile în practică și cum mineritul securizează sistemul fără o autoritate centrală.

##### 9.1 Noduri și mineri Bitcoin, 47 minute

**Noduri și mineri, roluri diferite**

Începe prin a separa clar cele două roluri.

Noduri Bitcoin:

* păstrează o copie a blockchain-ului
* verifică dacă tranzacțiile respectă regulile
* partajează informații cu alte noduri
* ajută portofelele și alte programe să acceseze datele din blockchain
* pot respinge tranzacții sau blocuri invalide

Capitolul descrie nodurile ca fiind portarii validării și extinde această idee cu analogia „ofițerului de circulație digital”. Aceasta este utilă deoarece arată nodurile ca verificatori și coordonatori, nu ca stăpâni. Diagrama întărește, de asemenea, faptul că multe noduri păstrează copii ale registrului în întreaga lume.

Minerii Bitcoin:

* adună tranzacții valide
* asamblează blocuri candidate
* concurează pentru a găsi un hash valid al blocului
* difuzează blocurile valide atunci când câștigă
* primesc recompense de bloc și comisioane de tranzacție

Un punct cheie de predare din capitol este că scopul mineritului nu este doar de a crea noi bitcoin, ci de a descentraliza securitatea Bitcoin. Noii bitcoin reprezintă stimulentul, în timp ce procesul de minerit în sine este mecanismul de securitate.

**Ce Fac De Fapt Nodurile**

Dezvoltă secțiunea despre noduri cu lista de funcții a nodurilor din capitol:

* Portari ai validării: verifică dacă tranzacțiile și blocurile respectă regulile
* Centru de comunicare: se conectează între ele și partajează date despre tranzacții
* Verificator de calitate: resping informațiile invalide
* Informator blockchain: furnizează date altor programe, cum ar fi portofelele
* Primitor de noduri noi: ajută nodurile noi să obțină blockchain-ul, în timp ce fiecare nod nou verifică totuși datele independent

Acesta este un moment bun pentru a sublinia că rularea unui nod oferă utilizatorului mai multă independență. În loc să depindă complet de servicii externe pentru a afla starea rețelei, pot verifica ei înșiși. face acest punct clar, inclusiv menționarea Bitcoin Core ca una dintre implementările pe care utilizatorii le pot rula.

**Ce Fac De Fapt Minerii**

Acum explică mineritul mai atent.

Minerii:

* colectează tranzacții verificate dar neconfirmate
* le grupează într-un bloc candidat
* calculează în mod repetat hash-ul datelor blocului în căutarea unui hash valid
* difuzează blocul câștigător în rețea
* câștigă recompense dacă blocul este acceptat

Folosește analogia „uriei grămezi de chei” din capitol dacă ajută. Oferă elevilor o imagine concretă a cursei de minerit. Ideea principală nu este că minerii rezolvă o problemă matematică utilă în sens obișnuit, ci că dovedesc că au consumat energie și calcul real pentru a securiza sistemul.

Acesta este, de asemenea, locul potrivit pentru a explica recompensele minerilor:

* recompensa de bloc: bitcoin nou emisi
* comisioane de tranzacție: comisioane atașate tranzacțiilor pe care utilizatorii doresc să le confirme

Clarifică faptul că minerii de obicei prioritizează tranzacțiile cu comisioane mai mari, deoarece acestea le cresc recompensa. Capitolul explică aici și înjumătățirile, așa că poți menționa pe scurt că recompensa de bloc scade la fiecare 210.000 de blocuri, aproximativ la fiecare patru ani, conform programului public de emisie al Bitcoin. Paginile 5 și 6 includ programul de emisie și tabelul cu următoarea înjumătățire, care pot ajuta la întărirea emisiunii previzibile a Bitcoin.

**Hash Valid de Bloc, Dovada Muncii și Ajustarea Dificultății**

Această secțiune este esența capitolului.

Explică faptul că minerii caută un hash valid de bloc, adică un hash care să respecte ținta rețelei. Capitolul explică acest lucru ca fiind găsirea unui număr mai mic decât ținta stabilită de rețea.

Apoi explică clar Dovada Muncii:

* minerii trebuie să efectueze muncă computațională repetată
* primul care găsește un hash valid dovedește că a făcut acea muncă
* acest lucru face costisitoare rescrierea sau atacarea registrului
* nodurile apoi verifică blocul înainte de a-l accepta

O frază puternică pentru predare este:

Dovada Muncii securizează Bitcoin făcând necinstea costisitoare și verificarea ușoară.

Explică și ajustarea dificultății:

* rețeaua ajustează dificultatea mineritului la fiecare 2.016 blocuri
* acest lucru se întâmplă aproximativ la fiecare două săptămâni
* scopul este să mențină timpul mediu de bloc aproape de 10 minute
* dacă mai multă putere de hash se alătură rețelei, dificultatea crește
* dacă este prezentă mai puțină putere de hash, dificultatea scade

Paginile 7 și 8 explică acest proces și arată cum țintele mai dificile necesită mai multă muncă. Acest lucru ajută elevii să înțeleagă că temporizarea Bitcoin nu este controlată de o autoritate centrală, ci de reguli de protocol care răspund automat la condițiile rețelei.

##### 9.2 Ce Este Mempool-ul?, 15 minute

Acum treci la mempool.

Explică faptul că mempool-ul este sala de așteptare pentru tranzacțiile valide, neconfirmate. Când un utilizator transmite o tranzacție, nodurile o verifică mai întâi. Dacă este validă, o adaugă în mempool-ul lor și o partajează cu alte noduri. Apoi minerii pot selecta dintre aceste tranzacții aflate în așteptare când construiesc un bloc. Paginile 10 și 11 explică direct acest proces.

Puncte importante de subliniat:

* mempool-ul nu este blockchain-ul
* tranzacțiile de acolo sunt încă neconfirmate
* fiecare nod își menține propriul mempool
* nu există un singur mempool universal
* tranzacțiile cu taxe mai mari au șanse mai mari să fie selectate mai repede

Capitolul explică, de asemenea, motivele obișnuite pentru care o tranzacție poate rămâne neconfirmată mult timp:

* taxă mică
* aglomerare în rețea
* tentativă de dublă cheltuire
* date incorecte sau incomplete
* tranzacție formatată greșit

Dacă este util, menționează activitatea cu mempool.space ca o modalitate practică de a vizualiza tranzacțiile neconfirmate și nivelurile taxelor. Precizează clar că mempool.space este doar un explorator, nu mempool-ul propriu-zis.

##### 9.3 Cum funcționează tranzacțiile Bitcoin, 20 de minute

Acum adună totul folosind secvența pas cu pas a capitolului.

O versiune clară pentru clasă este:



1. Expeditorul selectează un UTXO și creează o tranzacție
1. Expeditorul adaugă adresa destinatarului și taxa
1. Expeditorul semnează tranzacția cu cheia sa privată
1. Tranzacția este transmisă în rețea
1. Nodurile o verifică și o adaugă în mempool-urile lor
1. Minerii o selectează pentru un bloc candidat
1. Minerii concurează prin Proof of Work
1. Un miner găsește un hash valid de bloc și transmite blocul
1. Nodurile verifică blocul și îl adaugă la blockchain
1. Tranzacția primește confirmări pe măsură ce se adaugă noi blocuri
1. Fă explicit punctul final:
1. odată ce tranzacția este inclusă într-un bloc valid, este confirmată
1. inputurile cheltuite nu mai pot fi folosite
1. destinatarul controlează acum noile UTXO-uri create de acea tranzacție

Diagrama de sinteză este deosebit de utilă aici, deoarece conectează vizual întregul proces de la semnarea în portofel la includerea de către miner, validarea de către noduri și distribuirea blocului.

###### Încheiere și verificare a înțelegerii

Încheie cu câteva întrebări rapide:

* Care este diferența dintre un nod și un miner?
* Ce este mempool-ul?
* De ce unele tranzacții se confirmă mai repede decât altele?
* Ce dovedește Proof of Work?
* De ce ajustează Bitcoin dificultatea minării?
* Care sunt pașii principali între trimiterea unei tranzacții și primirea confirmării?

#### Note pentru educatori

Păstrează firul principal al predării clar: nodurile verifică, minerii concurează, Proof of Work asigură securitatea, iar mempool-ul păstrează tranzacțiile valide până la confirmare.

Acest capitol poate părea tehnic, așa că folosește des analogii și diagrame.

Evită să prezinți minarea ca pe „crearea de bitcoin din nimic”. Fii precis că recompensa este stimulentul, iar procesul de minare asigură securitatea rețelei.

Cele mai importante puncte de prioritizat, dacă timpul este scurt, sunt:



1. Rolurile nodului vs minerului
1. Mempool ca sală de așteptare
1. Proof of Work
1. Ajustarea dificultății
1. Fluxul tranzacției de la semnare la confirmare

##### Cum arată o predare bună

* Este important să clarifici imediat că Mineri ≠ Noduri, să prezinți minarea ca activitate economică cu costuri reale de hardware și electricitate, să folosești ajustarea dificultății și Proof of Work pentru a explica mecanismul de securitate și să testezi înțelegerea cu scenarii despre schimbările din rețea.
* Educatorii ar trebui să folosească cifre reale pentru a ancora discuțiile, să fie extrem de clari și repetitivi despre distincția dintre Mineri și Noduri, să fie realiști în privința preocupărilor legate de centralizarea pool-urilor de minare și să respecte sofisticarea autentică implicată.
* Elevii înțeleg că minarea este realizată de oameni inteligenți care fac muncă complexă deoarece sunt recompensați cu Bitcoin, recunosc că stimulentele determină comportamentul onest pentru că profiturile minerilor depind de succesul My First Bitcoin, văd sistemul autoreglându-se prin ajustarea automată a dificultății, înțeleg că minarea este o afacere reală, nu caritate, și apreciază că securitatea My First Bitcoin costă electricitate și bani reali.
* Rezultatele învățării ar trebui să fie atinse dacă elevii pot distinge minerii care creează blocuri de nodurile care le validează, înțeleg Proof of Work ca un mecanism de securitate care face atacurile exponențial mai costisitoare, recunosc că ajustarea dificultății menține timpul de bloc la aproximativ 10 minute, înțeleg stimulentele minerilor legate de recompensele de bloc și comisioane, pot explica de ce un atac de 51% nu funcționează și văd minarea ca o activitate economică cu costuri și beneficii reale.

##### Gestionarea timpului

Dacă timpul este limitat, prioritizează:

* Rolurile nodurilor vs. minerilor (distincția esențială)
* Mempool ca sală de așteptare
* Mecanismul Proof of Work
* Ajustarea dificultății (sistem autoreglabil)
* Fluxul tranzacției de la semnare la confirmare

Dacă ești înainte cu timpul, acordă atenție:

* Economia minării și detalii despre hardware
* Dinamica pool-urilor de minare și preocupările privind centralizarea
* Scenarii de atac de 51% și de ce eșuează matematic
* Securitate pe termen lung prin alinierea stimulentelor

##### Dacă elevii întâmpină dificultăți

* Mineri vs. noduri (confuzie) → „Nodurile validează, minerii propun; arbitri vs. jucători.”
* Proof of Work risipitor → „Securitatea costisitoare previne atacurile; le face inutile.”
* Ajustarea dificultății → „Mai mulți mineri = blocuri mai rapide = dificultate crește; sistemul respiră.”
