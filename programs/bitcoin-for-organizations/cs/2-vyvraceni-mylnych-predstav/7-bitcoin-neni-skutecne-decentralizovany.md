# 2.7 Bitcoin není skutečně decentralizovaný

> Složitost kryptoměn vychází ze snahy o decentralizaci—distribucí moci a správy v systému teoreticky odpadá potřeba důvěryhodných zprostředkovatelů, jako jsou finanční instituce. To byl základní předpoklad původního white paperu Bitcoinu, který nabídl kryptografické řešení umožňující posílat platby bez zapojení jakékoli finanční instituce nebo jiného důvěryhodného prostředníka. Nicméně Bitcoin se velmi rychle centralizoval a nyní závisí na malé skupině softwarových vývojářů a těžebních poolů, aby mohl fungovat.  
_Mezinárodní měnový fond_

Jak ukazuje výše uvedený citát z poměrně nedávného příspěvku Mezinárodního měnového fondu, hlavní finanční průmysl stále tvrdí, že Bitcoin není decentralizovaný, a zároveň zaměňuje Bitcoin s ostatními kryptoměnami.

##### Úvod

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/15f4dcae71ffb4d166aa2eda824def835c5beb36-161x167.svg)

Decentralizace je klíčovým aspektem Bitcoinu. Schopnost udržovat pravidla protokolu, jako je vzácnost a distribuce, bez centrální autority zajišťuje, že může fungovat jako bezpovolené peníze pro globální společnost.

Jak Satoshi poznamenal ve své online korespondenci, decentralizované služby jako BitTorrent „si vedly dobře“ proti zásahům vlád, na rozdíl od služeb s identifikovaným vlastníkem a centralizovanými servery. Zjevně se obával potenciálního rizika, že vlády nebo jiné zájmy by mohly Bitcoin vypnout nebo jinak negativně ovlivnit.

V tomto kontextu nás zajímá decentralizace:

* Vývoje a správy kódu, který řídí protokol; kdo smí měnit pravidla?
* Těžební funkce, která vytváří nové bloky v souladu s pravidly a ověřuje proti dvojímu utracení
* Uzlů, které ověřují transakce z hlediska platnosti a uchovávají kopii blockchainu

##### Vývojáři

Bitcoin je open-source protokol, na který se může kdokoli podívat, stáhnout si ho, zkopírovat nebo navrhnout změny. Je dostupný v knihovně GitHub, přičemž zdrojový kód byl původně spuštěn v roce 2009 Satoshim Nakamotem. Každý si může kód stáhnout a spustit uzel, přičemž většina běží na původním softwaru Bitcoin Core, který byl v průběhu času aktualizován.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Zdroj: https://river.com/learn/what-is-bitcoin-core/_

Vývoj Bitcoin Core se řídí nejlepšími postupy open source vývoje. V kterémkoli okamžiku může být libovolný počet vývojářů, kteří píší nebo kontrolují změny kódu. Musí naslouchat připomínkám provozovatelů uzlů a těžařů, stejně jako uživatelské základně, než provedou jakoukoli zásadní změnu v kódu, která bude přezkoumána a schválena, jak je znázorněno ve výše uvedeném diagramu, než se dostane do kódu.

Pravidla Bitcoinu jsou pak zakódována v tomto softwaru Bitcoin Core, který běží na každém uzlu. Každý může navrhnout změnu pravidel – pravidla jsou kód, ale nejsou_pouze_kód, jsou_dohodnutý_kód. Pokud by byla změněna jednostranně, nový kód již není součástí konsenzu a není již součástí Bitcoinu. Změnit něco na Bitcoinu a zůstat v konsenzu je složité. Navrhované změny kódu spadají do jedné ze tří kategorií:

* V rámci stávajících pravidel: Menší vylepšení, jako jsou opravy překlepů, lepší uživatelské rozhraní nebo správa dat, mohou spadat do této kategorie a je relativně snadné je schválit.
* Přidání nového pravidla, které přidává omezení k pravidlům – například snížení velikosti bloku. Toto se označuje jako „soft fork“. Uzly, které se rozhodnou neimplementovat změnu kódu a zůstanou na staré verzi, se stále mohou účastnit sítě.
* Přidání nového pravidla, které porušuje současná pravidla, např. zvýšení velikosti bloku. Uzly, které neupgradují na nový kód, označí blok vytvořený s větší velikostí za neplatný. Toto se označuje jako „hard fork“ a způsobí rozdělení řetězce mezi uzly běžící na původním a novém kódu a vznik nové mince. To se již v minulosti stalo, ale nikdy to nevedlo k dlouhodobému úspěchu nové mince, protože většina uzlů se rozhodla zůstat u původního kódu.

Proto žádná jednotlivá strana ani skupina lidí nemůže jednostranně změnit kód Bitcoinu bez dosažení konsenzu, jinak riskuje rozdělení řetězce a vznik nové mince podle jiných pravidel.

##### Těžba

Těžební funkce ověřuje transakce stejně jako jakýkoli jiný uzel v síti, ale poté vynaloží energii potřebnou k vytvoření nového bloku, který splňuje konsenzuální pravidla v kódu. Úspěch umožňuje těžaři získat odměny ve formě transakčních poplatků a odměn v Bitcoinu (v době psaní 3,125 mincí za blok).

Těžba se obvykle provádí prostřednictvím těžebních „poolů“, kde lidé sdružují těžební výkon nebo hash rate, aby zvýšili šanci na úspěšné vytěžení bloku a sdíleli odměny. Existuje riziko, že jeden nebo více těchto těžebních poolů by se mohlo spojit a dosáhnout 51% dominance v těžbě a v podstatě přehlasovat validační protokol sítě ve svůj prospěch, aby mohli dvakrát utratit mince. To by vyžadovalo obrovské množství zdrojů za vysokou cenu a jednotliví těžaři mohou kdykoli snadno přejít do jiného poolu. Takový útok by pravděpodobně také způsobil pád hodnoty bitcoinu, protože by bylo zřejmé, že integrita sítě byla narušena. Útočník by proto musel jakýkoli získaný bitcoin rychle převést na fiat, než jeho hodnota klesne. To by útok ještě více ztížilo udržet po delší dobu, a proto je pro těžaře nebo provozovatele poolu výhodnější dodržovat pravidla a snažit se těžit platné bloky.

Důležitá je také geografická distribuce těžební funkce, aby například vlády nemohly převzít těžební kapacitu nebo ji vypnout. Například nedávný zákaz těžby v Číně ukázal schopnost Bitcoinu přizpůsobit se a přežít takový zásah vlády, když se rychle přizpůsobil a zotavil z následné ztráty hash rate.

##### Uzly

Na rozdíl od těžby, která vyžaduje značnou finanční investici k efektivnímu soupeření v závodě o těžbu nových bloků, nebo vývoje kódu, který vyžaduje programátorské znalosti, provozování uzlu je něco, co může udělat kdokoli, kdo má zájem pomoci udržet decentralizaci Bitcoinu.

Uzly provozují software Bitcoin Core a vynucují pravidla, která kód obsahuje, aby zajistily, že těžaři nepodvádějí, například tím, že by si přidělili větší odměnu za blok, než je povoleno. Také vynucují limit nabídky 21 milionů, což je zásadní pro udržení vzácnosti Bitcoinu. Aby vláda nebo škodlivý aktér zastavil Bitcoin, musel by zničit každou jednotlivou kopii blockchainu, která v současnosti běží na tisících uzlů po celém světě, což je téměř nemožný úkol.

##### Lidé

Dalším aspektem potenciální centralizace jsou lidé. Každý jiný „altcoin“ má svého vůdce—někoho, koho by bylo možné přinutit prosazovat změny, které nejsou v nejlepším zájmu Bitcoinu. Satoshi Nakamoto zůstal dostatečně dlouho, aby zajistil, že Bitcoin je na cestě k úspěchu, a poté navždy zmizel, čímž jej ponechal v rukou ostatních, aby software vylepšovali a přizpůsobovali.

A co držitelé velkého množství Bitcoinu? Raní investoři, kteří své mince drželi a neztratili je, jsou v tuto chvíli extrémně bohatí. Je důležité poznamenat, že to může být pravda, ale to jim nedává větší vliv na systém než komukoli jinému, na rozdíl od „proof of stake“ mincí, kde raní uživatelé, kteří už jsou v dané minci bohatí, získávají výhody při rozhodování a distribuci budoucích mincí. To nevyhnutelně vedlo nebo povede k centralizaci v průběhu času.

##### Závěr

Jaké jsou potenciální hrozby, které může decentralizace pomoci zmírnit?

* Vláda vypínající nebo zakazující Bitcoin
* Nežádoucí změny kódu, které zvýhodňují jednu skupinu zájmů v Bitcoinu, např. zvýšení odměny za blok
* Nátlak na protokol ze strany vlády nebo škodlivých aktérů s cílem ovlivnit směřování protokolu
* Schopnost skupiny těžařů převzít síť a „dvakrát utratit“ Bitcoin – útok 51 %

Jak vidíme, kombinace uzlů, vývojářů kódu a těžařů, stejně jako použití mechanismu „proof of work“, decentralizuje Bitcoin na dostatečné úrovni, aby tyto potenciální hrozby nebyly považovány za zásadní. Komunita bude muset situaci nadále sledovat, aby tomu tak zůstalo.
