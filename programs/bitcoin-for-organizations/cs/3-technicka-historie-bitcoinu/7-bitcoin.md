# 3.7 Bitcoin

Po mnoha letech a neúspěšných pokusech začali Cypherpunks většinou ztrácet zájem o myšlenku digitální měny bez povolení, když Adam Back obdržel e-mail s odkazem na návrh white paperu s názvem „elektronická hotovost bez třetí strany“ od anonymní osoby, která si říkala Satoshi Nakamoto.

Abychom si to shrnuli, máme zde alespoň tyto myšlenky:

* Kryptografické podpisy, které by mohly zajistit určitou úroveň soukromí a anonymity
* Koncept nekryté měny (B-Money)
* Návrhy (ale žádný způsob), jak omezit vydávání nové měny
* Digitální mince, jejichž vlastnictví bylo určeno veřejnými klíči (B-Money) a které bylo možné přesouvat podepisováním a převádět na základě adresy příjemce (RPOW a Hashcash)
* Všechny uzly udržují kopii zcela distribuované účetní knihy (B-Money) (tehdy zamítnuto jako nepraktické)
* Protokol časového razítka – použití Merkleho stromového hashování k matematicky prokazatelnému určení chronologie událostí, kterou je obtížné zfalšovat, pokud všichni uživatelé uchovávají stejné záznamy
* Proof of work pro propojení skutečného úsilí se systémem (ale použití samotného hashe jako měny)
* Zcela decentralizované sítě, kde jsou si všichni účastníci rovni a mohou do sítě libovolně vstupovat a odcházet (BitTorrent)
* Koncept navazování nových hashů na předchozí hashe (Bit Gold a časové razítkování)

Co v té době chybělo:

* Životaschopné řešení pro vyřešení problému „byzantských generálů“
* Metoda, jak omezit množství peněz v oběhu navzdory neustálému zlepšování hardwaru
* Motivační schéma pro účastníky (problém slepice a vejce)

Dalším zásadním rozdílem mezi nedávnými pokusy a Bitcoinem bylo to, že Satoshi na kódu pracoval již delší dobu v duchu původního hesla „Cypherpunks píší kód“, než jej oznámil na mailing listech, na rozdíl od Bit Gold a B-Money, které byly spíše konceptuální.

Jaká byla inovace, která odlišila Bitcoin od předchozích pokusů o elektronickou hotovost?

Proof of work by byl použit jako konsenzuální mechanismus a způsob zajištění bezpečnosti a neměnnosti: místo použití hashe jako formy peněz by byl použit novým konceptuálním procesem zvaným těžba, kdy uzel seskupí sadu transakcí, přidá náhodné číslo a poté aplikuje hashování na „blok“ dat. Platný blok, který splňuje požadavek na hash, by byl následně oznámen síti. Tyto bloky by byly propojeny pomocí hashe předchozího bloku v každém z nich a v případě rovnosti, kdy různé uzly ověřují a oznamují různé bloky současně a vznikají rozdělení řetězce, by byla použita nejdelší blockchain. Proof of work se stal distribuovaným rozhodčím pro řešení problému byzantských generálů.

Těžaři byli také motivováni poskytovat potřebný výpočetní výkon pro proof-of-work tím, že za každý blok získali nové bitcoiny. Množství Bitcoinů, které získávají, je také naprogramováno tak, aby přibližně každé 4 roky klesalo, dokud nebudou všechny Bitcoiny vytvořeny, což vytváří pevný limit na celkové množství Bitcoinů, které kdy budou v oběhu – 21 milionů.

Nejoriginálnější myšlenkou byl způsob, jakým vyřešil otázku, kolik peněz je vytvořeno, když se hardware zlepšuje a do sítě lze zapojit více výkonu. Časová razítka určitého počtu bloků (2016) by byla zprůměrována a pokud by byly vytvářeny příliš rychle, hash potřebný k vytvoření nového bloku by byl ztížen, pokud příliš pomalu, byl by zjednodušen. Toto bylo zabudováno do decentralizovaného protokolu, který běží na všech uzlech, takže každý těžař, který by to ignoroval, by vynaložil energii na těžbu bloku bez užitku, protože by byl zbytkem sítě odmítnut. Tato úprava zajišťuje, že tvorba nových bloků zůstává v plánovaném harmonogramu vydávání a motivuje těžaře „dodržovat pravidla“.

####   
Shrnutí

Mnoho dílků skládačky toho, co je potřeba k vytvoření decentralizovaného peer-to-peer systému elektronické hotovosti založeného na principech zdravých peněz, bylo na svém místě ještě předtím, než Satoshi zveřejnil svůj whitepaper a krátce po počátečním vydání kódu.

> Povaha Bitcoinu je taková, že jakmile byla vydána verze 0.1, základní design byl na zbytek jeho existence vytesán do kamene  
_Satoshi Nakamoto_

Ačkoliv bylo navrženo a přijato mnoho nápadů na vylepšení (BIP), Bitcoin funguje na pozadí od roku 2009 podle protokolu navrženého v počátečním vydání a téměř bez jakýchkoliv narušení. Všechna vylepšení byla provedena při zachování zpětné kompatibility se všemi předchozími verzemi.



##### Poznámky

1. Vysvětlení problému byzantských generálů najdete na[https://cs.wikipedia.org/wiki/Byzantsk%C3%BD_probl%C3%A9m](https://en.wikipedia.org/wiki/Byzantine_fault)
