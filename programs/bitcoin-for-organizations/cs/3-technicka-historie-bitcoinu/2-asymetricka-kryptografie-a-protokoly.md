# 3.2 Asymetrická kryptografie a protokoly

Dnešní internet a většina moderních počítačových systémů spoléhají na kryptografii, což je metoda zakrývání informací tak, aby je mohl rozluštit pouze příjemce. Základy kryptografie, která se používá k zabezpečení Bitcoinu, lze vystopovat až do 70. let.

Prvním problémem, který je třeba vyřešit, je – jak poslat sdílené tajemství přes nezabezpečené médium.

Tímto se poprvé zabývali Whitfield Diffie a Martin Hellman.

Problém: dvě strany – obvykle označované jako Alice a Bob – chtějí sdílet tajné informace přes síť, kde mohou ostatní odposlouchávat. Aby toho dosáhli, vytvořili proces výměny klíčů Diffie-Hellman.

Toto sdílené tajemství pak může být použito jako počáteční hodnota pro vytvoření mnoha symetrických klíčů k šifrování a dešifrování zpráv, které si mohou navzájem posílat, aniž by museli klíč sdílet veřejně.

Protože soukromý klíč nikdy nemusí být sdílen a na každé straně se používají různé klíče pro šifrování a dešifrování, nazývá se tento postup asymetrický šifrovací algoritmus.

Příklady použití:

* Alice podepíše zprávu Bobovým veřejným klíčem – pouze on ji může dešifrovat pomocí svého soukromého klíče
* Alice podepíše zprávu svým soukromým klíčem – dešifrováním jejím veřejným klíčem může kdokoli ověřit, že zprávu poslala Alice, aniž by znal její soukromý klíč
* Kombinací těchto dvou přístupů se dvěma vrstvami šifrování lze poslat zprávu zašifrovanou tak, že ji může dešifrovat pouze Bob, a on pak může ověřit, že odesílatelem byla skutečně Alice.

Ačkoli nebyl na původním článku uveden jako autor, Ralph Merkle byl zásadní při řešení toho, co bylo do té doby považováno za neřešitelný problém – jak navázat nebo obnovit soukromou komunikaci přes otevřenou a potenciálně nepřátelskou síť.

Tento přístup je sám o sobě náchylný k útoku hrubou silou, kdy útočník může vzít sdílená čísla a nakonec s dostatkem času a prostředků znovu vytvořit sdílený klíč, takže sám o sobě není úplným řešením.

##### Protokoly pro kryptosystémy s veřejným klíčem

Kromě přispění k systému veřejného klíče Diffie-Hellman popsanému výše, **Ralph Merkle** pokračoval v přispívání do této oblasti po mnoho let a byl zásadní při vývoji některých klíčových komponent, které využívá Bitcoin.

Kryptografická hashovací funkce je matematický algoritmus, který přijímá vstupy libovolné velikosti a provádí složité výpočty, aby vrátil hash hodnotu v bitech, která je obvykle reprezentována jako výstup pevné délky v alfanumerickém tvaru pomocí šestnáctkové soustavy.

* Vstupy mohou být libovolné velikosti
* Výstup má vždy pevnou délku a je deterministický (stejný vstup vytvoří pokaždé stejný hash)
* Je snadné ověřit, ale mimořádně obtížné obrátit proces a zjistit původní vstup
* I drobná změna dat zcela změní výstup

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/d5e7c17d10c9aa7fced939a9c9460f1e9d7bb663-515x331.svg)

Hashování je nedílnou součástí protokolu Bitcoinu. SHA-256, používaný v Bitcoinu, byl vytvořen NSA a je příkladem kryptografického hashovacího algoritmu.

* Každý blok v řetězci je hashován tak, aby data nemohla být změněna – což zajišťuje integritu distribuované účetní knihy
* Vygenerovaný hash musí splňovat kritéria „důkazu práce“ (Proof of Work), aby byl blok považován za platný
* Merkleovy stromy – použitím větvení a hashů hashů umožňují hashovací stromy ověřování velkých datových sad s minimálním úložištěm
* Hashovací podpisy a klíče lze použít pro peněženky, adresy a autorizaci transakcí

Distribuované ověřování stavů blockchainu a modely účetních knih pouze pro přidávání odolné vůči zpětným úpravám jsou umožněny jednosměrným hashováním. Hashovací funkce poskytují spolehlivý, deterministický způsob ověřování událostí na veřejných účetních knihách, jako je Bitcoin, bez potřeby centralizovaného modelu důvěry.

Od těchto nových možností v oblasti kryptografie si jejich tvůrci slibovali příchod nové vlny inovací v této oblasti.

##### Kryptografie eliptických křivek

Jednou z těchto pozdějších inovací byla kryptografie eliptických křivek.

Kryptografie eliptických křivek byla představena v roce 1985 dvěma vědci, N. Koblitzem a V. Millerem. Navrhli myšlenku použití bodů definovaných eliptickými křivkami místo konečných prvočíselných polí, aby platil předpoklad problému diskrétního logaritmu, jak je běžně používán ve standardním protokolu výměny klíčů Diffie-Hellman. Podrobnosti o tom, jak to funguje, přesahují rámec této části, ale na vysoké úrovni je eliptická křivka množina bodů, které splňují určitou matematickou rovnici.

Rovnice eliptické křivky vypadá například takto:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

To má několik užitečných vlastností:

* Horizontální symetrie. Každý bod na křivce lze zrcadlit přes osu x a zůstane na stejné křivce.
* každá nevertikální přímka protne křivku maximálně ve třech bodech.
* Kompaktní velikosti klíčů jsou zásadní pro efektivní ukládání a přenos veřejných klíčů v blockchainu.

Tyto vlastnosti lze využít k vytváření párů klíčů podobně jako u algoritmu Diffie-Hellman. Bitcoin používá ECDSA, což je zkratka pro Elliptic Curve Digital Signature Algorithm. Je to proces, který využívá eliptickou křivku a konečné pole k „podepisování“ dat takovým způsobem, že třetí strany mohou ověřit pravost podpisu, zatímco podepisující má výhradní možnost podpis vytvořit. U bitcoinu jsou podepisovanými daty transakce, které převádějí vlastnictví.

Část „konečné“ je podobná přístupu „mod“ u Diffie-Hellmana, kde je výstup rovnice dělen a zbytek je použit k zajištění, že výsledek spadá do určitého rozsahu čísel.
