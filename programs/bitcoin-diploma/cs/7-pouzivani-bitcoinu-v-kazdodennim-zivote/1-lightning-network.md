# 7.1 Lightning Network

Lightning Network je platební systém, který umožňuje uživatelům posílat a přijímat bitcoin rychle a levně. Funguje tak, že obě strany si vytvoří společnou peněženku, do které vloží část svých bitcoinů. Poté mohou mezi sebou provádět neomezené množství transakcí, aniž by bylo nutné každou z nich zaznamenávat na hlavní blockchain. Tímto způsobem obcházejí nutnost ověřovat a zahrnovat každou jednotlivou transakci do bloku, což celý proces zrychluje a zlevňuje. Nižší poplatky znamenají, že Lightning Network lze využít i pro malé platby, které nejsou na hlavním řetězci vždy výhodné. Jakmile se strany rozhodnou spolupráci ukončit, na blockchain se zapíše pouze konečný zůstatek.

Představte si den strávený v kavárně. Plánujete zůstat déle, proto si otevřete účet a předem zaplatíte místo toho, abyste platili za každou objednávku zvlášť. Na konci dne si s majitelem kavárny účet zkontrolujete a vyrovnáte. Pokud jste složili více, než jste utratili, dostanete rozdíl zpět; pokud jste utratili více, doplatíte zbytek.

Tento systém lze rozšířit i na více účastníků. Například při jedné z vašich návštěv kavárny přivedete kamaráda, kterého barman nezná a nemůže mu otevřít účet. Nabídnete kamarádovi, že může využít váš stávající účet a domluvíte se, že vám to později soukromě vyrovná. Představte si nyní tisíce lidí, kteří dělají totéž najednou, a umožňují ostatním využívat existující účty k propojení s ještě více lidmi — takto funguje Lightning Network!

S Lightningem můžete platit komukoliv v síti, nejen osobě, se kterou máte otevřený účet — pokud je mezi vámi nalezena cesta. Vaše platba může putovat sítí, dokud nedorazí k cíli, i když nemáte otevřený kanál přímo s příjemcem.

Podívejme se na rozdíl mezi on-chain a off-chain transakcemi.

##### On-chain transakce

To jsou transakce, které probíhají přímo na Bitcoin blockchainu. Potvrzení trvá přibližně 10 minut a poplatky závisí na velikosti transakce ve virtuálních bytech. Jsou bezpečnější, ale pomalejší, protože vyžadují konsensus celé sítě.

##### Transakce v Lightning Network

Tyto transakce probíhají na samostatné síti postavené nad Bitcoin blockchainem. Jsou vypořádány rychleji a s nižšími poplatky. Běžně se používají tam, kde je důležitější rychlost a cena transakce. Ve srovnání s on-chain transakcemi jsou méně bezpečné.


|  | Bitcoinová síť | Lightning Network |
| --- | --- | --- |
| Definice | Decentralizovaná digitální síť, která využívá kryptografii k zabezpečení finančních transakcí. | Platební protokol druhé vrstvy, který funguje nad Bitcoin blockchainem a umožňuje rychlejší a levnější transakce. |
| Výhody | Decentralizovaná a bezpečná. Žádné zpětné platby ani podvody. Lze používat pseudonymně. Celosvětové přijetí. | Rychlejší a levnější transakce. Vyšší škálovatelnost. Off-chain transakce nezatěžují blockchain. |
| Nevýhody | Pomalé zpracování transakcí. Vysoké poplatky u některých typů transakcí. Složitost pro začátečníky. | Může vyžadovat důvěru v operátory kanálů. Pro otevření a uzavření kanálů je potřeba on-chain transakce. |
