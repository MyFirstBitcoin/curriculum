# 8.1 Povaha účetní knihy Bitcoinu

Bitcoinova účetní kniha transakcí (alternativně nazývaná timechain nebo blockchain) je veřejně přístupný, časově označený záznam každé platné transakce, která kdy na síti proběhla. V tradičním finančním systému jsou interní transakce viditelné pouze oprávněným účastníkům, jako jsou banky, regulátoři nebo provozovatelé dat jako SWIFT, BACS nebo SEPA. Přístup k údajům o platbách v tradičních systémech může být velmi omezený a drahý.

Naopak v síti Bitcoin si může každý s připojením k internetu prohlédnout každou transakci, od největší hodnoty až po jednotlivý Satoshi. Účastníci mohou v reálném čase sledovat celkovou nabídku bitcoinů, monitorovat aktivitu adres a peněženek a zobrazovat odměny těžařů a chování poplatků. Zatímco viditelná aktivita v účetní knize je spojena s adresami veřejných klíčů a ne s konkrétními identitami, je možné agregovat velké datové sady o chování při utrácení, což umožňuje každému shromažďovat a zkoumat ekonomickou aktivitu v reálném čase. Jak síť roste a je více přijímána jako zdroj ekonomické pravdy, můžeme pozorovat menší závislost na státních orgánech a poskytovatelích třetích stran při tvorbě statistických analýz a zpráv o chování při utrácení.



#### 8.1.1 Uzly a blokové průzkumníky

Každý, kdo si přeje nezávisle ověřit Bitcoinovou účetní knihu a přistupovat k jejím údajům, by měl provozovat plný uzel. Plný uzel je často popisován jako nejzákladnější způsob, jak se účastnit a ověřovat Bitcoinovou ekonomiku. Je celosvětově dostupný jako open-source software, který po spuštění stáhne a ověří celou Bitcoinovou účetní knihu od „Genesis Blocku“, zveřejněného v lednu 2009, až do současnosti. Také podporuje bezpečnost Bitcoinové sítě tím, že pomáhá ověřovat nové transakce přidávané do účetní knihy. Přístupem k Bitcoinové účetní knize tímto způsobem slouží plný uzel jako zdroj pravdy pro výzkumníky a auditory sítě. A pro uživatele Bitcoinu plní plný uzel roli „suverénní“ brány k transakčním informacím Bitcoinové ekonomiky, protože zvyšuje soukromí a bezpečnost tím, že odstraňuje závislost na službách třetích stran.

Zatímco plné uzly stahují surová data, blokové průzkumníky jako mempool.space nebo blockstream.info nabízejí vizuální rozhraní pro vyhledávání a interpretaci aktivity v účetní knize. Blokový průzkumník umožňuje sledovat jednotlivé transakce a zobrazovat zůstatky a historii peněženek. Zobrazuje také metriky aktivity těžařů, jako jsou odměny za bloky a údaje o transakčních poplatcích.

Společně jsou plné uzly a blokové průzkumníky nástroje, které činí transparentnost Bitcoinové sítě využitelnou.



#### 8.1.2 Aktivita: Prozkoumání Bitcoinové účetní knihy

1. Otevřete [mempool.space](https://mempool.space) a prozkoumejte domovskou stránku.
  * Jaká je výška posledního bloku?
  * Jaký je aktuální transakční poplatek (nízká, střední a vysoká priorita)?
  * Kolik transakcí čeká v mempoolu na další blok?
1. Přistupte k poslednímu bloku v účetní knize.
  * Kolik transakcí bylo zahrnuto?
  * Jaký těžař vytěžil tento blok?
  * Jaká byla odměna za blok?
1. Přistupte k transakci v bloku.
  * Kolik vstupů a výstupů má tato transakce?
  * Jaká je hodnota transakce v BTC a CZK?

Diskutujte rozdíly mezi tím, jak se peníze pohybují v tradičním systému, a tím, jak podnik nebo vláda využívá tento druh transparentnosti.
