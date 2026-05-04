# 9.1 Noduri și mineri Bitcoin

Nodurile Bitcoin pot părea tehnice, dar sunt pur și simplu programe care păstrează o copie a blockchain-ului Bitcoin pe un calculator. Blockchain-ul este o evidență comună a tuturor tranzacțiilor Bitcoin.

Când rulezi propriul tău nod, verifici singur tranzacțiile Bitcoin, în loc să ai încredere în altcineva. Acest lucru îți oferă mai multă independență și ajută la menținerea descentralizării rețelei Bitcoin.

Poți să te gândești la un nod Bitcoin ca la un agent de circulație digital cu câteva sarcini importante.

1. Păstrează o copie a blockchain-ului, care este istoricul tuturor tranzacțiilor Bitcoin.
1. Nodurile se conectează cu alte noduri din întreaga lume și împărtășesc informații. Un exemplu este lista tranzacțiilor noi care așteaptă să fie confirmate, numită mempool.
1. Nodurile verifică dacă fiecare tranzacție respectă regulile Bitcoin. Dacă o tranzacție este invalidă, nodul o respinge.

Nodurile ajută, de asemenea, nodurile noi să se alăture rețelei, împărtășindu-le blockchain-ul. Totuși, fiecare nod nou verifică independent toate regulile.

Oricine poate rula un nod instalând un program precum Bitcoin Core și descărcând blockchain-ul. Odată ce este configurat, nodul continuă să primească blocuri noi aproximativ la fiecare 10 minute și le verifică înainte de a le adăuga la copia sa de blockchain.

Rularea unui nod ajută la creșterea securității și descentralizării rețelei Bitcoin, deoarece mai mulți oameni verifică independent sistemul.

#### Ce este un nod Bitcoin?

> Scopul mineritului nu este crearea de noi bitcoin; acesta este sistemul de stimulente. Mineritul este mecanismul prin care securitatea Bitcoin este descentralizată.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Minerii colectează tranzacțiile neconfirmate, formează un bloc și folosesc energie pentru a găsi o cheie care adaugă și securizează blocul.


Minerii concurează pentru a adăuga următorul bloc de tranzacții la blockchain. Pentru a face acest lucru, trebuie să găsească un număr special care creează un hash valid al blocului. Îți poți imagina acest proces ca pe o căutare a cheii potrivite printre miliarde de posibilități. Primul miner care găsește hash-ul corect câștigă cursa și obține dreptul de a adăuga blocul său la blockchain.

Când un miner găsește un hash valid, își împărtășește blocul cu rețeaua. Alți mineri verifică rapid dacă soluția este corectă. Dacă este, blocul este adăugat la blockchain, ajutând la menținerea securității registrului public Bitcoin.

Minerii câștigă bitcoin în două moduri:

* **Recompense de bloc:** Noi bitcoin sunt creați și oferiți minerului care adaugă cu succes un bloc la blockchain.
* **Comisioane de tranzacție:** Când oamenii trimit bitcoin, includ un mic comision. Minerul care adaugă blocul primește comisioanele din tranzacțiile incluse în acel bloc.

#### Înjumătățirile Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Recompensele minerilor pentru completarea unui bloc se înjumătățesc la fiecare 210.000 de blocuri, aproximativ la fiecare patru ani.


Bitcoin are o limită maximă fixă de 21.000.000 de bitcoin, dar nu toți au fost creați când a început Bitcoin. În schimb, noi bitcoin sunt introduși treptat în circulație prin **minerit**.

Când minerii adaugă cu succes un nou bloc de tranzacții la rețeaua Bitcoin, primesc o **recompensă de bloc** în bitcoin. În primele zile ale Bitcoin, această recompensă era de 50 de bitcoin pe bloc. Această recompensă a încurajat oamenii să folosească putere de calcul și electricitate pentru a ajuta la securizarea rețelei.

Aproximativ la fiecare 210.000 de blocuri (cam la fiecare 4 ani), recompensa de bloc se înjumătățește. Acest eveniment se numește **înjumătățire**. Înjumătățirea încetinește crearea de noi bitcoin și ajută la asigurarea faptului că oferta totală nu va depăși niciodată 21 de milioane. În timp, acest lucru face ca bitcoin să fie din ce în ce mai rar.


> **Definition – Ofertă în circulație**
>
> **Ofertă în circulație** se referă la cantitatea totală disponibilă a unei monede. În cazul Bitcoin, oferta totală în circulație este numărul de monede care au fost minate și sunt în circulație la un moment dat.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/01f14432e83e6ce2aa6680496cbbc05c25967096-292x200.svg)


> **Definition – Programul de emisie Bitcoin**
>
> Programul de emisie **Bitcoin** este planul prestabilit și public pentru eliberarea de noi bitcoin în circulație, conceput pentru a menține raritatea Bitcoin în timp.


După fiecare eveniment de înjumătățire, recompensa în bitcoin pe care minerii o primesc pentru adăugarea unui bloc se reduce la jumătate. Acest lucru reduce ritmul în care sunt creați noi bitcoin.

Minerii câștigă în continuare comisioane de tranzacție din tranzacțiile incluse în blocul pe care îl minează. În timp, se așteaptă ca aceste comisioane să devină o parte mai importantă din veniturile minerilor.

Halving-urile sunt integrate în protocolul Bitcoin și au loc automat aproximativ la fiecare patru ani. Din acest motiv, programul de emisie al Bitcoin este previzibil și transparent.

Tabelul arată următoarele halving-uri, inclusiv data aproximativă, numărul blocului la care au loc, noua recompensă pe bloc și procentul din totalul de bitcoin care va fi minat.


| Eveniment | Data | Bloc | Recompensă | Minat |
| --- | --- | --- | --- | --- |
| Al 5-lea Halving | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| Al 6-lea Halving | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| Al 7-lea Halving | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Pe măsură ce mai mulți bitcoin sunt minați, oferta aflată în circulație continuă să crească până când se atinge oferta maximă de 21.000.000 de bitcoin, ceea ce este estimat să se întâmple în jurul anului 2140. Deoarece tot mai puțini bitcoin noi sunt creați în timp, dacă cererea crește, prețul Bitcoin poate să crească. Acest lucru îi motivează și pe mineri să continue să securizeze rețeaua prin contribuția cu puterea lor de calcul.

#### Ce este un hash valid de bloc în Bitcoin?

În Bitcoin, minerii concurează pentru a găsi un cod special numit **hash de bloc**. Acest cod identifică un bloc de tranzacții și permite adăugarea lui în blockchain.

Fiecare bloc conține informații despre tranzacțiile recente și include și hash-ul blocului anterior. Acest lucru leagă fiecare bloc între ele, formând un lanț de la primul bloc (Genesis Block) până la cel mai recent.

Un hash funcționează ca o **amprentă digitală** pentru datele din bloc. Dacă orice informație din bloc ar fi schimbată, amprenta s-ar schimba și ea. Acest lucru face ușor pentru oricine să verifice că istoricul tranzacțiilor din blockchain nu a fost modificat și ajută la menținerea securității rețelei.


> **Callout**
>
> Satoshi Nakamoto, creatorul Bitcoin, a minat Genesis Block, care a deblocat un total de 50 de bitcoin.


#### Cursa pentru a mina un bloc

Minerii concurează pentru a găsi un hash valid de bloc. Primul miner care găsește unul are dreptul să adauge noul bloc în blockchain și să primească o recompensă în bitcoin.

Pentru a fi valid, hash-ul blocului trebuie să fie mai mic decât un număr stabilit de rețea, numit ținta de dificultate. Deoarece hash-urile sunt aleatorii, minerii trebuie să încerce diferite intrări până găsesc una care funcționează.

Dacă prea mulți mineri concurează, blocurile ar fi găsite prea repede. Dacă prea puțini mineri participă, blocurile ar dura prea mult să fie găsite. Pentru a menține sistemul să funcționeze lin, Bitcoin ajustează automat dificultatea la fiecare 2.016 blocuri (aproximativ la fiecare două săptămâni).

Această ajustare asigură că, în medie, un bloc nou este adăugat în blockchain la fiecare 10 minute.


> **Definition – Definiția nivelului de dificultate**
>
> Nivelul de **dificultate** în mineritul Bitcoin măsoară cât de greu este să găsești un hash valid de bloc. Rețeaua ajustează această dificultate la fiecare 2.016 blocuri (aproximativ la fiecare două săptămâni) astfel încât blocuri noi să fie adăugate în blockchain la fiecare 10 minute. Cu cât dificultatea este mai mare, cu atât este mai greu pentru mineri să găsească un bloc valid.


Prin găsirea unui hash valid de bloc, un miner dovedește că a efectuat munca necesară pentru a adăuga un bloc nou în blockchain. Acest proces se numește **Proof of Work** (PoW). Este mecanismul de securitate care permite Bitcoin să confirme tranzacțiile și să adauge blocuri noi în blockchain. Minerul care găsește primul hash valid câștigă o recompensă în bitcoin, care include recompensa de bloc și taxele de tranzacție din tranzacțiile incluse în acel bloc.

Proof of Work (PoW) ajută la menținerea securității Bitcoin, făcând extrem de costisitor pentru oricine să încerce să trișeze sau să preia controlul asupra rețelei. În schimb, este mult mai profitabil să respecți regulile.

Minerii au patru roluri principale:

1. **Colectează tranzacții**: Minerii aleg tranzacțiile care au fost trimise în rețea și le plasează într-un bloc candidat.
1. **Efectuează Proof of Work**: Minerii concurează pentru a rezolva o problemă matematică dificilă, găsind un hash valid de bloc.
1. **Transmite blocul**: Primul miner care găsește o soluție validă partajează noul bloc cu rețeaua.
1. **Câștigă recompense**: Dacă blocul este valid, acesta este adăugat la blockchain, iar minerul primește bitcoin nou creați plus taxele de tranzacție.

Mulți mineri din întreaga lume încearcă să creeze următorul bloc în același timp. Când un miner găsește o soluție validă, rețeaua verifică blocul. Dacă totul este corect, acesta este adăugat la blockchain. Alte blocuri concurente sunt eliminate. Acest proces menține rețeaua în consens și previne dubla cheltuire.

* Minerii sunt calculatoare care ajută la menținerea și actualizarea registrului My First Bitcoin.
* Ei colectează tranzacții și le grupează într-un bloc. Apoi rulează datele blocului printr-un algoritm de hash pentru a crea un cod unic numit hash.
* Minerii repetă acest proces de multe ori, căutând un hash care să respecte regulile My First Bitcoin. Primul miner care găsește un hash valid primește bitcoin nou creați ca recompensă, iar blocul său este adăugat la blockchain.
* Hash-ul fiecărui bloc îl conectează și la blocul anterior. Dacă cineva ar încerca să modifice o tranzacție din trecut, hash-urile nu s-ar mai potrivi, iar rețeaua ar respinge lanțul modificat. Acesta este motivul pentru care registrul My First Bitcoin este sigur.
