# 8.2 Mesures pour l'analyse du grand livre

Parce que la transparence de Bitcoin est différente des systèmes financiers traditionnels — où la majeure partie des flux monétaires se déroule à huis clos, derrière les portes des institutions — elle donne naissance à un riche domaine d’analyses on-chain, où les données au niveau du réseau deviennent une lentille pour comprendre le comportement des utilisateurs, les flux monétaires et les tendances à long terme. Ces métriques peuvent aider à répondre à des questions spécifiques, telles que le niveau d’activité du réseau, si les coins sont accumulés ou vendus, et si le réseau devient plus sécurisé.

Comprendre ces métriques est utile non seulement pour les utilisateurs de Bitcoin, mais aussi pour les chercheurs ou les décideurs politiques cherchant à obtenir des informations sur ce système financier d’une transparence unique.

Cette section contient quelques métriques couramment utilisées pour analyser l’activité de Bitcoin, regroupées en sous-catégories. Il ne s’agit pas d’une liste exhaustive. Consultez [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) pour une liste plus complète et des descriptions.



#### 8.2.1 Métriques des adresses

Les métriques des adresses sont utiles à surveiller dans le temps car elles indiquent le niveau d’activité sur le réseau Bitcoin. Par exemple, à mesure que Bitcoin est adopté, le nombre d’adresses actives augmente. Nous pouvons examiner cela plus en détail en isolant le nombre d’adresses qui détiennent un montant minimum spécifié de Bitcoin, disons 0,1 BTC, sur une certaine période, comme un an. Bien que cela donne une vue de l’adoption de Bitcoin dans le temps, c’est imparfait car un individu peut posséder plusieurs adresses Bitcoin. À l’inverse, les plateformes d’échange ou les ETF peuvent apparaître comme des entités uniques alors qu’elles détiennent des fonds pour un grand nombre d’individus.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adresses détenant plus de X BTC par an. Source : Bitcoin Magazine Pro._

En comparant les adresses avec le prix actuel du marché du BTC, il est possible de voir le pourcentage global d’adresses Bitcoin en profit. Cela nous permet de suivre le sentiment du marché, car nous pouvons voir quelle proportion du marché conserve du BTC en profit ou en perte.

Par exemple, le **Pourcentage de profit non réalisé** du graphique ci-dessous montre la proportion de toutes les adresses du registre avec un profit non réalisé mesuré en dollars américains. Notez que, puisque le graphique ci-dessous a été pris près du sommet historique de Bitcoin, le pourcentage d’adresses affichant un profit non réalisé est proche de cent pour cent. Nous pouvons également voir que des périodes prolongées de pourcentage de profit non réalisé en dessous d’un écart-type de la moyenne sont inhabituelles. Par conséquent, une chute sous cette ligne peut suggérer un bon point d’entrée pour les acheteurs.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Pourcentage de profit non réalisé. Source : checkonchain.com_



#### 8.2.2 Indicateurs on-chain

Les indicateurs on-chain sont utiles car ils offrent un aperçu du comportement du réseau, au-delà de ce que les métriques de prix et d’adresses peuvent montrer. Ils aident les analystes à comprendre les actions et le sentiment des différents types de participants, comme les détenteurs à long terme par rapport aux traders à court terme, en suivant la manière dont les coins sont détenus, déplacés ou valorisés dans le temps. Ces indicateurs s’appuient sur la nature transparente du registre pour révéler des dynamiques de marché cachées comme l’accumulation, la distribution, ou même la conviction des investisseurs. Cela les rend particulièrement utiles pour identifier les tendances structurelles, évaluer si le marché est surchauffé ou sous-évalué, et anticiper les points de retournement dans un cycle de marché.

Par exemple, en examinant la valeur des avoirs en BTC depuis leur dernière transaction, nous pouvons déduire si le marché est en difficulté (comme cela pourrait être le cas lors d’un creux majeur du cycle). Cette métrique est appelée **Prix réalisé** et nous donne un « coût moyen d’acquisition » de tous les BTC en circulation. Si le prix du marché tombe en dessous du prix réalisé, cela montre qu’en moyenne la majorité des adresses détiennent une perte latente.

En regroupant davantage les données du registre en tranches d’âge, nous pouvons montrer comment la quantité de BTC se déplace entre les adresses au fil du temps, ce qui crée des motifs ondulatoires sur un graphique appelés **vagues HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Vagues HODL de Bitcoin. Source : Bitcoin Magazine Pro._

Les vagues HODL montrent ce que font les détenteurs à long terme, à moyen terme et à court terme avec leur BTC. Par exemple, dans le graphique ci-dessus, les détenteurs à court terme sont représentés en rouge et orange et nous pouvons voir des pics d’activité lorsque ce groupe se précipite pour acheter près des sommets du marché. À l’autre extrémité, nous pouvons voir que les détenteurs à très long terme (en violet et bleu) augmentent régulièrement leur part globale du réseau, indiquant une forte conviction parmi ces groupes. Le graphique est imparfait car certains coins peuvent passer d’anciennes à de nouvelles adresses sous le contrôle du même utilisateur. Cependant, il offre une vue intéressante de la conviction des détenteurs à long terme.

Une autre façon d’examiner le « smart money » des détenteurs à long terme est d’étudier le **Coin Days Destroyed** (CDD). Le concept de « Coin Days » est un multiple du nombre de BTC multiplié par le nombre de jours depuis le dernier mouvement des coins. Par exemple, 5 BTC qui n’ont pas bougé depuis 100 jours ont accumulé 500 coin days et 10 BTC qui n’ont pas bougé depuis 10 jours ont accumulé 100 coin days. De cette façon, nous donnons un poids supplémentaire aux coins détenus plus longtemps. Lorsque ces coins sont déplacés, ces coin days sont « détruits ». Cet indicateur montre des augmentations du CDD lors de mouvements de prix significatifs, ce qui fournit aux analystes un moyen de distinguer l’activité de marché de routine des changements significatifs dans le sentiment des détenteurs à long terme.

Une autre métrique qui peut aider à identifier si le marché sous-évalue ou surévalue le BTC est la valeur de marché sur la valeur réalisée, ou **MVRV**. Elle est simplement calculée comme le ratio de la valeur de marché (nombre de BTC en circulation multiplié par le prix du marché) divisé par la valeur réalisée (la somme de tous les BTC depuis leur dernier mouvement). Un MVRV élevé suggère que plus de coins sont en profit (souvent observé près des sommets du marché) et un MVRV faible indique que de nombreux coins sont détenus à perte (observé près des creux du marché).



#### 8.2.3 Métriques du minage

Les métriques du minage sont utiles pour comprendre la sécurité, les incitations économiques et la santé globale du réseau Bitcoin. Des métriques telles que le hashrate, les revenus des mineurs, la difficulté et les ratios de frais révèlent la quantité de puissance de calcul qui sécurise la blockchain et la façon dont les mineurs sont rémunérés pour leurs activités.

Le **Hashrate** du réseau Bitcoin est peut-être l’indicateur le plus souvent cité de la santé du réseau et de la force de sa sécurité. Puisque le processus de minage sécurise le réseau et confirme que les transactions sur le registre sont valides, plus le niveau de puissance de calcul (ou de hachage) est élevé, plus il serait difficile pour un acteur malveillant de submerger et d’attaquer le réseau.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate de Bitcoin. Source : Bitcoin Magazine Pro._

Le graphique ci-dessus montre qu’en mai 2025, la puissance de calcul totale du réseau s’élève à environ 900 TeraHash/s (900 mille milliards de calculs cryptographiques « hash » par seconde). Si le hashrate augmente, cela montre que le réseau devient plus sécurisé, ce qui est rassurant pour les utilisateurs.

Le Puell Multiple (élaboré par David Puell) examine le cycle du marché du point de vue des mineurs et de leurs revenus. La métrique est calculée en divisant l’émission quotidienne de BTC (en USD) par la moyenne mobile sur 365 jours de la valeur d’émission quotidienne. Cette métrique aide à identifier les périodes de stress ou de soulagement pour les mineurs. Historiquement, un multiple supérieur à 3 a précédé une baisse de la valeur du marché du BTC, car cela indique que les mineurs sont très rentables. Une valeur inférieure à 0,5 indique un stress et a historiquement signalé des creux de marché pour la valeur du BTC.
