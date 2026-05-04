# 3.7 Bitcoin

După mulți ani și încercări eșuate, Cypherpunks, în mare parte, își pierduseră interesul pentru ideea unei monede digitale fără permisiune, când Adam Back a primit un e-mail cu un link către un draft de white paper intitulat „electronic cash without a third party” de la o persoană anonimă care se prezenta drept Satoshi Nakamoto.

Pentru a recapitula până în acest punct, avem cel puțin următoarele idei:

* Semnături criptografice care pot oferi un anumit nivel de confidențialitate și anonimat
* Conceptul unei monede fără acoperire (B-Money)
* Propuneri (dar fără mijloace) pentru limitarea emisiunii de monedă nouă
* Monede digitale a căror proprietate era atribuită prin chei publice (B-Money) și care puteau fi transferate prin semnare și realocate pe baza adresei destinatarului (RPOW și Hashcash)
* Toate nodurile mențin o copie a unui registru complet distribuit (B-Money) (respins la acea vreme ca fiind nepractic)
* Protocol de marcare temporală – folosind hashing Merkle tree pentru a oferi o cronologie matematic demonstrabilă a evenimentelor, dificil de falsificat dacă toți utilizatorii păstrează aceleași înregistrări
* Proof of work pentru a lega efortul din lumea reală de sistem (dar folosind hash-ul însuși ca monedă)
* Rețele complet descentralizate în care toți participanții sunt egali și pot intra sau ieși din rețea (BitTorrent)
* Conceptul de a lega hash-urile noi de hash-urile anterioare (Bit Gold și marcare temporală)

Ce lipsea în acel moment includea:

* O soluție viabilă pentru a rezolva problema „generalilor bizantini”
* O metodă de a limita cantitatea de bani în circulație în ciuda îmbunătățirilor continue ale hardware-ului
* Un sistem de stimulente pentru ca oamenii să participe (problema oului și a găinii)

Cealaltă diferență majoră între încercările recente și Bitcoin a fost că Satoshi lucrase la cod de ceva timp, în adevăratul spirit original „Cypherpunks write code”, înainte de a-l anunța pe listele de discuții, spre deosebire de Bit Gold și B-Money care erau mai degrabă concepte.

Care a fost inovația care a diferențiat Bitcoin de încercările anterioare de monedă electronică?

Proof of work urma să fie folosit ca mecanism de consens și ca metodă de a oferi securitate și imuabilitate: În loc să folosească hash-ul ca formă de bani, acesta urma să fie folosit printr-un nou proces conceptual numit mining, unde un nod adună un set de tranzacții, adaugă un număr aleatoriu și apoi aplică hashing-ul pe „blocul” de date. Un bloc valid care îndeplinea cerința de hash era apoi anunțat rețelei. Aceste blocuri erau legate între ele folosind hash-ul blocului anterior, iar cel mai lung blockchain era folosit în caz de egalitate, când noduri diferite validau și anunțau blocuri diferite simultan, creând ramuri ale lanțului. Proof of work a devenit metoda distribuită de departajare pentru a rezolva problema generalilor bizantini.

Acești mineri au primit și un stimulent pentru a furniza puterea de procesare necesară pentru proof-of-work, fiind recompensați cu bitcoin nou pentru fiecare bloc. Cantitatea de Bitcoin acordată este programată să scadă aproximativ la fiecare 4 ani până când tot Bitcoin-ul va fi creat, stabilind astfel o limită fixă pentru totalul de Bitcoin care va exista vreodată în circulație, de 21 de milioane.

Cea mai originală idee a fost modul în care a rezolvat problema cantității de bani creați pe măsură ce hardware-ul se îmbunătățește și se poate aplica mai multă putere rețelei. Timpul mediu pentru un anumit număr de blocuri (2016) era calculat, iar dacă blocurile erau create prea repede, hash-ul necesar pentru a crea un bloc nou devenea mai dificil, iar dacă era prea lent, devenea mai ușor. Acest lucru era integrat în protocolul descentralizat pe care îl rulează toate nodurile, astfel încât orice miner care îl ignora consuma energie pentru a mina un bloc fără niciun beneficiu, deoarece acesta ar fi respins de restul rețelei. Această ajustare asigură că crearea de blocuri noi rămâne conform programului planificat de emisie și oferă stimulente minerilor să „respecte regulile”.

####   
Rezumat

Multe dintre piesele necesare pentru a construi un sistem de monedă electronică peer-to-peer descentralizat, bazat pe principii de bani sănătoși, erau deja puse la punct înainte ca Satoshi să publice whitepaper-ul și la scurt timp după lansarea inițială a codului.

> Natura Bitcoin este de așa fel încât, odată ce versiunea 0.1 a fost lansată, designul de bază a rămas neschimbat pentru tot restul existenței sale  
_Satoshi Nakamoto_

Deși multe idei de îmbunătățire (BIP-uri) au fost propuse și adoptate, Bitcoin a funcționat în fundal încă din 2009, urmând protocolul proiectat în versiunea inițială și cu foarte puține întreruperi. Toate îmbunătățirile au fost realizate păstrând compatibilitatea inversă cu toate versiunile anterioare.



##### Note

1. Pentru o explicație a problemei Generalilor Bizantini - vezi [https://en.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
