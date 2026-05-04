# 7.1 Rețeaua Lightning

Lightning Network este un sistem de plată care permite utilizatorilor să trimită și să primească bitcoin rapid și ieftin. Funcționează prin crearea unui portofel comun unde ambele părți depozitează o parte din bitcoin-ul lor. Astfel, pot efectua un număr nelimitat de tranzacții între ele, fără a fi nevoie să înregistreze fiecare tranzacție pe blockchain-ul principal. Procedând astfel, evită necesitatea de a verifica și include fiecare tranzacție într-un bloc, ceea ce face procesul atât rapid, cât și eficient din punct de vedere al costurilor. Taxele mai mici înseamnă că Lightning Network poate fi folosit pentru plăți mici, care nu sunt întotdeauna viabile pe lanț. Odată ce părțile decid să încheie colaborarea, doar soldul final este înregistrat pe blockchain.

Imaginează-ți o zi de lucru într-o cafenea. Plănuind să stai mai mult, deschizi o notă de plată și plătești în avans, în loc să plătești pentru fiecare comandă. La sfârșitul zilei, tu și proprietarul verificați nota pentru a achita suma datorată. Dacă depozitul tău este mai mare decât ai cheltuit, primești diferența înapoi; dacă ai cheltuit mai mult, plătești ce mai datorezi.

Această schemă poate fi extinsă pentru a include mai mulți participanți. De exemplu, la una dintre vizitele tale la cafenea, aduci un prieten pe care barmanul nu îl cunoaște și nu îi poate deschide o notă de plată. Îi oferi prietenului tău acces la nota ta pentru a-i acoperi cheltuielile și sunteți de acord că îți va returna banii în privat. Acum imaginează-ți mii de oameni făcând același lucru simultan, permițând altora să folosească note de plată existente pentru a se conecta cu și mai mulți indivizi — așa funcționează Lightning Network!

Cu Lightning, poți face plăți către oricine din rețea, nu doar către persoana cu care ai o notă de plată directă — atâta timp cât se poate găsi o rută între cele două părți. Plata ta poate naviga prin rețea până ajunge la destinație, chiar dacă nu ai un canal deschis direct cu destinatarul.

Să aruncăm o privire la diferența dintre tranzacțiile on-chain și off-chain.

##### Tranzacții On-Chain

Acestea sunt tranzacții care au loc direct pe blockchain-ul Bitcoin. Confirmarea lor durează aproximativ 10 minute, iar taxele depind de dimensiunea tranzacției în bytes virtuali. Sunt mai sigure, dar mai lente, deoarece necesită consensul rețelei.

##### Tranzacții Lightning Network

Aceste tranzacții au loc pe o rețea separată construită deasupra blockchain-ului Bitcoin. Se finalizează mai rapid și cu taxe mai mici. Sunt folosite în special acolo unde contează mai mult viteza și costul tranzacțiilor. Comparativ cu tranzacțiile on-chain, sunt mai puțin sigure.


|  | Rețeaua Bitcoin | Lightning Network |
| --- | --- | --- |
| Definiție | O rețea digitală descentralizată care folosește criptografia pentru a securiza tranzacțiile financiare. | Un protocol de plată de tip second layer care funcționează deasupra blockchain-ului Bitcoin, permițând tranzacții mai rapide și mai ieftine. |
| Avantaje | Descentralizată și sigură. Fără returnări de plată sau fraudă. Poate fi folosită pseudonim. Acceptare globală. | Tranzacții mai rapide și mai ieftine. Scalabilitate crescută. Tranzacțiile off-chain nu aglomerează blockchain-ul. |
| Dezavantaje | Timp de procesare lent pentru tranzacții. Taxe ridicate pentru anumite tipuri de tranzacții. Complex pentru începători. | Poate necesita încredere în operatorii canalelor. Necesită tranzacție on-chain pentru deschiderea și închiderea canalelor. |
