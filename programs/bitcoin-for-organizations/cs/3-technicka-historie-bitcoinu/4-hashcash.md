# 3.4 Hashcash

Hashcash vytvořil Adam Back, další z raných inovátorů v této oblasti. Adam měl silný zájem o svobodné trhy a soukromí na internetu a narazil na mailing list Cypherpunks, ke kterému se připojil a stal se jeho aktivním účastníkem.

Velmi ho zajímaly digitální peníze a navrhl, jak by skupina mohla potenciálně úžeji spolupracovat na DigiCash s Chaumem, ale tyto návrhy nikam nevedly. Poté obrátil svou pozornost k dalšímu vznikajícímu problému – nevyžádané poště (spamu). On i ostatní Cypherpunks chtěli najít řešení problému spamu, kdy bylo pro spamery triviální vytvořit a rozeslat tisíce e-mailů, které zahlcují sítě. Jeho inovativní řešení bylo založeno na hashování – schopnosti kryptografie převést jakýkoli kus dat na unikátní a náhodný řetězec určité délky, čímž vznikla obdoba digitální „známky“, kterou bylo třeba k e-mailu přidat, aby byl považován za platný a mohl být přenesen sítí. Pro běžný e-mail zanedbatelný náklad, pro spammera však nepřekonatelná překážka.

Klíčovou inovací, kterou Hashcash přinesl, bylo propojení reálných zdrojů – výpočetního výkonu – s digitální sítí. Zatímco digitální zdroje bylo do té doby možné replikovat bez omezení, počet vytvořených „hashcash“ byl omezen tím, kolik energie byli lidé ochotni do něj investovat.

Ačkoli řešení splňovalo některá kritéria, která Adam považoval za nutná v systému digitálních peněz – bylo anonymní, odolné a bez potřeby důvěry – každý hashcash nebyl znovupoužitelný a nebyl skutečně vzácný. Navrhl další způsoby, jak by bylo možné tyto problémy řešit pomocí externích třetích stran.

##### BitGold

Nick Szabo navázal na koncept Hashcash a důkazu prací (proof of work) a navrhl alternativní řešení, které popsal na mailing listu rok po zveřejnění Hashcash, v roce 1998.

Ačkoli se tím přiblížil k řešení, tento návrh stále čelil několika výzvám.

* Kdo by provozoval registr vlastnictví hashů a jak by mu bylo možné důvěřovat?
* Hashování by obecně časem zlevňovalo, což byla výzva i pro HashCash.

Protože propojené hashe by byly časově označeny, navrhl nějakou formu historického sledování obtížnosti hashování v dané době; dřívější hash by vyžadoval více výpočetních nákladů než pozdější, protože náklady klesaly. Bohužel to znamenalo, že hashe by nebyly „zaměnitelné“, tedy stejné hodnoty, což je považováno za klíčovou vlastnost digitálních peněz. Aby to Nick pomohl vyřešit, navrhl nějakou formu „svobodného bankovnictví“ fungujícího nad BitGold, které by mohlo agregovat různé skupiny hashů, jež by měly stejnou hodnotu.

##### B-Money

Krátce po návrhu Bit Gold přišel Wei Dai s podobným řešením. Již vyvinul několik dalších nástrojů pro Cypherpunks a měl své vlastní představy o digitálních penězích.

Jeho návrh se podobal Bit Gold v tom, že používal digitální podpisy k převodu peněz a záznamy o transakcích by byly uloženy v účetní knize, která by obsahovala veřejné klíče a množství měnových jednotek přiřazených každému z nich. Stejně jako u Bit-Gold byly důvěryhodné třetí strany považovány za bezpečnostní slabinu a panoval názor, že elektronický peněžní systém by se neměl spoléhat na jediný subjekt, který by sledoval zůstatky, transakce nebo zabraňoval dvojímu utrácení.

Wei Dai navrhl několik řešení těchto problémů, z nichž jedno bylo, že místo centrální entity (entit), která by vedla účetní knihu, by kopii vedly VŠECHNY uzly. Pokud by si všichni uživatelé kontrolovali vlastní účetní knihu a platnost každé transakce, pak pokud by všechny uzly zůstaly aktuální, měly by účetní knihy zůstat synchronizované v celé síti. Tento vysoce distribuovaný systém by bylo obtížné narušit.

Wei Dai si uvědomoval, že to neřeší problém byzantských generálů (1), protože uzly by mohly snadno ztratit synchronizaci nebo jednoduše lhát. Navrhl alternativní metody, například mít podmnožinu „důvěryhodných“ serverů, které by vedly účetní knihu, a vytvořit finanční pobídky, aby tyto servery zůstaly poctivé.

Pro měnovou politiku navrhl navázat kupní sílu B-Money na nějaký externí spotřebitelský cenový index. Chtěl, aby si stejný objem B-Money mohl v čase koupit stejný podíl indexu, což by zajistilo určitou cenovou stabilitu. Nové měnové jednotky by tak mohl vytvořit kdokoli, kdo by poskytl platný hash, ale obtížnost generování hashe by se mohla v čase měnit podle nákladů na CPU a cenového indexu, takže každá jednotka by byla „neměnná“.
