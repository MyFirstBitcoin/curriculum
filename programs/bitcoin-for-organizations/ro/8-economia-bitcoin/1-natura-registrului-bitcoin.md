# 8.1 Natura registrului Bitcoin

Registrul tranzacțiilor Bitcoin (numit alternativ timechain sau blockchain) este o evidență publică, cu marcaj temporal, a fiecărei tranzacții valide care a avut loc vreodată pe rețea. În sistemul financiar tradițional, tranzacțiile interne sunt vizibile doar pentru participanții autorizați, cum ar fi băncile, autoritățile de reglementare sau operatorii de date precum SWIFT, BACS sau SEPA. Accesul la datele de plată în sistemele tradiționale poate fi extrem de restricționat și costisitor.

Prin contrast, în rețeaua Bitcoin, oricine are o conexiune la internet poate vedea fiecare tranzacție, de la cele cu cea mai mare valoare până la fiecare Satoshi individual. Participanții pot urmări oferta totală de bitcoin în timp real, pot monitoriza activitatea adreselor și a portofelelor și pot vedea recompensele minerilor și comportamentul taxelor. Deși activitatea vizibilă pe registru este legată de adresele de chei publice și nu de identități individuale, este posibilă agregarea unor seturi mari de date despre comportamentul de cheltuire, permițând oricui să colecteze și să cerceteze activitatea economică în timp real. Pe măsură ce rețeaua crește și devine tot mai acceptată ca sursă de adevăr economic, este posibil să vedem o dependență mai mică de organismele guvernamentale și de furnizorii terți pentru producerea de analize statistice și rapoarte despre comportamentul de cheltuire.



#### 8.1.1 Noduri și Exploratoare de Blocuri

Oricine dorește să verifice independent registrul Bitcoin și să acceseze datele sale ar trebui să ruleze un nod complet. Nodul complet este adesea descris ca fiind cea mai fundamentală modalitate de a participa și de a verifica economia Bitcoin. Este disponibil la nivel global ca software open-source care, odată executat, va descărca și valida întregul registru Bitcoin începând cu „Blocul Genesis”, publicat în ianuarie 2009, până în prezent. De asemenea, sprijină securitatea rețelei Bitcoin prin ajutarea la verificarea noilor tranzacții adăugate în registru. Accesând registrul Bitcoin în acest mod, nodul complet servește drept sursă de adevăr pentru cercetătorii și auditorii rețelei. Iar pentru utilizatorii Bitcoin, nodul complet acționează ca o poartă „auto-suverană” către informațiile tranzacționale ale economiei Bitcoin, deoarece sporește confidențialitatea și securitatea prin eliminarea dependenței de servicii terțe.

În timp ce nodurile complete descarcă datele brute, exploratoarele de blocuri precum mempool.space sau blockstream.info oferă o interfață vizuală pentru a căuta și interpreta activitatea din registru. Exploratorul de blocuri permite urmărirea tranzacțiilor individuale și vizualizarea soldurilor și istoricului portofelelor. De asemenea, afișează metrici despre activitatea minerilor, cum ar fi recompensele de bloc și datele despre taxele de tranzacție.

Împreună, nodurile complete și exploratoarele de blocuri sunt instrumentele care fac utilizabilă transparența rețelei Bitcoin.



#### 8.1.2 Activitate: Explorarea Registrului Bitcoin

1. Deschide [mempool.space](https://mempool.space) și explorează pagina principală.
  * Care este înălțimea celui mai recent bloc?
  * Care este taxa de tranzacție curentă (Prioritate scăzută, medie și ridicată)?
  * Câte tranzacții așteaptă în mempool pentru următorul bloc?
1. Accesează cel mai recent bloc din registru.
  * Câte tranzacții au fost incluse?
  * Cum se numește minerul blocului?
  * Care a fost recompensa de bloc?
1. Accesează o tranzacție din bloc.
  * Câte intrări și ieșiri are tranzacția?
  * Care este valoarea tranzacției în BTC și USD?

Discută diferențele dintre modul în care circulă banii în sistemul tradițional și modul în care o afacere sau un guvern utilizează acest tip de transparență.
