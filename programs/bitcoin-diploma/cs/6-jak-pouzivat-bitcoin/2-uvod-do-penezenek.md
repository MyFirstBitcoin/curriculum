# 6.2 Úvod do peněženek

Na rozdíl od fyzických peněz nejsou bitcoiny ve skutečnosti uloženy v Bitcoin peněžence. Místo toho existují v distribuované účetní knize, kterou síť Bitcoin neustále ověřuje a zabezpečuje. Jak tedy můžete vlastnit bitcoiny?

Vlastnictví svých bitcoinů máte pouze tehdy, pokud ovládáte soukromé klíče, které vám umožňují podepisovat transakce a převádět vlastnictví svých bitcoinů na někoho jiného. To je samotný akt odeslání bitcoinů.

Podívejme se na dva pojmy, které používáme, když mluvíme o pojmu **peněženka**:

* Hlavní soukromý klíč, podobně jako heslo, ze kterého jsou generovány vaše veřejné klíče, podobně jako e-mailové adresy. Svou veřejnou adresu můžete sdílet s ostatními, abyste mohli přijímat a odesílat bitcoiny, ale svůj soukromý klíč nikdy nesmíte sdílet!
* Mobilní nebo desktopové rozhraní používané k interakci se sítí Bitcoin, kontrole zůstatku bitcoinů, odesílání a přijímání transakcí a jejich vysílání do sítě. Různé typy peněženek, spolu s jejich výhodami a nevýhodami, budou popsány v následujících sekcích.

#### Peněženky s vlastní správou vs. svěřenecké peněženky

Než podrobně popíšeme různé typy Bitcoin peněženek a jejich vlastnosti, je důležité rozlišit mezi peněženkami s vlastní správou a svěřeneckými peněženkami. Každý typ má své vlastní výhody, rizika a úroveň kontroly nad bitcoiny. Vlastní správa znamená, že uživatel drží soukromé klíče a skutečně ovládá své bitcoiny; u svěřeneckých peněženek drží bitcoiny pro uživatele třetí strana.


| Typ | Kontrola | Výhody | Rizika |
| --- | --- | --- | --- |
| Vlastní správa | Uživatel | Úplná kontrola nad prostředky a transakcemi, žádný schvalovací proces nebo zmrazení účtu, žádná firemní ani vládní kontrola, ochrana před konfiskací. | Žádná možnost obnovy, pokud je ztracena obnovovací fráze, veškerá odpovědnost je na uživateli. |
| Svěřenecká správa | Poskytovatel třetí strany | Snadná obnova při ztrátě přístupu, jednodušší zákaznická podpora. | Prostředky jsou připojeny k internetu, větší zranitelnost vůči hackingu. Správce může účty zmrazit. |


V peněžence s vlastní správou (také nazývané non-custodial peněženka) jste jediní, kdo má klíče k peněžence, a máte plnou kontrolu nad tím, co do ní vstupuje a co z ní odchází. Naopak u svěřenecké peněženky drží soukromý klíč někdo jiný, což mu dává plný přístup k přesunu jakýchkoli bitcoinů, které tento poskytovatel spravuje vaším jménem.

* Vlastní správa je jako být svou vlastní bankou. Transakce nepodléhají kontrole a dohledu
* Vlastní správa zajišťuje, že třetí strany nemohou vaše bitcoiny zabavit.
* Vlastní správa přináší klid v dobách nejistoty, protože víte, že vaše bitcoiny jsou v bezpečí.

Je důležité zvolit správný typ peněženky podle individuálních potřeb. Někdy je pro lidi těžké rozlišit, zda instalují peněženku s vlastní správou nebo svěřeneckou peněženku. Tato tabulka ukazuje rozdíly v instalačním procesu.


| Typ | Krok 1: Vyberte | Krok 2: Instalujte | Krok 3: Vytvořte | Krok 4: Zabezpečte |
| --- | --- | --- | --- | --- |
| Vlastní správa | Vyberte peněženku s vlastní správou | Postupujte podle pokynů peněženky | Vygenerujte obnovovací frázi | Uložte obnovovací frázi na bezpečné místo |
| Svěřenecká správa | Vyberte svěřeneckou peněženku | Postupujte podle pokynů peněženky | Vytvořte účet | N/A |


„**Nejsou-li vaše klíče, nejsou to vaše mince**“ je oblíbené rčení mezi držiteli bitcoinů. Odkazuje na myšlenku, že pokud nemáte přímou kontrolu nad soukromými klíči spojenými s vaší Bitcoin peněženkou, nemáte skutečné vlastnictví mincí.

Kdokoli získá přístup k vašim soukromým klíčům, má vlastnictví vašich bitcoinů. Proto je nesmírně důležité je chránit a držet mimo dosah zvědavých očí! Několik způsobů, jak to udělat, si ukážeme později v knize.

V dalším textu budeme mluvit pouze o peněženkách s vlastní správou, kde uživatel vlastní své klíče a má plnou kontrolu nad svými bitcoiny.

Nedělejte si starosti, pokud se to zdá složité nebo nerozumíte všemu — je to cesta a čím více začnete Bitcoin používat, tím lépe porozumíte!

#### Různé typy Bitcoin peněženek

To, kde je váš soukromý klíč vytvořen a uložen, určuje, jak Bitcoin peněženky popisujeme. Pokud jsou klíče ve vašem chytrém telefonu, jedná se o **mobilní peněženku**. Pokud jsou bezpečně uloženy na speciálním zařízení, jedná se o **hardware peněženku**.


| Typ | Popis | Výhody | Nevýhody | Příklad uživatele |
| --- | --- | --- | --- | --- |
| Online peněženka | Přístupná přes webový prohlížeč | Dostupná z jakéhokoliv zařízení s připojením k internetu | Méně bezpečná, protože může být hacknuta nebo kompromitována | Potřebuje často přistupovat ke své peněžence a nemá mnoho prostředků k uložení |
| Mobilní peněženka | Nainstalovaná na mobilním zařízení | Snadné použití | Může být ztracena, pokud je zařízení ukradeno nebo hacknuto | Potřebuje provádět transakce na cestách a nemá mnoho prostředků k uložení |
| Desktopová peněženka | Nainstalovaná na stolním počítači | Pohodlná a dostupná odkudkoliv | Může být hacknuta, pokud je počítač infikován malwarem | Chce uložit větší množství bitcoinu a je zvyklý používat stolní počítač |
| Hardware peněženka | Fyzické zařízení, které uchovává bitcoin offline | Bezpečnější než online peněženky a lze ji používat offline | Prostředky mohou být neobnovitelné | Chce uložit větší množství bitcoinu a je ochoten zaplatit za vyšší bezpečnost |


Protože klíče lze přesouvat z jednoho zařízení na druhé, „stav“ vaší Bitcoin peněženky není pevně daný. Například pokud vytvořím klíče své peněženky na počítači a později je přesunu do telefonu, „desktopová peněženka“ se stane „mobilní peněženkou“.

Pokud jde o uchovávání vašeho bitcoinu, nejde jen o to, kdo má kontrolu nad klíči — je třeba zvážit i mnoho dalších rizik. Proto je důležité najít řešení, které je zároveň bezpečné i pohodlné. Když budete analyzovat kompromisy různých typů peněženek, zjistíte, že neexistuje ideální peněženka, která by vyhovovala všem potřebám.

##### Na co myslet při výběru peněženky

* **Bezpečnost**: Ujistěte se, že peněženka má silná bezpečnostní opatření.
* **Soukromí**: Zvažte, zda peněženka vyžaduje osobní údaje.
* **Snadnost použití**: Vyberte si peněženku, která je snadná na používání a orientaci.
* **Kompatibilita**: Ujistěte se, že je peněženka kompatibilní s vaším zařízením.
* **Poplatky**: Porovnejte poplatky účtované různými peněženkami.
* **Reputace**: Prověřte reputaci vývojářů, abyste měli jistotu, že jsou důvěryhodní.
* **Kontrola**: Některé peněženky vám dávají větší kontrolu nad vašimi soukromými klíči.

##### Open source vs uzavřený zdrojový kód

Dalším důležitým faktorem při výběru Bitcoin peněženky je zjistit, zda je aplikace nebo software open-source. To je důležité, protože open-source projekty umožňují komunitě kontrolovat kód a pokračovat v projektu, pokud tým přestane pracovat. Stejně jako je kód Bitcoinu zcela otevřený pro každého k nahlédnutí, použití a úpravy, měl by být otevřený i kód peněženky, kterou používáte ke správě svého bitcoinu.

#### Aktivita: Diskuze a hodnocení Bitcoin peněženek

https://bitcoin.org/en/choose-your-wallet

Přejděte na následující webovou stránku: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Použijte své nové znalosti o Bitcoin peněženkách k výběru té, která nejlépe vyhovuje vašim potřebám podle kritérií, o kterých jsme dnes mluvili.
