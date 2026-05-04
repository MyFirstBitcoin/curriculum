# 8.2 Metody analýzy účetní knihy

Protože transparentnost Bitcoinu je na rozdíl od tradičních finančních systémů — kde většina peněžních toků probíhá za zavřenými institucionálními dveřmi — vzniká zde bohaté pole on-chain analytiky, kde data na úrovni sítě slouží jako lupa pro pochopení chování uživatelů, peněžních toků a dlouhodobých trendů. Tyto metriky mohou pomoci odpovědět na konkrétní otázky, například jak aktivně je síť využívána, zda jsou mince akumulovány nebo prodávány, a zda se síť stává bezpečnější.

Porozumění těmto metrikám je užitečné nejen pro uživatele Bitcoinu, ale také pro výzkumníky nebo tvůrce politik, kteří hledají vhled do tohoto jedinečně transparentního finančního systému.

Tato sekce obsahuje některé běžně používané metriky pro analýzu aktivity Bitcoinu rozdělené do podkategorií. Nejedná se o úplný seznam. Navštivte [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) pro úplnější seznam a popisy.



#### 8.2.1 Metriky adres

Metriky adres je užitečné sledovat v čase, protože ukazují úroveň aktivity v síti Bitcoinu. Například s rostoucím přijetím Bitcoinu roste počet aktivních adres. Můžeme to dále zkoumat tím, že vyfiltrujeme počet adres, které drží minimálně stanovené množství Bitcoinu, například 0,1 BTC, v určitém časovém období, například za jeden rok. I když to poskytuje pohled na adopci Bitcoinu v čase, je to nedokonalé, protože jeden člověk může vlastnit více bitcoinových adres. Naopak burzy nebo ETF se mohou jevit jako jediný subjekt, i když drží prostředky pro velké množství jednotlivců.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adresy držící Bitcoin > X BTC podle roku. Zdroj: Bitcoin Magazine Pro._

Porovnáním adres s aktuální tržní cenou BTC je možné zobrazit procento všech bitcoinových adres, které jsou v zisku. To nám umožňuje sledovat náladu na trhu, protože vidíme, jaká část trhu drží BTC se ziskem nebo se ztrátou.

Například, **Procento nerealizovaného zisku** na grafu níže ukazuje podíl všech adres v účetní knize s nerealizovaným ziskem měřeným v amerických dolarech. Všimněte si, že protože graf níže byl pořízen blízko historického maxima Bitcoinu, procento adres vykazujících nerealizovaný zisk je téměř sto procent. Také vidíme, že dlouhá období, kdy Procento nerealizovaného zisku klesne pod jednu směrodatnou odchylku od průměru, jsou neobvyklá. Proto pokles pod tuto linii může naznačovat vhodný vstupní bod pro kupující.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Procento nerealizovaného zisku. Zdroj: checkonchain.com_



#### 8.2.2 On-chain indikátory

On-chain indikátory jsou užitečné, protože nabízejí pohled na chování sítě, který samotné cenové a adresní metriky nemohou poskytnout. Pomáhají analytikům pochopit akce a nálady různých typů účastníků, například dlouhodobých držitelů oproti krátkodobým obchodníkům, tím, že sledují, jak jsou mince drženy, přesouvány nebo oceňovány v čase. Tyto indikátory využívají transparentní povahu účetní knihy k odhalení skrytých tržních dynamik, jako je akumulace, distribuce nebo dokonce přesvědčení investorů. Díky tomu jsou zvláště užitečné pro identifikaci strukturálních trendů, posouzení, zda je trh přehřátý nebo podhodnocený, a předvídání obratů v tržním cyklu.

Například zkoumáním hodnoty BTC držených od poslední transakce můžeme odvodit, zda je trh pod tlakem (například během hlavního cyklického minima). Tato metrika je známá jako **Realizovaná cena** a poskytuje nám „průměrnou pořizovací cenu“ všech BTC v oběhu. Pokud tržní cena klesne pod Realizovanou cenu, znamená to, že většina adres je v souhrnu ve ztrátě.

Dalším seskupením dat z účetní knihy do věkových pásem můžeme ukázat, jak se množství BTC v čase přesouvá mezi adresami, což vytváří vlnovité vzory na grafu známém jako **HODL vlny**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL vlny. Zdroj: Bitcoin Magazine Pro._

HODL vlny ukazují, co dlouhodobí, střednědobí a krátkodobí držitelé dělají se svými BTC. Například na grafu výše jsou krátkodobí držitelé zobrazeni červeně a oranžově a vidíme špičky aktivity, když tato skupina spěchá nakupovat blízko tržních vrcholů. Na druhé straně vidíme, že velmi dlouhodobí držitelé (fialově a modře) postupně zvyšují svůj celkový podíl v síti, což ukazuje na silné přesvědčení těchto skupin. Graf je nedokonalý, protože některé mince se mohou přesouvat ze starých na nové adresy pod kontrolou stejného uživatele. Přesto poskytuje zajímavý pohled na přesvědčení dlouhodobých držitelů.

Dalším způsobem, jak zkoumat „chytré peníze“ dlouhodobých držitelů, je sledovat **Zničené dny mincí** (CDD). Koncept „dnů mincí“ je násobek počtu BTC a počtu dní od posledního pohybu mincí. Například 5 BTC, které se nepohnuly 100 dní, má 500 dní mincí, a 10 BTC, které se nepohnuly 10 dní, má 100 dní mincí. Tímto způsobem dáváme větší váhu mincím drženým déle. Když jsou tyto mince přesunuty, tyto dny mincí jsou „zničeny“. Tento indikátor ukazuje nárůsty CDD v obdobích významných cenových pohybů, což analytikům umožňuje odlišit rutinní tržní aktivitu od významných posunů v sentimentu dlouhodobých držitelů.

Další metrika, která může pomoci určit, zda je trh podhodnocený nebo nadhodnocený, je poměr tržní hodnoty k realizované hodnotě, neboli **MVRV**. Vypočítá se jednoduše jako poměr tržní hodnoty (počet BTC v oběhu krát tržní cena) děleno realizovanou hodnotou (součet všech BTC od jejich posledního pohybu). Vysoké MVRV naznačuje, že více mincí je v zisku (často viděno u tržních vrcholů) a nízké MVRV znamená, že mnoho mincí je drženo se ztrátou (viděno u tržních minim).



#### 8.2.3 Metriky těžby

Metriky těžby jsou užitečné pro pochopení bezpečnosti, ekonomických pobídek a celkového zdraví bitcoinové sítě. Metriky jako hashrate, příjmy těžařů, obtížnost a poměry poplatků ukazují, kolik výpočetního výkonu zajišťuje blockchain a jak dobře jsou těžaři za svou činnost odměňováni.

Nejčastěji zmiňovaným indikátorem zdraví sítě a síly zabezpečení je **Hashrate** bitcoinové sítě. Protože proces těžby zajišťuje síť a potvrzuje, že transakce v účetní knize jsou platné, čím větší je úroveň výpočetního (nebo hashovacího) výkonu, tím obtížnější by bylo pro škodlivého aktéra síť přemoci a napadnout.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Zdroj: Bitcoin Magazine Pro._

Graf výše ukazuje, že v květnu 2025 činí celkový výpočetní výkon sítě přibližně 900 TeraHash/s (900 bilionů kryptografických „hashovacích“ výpočtů za sekundu). Pokud hashrate roste, znamená to, že síť je bezpečnější, což je pro uživatele uklidňující.

Puellův násobek (vytvořený Davidem Puellem) se dívá na tržní cyklus z pohledu těžařů a jejich příjmů. Metrika se vypočítá vydělením denní emise BTC (v USD) 365denním klouzavým průměrem denní hodnoty emise. Tato metrika pomáhá identifikovat období stresu nebo úlevy těžařů. Historicky násobek nad 3 předcházel poklesu tržní hodnoty BTC, protože naznačuje, že těžaři jsou vysoce ziskoví. Hodnota pod 0,5 značí stres a historicky signalizovala tržní minima hodnoty BTC.
