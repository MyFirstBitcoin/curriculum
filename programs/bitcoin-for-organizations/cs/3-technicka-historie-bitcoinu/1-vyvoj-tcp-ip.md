# 3.1 Vývoj TCP/IP

Většina z nás zná protokoly TCP/IP, které dnes tvoří základ internetu. Jejich původ sahá do konce 70. let, kdy vědci zkoumali alternativní návrhy k Arpanetu – ještě starší síti, kterou navrhl americký ministerstvo obrany pro sdílení zdrojů mezi vzdálenými počítači. TCP/IP se stal standardním protokolem pro Arpanet v roce 1983, což vedlo k tomu, že se do konce 90. let stal dominantním modelem sítí a základem internetu, na kterém dnes běží Bitcoin.


| OSI model | TCP/IP |
| --- | --- |
| Aplikační | Aplikační |
| Prezentační | Aplikační |
| Relační | Aplikační |
| Transportní | Transportní |
| Síťová | Síťová |
| Linková | Linková |
| Fyzická | Fyzická |


Ve stejnou dobu, kdy byl vyvíjen model TCP/IP, vznikal podobný, ale komplexnější rámec pod vedením Mezinárodní organizace pro normalizaci (ISO) a telekomunikačního průmyslu (CCITT). Proces vývoje nových protokolů nebo navrhování změn byl ve srovnání s decentralizovanějším přístupem TCP/IP pomalý a těžkopádný, což vedlo k dominanci TCP/IP, jak ji známe dnes.

##### Žádost o změnu

Jakýkoli návrh na rozvoj stávajících protokolů nebo nápad na nové lze v modelu TCP/IP navrhnout prostřednictvím **Žádosti o změnu** procesu. Tyto návrhy procházejí schvalovacím procesem, který spravuje Internet Engineering Task Force (IETF), a po schválení se stávají open source, aby je mohl kdokoli implementovat a používat. Některé významné příklady:

* 1969 RFC 1 Popsal, jak budou v Arpanetu posílány pakety
* 1981 RFC791 definoval internetový protokol V4 – stále široce používaný dodnes
* 1982 RFC 821 Simple Mail Transfer Protocol
* 1987 Domain Name System – jak se doménová jména převádějí na IP adresy
* 1999 RFC 2616 Hypertext Transfer Protocol – zásadní pro prohlížení webu


> **Callout**
>
> **Bitcoin Improvement Proposal** (BIP) používá podobný přístup jako RFC, ale zaměřuje se výhradně na vylepšení samotného Bitcoinu, nikoli na vývoj nových nebo alternativních protokolů. Bitcoin také přebírá tento vrstevnatý model a uvidíte další protokoly popisované jako druhá nebo třetí vrstva.


Stejně jako se základní vrstvy modelu TCP/IP za poslední desetiletí téměř nezměnily a inovace probíhá ve vyšších vrstvách, očekává se, že základní vrstva Bitcoinu se nyní bude měnit velmi pomalu, zatímco řešení škálování jako Lightning a Liquid probíhají nad ní.

Dobrým příkladem toho, jak se základní protokoly časem obtížně mění, je IPv6. Očekávané vyčerpání adresního prostoru v IPv4 vytvořilo poptávku po novém protokolu. První návrh standardu vznikl v roce 1998, ale jako internetový standard byl schválen až v roce 2017. Přestože vyřešil mnoho problémů IPv4 a je mnohem více připravený na budoucnost, jeho zavádění v průmyslu je stále velmi pomalé. Během této doby bylo ve vyšších vrstvách definováno mnoho nových protokolů pro multimédia, e-mail atd.

##### Stavební bloky, které používá Bitcoin

Toto oddělení problémů vzájemné konektivity umožňuje, aby se protokoly vyvíjely nezávisle na vrstvách nad a pod nimi. Místo toho, aby bylo nutné vymýšlet řešení pro každou vrstvu zvlášť, může síť Bitcoin spoléhat na základní schopnosti sítě poskytované na fyzické a linkové vrstvě.


| Vrstva | TCP/IP původní |
| --- | --- |
| Aplikační | Používá systém doménových jmen (DNS) k identifikaci sousedních uzlů. Port 8333 signalizuje Bitcoin protokol. |
| Transportní | UDP pro FIBRE komunikaci mezi těžaři pro nízkou latenci. TCP pro P2P komunikaci mezi uzly. |
| Transportní | TOR směrování: Umožňuje anonymitu a soukromí. Broadcast protokol: Směruje provoz napříč sítí. |
| Linková | Funguje přes jakékoli médium (např. Ethernet, Wi-Fi atd.) |
| Fyzická | Fyzický přenos přes bezdrát, Ethernet nebo jiné hardwarové rozhraní. |


##### Bitcoin je neutrální protokol pro převod hodnoty, stejně jako HTTPS je protokol pro přenos informací

* **HTTPS**: zabezpečené webové stránky
* **SMTP**: Posílat e-maily
* **FTP**: Přenášet soubory
* **DNS**: Spravovat doménová jména
* **BTC**: Uchovávat a převádět hodnotu

Bitcoin umožňuje spolehlivě přenášet hodnotu mezi lidmi nebo zařízeními přes internet bez nutnosti třetí strany. Očekává se, že to odemkne obrovskou hodnotu.
