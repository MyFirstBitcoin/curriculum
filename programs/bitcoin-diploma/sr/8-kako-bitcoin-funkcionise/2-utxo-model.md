# 8.2 UTXO model

##### Šta su UTXO-i?

Ne dozvolite da vas zastraši neobično ime. UTXO-e možete zamisliti kao delove bitkoina, slično novčanicama i kovanicama u vašem novčaniku. Na primer, ako platite predmet od 600 dinara novčanicom od 1.000 dinara, dobićete 400 dinara kusura. Bitcoin funkcioniše na sličan način.

Sav bitcoin koji posedujete sastoji se od različitih UTXO-a. Kada šaljete bitcoin, vaš novčanik koristi jedan ili više ovih delova da izvrši plaćanje.

Ako je deo koji trošite veći od iznosa koji šaljete, preostala vrednost vam se vraća kao kusur u obliku novog UTXO-a. Istovremeno, primalac dobija novi UTXO koji predstavlja bitcoin koji ste mu poslali.

Stanje vašeg novčanika je jednostavno zbir svih UTXO-a koje kontrolišete.


> **Callout – Privatnost**
>
> Ne bi trebalo da drugima otkrivate svoje UTXO-e, jer ako ih neko zna, može pratiti vaše transakcije i na kraju saznati koliko novca posedujete.


###### Primer

1. Ana želi da pošalje Bobanu 5 BTC.
1. Njen novčanik koristi dva njena UTXO-a koji zajedno vrede 6 BTC.
1. Transakcija šalje **5 BTC Bobanu**, čime se u Bobanovom novčaniku stvara novi UTXO.
1. Preostalih **0,99 BTC se vraća Ani kao kusur**, nakon plaćanja **0,01 BTC provizije za transakciju**.
1. Kada se transakcija potvrdi, ona se dodaje u Bitcoinovu knjigu i UTXO-i koje je Ana koristila se označavaju kao potrošeni, tako da se više ne mogu koristiti.

###### Resursi


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
