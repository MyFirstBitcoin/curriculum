# 8.2 Metrice pentru analizarea registrului

Deoarece transparența Bitcoin este diferită de sistemele financiare tradiționale — unde mare parte din fluxul monetar are loc în spatele ușilor închise ale instituțiilor — aceasta dă naștere unui domeniu bogat de analize on-chain, unde datele la nivel de rețea devin o lentilă pentru a înțelege comportamentul utilizatorilor, fluxurile monetare și tendințele pe termen lung. Aceste metrici pot ajuta la răspunsul unor întrebări specifice, cum ar fi cât de activă este rețeaua, dacă monedele sunt acumulate sau vândute și dacă rețeaua devine mai sigură.

Înțelegerea acestor metrici este utilă nu doar pentru utilizatorii Bitcoin, ci și pentru cercetători sau factori de decizie care caută să obțină perspective asupra acestui sistem financiar unic prin transparența sa.

Această secțiune conține câteva metrici utilizate frecvent pentru analiza activității Bitcoin, grupate în subcategorii. Nu este o listă exhaustivă. Vizitează [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) pentru o listă mai completă și descrieri.



#### 8.2.1 Metrici ale adreselor

Metricile adreselor sunt utile pentru monitorizare în timp, deoarece indică nivelul de activitate pe rețeaua Bitcoin. De exemplu, pe măsură ce Bitcoin este adoptat mai larg, numărul adreselor active crește. Putem examina acest aspect mai detaliat distilând numărul de adrese care dețin o cantitate minimă specificată de Bitcoin, să zicem 0,1 BTC, într-o anumită perioadă, cum ar fi un an. Deși aceasta oferă o perspectivă asupra adopției Bitcoin în timp, este imperfectă deoarece o persoană poate deține mai multe adrese Bitcoin. Pe de altă parte, exchange-urile sau ETF-urile pot apărea ca entități unice atunci când dețin fonduri pentru un număr mare de persoane.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adrese care dețin Bitcoin > X BTC pe an. Sursa: Bitcoin Magazine Pro._

Comparând adresele cu prețul actual de piață al BTC, este posibil să vedem procentul total al adreselor Bitcoin care sunt pe profit. Acest lucru ne permite să urmărim sentimentul pieței, deoarece putem vedea ce proporție din piață păstrează BTC cu profit sau pierdere.

De exemplu, **Procent Profit Nerealizat** din graficul de mai jos arată proporția tuturor adreselor din registru cu un profit nerealizat măsurat în dolari americani. Observă că, deoarece graficul de mai jos a fost preluat aproape de maximul istoric al Bitcoin, procentul adreselor care arată un profit nerealizat este aproape de o sută la sută. De asemenea, putem vedea că perioadele prelungite cu Procent Profit Nerealizat sub o deviație standard față de medie sunt neobișnuite. Prin urmare, o scădere sub această linie poate sugera un moment bun de intrare pentru cumpărători.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Procent Profit Nerealizat. Sursa: checkonchain.com_



#### 8.2.2 Indicatori On-Chain

Indicatorii on-chain sunt utili deoarece oferă o perspectivă asupra comportamentului rețelei, dincolo de ceea ce pot arăta doar prețul și metricile adreselor. Ei ajută analiștii să înțeleagă acțiunile și sentimentul diferitelor tipuri de participanți, cum ar fi deținătorii pe termen lung versus traderii pe termen scurt, urmărind modul în care monedele sunt deținute, mutate sau evaluate în timp. Acești indicatori se bazează pe natura transparentă a registrului pentru a dezvălui dinamici ascunse ale pieței, precum acumularea, distribuția sau chiar convingerea investitorilor. Acest lucru îi face deosebit de utili pentru identificarea tendințelor structurale, evaluarea dacă piața este supraîncălzită sau subevaluată și anticiparea punctelor de cotitură într-un ciclu de piață.

De exemplu, examinând valoarea deținerilor de BTC de la ultima lor tranzacționare, putem deduce dacă piața este sau nu sub stres (așa cum ar putea fi în timpul unui minim major de ciclu). Această metrică este cunoscută sub numele de **Preț Realizat** și ne oferă un „cost mediu de bază” al tuturor BTC în circulație. Dacă prețul de piață scade sub Prețul Realizat, acest lucru arată că, în ansamblu, majoritatea adreselor înregistrează o pierdere pe hârtie.

Prin gruparea suplimentară a datelor din registru în benzi de vârstă, putem arăta cum cantitatea de BTC se mișcă între adrese în timp, ceea ce creează modele de tip valuri pe un grafic cunoscut sub numele de **valuri HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Valuri HODL Bitcoin. Sursa: Bitcoin Magazine Pro._

Valurile HODL arată ce fac deținătorii pe termen lung, mediu și scurt cu BTC-ul lor. De exemplu, în graficul de mai sus, deținătorii pe termen scurt sunt reprezentați cu roșu și portocaliu și putem vedea creșteri de activitate pe măsură ce acest grup se grăbește să cumpere aproape de vârfurile pieței. La celălalt capăt, putem observa că deținătorii pe termen foarte lung (cu violet și albastru) își cresc constant ponderea în rețea, indicând o convingere ridicată în rândul acestor grupuri. Graficul este imperfect deoarece unele monede pot fi mutate de la adrese vechi la adrese noi sub controlul aceluiași utilizator. Totuși, oferă o perspectivă interesantă asupra convingerii deținătorilor pe termen lung.

O altă modalitate de a examina „banii deștepți” ai deținătorilor pe termen lung este să analizăm **Coin Days Destroyed** (CDD). Conceptul de „Coin Days” reprezintă un multiplu al numărului de BTC înmulțit cu numărul de zile de la ultima mișcare a monedelor. De exemplu, 5 BTC care nu s-au mișcat timp de 100 de zile au acumulat 500 de coin days, iar 10 BTC care nu s-au mișcat timp de 10 zile au acumulat 100 de coin days. În acest fel, acordăm o pondere suplimentară monedelor deținute mai mult timp. Când aceste monede sunt mutate, acele coin days sunt „distruse”. Acest indicator arată creșteri ale CDD în perioadele cu mișcări semnificative de preț, oferind analiștilor o modalitate de a separa activitatea de piață de rutină de schimbările semnificative în sentimentul deținătorilor pe termen lung.

O altă metrică ce poate ajuta la identificarea dacă piața subevaluează sau supraevaluează BTC este raportul dintre Valoarea de Piață și Valoarea Realizată sau **MVRV**. Se calculează pur și simplu ca raportul dintre Valoarea de Piață (numărul de BTC în circulație înmulțit cu prețul de piață) și Valoarea Realizată (suma tuturor BTC de la ultima lor mișcare). Un MVRV ridicat sugerează că mai multe monede sunt pe profit (adesea văzut aproape de vârfurile pieței), iar un MVRV scăzut indică faptul că multe monede sunt deținute în pierdere (văzut aproape de minimele pieței).



#### 8.2.3 Metrici de Minare

Metricile de minare sunt utile pentru a înțelege securitatea, stimulentele economice și sănătatea generală a rețelei Bitcoin. Metrici precum hashrate-ul, veniturile minerilor, dificultatea și raporturile de taxe arată câtă putere de calcul securizează blockchain-ul și cât de bine sunt recompensați minerii pentru activitatea lor.

**Hashrate-ul** rețelei Bitcoin este poate cel mai des menționat indicator al sănătății rețelei și al nivelului de securitate. Deoarece procesul de minare securizează rețeaua și confirmă că tranzacțiile din registru sunt valide, cu cât există mai multă putere de calcul (sau hashing), cu atât ar fi mai dificil pentru un actor rău intenționat să depășească și să atace rețeaua.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate Bitcoin. Sursa: Bitcoin Magazine Pro._

Graficul de mai sus arată că, în mai 2025, puterea totală de calcul a rețelei este de aproximativ 900 TeraHash/s (900 de trilioane de calcule criptografice „hash” pe secundă). Dacă hashrate-ul crește, arată că rețeaua devine mai sigură, ceea ce este liniștitor pentru utilizatori.

Puell Multiple (conceput de David Puell) analizează ciclul de piață din perspectiva minerilor și a veniturilor acestora. Metrica se calculează împărțind emisia zilnică de BTC (în USD) la media mobilă pe 365 de zile a valorii emisiunii zilnice. Metrica ajută la identificarea perioadelor de stres sau relaxare pentru mineri. Istoric, un multiplu peste 3 a precedat o scădere a valorii de piață a BTC, deoarece indică faptul că minerii sunt foarte profitabili. O valoare sub 0,5 indică stres și a semnalat istoric minimele pieței pentru valoarea BTC.
