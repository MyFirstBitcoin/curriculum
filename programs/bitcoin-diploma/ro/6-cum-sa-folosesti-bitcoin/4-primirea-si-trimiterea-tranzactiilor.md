# 6.4 Primirea și trimiterea tranzacțiilor

O tranzacție Bitcoin este un transfer de proprietate asupra bitcoin-ului către un nou proprietar. Observați că nu monedele propriu-zise sunt transferate, ci dreptul de proprietate asupra lor: cu alte cuvinte, dreptul de a le cheltui. De fiecare dată când o tranzacție este acceptată într-un bloc, toate nodurile din rețea își actualizează copia locală a registrului public pentru a reflecta schimbarea de proprietate. Din acest punct de vedere, o tranzacție Bitcoin seamănă mai mult cu o tranzacție imobiliară (sau de altă proprietate) decât cu o tranzacție în numerar.

Pentru a „trimite” bitcoin, expeditorul semnează un mesaj cu cheia sa privată, semnalând rețelei că proprietarul de drept al bitcoin-ului a transferat dreptul de proprietate către destinatar.

Bitcoin-ul va fi acum asociat adresei destinatarului, oferindu-i acestuia dreptul de proprietate asupra bitcoin-ului, astfel încât doar noul proprietar să poată cheltui monedele folosindu-și cheia privată.

Noi tranzacții Bitcoin sunt inițiate din portofele din întreaga lume, dar nu există un procesator central de plăți. În schimb, minerii concurează pentru a înregistra tranzacțiile în registru.

Să presupunem că Mihai îi datorează Elenei 0,5 BTC și este gata să îi returneze suma. Amândoi au portofele digitale.

1. Elena îi transmite adresa ei lui Mihai.
1. Mihai folosește software-ul portofelului său pentru a crea tranzacția, care include adresa Elenei, suma ce urmează a fi transferată (0,5 BTC) și o taxă pentru miner. Taxele mai mari cresc probabilitatea ca un miner să includă tranzacția în următorul bloc.
1. După semnarea tranzacției, aceasta este transmisă rețelei, unde este verificată de noduri. Acestea verifică dacă Mihai are suficiente fonduri și dacă este proprietarul de drept al monedelor pe care intenționează să le cheltuiască. Dacă nu, tranzacția este respinsă imediat.
1. Odată ce tranzacția este verificată, minerii aleg dacă să adauge tranzacția în următorul bloc, de obicei în funcție de taxa selectată. După ce tranzacția ajunge într-un bloc, este adăugată la blockchain și fondurile sunt transferate către adresa Elenei.
1. Dreptul de proprietate a fost transferat către Elena. Ea poate acum să folosească cheia sa privată pentru a cheltui fondurile.

_Este important de reținut că, odată ce tranzacția este finalizată, aceasta nu poate fi anulată._


> **Light – Cum funcționează o tranzacție Bitcoin**
>
> 1. Cineva solicită o tranzacție
> 1. Tranzacția este transmisă computerelor P2P (noduri)
> 1. Minerii verifică tranzacția
> 1. Tranzacțiile sunt combinate pentru a forma un bloc de date
> 1. Noul bloc este adăugat la blockchain-ul existent
> 1. Tranzacția este finalizată



> **Light – Primirea tranzacțiilor Bitcoin**
>
> Pentru a primi bitcoin, va trebui să oferiți expeditorului o adresă publică Bitcoin. Aceasta este un șir unic de litere și cifre care reprezintă portofelul dumneavoastră și este folosit pentru a-l identifica pe rețeaua Bitcoin.
>
> Puteți găsi adresa publică deschizând portofelul Bitcoin și căutând opțiunea „Primește” sau „Depune” bitcoin.
>
> Puteți apoi să partajați adresa Bitcoin în unul dintre următoarele moduri:
>
> 1. **Copiați și lipiți adresa**: Puteți copia adresa selectând-o și apăsând „Copiază”, apoi să o lipiți într-un e-mail sau mesaj.
> 1. **Partajați un link către portofelul Bitcoin**: Unele portofele Bitcoin vă permit să creați un link către portofelul dumneavoastră pe care îl puteți partaja cu expeditorul. Acesta poate apoi să dea click pe link pentru a accesa portofelul și a trimite bitcoin.
> 1. **Partajați un cod QR**: Dacă expeditorul are un smartphone cu o aplicație de portofel Bitcoin instalată, poate scana codul QR pentru a obține adresa dumneavoastră Bitcoin.


Odată ce expeditorul are adresa dumneavoastră, vă poate trimite bitcoin introducând adresa și suma pe care dorește să o trimită. Bitcoin-ul este apoi trimis din portofelul său către portofelul dumneavoastră.

Tranzacția este confirmată de Rețeaua Bitcoin și, de obicei, durează aproximativ 10 minute. Pentru o siguranță sporită, se recomandă să așteptați două confirmări, ceea ce durează aproximativ 20 de minute.


> **Light – Trimiterea tranzacțiilor Bitcoin**
>
> Pentru a trimite bitcoin, veți avea nevoie de câteva lucruri: un portofel Bitcoin, adresa publică a destinatarului și suma de bitcoin pe care doriți să o trimiteți.
>
> 1. Deschideți portofelul Bitcoin.
> 1. Navigați la butonul „Trimite” și lipiți adresa destinatarului în câmpul „Către”. Alternativ, puteți scana codul QR dacă destinatarul vă oferă unul.
> 1. Introduceți suma de bitcoin pe care doriți să o trimiteți în câmpul „Sumă”.
> 1. Verificați cu atenție adresa destinatarului și suma care urmează să fie trimisă. Rețineți că tranzacțiile sunt ireversibile!
> 1. Înainte de a apăsa „Confirmă și Trimite”, vă recomandăm să verificați încă o dată detaliile tranzacției pentru a vă asigura că trimiteți suma corectă de bitcoin la adresa corectă.
> 1. Transmiteți tranzacția și așteptați ca rețeaua să confirme tranzacția.
>
> Acum știți cum să evaluați, să selectați și să configurați un portofel Bitcoin cu auto-custodie. Trimiterea și primirea de bitcoin pe rețeaua Bitcoin sunt denumite tranzacții „on-chain”. Acest lucru se datorează faptului că tranzacțiile au loc pe rețeaua principală Bitcoin și sunt înregistrate în blockchain.
>
> Tranzacțiile on-chain sunt cea mai sigură modalitate de a tranzacționa cu bitcoin datorită verificării descentralizate oferite de rețea.
>
> Totuși, tranzacțiile on-chain sunt mai lente și pot fi semnificativ mai scumpe decât alte opțiuni (pe care le vom discuta în Modulul 7) din cauza taxei pentru mineri.


#### Activitate: Tranzacțiile în acțiune


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Acesta este un exercițiu cooperativ care simplifică rolurile de bază ale persoanelor implicate într-o tranzacție Bitcoin.**

###### Puncte cheie

1. Există patru tipuri de participanți în fiecare tranzacție bitcoin: expeditorul, destinatarul, minerii și operatorii de noduri.
1. Expeditorul trebuie să aprobe (să semneze criptografic) **suma de bitcoin** de trimis ȘI **adresa specifică** către care să trimită.
1. Destinatarul trebuie să furnizeze un **adresă validă** expeditorului ȘI să verifice că tranzacția a fost confirmată cu succes pe blockchain.
1. Minerii se asigură că toate criteriile sunt valide înainte de a adăuga tranzacțiile în blocurile viitoare.
1. Operatorii de noduri verifică dacă blocurile minate sunt valide înainte de a-și actualiza propria versiune a blockchain-ului (registrul).

###### Sfat pentru studenți

Rotiți-vă prin toate cele patru roluri pentru a experimenta ce face fiecare participant.
