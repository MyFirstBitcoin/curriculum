# 6.4 Přijímání a odesílání transakcí

Bitcoinová transakce je převod vlastnictví bitcoinů na nového majitele. Všimněte si, že se nepřevádějí samotné mince, ale jejich vlastnictví: jinými slovy právo je utratit. Pokaždé, když je transakce přijata do bloku, všechny uzly v síti aktualizují svou místní kopii veřejné účetní knihy, aby odrážela změnu vlastnictví. V tomto ohledu je bitcoinová transakce více podobná transakci s nemovitostmi (nebo jiným majetkem) než hotovostní transakci.

Aby bylo možné „odeslat“ bitcoiny, odesílatel podepíše zprávu svým soukromým klíčem, čímž signalizuje síti, že oprávněný vlastník bitcoinů převedl jejich vlastnictví na příjemce.

Bitcoiny budou nyní vázány na adresu příjemce, což mu dává vlastnictví bitcoinů, takže je může utratit pouze nový majitel pomocí svého soukromého klíče.

Nové bitcoinové transakce jsou zahajovány z peněženek po celém světě, ale neexistuje žádný centrální platební zprostředkovatel. Místo toho těžaři soutěží o záznam transakcí do účetní knihy.

Řekněme, že Petr dluží Elišce 0,5 BTC a je připraven jí to vrátit. Oba mají digitální peněženky.

1. Eliška sdílí svou adresu s Petrem.
1. Petr použije svůj peněženkový software k vytvoření transakce, která obsahuje Eliščinu adresu, částku k převodu (0,5 BTC) a poplatek pro těžaře. Vyšší poplatky zvyšují pravděpodobnost, že těžař zahrne transakci do dalšího bloku.
1. Po podepsání transakce je tato vyslána do sítě, kde je ověřena uzly. Ty kontrolují, zda má Petr dostatek prostředků a je oprávněným vlastníkem mincí, které chce utratit. Pokud tomu tak není, transakci ihned odmítnou.
1. Jakmile je transakce ověřena, těžaři se rozhodnou, zda ji přidají do dalšího bloku, obvykle na základě zvoleného poplatku. Jakmile se transakce dostane do bloku, je přidána do blockchainu a prostředky jsou převedeny na Eliščinu adresu.
1. Vlastnictví bylo převedeno na Elišku. Nyní může použít svůj soukromý klíč k utracení prostředků.

_Je důležité si uvědomit, že jakmile je transakce dokončena, nelze ji vrátit zpět._


> **Note – Jak funguje bitcoinová transakce**
>
> 1. Někdo požádá o transakci
> 1. Transakce je vyslána do P2P počítačů (uzlů)
> 1. Těžaři ověřují transakci
> 1. Transakce jsou spojeny do datového bloku
> 1. Nový blok je přidán k existujícímu blockchainu
> 1. Transakce je dokončena



> **Note – Přijímání bitcoinových transakcí**
>
> Pro přijetí bitcoinů budete muset poskytnout odesílateli bitcoinovou veřejnou adresu. Jedná se o jedinečný řetězec písmen a čísel, který reprezentuje vaši peněženku a slouží k její identifikaci v bitcoinové síti.
>
> Svoji veřejnou adresu najdete tak, že otevřete svou bitcoinovou peněženku a vyhledáte možnost „Přijmout“ nebo „Vložit“ bitcoiny.
>
> Svoji bitcoinovou adresu pak můžete sdílet několika způsoby:
>
> 1. **Zkopírujte a vložte adresu**: Adresu můžete zkopírovat jejím označením a stisknutím "Kopírovat", poté ji vložit do e-mailu nebo zprávy.
> 1. **Sdílejte odkaz na svou bitcoinovou peněženku**: Některé bitcoinové peněženky umožňují vytvořit odkaz na vaši peněženku, který můžete sdílet s odesílatelem. Ten pak může na odkaz kliknout a poslat vám bitcoiny.
> 1. **Sdílejte QR kód**: Pokud má odesílatel chytrý telefon s aplikací bitcoinové peněženky, může naskenovat QR kód a získat vaši bitcoinovou adresu.


Jakmile má odesílatel vaši adresu, může vám poslat bitcoiny tak, že zadá vaši adresu a částku, kterou chce poslat. Bitcoiny jsou pak odeslány z jeho peněženky do vaší peněženky.

Transakce je potvrzena bitcoinovou sítí a obvykle trvá asi 10 minut. Pro větší bezpečnost se doporučuje počkat na dvě potvrzení, což trvá přibližně 20 minut.


> **Note – Odesílání bitcoinových transakcí**
>
> K odeslání bitcoinů budete potřebovat několik věcí: bitcoinovou peněženku, veřejnou adresu příjemce a částku bitcoinů, kterou chcete odeslat.
>
> 1. Otevřete svou bitcoinovou peněženku.
> 1. Přejděte na tlačítko „Odeslat“ a vložte adresu příjemce do pole "Komu". Případně můžete také naskenovat QR kód, pokud jej příjemce poskytne.
> 1. Zadejte částku bitcoinů, kterou chcete odeslat, do pole „Částka“.
> 1. Dvakrát zkontrolujte adresu příjemce a částku k odeslání. Pamatujte, že transakce jsou nevratné!
> 1. Před kliknutím na „Potvrdit a odeslat“ doporučujeme ještě jednou zkontrolovat detaily transakce, abyste se ujistili, že posíláte správnou částku bitcoinů na správnou adresu.
> 1. Odešlete transakci a počkejte, až síť transakci potvrdí.
>
> Nyní víte, jak vyhodnotit, vybrat a nastavit si vlastní bitcoinovou peněženku. Odesílání a přijímání bitcoinů v síti Bitcoin se označuje jako „on-chain“ transakce. Je to proto, že transakce probíhají na hlavní bitcoinové síti a jsou zaznamenány v blockchainu.
>
> On-chain transakce jsou nejbezpečnějším způsobem, jak s bitcoiny obchodovat, díky decentralizovanému ověřování poskytovanému sítí.
>
> On-chain transakce jsou však pomalejší a mohou být výrazně dražší než jiné možnosti (které probereme v modulu 7) kvůli poplatku těžařům.


#### Aktivita: Transakce v praxi

https://qr.myfirstbitcoin.org/transactions.pdf

**Toto je kooperativní cvičení, které zjednodušuje základní role lidí zapojených do bitcoinové transakce.**

###### Klíčové body

1. V každé bitcoinové transakci jsou čtyři typy účastníků: odesílatel, příjemce, těžaři a provozovatelé uzlů.
1. Odesílatel musí schválit (kryptograficky podepsat) **částku bitcoinů** k odeslání A **konkrétní adresu** na kterou se má odeslat.
1. Příjemce musí poskytnout **platnou adresu** odesílateli A ověřit, že transakce byla úspěšně potvrzena na blockchainu.
1. Těžaři zajišťují, že všechna kritéria jsou platná, než přidají transakce do budoucích bloků.
1. Provozovatelé uzlů ověřují, že vytěžené bloky jsou platné, než aktualizují svou verzi blockchainu (účetní knihy).

###### Tip pro studenty

Vystřídejte si všechny čtyři role, abyste zažili, co každý účastník dělá.
