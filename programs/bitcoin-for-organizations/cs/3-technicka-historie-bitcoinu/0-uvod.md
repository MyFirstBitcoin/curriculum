# 3.0 Úvod

> **Dark – Abstrakt Bitcoin White Paper**
>
> **Čistě peer-to-peer verze elektronické hotovosti** by umožnila posílat online platby přímo od jedné strany ke druhé bez nutnosti procházet finanční institucí. **Digitální podpisy poskytují část řešení**, ale hlavní výhody jsou ztraceny, pokud je **důvěryhodná třetí strana** stále vyžadována k zabránění dvojitému utrácení. Navrhujeme řešení problému dvojitého utrácení pomocí **peer-to-peer sítě**. **Síť časově označuje transakce** tím, že je hashováním řetězí do probíhajícího řetězce **důkazu o vykonané práci založeného na hashi,** čímž vytváří záznam, který nelze změnit bez opětovného provedení **důkazu o vykonané práci**. Nejdelší řetězec slouží nejen jako důkaz posloupnosti událostí, ale i jako důkaz, že pochází z největšího fondu výpočetního výkonu CPU. Dokud většinu výpočetního výkonu ovládají uzly, které nespolupracují na útoku na síť, budou generovat nejdelší řetězec a předběhnou útočníky. **Samotná síť vyžaduje minimální strukturu. Zprávy jsou vysílány podle nejlepší snahy a uzly mohou síť kdykoliv opustit a znovu se připojit**, přičemž přijímají nejdelší řetězec důkazu o vykonané práci jako důkaz toho, co se stalo během jejich nepřítomnosti.


Bitcoin se neobjevil ve vakuu, ale stavěl na práci mnoha lidí v předchozích desetiletích. Tento modul prozkoumá základy internetu, na kterých Bitcoin staví, stejně jako výzkum a vývoj uznaný v whitepaperu.

V 70. letech se skupina jednotlivců zaměřila na to, jak se zejména vláda USA snažila omezit přístup ke kryptografii, a rozhodla se zajistit, aby tato technologie byla dostupná všem lidem k ochraně jejich soukromí online. Někteří z těchto raných průkopníků se také zaměřovali na potenciální přínosy digitálního systému „zdravých peněz“, který by bylo možné použít k uchovávání a výměně hodnoty přes vznikající internet. Friedrich Hayek – přední představitel rakouské ekonomie – si představoval, jak by mohla vypadat ideální měna založená na volné tržní soutěži, a to ještě před érou internetu, ale rozhodl se, že je to technicky a politicky neproveditelné. Tato skupina, která se vyvinula v Cypherpunks, se kromě digitálního soukromí pokusila realizovat Hayekovu vizi digitálních peněz, ale tyto pokusy selhaly až do chvíle, kdy Satoshi zveřejnil své myšlenky na mailing listu.

* Protokol TCP/IP (1976)
* Protokoly pro kryptosystémy s veřejným klíčem – Ralph Merkle (1980)
* Digicash – David Chaum (1989)
* Digitální časové razítkování (90. léta)
* Hashcash – Adam Back (1997)
* BitTorrent – Bram Cohen (2001)
* Znovupoužitelný POW – Hal Finney (2004)
* Bitcoin Whitepaper – Satoshi Nakamoto (2008)

Klíčovým vlivem na vývoj Bitcoinu byl vznik hnutí Cypherpunk v 90. letech. Vyvinuli několik kryptografických technologií včetně kryptografie s veřejným klíčem, která uživatelům umožňuje bezpečně a soukromě komunikovat a sdílet informace. Mnoho zde popsaných vývojů a lidé, kteří se na nich podíleli, byli součástí této skupiny.

Potřeba digitální hotovosti byla také rozpoznána a bylo učiněno několik pokusů ji vytvořit, ale ty měly omezení, která jim zabránila v úspěchu. Geniálnost Satoshiho Nakamota spočívala v tom, že tyto schopnosti spojil dohromady a spolu s vlastními inovacemi na nich postavil Bitcoin protokol, který se používá dodnes. V následujících sekcích prozkoumáme některé z těchto vývojů a vysvětlíme, jak pomohly utvářet návrh Bitcoinu. Také si povíme, jaké chybějící dílky skládačky Satoshi dokázal vyřešit.
