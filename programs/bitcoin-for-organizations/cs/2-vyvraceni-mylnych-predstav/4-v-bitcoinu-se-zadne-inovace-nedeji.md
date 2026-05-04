# 2.4 V Bitcoinu se žádné inovace nedějí.

> Vytvoření tisíce lesů je ukryto v jednom žaludu.  
_Ralph Waldo Emerson_

Kritici se často snaží tvrdit, že Bitcoin je „zastaralá“ nebo „mrtvá“ technologie, protože základní protokol se nemění tak často jako u konkurenčních blockchainů. Toto tvrzení však ignoruje jak důvody, proč jsou změny v Bitcoinu přijímány pomalu, tak množství inovací, které probíhají na vyšších vrstvách sítě, například v Lightning Network. Také přehlíží, že mnoho našich nejodolnějších a nejflexibilnějších technologií se na základní vrstvě také nevyvíjí rychle.

Například žádné inovace neprobíhají ani v Transmission Control Protocolu (TCP), který je základem internetu. TCP byl poprvé vytvořen v roce 1974. Naposledy byl TCP aktualizován v roce 1982. Plní to, co má. Není dokonalý a vedou se debaty o tom, zda je potřeba upgradovat IPv4, aby podporoval budoucí rozvoj internetu. Nicméně tvrdit, že od roku 1982 na internetu neproběhla žádná inovace, by bylo opravdu pozoruhodné. Veškeré inovace totiž probíhají „na“ TCP, nikoliv „v“ TCP.

Drtivá většina inovací, které probíhají, není „v“ Bitcoinu, ale „na“ Bitcoinu. Jednoho dne pravděpodobně nebude žádná inovace „v“ Bitcoinu, a to by mělo být cílem, nikoliv kritikou, protože to bude odrazem toho, jak zásadní se stal pro podporu globální ekonomiky tím, že poskytuje základy pro globální, neutrální a bezpovolené zdravé peníze. Peníze, které jsou zdravé jak v ekonomickém smyslu díky pevně stanovené nabídce a neměnné účetní knize, tak i v technologickém smyslu, protože se nemění a běží bez přerušení po mnoho let. Bitcoin již dosáhl 100% dostupnosti za posledních 10 let.

Bylo by však znepokojivé, kdyby se žádné inovace neděly „na“ Bitcoinu. Podívejme se na to za posledních 10 let:



#### „V“ Bitcoinu

Segregated Witness (SegWit) byl implementován v roce 2017, aby chránil před změnitelností transakcí a zvýšil kapacitu bloků. SegWit byl také nezbytným předpokladem pro efektivní fungování lightningu a některých sidechainů.

Taproot byl implementován v roce 2021 a umožňuje seskupování a ověřování více podpisů díky začlenění Schnorrova podpisu, zavádí skriptovací jazyk pro složitější funkce a zvyšuje soukromí a odolnost transakcí vůči cenzuře.



#### „Na“ Bitcoinu

##### Liquid Sidechain

Liquid sidechain byl spuštěn v roce 2018. Liquid, stejně jako jiné sidechainy, je samostatná blockchainová účetní kniha, která je propojena s hlavním Bitcoin blockchainem podle předem stanovených pravidel. Tato pravidla jsou dostatečně flexibilní, aby umožnila Liquid chainu rozvíjet se a začleňovat vylepšení designu a škálovatelnosti v průběhu času. Propojení s Bitcoin blockchainem však zajišťuje, že celkový limit nabídky 21 milionů bitcoinů je zachován na obou řetězcích.

Aktivum v Liquid, L-BTC, je dvoucestně navázáno na bitcoin na hlavním řetězci. Existují kompromisy mezi náklady, rychlostí, soukromím a bezpečností, které činí L-BTC ideálním pro některé aplikace. Náklady, rychlost a soukromí jsou u L-BTC zlepšeny, za cenu určité důvěry v organizace tvořící Liquid Federaci, které společně ovládají proces 11 z 15 multisig pro převod L-BTC na bitcoin a zpět.

##### Lightning Network

Lightning Network byla spuštěna v roce 2018. Lightning je navržen jako síť plateb peer-to-peer ve formě grafu uzlů propojených kanály; není to blockchain. Bitcoin je uzamčen provozovatelem uzlu na hlavním blockchainu, aby byl k dispozici pro použití v Lightning Network, což zajišťuje, že je používán pouze „skutečný“ bitcoin. Uzly pak mohou mezi sebou otevírat likviditní kanály prostřednictvím multisig chytrých kontraktů. Platby hledají cestu sítí od zdroje k cíli, optimalizují náklady s ohledem na to, že mezi každým krokem v cestě musí být dostatečná likvidita správným směrem. Lightning Network výrazně zlepšuje náklady, rychlost a soukromí výměnou za snížení bezpečnosti (nebo zvýšení požadované důvěry) a zvýšení složitosti. Je však určena pro vysoký objem, nízkou hodnotu každodenních plateb, takže tento kompromis je považován za velmi rozumný pro miliony denních transakcí (zdroj: River, 2023).

##### Chaumovské eCash mincovny

Fediminty lze chápat jako komunitně omezenou lightning síť. Jsou navrženy tak, aby využívaly přirozenou důvěru, která existuje v určitých komunitách (např. rodiny, vesnice, skupiny přátel), výměnou za zjednodušení složitosti a zvýšení soukromí uživatelů. Jsou to modulární, open source protokoly pro úschovu a transakce s bitcoinem v komunitním kontextu. Jsou interoperabilní s Lightning Network.

**Cashu** je doručitelný token, který lze uložit na zařízení, například na mobilní telefon; jeho design je zaměřen na reprodukci výhod fyzické hotovosti v digitální podobě. Cashu je příkladem Chaumovského eCash postaveného na Bitcoinu a zvyšuje soukromí a odolnost vůči cenzuře a snižuje složitost výměnou za důvěru v používanou eCash mincovnu. Cashu mincovny vydávají eCash tokeny, které představují bitcoin a mohou být utraceny uživateli bez odhalení jejich identity. Cashu je interoperabilní s Lightning Network.

V budoucnu pravděpodobně vznikne mnoho dalších aplikací druhé vrstvy a na nich pak další aplikace třetí vrstvy.

Jako příklad neuvěřitelného množství aplikací budovaných na Lightningu zde uvádíme výňatek ze zprávy Lightning Network Research Report od společnosti River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
