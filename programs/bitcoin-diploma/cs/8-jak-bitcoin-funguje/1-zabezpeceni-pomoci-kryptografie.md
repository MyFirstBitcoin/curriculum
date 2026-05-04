# 8.1 Zabezpečení pomocí kryptografie

> Co nám Bitcoin dává, je pevný slib: program se provede přesně tak, jak je zadáno.  
_Andreas M. Antonopoulos_

#### Šifrování s veřejným a soukromým klíčem


> **Definition – Definice kryptografie**
>
> **Kryptografie** je praxe převádění informací na tajemství, které si mohou přečíst jen ti správní lidé.


* **Šifrování** je proces převádění informací do kódované podoby, aby si je mohl přečíst pouze ten, kdo má správný klíč.
* **Dešifrování** je proces převádění této kódované informace zpět do čitelné podoby.

V tradiční kryptografii musí dvě osoby, které chtějí komunikovat soukromě, nejprve sdílet stejný tajný klíč, podobně jako sdílené heslo. Jeden člověk tento klíč použije k zašifrování zprávy před jejím odesláním a druhý člověk použije stejný klíč k dešifrování a přečtení zprávy.

Problém tohoto systému je, že oba lidé už musí sdílet tajný klíč. Pokud se k tomuto klíči dostane někdo jiný, může si přečíst jakoukoli zachycenou zprávu.

Bitcoin tento problém řeší jiným přístupem zvaným kryptografie s veřejným klíčem, kde uživatelé nemusí předem sdílet tajné klíče.

Kryptografie s veřejným a soukromým klíčem řeší problém sdílení tajemství. Místo sdílení hesla má každý člověk dva klíče: veřejný klíč a soukromý klíč.

* **veřejný klíč** lze sdílet s kýmkoli.
* **soukromý klíč** musí být vždy uchován v tajnosti.

Pokud chce Jan poslat něco Karlovi, může použít Karlův veřejný klíč. Odemknout to ale může pouze Karel pomocí svého soukromého klíče. I kdyby někdo zprávu zachytil, bez soukromého klíče ji nemůže přečíst ani použít.

V Bitcoinu se tento systém používá k vytváření digitálních podpisů. Digitální podpis dokazuje, že majitel soukromého klíče schválil transakci, podobně jako když podepisujete dokument svým jménem. Díky tomu jsou bitcoinové transakce bezpečné a ověřitelné bez nutnosti důvěřovat třetí straně.

Bitcoinové transakce zahrnují převod vlastnictví bitcoinu z jedné adresy na druhou.

Šifrování se používá k zajištění toho, že pouze skutečný držitel bitcoinu má právo poslat své peníze někomu jinému. Zajišťuje, že jeho majetek je chráněn před škodlivými aktéry.

Jako další ochranné opatření získá každá bitcoinová transakce automaticky JEDINEČNÝ digitální podpis. Tento jedinečný digitální podpis je poháněn technologií odolnou proti manipulaci, která pomáhá síti ověřit, že bitcoin skutečně odeslal jeho pravý vlastník, a ne někdo jiný.


> **Info**
>
> Každý uživatel má dva klíče: **soukromý klíč**, který je **uchováván v tajnosti**, a **veřejný klíč** který lze **sdílet s ostatními**. **Soukromý klíč** slouží jako forma identifikace a důkaz vlastnictví, potvrzující: „Tato adresa patří mně a mám nad ní kontrolu.“


###### Jak funguje bitcoinová transakce

1. **Vytvoření transakce**: Uživatel zahájí bitcoinovou transakci zadáním údajů, jako je adresa příjemce a množství bitcoinu, které chce odeslat.
1. **Generování digitálního podpisu**: Odesílatel vytvoří jedinečný **digitální podpis** pomocí svého **soukromého klíče**. Tento podpis je jedinečný kód, který ověřuje pravost transakce.
1. **Odeslání transakce do sítě**: Podepsaná transakce je odeslána do bitcoinové sítě, což značí záměr převést vlastnictví bitcoinu od odesílatele k příjemci.
1. **Ověření v síti**: Uzly v bitcoinové síti přijmou transakci a použijí příjemcův **veřejný klíč** k ověření pravosti podpisu transakce. Současně používají odesílatelův **veřejný klíč** k ověření **digitálního podpisu**.
1. **Potvrzení v síti Bitcoin**: Pokud je ověření úspěšné, transakce bude přidána do účetní knihy, která slouží jako bezpečný a transparentní záznam všech transakcí. Po potvrzení je vlastnictví bitcoinu oficiálně převedeno od odesílatele k příjemci.


> **Callout – Shrnutí**
>
> **digitální podpis**, vytvořený pomocí odesílatelova **soukromého klíče**, dokazuje, že transakci autorizoval vlastník bitcoinu. Síť Bitcoin pak může tento důkaz ověřit a transakci zaznamenat.


#### Vysvětlení hashování

Nenechte se odradit technickými pojmy a matematickými koncepty, které nás čekají. Chápeme, že ne každý je nadšený z matematiky, ale možná sami sebe překvapíte a zjistíte, že i ty nejsložitější myšlenky lze pochopit s trochou úsilí.


> **Definition – Definice funkce**
>
> **funkce** je jako stroj, který vezme nějakou informaci a přemění ji v něco nového. Informace, kterou funkci zadáte, je **vstup**. Nová informace, kterou funkce vytvoří, je **výstup**. Funkce pomáhají počítačům vykonávat úkoly a řešit problémy.


##### Co je to funkce?

Funkce je sada instrukcí, která přijímá vstup a vytváří výstup. Můžete si ji představit jako recept: postupujete podle kroků s určitými ingrediencemi a vždy skončíte s předvídatelným výsledkem.

V Bitcoinu se funkce používají ke zpracování a ověřování transakcí. Když někdo posílá bitcoin, kryptografické funkce pomáhají ověřit, že je transakce platná, potvrdit, že odesílatel má dostatek prostředků, a aktualizovat zůstatky v účetní knize Bitcoinu. Jakmile je transakce ověřena a přidána do bloku, stává se trvalou součástí záznamu na blockchainu.

##### Co je to jednosměrná funkce?

Jednosměrná funkce je speciální typ funkce, kterou je snadné vypočítat jedním směrem, ale extrémně obtížné ji obrátit. Například rozmixovat ingredience do smoothie je snadné, ale už je nedokážete oddělit zpět na původní suroviny.

Bezpečnost Bitcoinu spoléhá na jednosměrné funkce. Ty se používají v kryptografii s veřejným a soukromým klíčem, což lidem umožňuje sdílet veřejný klíč a zároveň si uchovat soukromý klíč v tajnosti. I když je veřejný klíč viditelný, není možné z něj odvodit soukromý klíč. To je to, co dělá bitcoinové transakce bezpečnými.

##### Co je to hashovací funkce?

**hashovací funkce** je jako stroj na tajné kódy. Vezme zprávu a převede ji na kód.

###### Jak funguje hashování v bitcoinových transakcích

V Bitcoinu je každá transakce převedena na hash dříve, než je přidána do blockchainu. Hash je jedinečný digitální otisk transakce. Pokud se někdo pokusí změnit byť jen malou část transakce, hash se úplně změní. Díky tomu může síť snadno odhalit jakoukoli manipulaci.

###### Role hashování v bezpečnosti Bitcoinu

Hashování pomáhá chránit síť Bitcoin tím, že transakce jsou snadno ověřitelné a nelze je tiše upravit. Protože každá transakce má svůj vlastní jedinečný hash, síť může rychle zjistit, zda bylo něco změněno.

Hashovací funkce vezme data a převede je na pevně dlouhý řetězec čísel a písmen, kterému se říká hash. Stejný vstup vždy vytvoří stejný hash, ale i nepatrná změna vstupu vytvoří úplně jiný výsledek. Tato vlastnost umožňuje počítačům ověřit, že data nebyla změněna.


> **Definition – Definice hashování**
>
> **Hashování** je jako vytvoření otisku prstu pro digitální data. Je to proces, při kterém se digitální zpráva převede na kód pevné délky, který slouží jako jedinečný identifikátor. Stejně jako otisk prstu může identifikovat člověka, hash může identifikovat digitální zprávu.


**výstup**, neboli hash, má vždy stejnou délku, bez ohledu na to, jak dlouhá byla původní informace. Bitcoin používá několik konkrétních typů hashovacích funkcí, například **SHA-256** a **RIPEMD160**.

Několik příkladů je níže:

* SHA256 hash řetězce **ahoj světe**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256 hash řetězce **ahoj světe.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Všimněte si, že i malá změna vstupu zcela změní výstup ve srovnání s tím prvním
* SHA256 hash stažitelného iso souboru **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Tento vstup je obrovský soubor, ale výstup má stále stejnou pevnou délku

Hashování si můžete představit také jako notový zápis, který zachycuje podstatu hudebního díla. Stejně jako notový zápis je jedinečným vyjádřením melodie, je hash hodnota jedinečným vyjádřením dat.

Porovnáním notového zápisu skladby se skutečným provedením může hudebník zjistit, zda je provedení přesné. Podobně lze porovnáním hash hodnoty přijatých dat s původní hash hodnotou zjistit, zda byla data během přenosu změněna.

Stejně jako i malá odchylka v hudebním provedení může způsobit, že skladba zní jinak, i ta nejmenší změna původních dat povede k jiné hash hodnotě. Díky tomu je hashování mocným nástrojem pro zajištění integrity a pravosti Bitcoin transakce.

Proces kódování **veřejného klíče** pomocí hashování slouží ke zvýšení bezpečnosti informací tím, že je převede do formátu s pevnou délkou, který není čitelný. Bitcoin používá algoritmy SHA-256 a RIPEMD160 k vytvoření veřejných adres. Výsledný výstup slouží jako jedinečný identifikátor pro **veřejný klíč** a pomáhá zajistit integritu a bezpečnost transakcí uložených v účetní knize. Takovýmto šifrováním informací je pro neoprávněné osoby mnohem obtížnější k datům přistupovat a manipulovat s nimi.

##### Vlastnosti hashovací funkce

* **Deterministická**: Stejné ingredience vždy vytvoří stejný smoothie. Stejně tak stejná data vždy vytvoří stejný hash.
* **Odolnost vůči zpětnému získání vstupu**: Pokud máte jen smoothie, nemůžete zjistit přesně, jaké ovoce bylo použito. Podobně, pokud máte pouze hash, nemůžete určit původní data.
* **Lavínový efekt**: Změna i malé části ingrediencí vytvoří zcela jiný smoothie. U hashování i velmi malá změna dat vytvoří zcela jiný hash.
* **Odolnost vůči kolizím**: Je extrémně obtížné najít dvě různé sady ingrediencí, které vytvoří naprosto stejný smoothie. Stejně tak je extrémně nepravděpodobné, že dvě různá data vytvoří stejný hash.
* **Rychlé ověření**: Vyrobit smoothie je rychlé a snadno ověříte, že jde o smoothie. Hashovací funkce jsou rychlé na výpočet a snadné k ověření pro kohokoli.

#### Aktivita: Vygenerujte SHA 256 hash

https://tools.keycdn.com/sha256-online-generator

Zajímá vás, jak hashování funguje? Naskenujte QR kód a okamžitě si vygenerujte SHA256 hash z jakéhokoli slova, věty nebo vstupu, který si vyberete. Hashovací funkce jsou jako digitální otisky prstů: jsou jednosměrné, což znamená, že jakmile je něco zahashováno, nelze to převrátit zpět. Vyzkoušejte si to sami!
