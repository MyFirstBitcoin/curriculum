# 2.7 Bitcoin nu este cu adevărat descentralizat

> Complexitatea criptomonedelor provine din încercările de descentralizare—prin distribuirea puterii și a guvernanței în sistem, teoretic nu mai este nevoie de intermediari de încredere precum instituțiile financiare. Aceasta a fost premisa inițială a white paper-ului Bitcoin, care a oferit o soluție criptografică menită să permită trimiterea plăților fără implicarea vreunei instituții financiare sau a altui intermediar de încredere. Totuși, Bitcoin a devenit centralizat foarte rapid și acum depinde de un grup restrâns de dezvoltatori de software și de pool-uri de minare pentru a funcționa.  
_Fondul Monetar Internațional_

Așa cum arată citatul de mai sus dintr-o postare relativ recentă a Fondului Monetar Internațional, industria financiară tradițională continuă să susțină că Bitcoin nu este descentralizat și, de asemenea, confundă Bitcoin cu alte active cripto.

##### Introducere

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/2597a45d669edc1831523806e7070773016e52f0-161x167.svg)

Descentralizarea este un aspect esențial al Bitcoin. Capacitatea de a menține regulile protocolului, precum raritatea și distribuția, fără o autoritate centrală, asigură că poate funcționa ca bani fără permisiune pentru o societate globală.

Așa cum a menționat Satoshi în corespondența sa online, serviciile descentralizate precum BitTorrent „rezistau” împotriva represiunilor guvernamentale, în comparație cu serviciile cu proprietar(i) identificați și servere centralizate. Era clar îngrijorat de riscul potențial ca guvernele sau alte interese să închidă sau să afecteze negativ Bitcoin.

În acest context, ne interesează descentralizarea:

* Dezvoltarea și gestionarea codului care rulează protocolul; cine are voie să schimbe regulile?
* Funcția de minare care creează noi blocuri în conformitate cu regulile și validează împotriva dublei cheltuieli
* Node-urile care validează tranzacțiile pentru validitate și păstrează o copie a blockchain-ului

##### Dezvoltatori

Bitcoin este un protocol open-source pe care oricine îl poate examina, descărca, copia sau propune modificări. Este disponibil într-o bibliotecă GitHub, codul sursă fiind lansat inițial în 2009 de Satoshi Nakamoto. Oricine este liber să descarce codul și să ruleze un nod, majoritatea folosind software-ul original Bitcoin Core, care a fost actualizat de-a lungul timpului.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Sursa: https://river.com/learn/what-is-bitcoin-core/_

Dezvoltarea Bitcoin Core urmează cele mai bune practici ale dezvoltării open source. În orice moment, pot exista oricâți dezvoltatori care scriu sau revizuiesc modificări de cod. Ei trebuie să asculte preocupările operatorilor de noduri și ale minerilor, precum și ale utilizatorilor, înainte de a face orice schimbare critică în cod, care va fi revizuită și aprobată, așa cum se arată în diagrama de mai sus, înainte de a fi integrată în cod.

Regulile Bitcoin sunt apoi codificate în acest software Bitcoin Core, care rulează pe fiecare nod. Oricine poate propune o schimbare a regulilor – regulile sunt cod, dar nu sunt_doar_cod, ele sunt_cod convenit_de comun acord. Dacă sunt schimbate unilateral, noul cod nu mai face parte din consens și nu mai face parte din Bitcoin. Schimbarea a ceva la Bitcoin și menținerea consensului este dificilă. Modificările propuse la cod se încadrează într-una din trei categorii:

* În cadrul regulilor existente: Upgrade-uri minore precum corectarea greșelilor de ortografie, o interfață mai plăcută sau gestionarea datelor pot intra în această categorie și sunt relativ ușor de aprobat.
* Adăugarea unei noi reguli care adaugă restricții regulilor – cum ar fi reducerea dimensiunii blocului. Aceasta este denumită „soft fork”. Nodurile care aleg să nu implementeze schimbarea de cod și rămân pe versiunea veche vor putea totuși să participe la rețea.
* Adăugarea unei noi reguli care încalcă regulile actuale, de exemplu o creștere a dimensiunii blocului. Nodurile care nu fac upgrade la noul cod vor respinge un bloc creat cu dimensiune mai mare ca fiind invalid. Aceasta este denumită „hard fork” și va crea o scindare a lanțului între nodurile care rulează codul original și cele cu noul cod, creând o monedă nouă. Acest lucru s-a întâmplat anterior, dar nu a dus la succes pe termen lung pentru noua monedă, deoarece majoritatea nodurilor au decis să păstreze codul original.

Prin urmare, o singură parte sau un grup de persoane nu poate schimba unilateral codul Bitcoin fără a obține un acord de consens, altfel riscă o scindare a lanțului și crearea unei noi monede care urmează un set diferit de reguli.

##### Minare

Funcția de minare validează tranzacțiile la fel ca orice alt nod din rețea, dar apoi consumă energia necesară pentru a crea un nou bloc care respectă regulile de consens din cod. Succesul permite minerului să obțină recompense sub formă de comisioane de tranzacție și recompense Bitcoin (la momentul scrierii, 3,125 monede pe bloc).

Minarea este realizată de obicei de „pool-uri” de minare, unde oamenii își consolidează puterea de minare sau rata de hash pentru a crește șansele de a mina cu succes un bloc și de a împărți recompensele. Există riscul ca unul sau mai multe dintre aceste pool-uri de minare să se combine pentru a atinge o dominanță de 51% în minare și, practic, să anuleze protocolul de validare al rețelei în favoarea lor pentru a cheltui dublu monedele. Acest lucru ar necesita resurse uriașe la un cost foarte mare, iar minerii individuali pot foarte ușor să se mute la un alt pool de minare oricând. Un astfel de atac ar duce probabil și la prăbușirea valorii bitcoin, deoarece ar fi evident că integritatea rețelei a fost compromisă. Un atacator ar trebui, așadar, să convertească rapid orice bitcoin obținut în fiat înainte ca valoarea să se erodeze. Acest lucru ar face și mai dificilă menținerea unui atac pe termen lung și, prin urmare, este mai profitabil pentru un miner sau un operator de pool să respecte regulile și să încerce să mineze blocuri valide.

Distribuția geografică a funcției de minare este de asemenea importantă pentru a evita, de exemplu, ca guvernele să preia capacitatea de minare sau să o închidă. De exemplu, o interdicție recentă asupra minării impusă de China a demonstrat capacitatea Bitcoin de a se adapta și de a supraviețui unei astfel de intervenții guvernamentale, adaptându-se și recuperându-se rapid după pierderea rezultată a puterii de hash.

##### Node-uri

Spre deosebire de minare, care necesită o investiție financiară semnificativă pentru a concura eficient în cursa pentru noi blocuri, sau de dezvoltarea de cod care necesită expertiză în programare, rularea unui nod este ceva ce oricine interesat să ajute la menținerea descentralizării Bitcoin poate face.

Node-urile rulează software-ul Bitcoin Core și aplică regulile incluse în cod pentru a se asigura că minerii nu trișează, de exemplu alocându-și o recompensă de bloc mai mare decât este permis. Ele aplică și plafonul de 21 de milioane de monede, care este esențial pentru menținerea rarității Bitcoin. Pentru ca un guvern sau un actor rău intenționat să oprească Bitcoin, ar trebui să distrugă fiecare copie a blockchain-ului, care rulează în prezent pe mii de noduri distribuite la nivel global, o sarcină aproape imposibilă.

##### Oameni

Un alt aspect al potențialei centralizări este cel al oamenilor. Orice alt „alt-coin” are un lider—cineva care ar putea fi constrâns să susțină schimbări care nu sunt în interesul Bitcoin. Satoshi Nakamoto a rămas suficient de mult timp pentru a se asigura că Bitcoin este pe drumul cel bun înainte de a dispărea definitiv, lăsându-l în mâinile altora pentru a îmbunătăți și adapta software-ul.

Ce se întâmplă cu deținătorii unor cantități mari de Bitcoin? Investitorii timpurii, care și-au păstrat monedele și nu le-au pierdut, sunt extrem de bogați în acest moment. Este important de menționat că acest lucru poate fi adevărat, dar nu le oferă mai multă influență asupra sistemului decât oricui altcuiva, spre deosebire de monedele „proof of stake”, unde primii adoptați, deja bogați în acea monedă, obțin avantaje în luarea deciziilor și în distribuția viitoarelor monede. Acest lucru a dus sau va duce inevitabil la centralizare în timp.

##### Concluzie

Care sunt amenințările potențiale pe care descentralizarea le poate încerca să le atenueze?

* Guvernul interzice sau închide Bitcoin
* Schimbări nedorite ale codului care favorizează un anumit set de interese în Bitcoin, de exemplu creșterea recompensei de bloc
* Constrângerea protocolului de către guvern sau actori rău intenționați pentru a influența direcția protocolului
* Posibilitatea ca un pool de mineri să preia rețeaua și să „cheltuiască dublu” Bitcoin – un atac de 51%

După cum putem vedea, combinația dintre noduri, dezvoltatori de cod și mineri, precum și utilizarea mecanismului „proof of work”, descentralizează Bitcoin la un nivel suficient încât aceste amenințări potențiale nu sunt considerate a fi de mare îngrijorare. Comunitatea va trebui să continue să monitorizeze situația pentru a se asigura că acest lucru rămâne valabil.
