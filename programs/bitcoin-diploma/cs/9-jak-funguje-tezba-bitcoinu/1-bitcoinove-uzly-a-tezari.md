# 9.1 Bitcoinové uzly a těžaři

Bitcoinové uzly mohou znít technicky, ale ve skutečnosti jsou to jen programy, které uchovávají kopii bitcoinového blockchainu na počítači. Blockchain je sdílený záznam všech bitcoinových transakcí.

Když provozujete vlastní uzel, ověřujete bitcoinové transakce sami, místo abyste důvěřovali někomu jinému. To vám dává větší nezávislost a pomáhá udržovat síť Bitcoin decentralizovanou.

Bitcoinový uzel si můžete představit jako digitálního dopravního policistu s několika důležitými úkoly.

1. Udržuje kopii blockchainu, což je historie všech bitcoinových transakcí.
1. Uzly se propojují s ostatními uzly po celém světě a sdílejí informace. Jedním příkladem je seznam nových transakcí čekajících na potvrzení, kterému se říká mempool.
1. Uzly kontrolují, že každá transakce dodržuje pravidla Bitcoinu. Pokud je transakce neplatná, uzel ji odmítne.

Uzly také pomáhají novým uzlům připojit se k síti tím, že s nimi sdílejí blockchain. Každý nový uzel však stále kontroluje všechna pravidla nezávisle.

Kdokoli může provozovat uzel instalací softwaru, například Bitcoin Core, a stažením blockchainu. Jakmile je vše nastaveno, uzel přijímá nové bloky přibližně každých 10 minut a ověřuje je, než je přidá do své kopie blockchainu.

Provozování uzlu pomáhá zvyšovat bezpečnost a decentralizaci bitcoinové sítě, protože více lidí nezávisle ověřuje systém.

#### Co je to bitcoinový uzel?

> Účelem těžby není vytváření nových bitcoinů; to je pouze motivační systém. Těžba je mechanismus, kterým je bezpečnost Bitcoinu decentralizována.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Těžaři shromažďují nepotvrzené transakce, vytvoří blok a využívají energii k nalezení klíče, který blok přidá a zabezpečí.


Těžaři soutěží o to, kdo přidá další blok transakcí do blockchainu. Aby to dokázali, musí najít speciální číslo, které vytvoří platný hash bloku. Můžete si to představit jako hledání správného klíče mezi miliardami možností. První těžař, který najde správný hash, vyhrává závod a získává právo přidat svůj blok do blockchainu.

Když těžař najde platný hash, sdílí svůj blok se sítí. Ostatní těžaři rychle ověří, že řešení je správné. Pokud ano, blok je přidán do blockchainu a pomáhá udržovat veřejnou účetní knihu Bitcoinu bezpečnou.

Těžaři vydělávají bitcoiny dvěma způsoby:

* **Odměny za blok:** Nové bitcoiny jsou vytvořeny a uděleny těžaři, který úspěšně přidá blok do blockchainu.
* **Transakční poplatky:** Když lidé posílají bitcoiny, připojují malý poplatek. Těžař, který přidá blok, získá poplatky z transakcí zahrnutých v tomto bloku.

#### Bitcoinové půlení


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Odměny těžařů za dokončení jednoho bloku se snižují na polovinu každých 210 000 bloků, což je přibližně každé čtyři roky.


Bitcoin má pevně stanovený maximální počet 21 000 000 bitcoinů, ale všechny nebyly vytvořeny při spuštění Bitcoinu. Místo toho jsou nové bitcoiny postupně uváděny do oběhu prostřednictvím **těžby**.

Když těžaři úspěšně přidají nový blok transakcí do bitcoinové sítě, obdrží **odměnu za blok** v bitcoinech. V počátcích Bitcoinu byla tato odměna 50 bitcoinů za blok. Tato odměna motivovala lidi využívat výpočetní výkon a elektřinu k zabezpečení sítě.

Přibližně každých 210 000 bloků (zhruba každé 4 roky) se odměna za blok sníží na polovinu. Tato událost se nazývá **půlení**. Půlení zpomaluje vytváření nových bitcoinů a pomáhá zajistit, že celkový počet nikdy nepřekročí 21 milionů. Postupem času to činí bitcoiny stále vzácnějšími.


> **Definition – Oběžné množství**
>
> **Oběžné množství** označuje celkové dostupné množství měny. U Bitcoinu je celkové oběžné množství počet mincí, které byly vytěženy a jsou v danou chvíli v oběhu.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/66192d7db275fec20d627456e43c9874cd142555-292x200.svg)


> **Definition – Plán emise bitcoinů**
>
> **Plán emise bitcoinů** je předem stanovený a veřejný plán uvolňování nových bitcoinů do oběhu, navržený tak, aby udržoval vzácnost Bitcoinu v průběhu času.


Po každém půlení se odměna v bitcoinech, kterou těžaři získávají za přidání bloku, sníží na polovinu. To snižuje rychlost, jakou jsou vytvářeny nové bitcoiny.

Těžaři stále získávají transakční poplatky z transakcí zahrnutých v bloku, který vytěží. Postupem času se očekává, že tyto poplatky budou tvořit větší část příjmů těžařů.

Halvingy jsou zabudovány do protokolu Bitcoinu a probíhají automaticky přibližně každé čtyři roky. Díky tomu je plán vydávání Bitcoinu předvídatelný a transparentní.

Tabulka ukazuje nadcházející halvingy, včetně přibližného data, čísla bloku, kdy k nim dojde, nové odměny za blok a procenta z celkové zásoby bitcoinů, které již byly vytěženy.


| Událost | Datum | Blok | Odměna | Vytěženo |
| --- | --- | --- | --- | --- |
| 5. halving | 2028 | 1 050 000 | 1,5625 BTC | 98,44 % |
| 6. halving | 2032 | 1 260 000 | 0,78125 BTC | 99,22 % |
| 7. halving | 2036 | 1 470 000 | 0,390625 BTC | 99,61 % |


Jak se těží více bitcoinů, oběžná zásoba stále roste, dokud není dosaženo maximálního množství 21 000 000 bitcoinů, což se očekává kolem roku 2140. Protože se v průběhu času vytváří méně nových bitcoinů, pokud poptávka roste, cena Bitcoinu může stoupat. To také motivuje těžaře, aby nadále zabezpečovali síť tím, že přispívají svým výpočetním výkonem.

#### Co je platný hash bloku v Bitcoinu?

V Bitcoinu těžaři soutěží o nalezení speciálního kódu zvaného **hash bloku**. Tento kód identifikuje blok transakcí a umožňuje jeho přidání do blockchainu.

Každý blok obsahuje informace o nedávných transakcích a také zahrnuje hash předchozího bloku. To propojuje všechny bloky dohromady a vytváří řetězec od úplně prvního bloku (Genesis Block) až po ten nejnovější.

Hash funguje jako **digitální otisk prstu** pro data v bloku. Pokud by se jakákoli informace v bloku změnila, otisk prstu by se také změnil. Díky tomu může kdokoli snadno ověřit, že historie transakcí v blockchainu nebyla změněna, a pomáhá to udržovat síť v bezpečí.


> **Callout**
>
> Satoshi Nakamoto, tvůrce Bitcoinu, vytěžil Genesis Block, který uvolnil celkem 50 bitcoinů.


#### Závod o vytěžení bloku

Těžaři soutěží o nalezení platného hashe bloku. První těžař, který jej najde, může přidat nový blok do blockchainu a získá odměnu v bitcoinech.

Aby byl hash platný, musí být nižší než číslo nastavené sítí, které se nazývá cílová obtížnost. Protože hashe jsou náhodné, těžaři musí zkoušet různé vstupy, dokud nenajdou ten správný.

Pokud by soutěžilo příliš mnoho těžařů, bloky by se nacházely příliš rychle. Pokud by se účastnilo příliš málo těžařů, nalezení bloku by trvalo příliš dlouho. Aby systém fungoval plynule, Bitcoin automaticky upravuje obtížnost každých 2 016 bloků (přibližně každé dva týdny).

Tato úprava zajišťuje, že v průměru je do blockchainu přidán nový blok přibližně každých 10 minut.


> **Definition – Definice úrovně obtížnosti**
>
> Úroveň **obtížnosti** v těžbě Bitcoinu měří, jak těžké je najít platný hash bloku. Síť tuto obtížnost upravuje každých 2 016 bloků (přibližně každé dva týdny), aby byly nové bloky přidávány do blockchainu zhruba každých 10 minut. Čím vyšší je obtížnost, tím těžší je pro těžaře najít platný blok.


Nalezením platného hashe bloku těžař dokazuje, že odvedl práci potřebnou k přidání nového bloku do blockchainu. Tento proces se nazývá **Proof of Work** (PoW). Je to bezpečnostní mechanismus, který umožňuje Bitcoinu potvrzovat transakce a přidávat nové bloky do blockchainu. Těžař, který jako první najde platný hash, získává odměnu v bitcoinech, která zahrnuje odměnu za blok a transakční poplatky z transakcí zahrnutých v tomto bloku.

Proof of Work (PoW) pomáhá udržovat Bitcoin v bezpečí tím, že je extrémně drahé pokusit se podvádět nebo ovládnout síť. Mnohem výhodnější je proto dodržovat pravidla.

Těžaři hrají čtyři hlavní role:

1. **Sbírají transakce**: Těžaři vybírají transakce, které byly odeslány do sítě, a vkládají je do kandidátního bloku.
1. **Provádějí Proof of Work**: Těžaři soutěží v řešení obtížné matematické hádanky nalezením platného hashe bloku.
1. **Vysílání bloku**: První těžař, který najde platné řešení, sdílí nový blok se sítí.
1. **Získání odměn**: Pokud je blok platný, je přidán do blockchainu a těžař obdrží nově vytvořený bitcoin a transakční poplatky.

Mnoho těžařů po celém světě se snaží vytvořit další blok současně. Když jeden těžař najde platné řešení, síť blok zkontroluje. Pokud je vše v pořádku, je přidán do blockchainu. Ostatní konkurenční bloky jsou zahozeny. Tento proces udržuje síť ve shodě a zabraňuje dvojímu utrácení.

* Těžaři jsou počítače, které pomáhají udržovat a aktualizovat účetní knihu Bitcoinu.
* Sbírají transakce a seskupují je do bloku. Poté data bloku proženou hashovacím algoritmem, aby vytvořili jedinečný kód zvaný hash.
* Těžaři tento proces opakují mnohokrát a hledají hash, který splňuje pravidla Bitcoinu. První těžař, který najde platný hash, získá nově vytvořený bitcoin jako odměnu a jeho blok je přidán do blockchainu.
* Hash každého bloku jej také propojuje s předchozím blokem. Pokud by se někdo pokusil změnit minulou transakci, hashe by již nesouhlasily a síť by upravený řetězec odmítla. To je to, co udržuje účetní knihu Bitcoinu bezpečnou.
