# 9 - Jak funguje těžba Bitcoinu

Délka: 90 minut

Hlavní myšlenka: Bitcoinová těžba a ověřování uzlů spolupracují na zabezpečení sítě, potvrzování transakcí a prosazování pravidel systému prostřednictvím Proof of Work.

#### Výukové cíle

Na konci této lekce by studenti měli být schopni:

* Vysvětlit rozdíl mezi rolí bitcoinových uzlů a rolí bitcoinových těžařů.
* Popište, jak uzly ověřují transakce, sdílejí informace a pomáhají prosazovat pravidla Bitcoinu.
* Vysvětlete, co dělají těžaři, včetně výběru transakcí, vytváření kandidátních bloků a soutěžení o nalezení platného hash bloku.
* Definujte mempool a vysvětlete, proč funguje jako čekárna pro nepotvrzené transakce.
* Popište, jak transakční poplatky ovlivňují výběr těžařů a rychlost potvrzení.
* Vysvětlete Proof of Work jako mechanismus, který zabezpečuje Bitcoin tím, že útoky činí drahými.
* Popište, jak úprava obtížnosti pomáhá udržovat průměrný čas bloku kolem 10 minut.
* Projděte celý životní cyklus bitcoinové transakce, od vytvoření a podepsání až po potvrzení v bloku.

#### Nástroje a zdroje

##### Vizuální pomůcky

* Kapitola 9 – Jak funguje bitcoinová těžba?

##### Podpůrná knihovna

* Slovníček pojmů — Kapitola 9 — Termíny: těžba, Proof of Work, hash hádanka, úprava obtížnosti, odměna za blok, mempool, 51% útok
* Knihovny mylných představ — Kapitola 9 — Vyvrácení: „těžaři vytvářejí Bitcoin z ničeho“, „těžaři ovládají Bitcoin“, „více těžby = méně bezpečí“
* Srovnávací tabulky a referenční listy — Ekonomika těžby: příjmy, náklady, sladění motivací; úprava obtížnosti
* Technické vysvětlivky a detailní rozbory — Bezpečnost Proof of Work; proč je útok drahý; hranice 51 %

#### Aktivity

* Prozkoumání mempoolu
* Transakce v akci

#### Online výuka

* Použijte jeden přehledný diagram toku transakce od podepsání v peněžence po potvrzení.
* Udržujte uzly a těžaře vizuálně oddělené na obrazovce po celou dobu lekce.
* Použijte mempool.space nebo jeho snímek obrazovky k zobrazení nepotvrzených transakcí a tlaku na poplatky.
* Po každé fázi těžebního procesu udělejte pauzu a položte jednu krátkou otázku na porozumění.

#### Příprava

* Připravte diagram těžebního procesu (mempool → výběr transakcí → tvorba bloku → úprava obtížnosti) k zobrazení.
* Uložte si stránku mempool.space nebo stránku těžby na blockchain.com; připravte snímky aktuálních statistik těžby a úprav obtížnosti.
* Vytvořte vizuální vysvětlení Proof of Work jako bezpečnostního mechanismu; ukažte úpravu obtížnosti za posledních 3–6 měsíců.

#### Postup

Tato lekce se podrobněji zabývá tím, jak bitcoinové transakce procházejí sítí a stávají se součástí blockchainu. Nyní přímo sleduje strukturu Diplomového programu, takže hlavní sekce odpovídají studentskému průvodci a zároveň zachovávají podrobnější vysvětlení pro lektora v každé sekci.

##### 9.0 Úvod, 8 minut

Začněte propojením této kapitoly s předchozí:

* Pokud uživatel podepíše transakci soukromým klíčem, co se stane dál?
* Kdo ověřuje, zda je tato transakce platná?
* Jak se dostane do blockchainu?
* Proč Bitcoin potřebuje jak uzly, tak těžaře?

Ujasněte, že tato kapitola vysvětluje, jak síť ve skutečnosti zpracovává transakce a jak těžba zabezpečuje systém bez centrální autority.

##### 9.1 Bitcoinové uzly a těžaři, 47 minut

**Uzly a těžaři, různé role**

Začněte jasným oddělením těchto dvou rolí.

Bitcoinové uzly:

* uchovávají kopii blockchainu
* ověřují, zda transakce splňují pravidla
* sdílejí informace s ostatními uzly
* pomáhají peněženkám a dalšímu softwaru přistupovat k datům blockchainu
* mohou odmítnout neplatné transakce nebo neplatné bloky

Kapitola popisuje uzly jako strážce ověřování a rozšiřuje to pomocí analogie „digitálního dopravního policisty“. To je užitečné, protože ukazuje uzly jako kontrolory a koordinátory, nikoli vládce. Schéma také zdůrazňuje, že mnoho uzlů uchovává kopie účetní knihy po celém světě.

Těžaři Bitcoinu:

* shromažďují platné transakce
* sestavují kandidátní bloky
* soutěží o nalezení platného hash bloku
* vysílají platné bloky, když vyhrají
* obdrží odměny za blok a transakční poplatky

Klíčovým bodem výuky z této kapitoly je, že účelem těžby není pouze vytvářet nové bitcoiny, ale decentralizovat bezpečnost Bitcoinu. Nové bitcoiny jsou pobídkou, zatímco samotný proces těžby je bezpečnostním mechanismem.

**Co uzly skutečně dělají**

Navazujte na sekci o uzlech pomocí seznamu funkcí uzlů z kapitoly:

* Strážci ověřování: kontrolují, že transakce a bloky dodržují pravidla
* Komunikační uzel: propojují se navzájem a sdílejí data o transakcích
* Kontrolor kvality: odmítají neplatné informace
* Informátor o blockchainu: poskytují data jinému softwaru, například peněženkám
* Uvítání nového uzlu: pomáhají novým uzlům získat blockchain, přičemž každý nový uzel si data ověřuje nezávisle

Toto je vhodný okamžik zdůraznit, že provozování uzlu dává uživateli větší nezávislost. Místo toho, aby byl zcela závislý na vnějších službách, které mu sdělují stav sítě, může si jej ověřit sám. to jasně vysvětluje, včetně zmínky o Bitcoin Core jako jedné z implementací, kterou mohou uživatelé spustit.

**Co těžaři skutečně dělají**

Nyní vysvětlete těžbu podrobněji.

Těžaři:

* sbírají ověřené, ale nepotvrzené transakce
* seskupují je do kandidátního bloku
* opakovaně hashují data bloku při hledání platného hash bloku
* vysílají vítězný blok do sítě
* získávají odměny, pokud je blok přijat

Použijte analogii kapitoly „obrovská hromada klíčů“, pokud to pomůže. Dává studentům konkrétní představu o závodu v těžbě. Hlavní myšlenkou není, že těžaři řeší užitečný matematický problém v běžném smyslu, ale že dokazují, že vynaložili skutečnou energii a výpočetní výkon na zabezpečení systému.

Toto je také vhodné místo pro vysvětlení odměn těžařů:

* odměna za blok: nově vydané bitcoiny
* transakční poplatky: poplatky připojené k transakcím, které uživatelé chtějí potvrdit

Ujasněte, že těžaři obvykle upřednostňují transakce s vyššími poplatky, protože ty zvyšují jejich odměnu. Kapitola zde také vysvětluje půlení, takže můžete stručně poznamenat, že odměna za blok se snižuje každých 210 000 bloků, přibližně každé čtyři roky, podle veřejného harmonogramu emise Bitcoinu. Strany 5 a 6 obsahují harmonogram emise a tabulku nadcházejícího půlení, což může pomoci posílit předvídatelné vydávání Bitcoinu.

**Platný hash bloku, Proof of Work a úprava obtížnosti**

Tato sekce je jádrem kapitoly.

Vysvětlete, že těžaři hledají platný hash bloku, což znamená hash bloku, který splňuje cíl sítě. Kapitola to vysvětluje jako hledání čísla nižšího než cíl stanovený sítí.

Poté jasně vysvětlete Proof of Work:

* těžaři musí opakovaně provádět výpočetní práci
* ten, kdo jako první najde platný hash, dokazuje, že tuto práci vykonal
* to ztěžuje přepisování nebo útok na účetní knihu
* uzly poté blok ověří, než jej přijmou

Silná věta pro výuku je:

Proof of Work zabezpečuje Bitcoin tím, že činí nepoctivost drahou a ověření snadným.

Vysvětlete také úpravu obtížnosti:

* síť upravuje obtížnost těžby každých 2 016 bloků
* to se děje přibližně každé dva týdny
* cílem je udržet průměrný čas bloku blízko 10 minut
* pokud se k síti připojí více výpočetního výkonu, obtížnost stoupá
* pokud je výpočetního výkonu méně, obtížnost klesá

Strany 7 a 8 tento proces vysvětlují a ukazují, jak těžší cíle vyžadují více práce. To pomáhá studentům pochopit, že časování Bitcoinu není řízeno centrální autoritou, ale protokolovými pravidly, která automaticky reagují na podmínky v síti.

##### 9.2 Co je to mempool?, 15 minut

Nyní přejděte k mempoolu.

Vysvětlete, že mempool je čekárna pro platné, nepotvrzené transakce. Když uživatel odešle transakci, uzly ji nejprve ověří. Pokud je platná, přidají ji do svého mempoolu a sdílí ji s ostatními uzly. Poté si těžaři mohou z těchto čekajících transakcí vybírat při sestavování bloku. Strany 10 a 11 tento proces přímo vysvětlují.

Důležité body, které je třeba zdůraznit:

* mempool není blockchain
* transakce zde jsou stále nepotvrzené
* každý uzel si udržuje svůj vlastní mempool
* neexistuje jeden univerzální mempool
* transakce s vyšším poplatkem mají větší šanci být vybrány dříve

Kapitola také vysvětluje běžné důvody, proč může transakce zůstat dlouho nepotvrzená:

* nízký poplatek
* přetížení sítě
* pokus o dvojí utracení
* nesprávná nebo neúplná data
* chybně vytvořená transakce

Pokud je to užitečné, zmiňte aktivitu s mempool.space jako praktický způsob, jak vizualizovat nepotvrzené transakce a výši poplatků. Také jasně uveďte, že mempool.space je pouze jeden z průzkumníků, ne samotný mempool.

##### 9.3 Jak fungují bitcoinové transakce, 20 minut

Nyní spojte vše dohromady pomocí postupného sledu kroků z kapitoly.

Jasná verze pro třídu je:



1. Odesílatel vybere UTXO a vytvoří transakci
1. Odesílatel přidá adresu příjemce a poplatek
1. Odesílatel podepíše transakci svým soukromým klíčem
1. Transakce je rozeslána do sítě
1. Uzel ji ověří a přidá do svého mempoolu
1. Těžaři ji vyberou do kandidátského bloku
1. Těžaři soutěží pomocí Proof of Work
1. Jeden těžař najde platný hash bloku a rozesílá blok
1. Uzel ověří blok a přidá jej do blockchainu
1. Transakce získává potvrzení, jakmile jsou přidávány další bloky
1. Udělejte závěrečný bod explicitní:
1. jakmile je transakce zahrnuta v platném bloku, je potvrzena
1. utrácené vstupy již nelze použít
1. příjemce nyní ovládá nové UTXO vytvořené touto transakcí

Souhrnný diagram je zde obzvlášť užitečný, protože vizuálně propojuje celý proces od podepsání v peněžence přes zařazení těžařem až po ověření uzlem a distribuci bloku.

###### Závěr a ověření porozumění

Ukončete několika rychlými otázkami:

* Jaký je rozdíl mezi uzlem a těžařem?
* Co je mempool?
* Proč se některé transakce potvrzují rychleji než jiné?
* Co dokazuje Proof of Work?
* Proč Bitcoin upravuje obtížnost těžby?
* Jaké jsou hlavní kroky mezi odesláním transakce a jejím potvrzením?

#### Poznámky pro lektora

Udržujte hlavní výukovou linii jasnou: uzly ověřují, těžaři soutěží, Proof of Work zajišťuje bezpečnost a mempool drží platné transakce, dokud nejsou potvrzeny.

Tato kapitola může působit technicky, proto často používejte analogie a diagramy.

Vyhněte se tomu, aby těžba zněla jako „vytváření bitcoinů z ničeho“. Buďte přesní, že odměna je pobídkou, zatímco samotný proces těžby zajišťuje síť.

Nejsilnější body, na které se zaměřit, pokud je málo času, jsou:



1. Role uzlu vs těžaře
1. Mempool jako čekárna
1. Proof of Work
1. Úprava obtížnosti
1. Tok transakce od podepsání po potvrzení

##### Jak vypadá dobrý výsledek

* Je důležité hned na začátku objasnit, že těžaři ≠ uzly, ukázat těžbu jako ekonomickou činnost se skutečnými náklady na hardware a elektřinu, použít úpravu obtížnosti a Proof of Work k vysvětlení bezpečnostního mechanismu a ověřit porozumění pomocí scénářů o změnách v síti.
* Lektoři by měli používat reálná čísla k ukotvení diskuse, být naprosto jasní a opakovaně zdůrazňovat rozdíl mezi těžaři a uzly, být realističtí ohledně centralizačních rizik u těžebních poolů a respektovat skutečnou sofistikovanost, která je v tom zapojená.
* Studenti chápou, že těžba znamená, že chytří lidé dělají složitou práci, protože za to dostávají Bitcoin, rozpoznávají, že pobídky vedou k poctivému chování, protože zisk těžařů závisí na úspěchu Bitcoinu, vidí, že systém se sám reguluje automatickým nastavováním obtížnosti, chápou, že těžba je skutečný byznys, ne charita, a oceňují, že bezpečnost Bitcoinu stojí skutečnou elektřinu a peníze.
* Výukové cíle jsou splněny, pokud studenti dokážou rozlišit těžaře, kteří vytvářejí bloky, od uzlů, které je ověřují, chápou Proof of Work jako bezpečnostní mechanismus, který dělá útoky exponenciálně dražšími, rozpoznají, že úprava obtížnosti udržuje čas bloku přibližně na 10 minutách, rozumí pobídkám těžařů ohledně odměn za bloky a poplatků, vysvětlí, proč útok 51 % nefunguje, a vidí těžbu jako ekonomickou činnost se skutečnými náklady a přínosy.

##### Správa času

Pokud je málo času, upřednostněte:

* Role uzlu vs. těžaře (zásadní rozdíl)
* Mempool jako čekárna
* Mechanismus Proof of Work
* Úprava obtížnosti (samo-regulační systém)
* Tok transakce od podepsání po potvrzení

Pokud máte náskok, věnujte čas:

* Ekonomika těžby a specifika hardwaru
* Dynamika těžebních poolů a obavy z centralizace
* Scénáře útoku 51 % a proč matematicky selhávají
* Dlouhodobá bezpečnost díky sladění pobídek

##### Pokud mají studenti potíže

* Těžaři vs. uzly (zmatek) → "Uzly ověřují, těžaři navrhují; rozhodčí vs. hráči."
* Proof of Work je plýtvání → "Drahá bezpečnost brání útokům; dělá je zbytečnými."
* Úprava obtížnosti → "Více těžařů = rychlejší bloky = obtížnost stoupá; systém dýchá."
