# 6 - Jak používat Bitcoin

Délka: 90 minut

Hlavní myšlenka: Používání Bitcoinu na blockchainu učí studenty, jak v praxi funguje vlastnictví, samospráva a ověřování, a proměňuje teorii v přímou finanční akci.

#### Výukové cíle

Na konci této lekce by studenti měli být schopni:

* Identifikovat běžné způsoby, jak získat a směnit bitcoin, včetně peer-to-peer a centralizovaných směnáren.
* Vysvětlit rozdíl mezi samosprávnými a spravovanými peněženkami a proč je samospráva v Bitcoinu důležitá.
* Popište účel soukromých klíčů, veřejných adres, seed frází a rozhraní peněženek.
* Porovnat různé typy peněženek a zhodnotit jejich výhody a nevýhody z hlediska bezpečnosti, pohodlí, soukromí a kontroly.
* Nastavit mobilní bitcoinovou peněženku a vysvětlit základní proces obnovy.
* Předvést, jak přijmout a odeslat on-chain bitcoinovou transakci.

Aplikovat princip "Nevěř, ověřuj" při výběru peněženky, transakcích a širším používání Bitcoinu.

#### Nástroje a zdroje

##### Vizuální pomůcky

* Kapitola 6 – Jak používat Bitcoin

##### Support Library

* Slovníček pojmů — Kapitola 6 — Termíny: peněženka, soukromý klíč, veřejná adresa, seed fráze, spravovaná, samosprávná, UTXO, transakční poplatek
* Srovnávací tabulky a referenční listy — Srovnání typů peněženek (spravovaná, mobilní, hardwarová, papírová)
* Technické vysvětlivky a podrobné rozbory — Veřejné/soukromé klíče, UTXO model, potvrzování transakcí
* Podrobný rozbor bezpečnosti soukromého klíče — Seed fráze, odvozování klíčů, zálohovací metody, vektory útoků
* Průvodce anatomií transakce — Krok za krokem, jak funguje bitcoinová transakce
* Kontrolní seznam nejlepších bezpečnostních postupů — Před začátkem, vytvoření peněženky, přijímání, odesílání, prevence phishingu

#### Aktivity

* Transakce v praxi
* Lightning štafeta
* Zkoumání mempoolu

#### Online výuka

* Od začátku jasně sdělte, zda studenti sledují ukázku, nebo si sami nastavují peněženku.
* Používejte velké, čitelné snímky obrazovky pro každý krok nastavení peněženky.
* Po každém kroku udělejte pauzu a požádejte studenty, aby v chatu potvrdili porozumění, než budete pokračovat.
* Před sekcí se seed frází dejte přímé varování a připomeňte studentům, aby nikdy nesdíleli citlivé informace online.

#### Příprava

* Stáhněte a otestujte mobilní peněženku (Blue Wallet nebo Muun); připravte snímky klíčových kroků nastavení.
* Připravte návod na nastavení peněženky (stažení → vytvoření → záloha seedu → přijímání) pro referenci.
* Zajistěte funkční síť/WiFi; mějte připravenou demo adresu a QR kód k ukázce.

#### Postup

Tato lekce přechází od teorie k přímé praxi. Nyní přímo odpovídá struktuře Diplomového programu, takže získávání, peněženky, nastavení, transakce a ověřování jsou pod stejnými hlavními nadpisy jako v průvodci pro studenty. Další podpůrné materiály zůstávají v těchto sekcích vnořené.

##### 6.0 Úvod, 8 minut

Začněte propojením této kapitoly s předchozí:

* Pokud je Bitcoin peníze, jak je lidé vlastně získávají a používají?
* Co znamená skutečně ovládat svůj bitcoin?
* Proč je používání Bitcoinu jiné než používání bankovní aplikace?

Ujasněte, že tato kapitola je o praktickém použití. Studenti se už neučí jen, co je Bitcoin, ale učí se s ním přímo pracovat.

##### 6.1 Získávání a směna Bitcoinu, 12 minut

Vysvětlete, že lidé mohou bitcoin získat různými způsoby, například:

* dostat zaplaceno v bitcoinu
* těžit bitcoin
* směnit hotovost za bitcoin osobně
* směnit hotovost za bitcoin online

Poté se zaměřte na dva hlavní způsoby získání, které jsou v kapitole probírány:

* peer-to-peer, osobně
* peer-to-peer, online
* centralizované burzy

Udělejte kompromisy jasné.

U osobního P2P zdůrazněte přímou výměnu bez banky nebo prostředníka, ale také zmiňte praktická rizika setkání s lidmi kvůli obchodům za hotovost.

U online P2P vysvětlete escrow jednoduše, jako způsob, jak snížit riziko protistrany a přitom umožnit přímou výměnu mezi lidmi.

U centralizovaných burz jasně řekněte, že jsou pohodlné, ale uživatelé musí důvěřovat společnosti, často sdílet osobní údaje a jejich prostředky jsou pod kontrolou třetí strany, dokud nejsou vybrány. Toto je vhodné místo zdůraznit, že pohodlí často přináší kompromisy v oblasti soukromí a svrchovanosti.

##### 6.2 Úvod do bitcoinových peněženek, 35 minut

**Co je to vlastně bitcoinová peněženka**

Hned na začátku objasněte běžné nedorozumění: bitcoin není uložený v aplikaci peněženky jako fyzické peníze v tašce.  
Bitcoin existuje v účetní knize, kterou spravuje síť. To, co uživatel ovládá, je možnost jej utratit pomocí soukromých klíčů.

Poté vysvětlete dvě věci, které lidé často myslí slovem „peněženka“:

* systém soukromých klíčů, ze kterého se generují adresy
* aplikace nebo rozhraní používané k interakci se sítí

Použijte analogii s e-mailem z této kapitoly, pokud to pomůže:

* veřejná adresa = jako e-mailová adresa, kterou můžete sdílet
* soukromý klíč = jako heslo, které musíte chránit

Buďte zde velmi jasní: kdo ovládá soukromé klíče, ovládá bitcoin. To je základní koncept, který si studenti musí osvojit.

**Peněženky s vlastní správou vs. svěřenecké peněženky**

Toto je jedna z nejdůležitějších částí kapitoly.

Jasně vysvětlete rozdíl:

* Peněženka s vlastní správou: uživatel ovládá soukromé klíče
* Svěřenecká peněženka: soukromé klíče ovládá třetí strana jménem uživatele

Poté projděte kompromisy:

Vlastní správa

* plná kontrola nad prostředky
* žádný schvalovací proces
* ochrana proti svévolnému zabavení
* větší odpovědnost
* žádné snadné obnovení při ztrátě seed fráze

Svěřenecká správa

* snazší obnovení a podpora
* jednodušší pro začátečníky
* větší riziko zmrazení účtu, hacknutí a kontroly třetí strany
* uživatel ve skutečnosti bitcoin nedrží

Toto je vhodný okamžik zdůraznit frázi:

"Not your keys, not your coins."

Studenti by si z této části měli odnést nejen slogan, ale i to, co ve skutečnosti znamená v praxi.

**Různé typy peněženek a jak si vybrat**

Představte typy peněženek, které jsou v kapitole popsány:

* online peněženka
* mobilní peněženka
* desktopová peněženka
* hardwarová peněženka
* papírová peněženka

Neříkejte, že některá je dokonalá. Místo toho vysvětlete, že každá má kompromisy mezi:

* bezpečností
* soukromím
* pohodlím
* kompatibilitou
* poplatky
* kontrolou
* pověst

Také jasně uveďte, že doporučujeme věnovat pozornost tomu, zda je peněženka open-source, protože open-source nástroje může komunita kontrolovat, auditovat a dále rozvíjet. To přímo souvisí se zásadou ověřování v Bitcoinu.

##### 6.3 Nastavení mobilní bitcoinové peněženky, 10 minut

Projděte se studenty základní postup popsaný v kapitole:

* stáhněte si peněženku
* vytvořte novou peněženku
* vygenerujte a zapište si obnovovací frázi
* potvrďte obnovovací frázi
* přidejte dodatečné zabezpečení, pokud je k dispozici
* otevřete peněženku a najděte funkci přijímání

Upozornění na seed frázi učiňte velmi jasným:

* pokud je seed fráze ztracena, může být ztracen přístup k prostředkům
* pokud se k seed frázi dostane někdo jiný, může prostředky převzít

Pokud studenti provádějí tento postup prakticky, měl by lektor u každého kroku zastavit a ověřit, že všichni rozumí tomu, co dělají. Pokud je výuka spíše koncepční, lze tuto část vysvětlit jako průchod postupem, nikoli provádět živě. Možnost obnovy ukázaná v kapitole je také užitečná pro vysvětlení, že peněženky lze obnovit, pokud byla seed fráze správně zálohována.

##### 6.4 Přijímání a odesílání transakcí, 17 minut

**Přijímání a odesílání on-chain transakcí**

Nyní vysvětlete, jak fungují on-chain transakce.

Pro přijímání bitcoinu:

* otevřete peněženku
* klepněte na přijmout nebo vložit
* zkopírujte adresu, sdílejte odkaz nebo ukažte QR kód

Pro odesílání bitcoinu:

* otevřete peněženku
* vložit nebo naskenovat adresu příjemce
* zadejte částku
* důkladně zkontrolujte všechny údaje
* odeslat transakci do sítě
* počkat na potvrzení

Ujasněte tyto klíčové body:

* transakce převádí vlastnictví, nikoli fyzické mince
* transakce jsou nevratné
* uzly ověřují platnost
* těžaři zahrnují transakce do bloků
* poplatky ovlivňují prioritu potvrzení
* on-chain transakce jsou obecně bezpečné, ale pomalejší a často dražší než transakce přes Lightning

Schéma toku transakce v kapitole je zde obzvlášť užitečné, protože studentům pomáhá vizualizovat cestu od požadavku v peněžence až po potvrzení v síti.

**Transakce v praxi a cvičení podle rolí**

Použijte kooperativní cvičení z kapitoly k upevnění pochopení. Vysvětlete čtyři zapojené role:

* odesílatel
* příjemce
* těžař
* provozovatel uzlu

Jednoduchý přístup ve třídě je přiřadit role a projít jednu transakci krok za krokem. To studentům pomáhá vidět, že bitcoinová transakce není magie, ale koordinovaný proces zahrnující schválení, ověření, zařazení do bloku a aktualizaci účetní knihy.

Cílem zde není technická hloubka. Jde o to, aby studenti pochopili, kdo co v transakci dělá a proč je ověřování důležité.

##### 6.5 Nedůvěřuj, ověřuj, 8 minut

Vysvětlete, že toto platí pro:

* peněženky
* směnárny
* aplikace
* podrobnosti transakce
* tvrzení o „snadných ziscích“
* projekty, které se tváří jako Bitcoin

Ujasněte, že Bitcoin vyžaduje, aby uživatelé kriticky přemýšleli, ověřovali, co používají, a vyhýbali se slepé důvěře. Vysvětlete také, proč jsou v tomto kontextu důležité open-source nástroje: umožňují nezávislé ověření.

###### Shrnutí a ověření porozumění

Zakončete několika rychlými otázkami:

* Jaký je rozdíl mezi úschovnou (custodial) a vlastní (self-custodial) peněženkou?
* Proč je seed fráze tak důležitá?
* Co se stane, když odešlete on-chain transakci?
* Proč jsou on-chain transakce pomalejší než některé jiné bitcoinové platby?
* Co v praxi znamená „Nedůvěřuj, ověřuj“?

#### Poznámky pro lektory

Tato kapitola je velmi praktická, proto upřednostněte srozumitelnost, bezpečnost a opakování.

Studenti nemusí zvládnout všechny typy peněženek během jedné lekce. Hlavní cíle jsou:

* pochopení základů peněženek
* pochopení vlastní správy (self-custody)
* osvojení základního průběhu transakce
* přijetí odpovědného ověřovacího přístupu

Buďte obzvlášť opatrní při vysvětlování seed frází a nastavení peněženky. Studenti by měli odcházet s pochopením, že to nejsou drobnosti, ale základ vlastnictví Bitcoinu.

Nejužitečnější vizuální pomůcky a aktivity v této kapitole jsou:

* srovnání vlastní a úschovné peněženky
* tabulka kompromisů typů peněženek
* cvičení krok za krokem při nastavování peněženky
* diagram průběhu transakce
* aktivita s transakcí podle rolí

##### Jak vypadá dobrý výsledek

* Je důležité, aby si studenti skutečně nastavili peněženku nebo sledovali pečlivou ukázku, aby byla seed fráze středobodem s větou „Těchto 12 slov JE váš Bitcoin“, aby si vyzkoušeli scénáře jako „Co se stane, když ztratíte telefon?“ a procvičili rozpoznávání phishingu.
* Lektor by měl být praktickým průvodcem, který to již sám absolvoval, být bezpečnostně uvědomělý, ale ne paranoidní, a být upřímný ohledně obtížnosti a nutnosti učení.
* Studenti mají pocit, že se naučili skutečnou dovednost, kterou mohou využít, chápou, že seed fráze je skutečná a důležitá, nikoli abstraktní, cítí se schopni držet vlastní Bitcoin a rozumí tomu, že decentralizace vyžaduje osobní odpovědnost.
* Výukové cíle jsou splněny, pokud studenti umí nastavit peněženku a rozumí rozdílu mezi veřejným a soukromým klíčem, chápou kompromisy mezi úschovnou a vlastní peněženkou, dokáží vysvětlit, jak funguje transakce včetně vstupů, výstupů a poplatků, prokáží povědomí o bezpečnosti včetně ochrany seed fráze a kladou kritické otázky ohledně vlastnictví a kontroly.

##### Řízení času

Pokud je málo času, upřednostněte:

* Pochopení základů peněženek
* Pochopení vlastní správy (self-custody)
* Osvojení základního průběhu transakce
* Přijetí odpovědného ověřovacího přístupu

Pokud máte náskok, věnujte čas:

* Srovnávací tabulka vlastní a úschovné peněženky
* Tabulka kompromisů typů peněženek
* Cvičení krok za krokem při nastavování peněženky s živou ukázkou
* Diagram průběhu transakce s výpočtem poplatků
* Pokročilé bezpečnostní postupy a úvahy o hardwarových peněženkách

##### Pokud mají studenti potíže

* Seed fráze jako „skutečné“ → „Tato fráze JE váš bitcoin; žádný zákaznický servis.“
* Veřejné vs. soukromé klíče → Přirovnání k e-mailu (adresa vs. heslo).
* Proč je to těžké → „Vy to ovládáte; jste zodpovědní.“ Uznat kompromis.
