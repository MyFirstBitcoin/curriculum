# 8 - Jak Bitcoin funguje

Délka: 90 minut

Hlavní myšlenka: Bezpečnost Bitcoinu závisí na jednoduchých, ale silných technických principech, jako jsou klíče, podpisy, hashování a UTXO, které umožňují vlastnictví a ověřování bez centrální autority.

#### Výukové cíle

Na konci této lekce by studenti měli být schopni:

* Vysvětlit, jak veřejné a soukromé klíče pomáhají zabezpečit vlastnictví a transakce Bitcoinu.
* Popište, co je digitální podpis a jak dokazuje, že transakce byla autorizována oprávněným vlastníkem.
* Vysvětlete jednoduchými slovy, co znamená kryptografie, šifrování a dešifrování v kontextu Bitcoinu.
* Definujte hashování a popište, proč jsou hashovací funkce důležité pro bezpečnost a integritu dat Bitcoinu.
* Identifikujte základní vlastnosti hashovací funkce, jako je výstup pevné délky, jednosměrnost a citlivost na malé změny vstupu.
* Vysvětlete model UTXO a jak jsou bitcoiny utráceny, přijímány a vraceny jako drobné prostřednictvím výstupů transakcí.
* Popište, jak uzly pomáhají zabránit dvojímu utrácení tím, že kontrolují, zda již výstup nebyl utracen.

#### Nástroje a zdroje

##### Vizuální pomůcky

* Kapitola 8 – Jak Bitcoin funguje

##### Podpůrná knihovna

* Slovníček pojmů — Kapitola 8 — Termíny: kryptografie, hash, UTXO, digitální podpis, soukromý/veřejný klíč, merkle tree, blockchain
* Knihovna omylů — Kapitola 8 — Adresuje: „ztracenou seed frázi lze obnovit“, „soukromý klíč = heslo“, „blockchain je anonymní“
* Technické vysvětlivky a podrobnosti — Hashovací funkce, veřejné/soukromé klíče, model UTXO, bezpečnost Proof of Work

#### Aktivity

* Transakce v praxi
* Zkoumání mempoolu

#### Online výuka

* Použijte digitální tabuli a kreslete každý koncept živě místo pouhého slovního vysvětlování.
* Učte jednu technickou myšlenku najednou a často dělejte pauzy na kontrolní otázky.
* Používejte vizuální pomůcky pro klíče, podpisy, hashe a UTXO, aby studenti mohli sledovat strukturu.
* Držte se konceptuální úrovně a vyhněte se přílišné matematice nebo žargonu.

#### Příprava

* Připravte a zalaminujte diagramy: páry veřejného/soukromého klíče, digitální podpisy, model UTXO, hashování (jednosměrná funkce).
* Připravte si záložky na blockchain explorer a SHA-256 hash kalkulačku; vyberte 2–3 skutečné Bitcoin transakce k podrobnému rozboru.
* Připravte si poznámky na tabuli pro vysvětlení vstupů, výstupů a jak se transakce potvrzují na blockchainu.

#### Postup

Tato lekce dává studentům první pohled na technickou stránku Bitcoinu bez předpokladu předchozích technických znalostí. Průvodce nyní následuje stejnou zhuštěnou strukturu jako Diplom, přičemž kryptografie je seskupena pod jednu hlavičku a UTXO pod druhou.

##### 8.0 Úvod, 8 minut

Začněte nastavením očekávání:

* Co dělá Bitcoin bezpečným, když ho neřídí žádná centrální banka?
* Jak může síť vědět, že osoba skutečně vlastní bitcoiny, které se snaží odeslat?
* Co se vlastně děje na pozadí, když někdo provede Bitcoin transakci?

Ujasněte, že tato kapitola se zaměřuje na základní technické základy Bitcoinu, zejména klíče, podpisy, hashování a UTXO. Také ujistěte studenty, že nemusí být inženýry, aby pochopili základní logiku. Kapitola to jasně ukazuje přirovnáním Bitcoinu k internetu – mnoho lidí ho používá každý den, aniž by rozuměli všem jeho vrstvám.

##### 8.1 Bezpečnost díky kryptografii, 57 minut

**Bitcoin jako účetní kniha uložená na mnoha počítačích**

Začněte jednoduchým rámcem této kapitoly o síti Bitcoinu:

* Bitcoin je záznam transakcí
* tento záznam je uložen na mnoha počítačích zvaných uzly
* účetní kniha je veřejná a pseudonymní
* zobrazuje adresy a historii transakcí, ne osobní údaje

Tato část pomáhá studentům navázat na to, co už znají z předchozích kapitol. Bitcoin není založen na skrytých účtech v bance. Je založen na sdílené účetní knize, kterou může ověřit mnoho účastníků. je zde obzvlášť užitečný, protože ukazuje uživatele, peněženky a širší Bitcoin síť propojenou s veřejnou účetní knihou.

**Veřejné a soukromé klíče**

Nyní přejděte ke kryptografii.

Vysvětlete, že každý uživatel Bitcoinu má:

* soukromý klíč, který musí zůstat v tajnosti
* veřejný klíč, který lze sdílet

Vysvětlete jejich účel jednoduše:

* soukromý klíč dokazuje vlastnictví a umožňuje utrácení
* veřejný klíč pomáhá ostatním ověřit, že transakce byla správně autorizována

Silným výukovým bodem této kapitoly je, že Bitcoin používá kryptografii s veřejným a soukromým klíčem, nikoli starší model, kde si dva lidé musí nejprve sdílet stejný tajný klíč. To je důležité, protože to umožňuje bezpečné ověření bez nutnosti odhalit tajemství, které chrání jejich prostředky.

Můžete to vysvětlit takto:

* soukromý klíč je jako tajný důkaz, že bitcoin patří vám
* veřejný klíč je součástí toho, co umožňuje síti ověřit vaše oprávnění
* kdo ovládá soukromý klíč, ovládá možnost utratit bitcoin

Dávejte pozor, abyste zde příliš nekomplikovali jazyk šifrování. Nejpodstatnější pro studenty je vlastnictví a oprávnění.

**Digitální podpisy a autorizace transakcí**

Nyní vysvětlete, co se stane, když někdo pošle bitcoin.

Použijte posloupnost z kapitoly:

* uživatel vytvoří transakci
* odesílatel vytvoří digitální podpis pomocí svého soukromého klíče
* transakce je rozeslána do sítě
* uzly ověřují, že podpis je platný
* po ověření a potvrzení je vlastnictví převedeno v účetní knize

Ujistěte se, že digitální podpis není totéž jako napsat své jméno. Je to kryptografický důkaz, že skutečný vlastník transakci autorizoval. Toto je jeden ze základních mechanismů, které umožňují Bitcoinu fungovat bez centrální autority, která by transakce schvalovala ručně. Schéma je užitečné, protože vizuálně ukazuje podepisování a ověřování i cestu transakce od odesílatele k ověření sítí.

Dobrá věta do výuky je:

Bitcoinové transakce nejsou schvalovány proto, že to řekne banka. Jsou přijímány, protože síť dokáže ověřit platný kryptografický důkaz.

**Hashování a jednosměrné funkce**

Nyní vysvětlete hashování.

Začněte jednoduše:

* funkce vezme vstup a vytvoří výstup
* jednosměrná funkce se snadno provede jedním směrem, ale prakticky nelze obrátit
* hashovací funkce vezme data libovolné velikosti a převede je na výstup pevné délky zvaný hash

Použijte jednu z analogií z kapitoly, která je pro vaše publikum nejjasnější:

* analogie smoothie pro jednosměrné funkce
* analogie otisku prstu pro hashe
* analogie hudební partitury pro kontrolu, zda se něco změnilo

Analogie otisku prstu je pravděpodobně pro většinu tříd nejjasnější:

* hash je jako digitální otisk prstu pro data
* pokud se vstup změní byť jen trochu, hash se úplně změní
* to pomáhá počítačům kontrolovat integritu a odhalit manipulaci

Poté vysvětlete, proč je hashování v Bitcoinu důležité:

* transakce jsou hashovány
* síť používá hashe k ověření integrity
* pokud se transakce změní, hash se změní
* to pomáhá chránit účetní knihu před nepozorovanou manipulací

Vizuály na stranách 7 až 10 jsou zde velmi užitečné. Kapitola ukazuje jak myšlenku výstupu pevné délky, tak princip „malá změna, úplně jiný výsledek“, což je jeden z nejdůležitějších konceptů, které by studenti měli pochopit.

**Základní vlastnosti hashovacích funkcí**

Stručně projděte vlastnosti zvýrazněné v kapitole, aniž byste je dělali příliš akademické:

* Deterministická: stejný vstup dává vždy stejný výstup
* Jednosměrná / odolnost vůči zpětnému získání: proces nelze realisticky obrátit
* Citlivá na změnu: i malá změna vstupu vytvoří velmi odlišný výstup
* Odolnost vůči kolizím: je extrémně obtížné najít dva různé vstupy se stejným výstupem
* Rychlá na ověření: funkce je efektivní na spuštění i kontrolu

Není třeba, aby si studenti pamatovali každý pojem, ale měli by pochopit hlavní myšlenku: hashování dává Bitcoinu spolehlivý způsob, jak identifikovat data a detekovat změny.

##### 8.2 Model UTXO, 25 minut

**UTXO model**

Nyní přejděte k druhé hlavní části kapitoly: UTXO, neboli nevydané výstupy transakcí.

Vysvětlete to jednoduše pomocí peněžní analogie z kapitoly:

* bitcoin se nesleduje pouze jako zůstatek na bankovním účtu
* místo toho je tvořen utratitelnými částmi zvanými UTXO
* když utrácíte bitcoin, použijete jeden nebo více existujících UTXO jako vstupy
* poté jsou vytvořeny nové UTXO jako výstupy

Použijte příklad z kapitoly:

* pokud máte UTXO v hodnotě 10 BTC
* a pošlete 6 BTC
* nový UTXO v hodnotě 6 BTC jde příjemci
* nový UTXO jako drobné se vrací vám
* malá část je zaplacena jako poplatek těžaři

To pomáhá studentům pochopit, že Bitcoin funguje spíše jako utrácení hotovosti a vracení drobných než jako odečítání čísel z jednoduchého účtu. Diagramy jsou zde obzvlášť silné, protože vizuálně ukazují, jak se jeden UTXO rozděluje na výstup pro příjemce, výstup pro drobné a poplatek.

Zdůrazněte dva klíčové body:

* zůstatek vaší peněženky je součtem vašich UTXO
* když utrácíte, staré UTXO jsou spotřebovány a vznikají nové

**Zabránění dvojímu utrácení**

Ukončete obsah vysvětlením jednoho z nejdůležitějších důsledků UTXO modelu.

Pokud se někdo pokusí utratit stejný výstup dvakrát, uzly druhý pokus odmítnou, protože udržují účetní knihu a mohou ověřit, zda už byl daný UTXO utracen. Takto Bitcoin zabraňuje dvojímu utrácení bez potřeby centrální platební společnosti, která by spravovala záznamy. Příklad je zde velmi užitečný, protože ukazuje, jak Alice kombinuje UTXO, posílá prostředky Bobovi, dostává drobné a potvrzená transakce aktualizuje účetní knihu napříč uzly.

Jasný způsob, jak to říct ve třídě, je:

Bitcoin zabraňuje dvojímu utrácení, protože síť sleduje, které výstupy zůstávají neutracené a které už byly použity.

###### Shrnutí a ověření pochopení

Ukončete několika rychlými otázkami:

* Jaký je rozdíl mezi veřejným a soukromým klíčem?
* Co dokazuje digitální podpis?
* Proč je hashování v Bitcoinu užitečné?
* Co se stane, když je transakce po zahashování změněna?
* Co je UTXO jednoduše řečeno?
* Jak síť zabrání tomu, aby někdo utratil stejný bitcoin dvakrát?

#### Poznámky pro lektory

Tato kapitola obsahuje techničtější jazyk než předchozí, proto upřednostněte srozumitelnost, analogie a opakování.

Cílem není udělat ze studentů vývojáře. Cílem je pomoci jim pochopit, proč zabezpečení Bitcoinu funguje.

Nejsilnější body, na které se zaměřit, pokud je málo času, jsou:

* soukromý klíč vs veřejný klíč
* digitální podpisy
* co dělá hashování
* UTXO jako utratitelné části bitcoinu
* jak je zabráněno dvojímu utrácení

Nejužitečnější vizuály v této kapitole jsou:

* diagram uživatel-peněženka-síť
* vizuál digitálního podpisu
* příklady hashování a diagramy s výstupem pevné délky na stranách 7 až 10
* UTXO diagramy na stranách 10 až 12

##### Jak vypadá dobrý výsledek

* Je důležité chápat kryptografii jako základ, ne jako záhadu, používat hodně vizuálních pomůcek, vyhnout se hluboké matematice, navazovat na předchozí kapitoly a ověřovat pochopení pomocí aplikací jako "Pokud někdo změní jednu transakci, co se pokazí?"
* Lektoři by měli být trpěliví se studenty, kteří mají potíže, myslet vizuálně a vše kreslit, být upřímní ohledně toho, co studenti nemusí chápat, nebát se říct "Nevím, ale zjistíme to takto," a zůstat povzbudiví po celou dobu.
* Studenti chápou, proč My First Bitcoin nemůže být hacknutý, protože je chráněn matematikou, oceňují elegantní design systému, cítí se v pohodě s komplexitou, i když nemusí znát každý detail, získávají sebevědomí v kladení otázek bez obav z odsouzení a uvědomují si, že se posunuli v pochopení něčeho, co většina lidí nezná.
* Výukové cíle by měly být splněny, pokud studenti dokážou vysvětlit základy kryptografie jako jednosměrné funkce a digitální podpisy bez hluboké matematiky, pochopí UTXO model a to, že vlastníte mince, ne účty, rozpoznají hashování jako základ bezpečnosti Bitcoinu, pochopí anatomii transakce včetně podpisů a potvrzení, vysvětlí, proč je Bitcoin neměnný, a kladou kritické otázky ohledně možných útoků nebo zranitelností.

##### Řízení času

Pokud je málo času, upřednostněte:

* Soukromý klíč vs veřejný klíč
* Digitální podpisy
* Co dělá hashování
* UTXO jako utratitelné části bitcoinu
* Jak je zabráněno dvojímu utracení

Pokud jste napřed, věnujte čas:

* Schéma uživatel-peněženka-síť a vizuální bezpečnostní model
* Vizuální znázornění digitálního podpisu: detailní kryptografický proces
* Merkleovy stromy a bezpečnost řetězce
* Pokročilé vektory útoků a proč selhávají

##### Pokud mají studenti potíže

* Kryptografie jako hrozba → „Používáte ji denně; My First Bitcoin ji používá stejným způsobem.“
* Hashování jako pojem → Přirovnání k otisku prstu; jedinečné, nelze změnit bez změny hashe.
* Digitální podpisy → „Dokazuje oprávnění bez odhalení hesla.“
