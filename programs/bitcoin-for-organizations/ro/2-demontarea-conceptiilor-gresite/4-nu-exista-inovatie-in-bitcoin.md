# 2.4 Nu există inovație în Bitcoin

> Crearea a o mie de păduri se află într-o singură ghindă.   
_Ralph Waldo Emerson_

Criticii încearcă adesea să susțină că Bitcoin este o tehnologie „veche” sau „moartă” deoarece nu modifică protocolul de bază la fel de des ca alte blockchain-uri concurente. Această afirmație ignoră atât motivele pentru care schimbările la Bitcoin sunt adoptate lent, cât și cantitatea de inovație care are loc pentru a scala rețeaua pe straturi superioare, cum ar fi Lightning Network. De asemenea, ignoră faptul că multe dintre cele mai flexibile și durabile tehnologii ale noastre nu evoluează rapid la nivelul de bază.

De exemplu, nu există inovație nici în Transmission Control Protocol (TCP), care stă la baza internetului. TCP a fost creat pentru prima dată în 1974. Ultima dată când TCP a fost actualizat a fost în 1982. Își face treaba pentru care a fost conceput. Nu este perfect și există dezbateri dacă ar trebui să actualizăm IPv4 pentru a susține dezvoltările viitoare ale internetului. Totuși, a spune că nu a existat nicio inovație pe internet din 1982 ar fi o afirmație remarcabilă. Toată această inovație a avut loc „pe” TCP, nu „în” TCP.

Marea majoritate a inovației care are loc nu este „în” Bitcoin, ci „pe” Bitcoin. Într-o zi, probabil nu va mai exista inovație „în” Bitcoin, iar acest lucru ar trebui să fie un obiectiv, nu o critică, deoarece va reflecta cât de fundamental a devenit în susținerea economiei globale, oferind fundația pentru o monedă solidă globală, neutră și fără permisiuni. O monedă care este solidă atât din punct de vedere economic, având o ofertă fixă și un registru imuabil, cât și din punct de vedere tehnologic, deoarece nu se schimbă și ceea ce rulează a avut ani de funcționare neîntreruptă. Bitcoin a atins deja 100% funcționare neîntreruptă în ultimii 10 ani.

Totuși, ar fi o problemă dacă nu ar exista inovație „pe” Bitcoin. Să aruncăm o privire asupra ultimilor 10 ani:



#### „În” Bitcoin

Segregated Witness (SegWit) a fost implementat în 2017 pentru a proteja împotriva maleabilității tranzacțiilor și pentru a crește capacitatea blocurilor. SegWit a fost, de asemenea, un precursor necesar pentru ca Lightning și unele sidechain-uri să funcționeze eficient.

Taproot a fost implementat în 2021 pentru a permite gruparea și validarea mai multor semnături prin incorporarea semnăturilor Schnorr, introducând un limbaj de scripting pentru funcționalități mai complexe și crescând confidențialitatea și rezistența la cenzură a tranzacțiilor.



#### „Pe” Bitcoin

##### Liquid Sidechain

Sidechain-ul Liquid a fost implementat în 2018. Liquid, ca și alte sidechain-uri, este un registru blockchain separat care este legat de blockchain-ul principal Bitcoin, conform unui set de reguli predefinite. Aceste reguli sunt suficient de flexibile pentru a permite ca lanțul Liquid să se dezvolte și să încorporeze îmbunătățiri de design și scalabilitate în timp. Totuși, legătura cu blockchain-ul Bitcoin asigură că plafonul total de 21 de milioane de bitcoin este menținut pe ambele lanțuri.

Activul din Liquid, L-BTC, este legat bidirecțional de bitcoin-ul de pe lanțul principal. Există compromisuri de cost, viteză, confidențialitate și securitate care fac ca L-BTC să fie ideal pentru anumite aplicații. Costul, viteza și confidențialitatea sunt toate îmbunătățite cu L-BTC, în schimbul plasării unei părți din încredere în organizațiile care formează Federația Liquid, care controlează împreună un proces multisig 11 din 15 pentru a transfera L-BTC către bitcoin și invers.

##### Lightning Network

Lightning Network a fost implementată în 2018. Lightning este concepută ca o rețea de plăți peer-to-peer sub forma unui graf de noduri conectate prin canale; nu este un blockchain. Bitcoin este blocat de către un operator de nod pe blockchain-ul principal pentru a-l face disponibil pe Lightning Network, ceea ce asigură că doar bitcoin „real” este folosit. Nodurile pot apoi deschide canale de lichiditate prin contracte inteligente multisig între ele. Plățile găsesc rute prin rețea de la sursă la destinație, optimizând costul în funcție de cerința ca lichiditatea suficientă să existe în direcția corectă între fiecare pas al rutei. Lightning Network îmbunătățește masiv costul, viteza și confidențialitatea în schimbul unei pierderi de securitate (sau a unei creșteri a încrederii necesare) și a unei creșteri a complexității. Totuși, este destinată plăților zilnice cu volum mare și valoare mică, astfel încât acest compromis este considerat foarte rezonabil pentru milioanele de tranzacții zilnice (sursa: River, 2023).

##### Chaumian eCash Mints

Fedimint-urile pot fi privite ca o rețea Lightning limitată la o comunitate. Sunt concepute pentru a valorifica încrederea inerentă care există în anumite comunități (de exemplu, familii, sate, grupuri de prieteni) în schimbul simplificării complexității și creșterii confidențialității pentru utilizatori. Sunt protocoale modulare, open source, pentru custodia și tranzacționarea bitcoin într-un context comunitar. Sunt interoperabile cu Lightning Network.

**Cashu** este un token la purtător care poate fi stocat pe un dispozitiv, cum ar fi un telefon mobil; designul său urmărește să reproducă beneficiile banilor fizici, dar în formă digitală. Cashu este un exemplu de Chaumian eCash construit pe Bitcoin și crește confidențialitatea și rezistența la cenzură, reducând complexitatea în schimbul încrederii în mint-ul eCash folosit. Mint-urile Cashu emit tokenuri eCash, care reprezintă bitcoin, ce pot fi cheltuite de utilizatori fără a-și dezvălui identitatea. Cashu este interoperabil cu Lightning Network.

Este probabil să apară multe alte aplicații de nivel 2 în viitor, cu multe aplicații de nivel 3 construite la rândul lor peste fiecare dintre acestea.

Ca exemplu al numărului incredibil de aplicații construite peste Lightning, iată un extras dintr-un raport de cercetare despre Lightning Network realizat de River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
