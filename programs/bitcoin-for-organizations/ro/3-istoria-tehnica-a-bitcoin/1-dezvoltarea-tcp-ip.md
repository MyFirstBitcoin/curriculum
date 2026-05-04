# 3.1 Dezvoltarea TCP/IP

Majoritatea dintre noi suntem familiarizați cu protocoalele TCP/IP folosite astăzi ca fundație pentru internet. Originile lor datează din anii '70, când oamenii de știință explorau alternative la Arpanet – o rețea și mai veche, concepută de Departamentul Apărării al SUA pentru a permite partajarea resurselor între calculatoare aflate la distanță. TCP/IP a devenit standardul de protocol pentru Arpanet în 1983, ceea ce a dus la transformarea sa în modelul dominant de rețea până la sfârșitul anilor '90 și la baza internetului pe care rulează astăzi Bitcoin.


| Modelul OSI | TCP/IP |
| --- | --- |
| Aplicație | Aplicație |
| Prezentare | Aplicație |
| Sesiune | Aplicație |
| Transport | Transport |
| Rețea | Rețea |
| Legătură de date | Legătură de date |
| Fizic | Fizic |


În același timp cu dezvoltarea modelului TCP/IP, un cadru similar, dar mai cuprinzător, era dezvoltat de Organizația Internațională de Standardizare (ISO) și industria telecomunicațiilor (CCITT). Procesul de dezvoltare a unor noi protocoale sau de propunere a unor modificări era lent și greoi în comparație cu abordarea mai descentralizată folosită pentru TCP/IP, ceea ce a dus la dominanța acestei ultime abordări astăzi.

##### Cerere de modificare

Orice dezvoltare sugerată pentru protocoalele existente sau idei pentru unele noi pot fi propuse în modelul TCP/IP printr-o **Cerere de modificare** (RFC). Acestea trec printr-un proces de aprobare, gestionat de Internet Engineering Task Force (IETF), și devin open source odată aprobate, pentru a permite oricui să le implementeze și să le adopte. Câteva exemple notabile:

* 1969 RFC 1 Documenta modul în care pachetele urmau să fie trimise în Arpanet
* 1981 RFC791 a definit protocolul Internet V4 – încă larg folosit astăzi
* 1982 RFC 821 Protocol simplu de transfer al poștei electronice
* 1987 Sistemul de nume de domeniu – modul în care numele de domenii sunt asociate cu adresele IP
* 1999 RFC 2616 Protocol de transfer hypertext – esențial pentru navigarea pe web


> **Callout**
>
> **Propunere de îmbunătățire Bitcoin** (BIP) urmează o abordare similară cu RFC, dar se concentrează exclusiv pe îmbunătățirile aduse Bitcoin, nu pe dezvoltarea de protocoale noi sau alternative. Bitcoin împrumută și el din acest model pe straturi, iar vei vedea protocoale suplimentare descrise ca fiind de nivelul doi sau trei.


În același mod în care straturile de bază ale modelului TCP/IP s-au schimbat foarte puțin în ultimele decenii, inovația având loc la straturile superioare, și stratul de bază al Bitcoin se așteaptă să se schimbe foarte lent de acum înainte, soluțiile de scalare precum Lightning și Liquid fiind dezvoltate deasupra.

Un exemplu bun despre cum protocoalele de bază devin greu de schimbat în timp este IPv6. Epuizarea anticipată a spațiului de adrese în IPv4 a creat cererea pentru un nou protocol. Primul standard draft a fost creat în 1998, dar nu a fost ratificat ca standard de internet până în 2017. Deși a rezolvat multe probleme ale IPv4 și este mult mai pregătit pentru viitor, adoptarea sa în industrie este încă foarte lentă. În acest timp, multe protocoale noi au fost definite la straturile superioare pentru a permite multimedia, email etc.

##### Elementele de bază folosite de Bitcoin

Această separare a problemelor de interconectivitate permite ca protocoalele să fie dezvoltate independent de straturile de deasupra și de dedesubt. În loc să fie nevoie să reinventezi soluții pentru fiecare strat, rețeaua Bitcoin se poate baza pe capabilitățile de bază ale rețelei oferite la nivelul fizic și de legătură de date.


| Strat | TCP/IP Original |
| --- | --- |
| Aplicație | Folosește Sistemul de Nume de Domeniu (DNS) pentru a identifica nodurile vecine. Portul 8333 semnalează protocolul Bitcoin. |
| Transport | UDP pentru comunicații FIBRE între mineri pentru latență redusă. TCP pentru comunicații P2P între noduri. |
| Transport | Rutare TOR: Permite anonimatul și confidențialitatea. Protocol de difuzare: Rutează traficul prin rețea. |
| Legătură | Funcționează pe orice mediu (de exemplu, Ethernet, Wi-Fi etc.) |
| Fizic | Transmitere fizică prin wireless, Ethernet sau alte interfețe hardware. |


##### Bitcoin este un protocol neutru pentru transferul de valoare, așa cum HTTPS este un protocol pentru transferul de informații

* **HTTPS**: Site-uri securizate
* **SMTP**: Trimite emailuri
* **FTP**: Transferă fișiere
* **DNS**: Gestionează nume de domenii
* **BTC**: Stochează și transferă valoare

Bitcoin permite transportul valorii în mod fiabil și fără a necesita o terță parte între persoane sau dispozitive prin Internet. Se așteaptă ca acest lucru să deblocheze o valoare uriașă.
