# 8.2 Modelul UTXO

##### Ce sunt UTXO-urile?

Nu te lăsa intimidat de acest nume ciudat. Poți să te gândești la UTXO-uri ca la bucăți de bitcoin, asemănătoare bancnotelor și monedelor din portofelul tău. De exemplu, dacă plătești un produs de 28 lei cu o bancnotă de 50 lei, primești 22 lei rest. Bitcoin funcționează într-un mod similar.

Toți bitcoinii pe care îi deții sunt formați din diferite UTXO-uri. Când trimiți bitcoin, portofelul tău folosește una sau mai multe dintre aceste bucăți pentru a face plata.

Dacă bucata pe care o cheltuiești este mai mare decât suma pe care o trimiți, valoarea rămasă îți revine ca rest sub forma unui nou UTXO. În același timp, destinatarul primește un nou UTXO care reprezintă bitcoinul trimis de tine.

Soldul portofelului tău este pur și simplu valoarea totală a tuturor UTXO-urilor pe care le controlezi.


> **Callout – Confidențialitate**
>
> Nu ar trebui să faci cunoscute altora UTXO-urile tale, deoarece dacă cineva le știe, îți poate urmări tranzacțiile și, în cele din urmă, va ști câți bani deții.


###### Exemplu

1. Ana vrea să îi trimită lui Bogdan 5 BTC.
1. Portofelul ei folosește două dintre UTXO-urile sale care împreună valorează 6 BTC.
1. Tranzacția trimite **5 BTC către Bogdan**, creând un nou UTXO în portofelul lui Bogdan.
1. Restul de **0,99 BTC se întoarce la Ana ca rest**, după plata unui **comision de tranzacție de 0,01 BTC**.
1. Odată ce tranzacția este confirmată, ea este adăugată în registrul Bitcoin, iar UTXO-urile folosite de Ana sunt marcate ca fiind cheltuite, astfel încât nu mai pot fi folosite din nou.

###### Resurse


[▶ Urmărește „How Bitcoin Works under the Hood”](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
