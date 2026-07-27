# 9.3 Cum funcționează tranzacțiile

Acum că înțelegi cheile publice și private, precum și rolurile nodurilor și minerilor, iată cum funcționează o tranzacție Bitcoin de la început până la sfârșit.

1. Andrei vrea să trimită bitcoin către Radu. El creează o tranzacție cu adresa lui Radu, suma de trimis și o taxă.
1. Andrei semnează tranzacția cu cheia sa privată pentru a dovedi că este proprietarul.
1. El transmite tranzacția către rețeaua Bitcoin.
1. Nodurile o primesc și verifică dacă respectă regulile, inclusiv semnătura și dacă Andrei are suficient bitcoin.
1. Dacă este validă, tranzacția este distribuită în rețea și adăugată în mempool, unde tranzacțiile în așteptare stau până sunt procesate.
1. Minerii aleg tranzacții din mempool și le includ într-un bloc pe care încearcă să-l mineze.
1. Când un miner minează cu succes un bloc, acesta este distribuit în rețea și verificat de celelalte noduri.
1. Dacă este valid, blocul este adăugat la blockchain. Radu primește bitcoinul.
1. Pe măsură ce se adaugă mai multe blocuri, tranzacția primește confirmări, devenind mai sigură.

Odată inclusă într-un bloc, tranzacția este confirmată. Andrei nu mai poate cheltui acel bitcoin, iar Radu poate folosi ceea ce a primit într-o nouă tranzacție.


> **Light**
>
> Tranzacția și taxa selectate → Semnată de portofel și trimisă → Distribuită de noduri → Minerul adaugă tranzacția în șablonul de bloc → Minerul câștigă concursul Proof-of-Work → Noul bloc este validat → Noul bloc este distribuit de noduri


###### Resurse


[▶ Urmărește acest videoclip despre nodurile Bitcoin](https://www.youtube.com/watch?v=xc_TxlByxeY)
