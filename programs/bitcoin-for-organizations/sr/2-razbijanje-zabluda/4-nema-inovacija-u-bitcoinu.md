# 2.4 Nema inovacija u Bitcoinu.

> Stvaranje hiljadu šuma nalazi se u jednom žiru.  
_Ralph Waldo Emerson_

Kritičari često pokušavaju da tvrde da je Bitcoin „stara“ ili „mrtva“ tehnologija zato što se osnovni protokol ne menja tako često kao kod konkurentskih blokčejna. Ova tvrdnja zanemaruje i razloge zbog kojih se promene u Bitcoinu usvajaju sporo, kao i količinu inovacija koje se dešavaju radi skaliranja mreže na višim slojevima, kao što je Lightning Network. Takođe se zanemaruje činjenica da mnoge naše najfleksibilnije i najtrajnije tehnologije takođe ne napreduju brzo na osnovnom sloju.

Na primer, nema inovacija ni u Transmission Control Protocol (TCP), koji je osnova interneta. TCP je prvi put napravljen 1974. godine. Poslednji put je TCP ažuriran 1982. godine. Radi ono što treba da radi. Nije savršen, i postoje debate o tome da li treba unaprediti IPv4 kako bi podržao budući razvoj interneta. Međutim, reći da nije bilo inovacija na internetu od 1982. godine bila bi izuzetna tvrdnja. Sve te inovacije su se dešavale „na“ TCP-u, a ne „u“ njemu.

Velika većina inovacija koje se dešavaju nisu „u“ Bitcoinu, već „na“ Bitcoinu. Jednog dana verovatno neće biti nikakvih inovacija „u“ Bitcoinu, i to bi trebalo da bude cilj, a ne kritika, jer će to biti odraz toga koliko je postao fundamentalna podrška globalnoj ekonomiji, obezbeđujući temelje za globalni, neutralni i dozvolama neograničeni zdrav novac. Novac koji je zdrav i u ekonomskom smislu, jer ima fiksnu ponudu i nepromenljivu knjigu, ali i u tehnološkom smislu, jer se ne menja i ono što radi ima godine neprekidnog rada bez prekida. Bitcoin je već postigao 100% dostupnosti u poslednjih 10 godina.

Međutim, bilo bi zabrinjavajuće kada se ne bi dešavale inovacije „na“ Bitcoinu. Hajde da pogledamo kako je to izgledalo u poslednjih 10 godina:



#### „U“ Bitcoinu

Segregated Witness (SegWit) je implementiran 2017. godine kako bi zaštitio od promenljivosti transakcija i povećao kapacitet blokova. SegWit je takođe bio neophodan preduslov za efikasan rad lightning mreže i nekih sidechain-ova.

Taproot je implementiran 2021. godine kako bi omogućio grupisanje i verifikaciju više potpisa korišćenjem Schnorr potpisa, uveo skriptni jezik za složeniju funkcionalnost i povećao privatnost i otpornost na cenzuru transakcija.



#### „Na“ Bitcoinu

##### Liquid Sidechain

Liquid sidechain je implementiran 2018. godine. Liquid, kao i drugi sidechain-ovi, je zasebna blokčejn knjiga koja je povezana sa glavnim Bitcoin blokčejnom prema unapred definisanom skupu pravila. Ta pravila su dovoljno fleksibilna da omoguće Liquid lancu da se razvija i uključuje dizajnerska i skalabilna poboljšanja tokom vremena. Međutim, veza sa Bitcoin blokčejnom obezbeđuje da ukupna ponuda bitcoina od 21 milion ostane dosledna na oba lanca.

Imovina na Liquid-u, L-BTC, je dvosmerno vezana za bitcoin na glavnom lancu. Postoje kompromisi u pogledu troškova, brzine, privatnosti i bezbednosti, što čini L-BTC idealnim za određene primene. Troškovi, brzina i privatnost su poboljšani sa L-BTC, ali uz cenu poverenja u organizacije koje čine Liquid Federaciju, koje zajedno kontrolišu proces 11 od 15 multisig za prebacivanje L-BTC u bitcoin i obrnuto.

##### Lightning Network

Lightning mreža je implementirana 2018. godine. Lightning je zamišljen kao peer-to-peer mreža za plaćanja u obliku grafa čvorova povezanih kanalima; nije blokčejn. Bitcoin se zaključava od strane pokretača čvora na glavnom blokčejnu kako bi bio dostupan za korišćenje na Lightning Network-u, što obezbeđuje da se koristi samo „pravi“ bitcoin. Čvorovi zatim mogu otvarati kanale likvidnosti putem multisig pametnih ugovora jedni sa drugima. Plaćanja pronalaze rute kroz mrežu od izvora do odredišta, optimizujući troškove uz uslov da postoji dovoljna likvidnost u pravom smeru između svakog čvora na ruti. Lightning Network značajno poboljšava troškove, brzinu i privatnost u zamenu za gubitak bezbednosti (ili povećanje potrebnog poverenja) i povećanje složenosti. Međutim, namenjen je za plaćanja velikog obima i male vrednosti u svakodnevnim transakcijama, tako da se ovaj kompromis smatra veoma razumnim za milione dnevnih transakcija (izvor: River, 2023).

##### Chaumian eCash Mints

Fedimints se mogu posmatrati kao lightning mreža ograničena na zajednicu. Dizajnirani su da iskoriste inherentno poverenje koje postoji unutar određenih zajednica (npr. porodice, sela, grupe prijatelja) u zamenu za pojednostavljenje složenosti i povećanje privatnosti za korisnike. To su modularni, open source protokoli za čuvanje i transakciju bitcoina u kontekstu zajednice. Oni su interoperabilni sa samim Lightning Network-om.

**Cashu** je prenosivi token koji može biti sačuvan na uređaju kao što je mobilni telefon; dizajniran je da reprodukuje prednosti fizičkog novca, ali u digitalnom obliku. Cashu je primer Chaumian eCash-a izgrađenog na Bitcoinu i povećava privatnost i otpornost na cenzuru, a smanjuje složenost u zamenu za poverenje u eCash mint koji se koristi. Cashu mintovi izdaju eCash tokene koji predstavljaju bitcoin i mogu se trošiti bez otkrivanja identiteta korisnika. Cashu je interoperabilan sa Lightning Network-om.

Verovatno će u budućnosti biti izgrađeno još mnogo aplikacija na drugom sloju, a na svakom od njih i aplikacije trećeg sloja.

Kao primer neverovatnog broja aplikacija koje se grade na Lightning-u, evo isečka iz Lightning Network Research Report-a kompanije River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
