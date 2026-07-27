# 2.3 Bitcoin este prea lent pentru a fi o monedă globală

> Vizionarii văd un viitor cu angajați care lucrează de la distanță, biblioteci interactive și săli de clasă multimedia. Ei vorbesc despre adunări publice electronice și comunități virtuale... Adevărul este că nicio bază de date online nu va înlocui ziarul tău zilnic, niciun CD-ROM nu poate lua locul unui profesor competent și nicio rețea de calculatoare nu va schimba modul în care funcționează guvernul.  
_Clifford Stroll_

17 ani mai târziu, Newsweek a încetat publicarea tipărită și a devenit disponibil exclusiv online. Imaginează-ți cum era să fii în viață în 1974, când a fost creat pentru prima dată Protocolul de Control al Transmisiunii (TCP).

Nimeni nu a prevăzut smartphone-ul, cu toate aplicațiile sale, ținut în mână. Nimeni nu a anticipat sistemul de navigație prin satelit din mașina ta.

Internetul nu a apărut dintr-o dată, ci treptat, ca o evoluție a protocoalelor și a straturilor. Aceste evoluții s-au construit pe TCP, dar în mare parte nu l-au schimbat.

> Așadar, privind către tranziția către platformele de comunicare ale viitorului, văd că frumusețea protocoalelor Internet constă în separarea straturilor dintre serviciu și tehnologie.  
_Michael K Powell_



##### Compară evoluția Bitcoin cu cea a internetului

TCP a fost necesar, dar nu suficient pentru apariția tuturor celorlalte lucruri pe internet. Evoluția Bitcoin pare să urmeze o cale similară. Sistemele deschise par să fie mai rezistente și mai de succes atunci când sunt dezvoltate în straturi, deși poate trece mult timp între punerea bazelor inițiale și adoptarea pe scară largă. Soluțiile „all in one” nu par să fie la fel de eficiente în sistemele deschise precum cele construite în straturi pe protocoale. Așa cum nimeni nu a trebuit să reconstruiască internetul pentru că filmele nu puteau fi transmise prin TCP, la fel este probabil să fie și cu Bitcoin.

Există deja o serie de protocoale de nivel 2 care funcționează peste Bitcoin, și multe aplicații care rulează peste aceste protocoale de nivel 2 (vezi secțiunea 201.4 pentru mai multe detalii despre acestea).

În loc să te concentrezi pe ceea ce bitcoin și rețeaua Bitcoin nu pot face astăzi, gândește-te la ceea ce deja se poate face astăzi și compară cu ce putea face acum 10 ani. Fă acest exercițiu cu internetul din 1985 până în 1995, apoi privește cât de rapid a evoluat internetul în următorii 30 de ani și ce aplicații au devenit posibile. Folosește această perspectivă pentru a proiecta Bitcoin în viitor și imaginează-ți cum ar putea arăta peste încă 10 ani, sau 30 dacă imaginația ta poate merge atât de departe.



##### Compară Bitcoin cu sistemul monetar global existent

Afirmația centrală că Bitcoin este prea lent pentru a fi bani globali este, probabil, adevărată dacă ar trebui să ne limităm la stratul de bază al Bitcoin. Este de asemenea adevărat că stratul de bază al sistemelor noastre monetare existente este prea lent pentru a fi bani globali, dacă o restricție similară ar însemna că nu există infrastructură de plăți construită peste el de către băncile private și serviciile de plăți precum Visa și Mastercard. Sistemul nostru actual este construit în straturi, deci ne-am putea aștepta ca viitorul să arate similar. Unele compromisuri de proiectare, precum cele dintre încredere, viteză și cost, pot fi transferate între sisteme care oferă aceleași soluții, chiar dacă sunt construite pentru a transfera diferite tipuri de valoare.

Unele dintre protocoalele de nivel 2 existente pe Bitcoin abordează direct problema vitezei, de exemplu Liquid și Lightning Network (vezi secțiunea 201.4 pentru mai multe detalii). Liquid este mai rapid și mai ieftin decât blockchain-ul Bitcoin, iar Lightning Network este chiar mai rapid și mai ieftin decât Liquid. O proliferare a protocoalelor de nivel 2, fiecare cu compromisuri diferite, este de așteptat și este sănătoasă.

Probabil vor apărea mai multe straturi 2 și 3 și o explozie de aplicații care le folosesc, exact cum s-a întâmplat cu evoluția internetului.



##### Motivație

Când apare această critică, merită să te întrebi dacă persoana care critică are alte motivații. De exemplu, are un proiect blockchain nou sau diferit? Acest lucru poate fi similar cu încercarea de a vinde un Protocol de Control al Transmisiunii mai bun.

Trilema Scalabilității, sau a Blockchain-ului, a fost ridicată pentru prima dată de Vitalik Buterin în 2017. Ea spune că există întotdeauna un compromis în proiectarea blockchain-ului între proprietățile de Descentralizare, Securitate și Scalabilitate. Oricine ridică critica că Bitcoin este prea lent și că are o soluție mai rapidă într-un blockchain de nivel 1 va sacrifica o parte din securitate sau descentralizare pentru a o obține. Deși un astfel de compromis pentru un blockchain proiectat pentru alte utilizări poate avea sens, ordinea de prioritate pentru bani globali trebuie să fie:


> **Light**
>
> * **Descentralizare**
>   * Face posibilă eliminarea părților de încredere
> * **Securitate**
>   * Împiedică actorii rău intenționați să modifice tranzacțiile sau registrul
> * **Scalabilitate**
>   * Permite sistemului să se extindă economic în utilizatori și viteză


Primele două caracteristici creează mediul pentru emitere fără creatori, plăți fără intermediari și custodie fără administratori.

Bitcoin face alegerea corectă între cele trei caracteristici de proiectare a blockchain-ului, având în vedere că scopul său țintă este să fie bani globali, și atenuează compromisurile de scalabilitate și viteză folosind straturi.

> Satoshi a descoperit cum să protejeze integritatea banilor digitali fără părți de încredere – nu sunt necesari creatori, intermediari sau administratori.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
