# 5.1 L'impact du Bitcoin sur les responsables informatiques

> Toute personne informée doit connaître le Bitcoin, car il pourrait s'agir de l'un des développements les plus importants au monde.  
_Leon Luow_



#### 5.1.0 Introduction

Les responsables informatiques ont des responsabilités envers l'entreprise, utilisant la technologie à la fois pour stimuler l'innovation et la compétitivité de leur société, ainsi que pour trouver des moyens d'améliorer l'efficacité interne afin de réduire les coûts.

Il existe plusieurs risques et idées reçues courants autour du Bitcoin qu'il est utile de comprendre et sur lesquels il convient de donner des conseils :

* Il est souvent perçu comme faisant partie d'une industrie ‘crypto’ plus large, et de solutions basées sur l'une des innovations clés utilisées, la blockchain.
* Il est perçu comme ‘gaspillant de l'énergie’ pour faire fonctionner le réseau.
* Il existe un risque pour les utilisateurs du Cloud Public que l'environnement puisse être piraté et utilisé pour ‘miner’ du Bitcoin ou d'autres crypto-monnaies par un acteur malveillant, entraînant une facture très importante et inattendue, ainsi que des impacts sur les performances des applications métier.
* Il y a un manque de connaissance de la technologie derrière le Bitcoin.

Du côté positif, le Bitcoin pourrait bénéficier à toute entreprise en :

* Étant ajouté à la trésorerie comme un actif, soit miné directement, soit acheté sur le marché ouvert.
* Utilisant des ressources autrement inactives pour miner du Bitcoin pour l'entreprise.
* Fournissant une justification pour des investissements dans des solutions d'IA nécessitant des ressources de calcul haute performance similaires.
* Ajoutant un moyen de paiement alternatif pour l'achat de services ou produits de l'entreprise.
* Réduisant les frais de transaction FX mondiaux.
* Offrant un avantage supplémentaire aux employés via des incitations basées sur les paiements Lightning.
* Créant de nouveaux flux de revenus pour l'entreprise basés sur le Bitcoin.

Tout responsable informatique doit prendre le temps de comprendre le Bitcoin, son impact potentiel et les risques associés, ainsi que les avantages potentiels, afin de pouvoir fournir des conseils et un leadership à l'entreprise.

> Le Bitcoin est une réalisation cryptographique remarquable. La capacité de créer quelque chose qui n'est pas duplicable dans le monde numérique a une valeur énorme. Beaucoup de gens construiront des entreprises sur cette base.  
_Eric Schmidt_



#### 5.1.1 Risques et idées reçues autour du Bitcoin

##### Le Bitcoin comme partie d'une industrie ‘crypto’ plus large.

Le Bitcoin a été la première tentative réussie de créer un actif numérique fini et a donné naissance à toute une industrie d’‘alt-coins’ qui tentent d’utiliser une partie de la technologie sous-jacente pour soit ‘améliorer’ le Bitcoin, soit construire une solution pour répondre à d’autres opportunités de marché potentielles.

Les fournisseurs de cloud public ont créé des plateformes blockchain pour permettre aux entreprises de construire ces solutions, cependant l'intérêt pour celles-ci a tendance à fluctuer en fonction de la mode dans l'industrie ; en effet, Microsoft a arrêté son service blockchain en 2021.

* Jusqu'en 2017, le Bitcoin représentait jusqu'à 95 % de la capitalisation totale du marché crypto.
* La première vague d’ICOs crypto ‘alternatives’ a vu la domination chuter à un niveau historiquement bas de 37,6 %.
* Comme celles-ci n'ont pas apporté de véritables bénéfices commerciaux et ont commencé à disparaître, la domination du Bitcoin a recommencé à augmenter.
* En 2021, alors que le prix du Bitcoin augmentait, une nouvelle vague de solutions alternatives basées sur les NFT est apparue sur le marché, ce qui a de nouveau fait baisser la domination du Bitcoin.
* Après que cette mode n'a elle aussi pas apporté de réels bénéfices, la domination du Bitcoin a recommencé à grimper.
* Lorsque le Bitcoin entrera dans un nouveau marché haussier, il est possible qu'une nouvelle vague d’‘alt-coins’ émerge pour capitaliser sur une nouvelle tendance, mais il est probable qu'elle connaisse un sort similaire.

Si l'entreprise vient voir le responsable informatique avec le dernier ‘objet brillant’ promu pour une application particulière de la blockchain, ou comme alternative au Bitcoin, il est important de garder cette tendance à l'esprit et de se demander :

* Quel est le but de la blockchain ?
* Une blockchain est-elle nécessaire ou souhaitable, étant donné ses inconvénients de performance par rapport à une base de données relationnelle centralisée ?
* Qui peut modifier le protocole et quel est l'impact sur la solution ?
* Quels sacrifices ont été faits en matière de sécurité ou de décentralisation pour fournir la performance annoncée ?
* Quel avantage cela peut-il apporter qui ne peut pas être fourni en utilisant le Bitcoin et les protocoles associés, comme Lightning ?

##### Les implications de l'exploitation du Bitcoin

Selon le secteur dans lequel l'entreprise opère, il peut y avoir des avantages potentiels à l'activité de minage de Bitcoin, généralement lorsque la chaleur générée peut être utilisée à bon escient. Cependant, il y a souvent des réticences en raison de la perception que le Bitcoin est mauvais pour l'environnement, gaspille de l'énergie ou a peu d'intérêt.

En tant que responsable informatique, comprendre cette dynamique et s'il existe des avantages potentiels pour l'entreprise est nécessaire pour fournir des conseils efficaces. La position par défaut a généralement été que le Bitcoin n'est pas ‘bon pour l'environnement’ et ‘gaspille de l'énergie’. Cependant, cela change rapidement, des rapports plus positifs sont publiés, et il est attendu que ce récit évolue vers une vision où le minage de Bitcoin peut être vu comme positif pour l'environnement et la transition vers les énergies renouvelables. C'est un point sur lequel de nombreuses entreprises se concentrent dans leurs initiatives ESG.

##### Comprendre les risques potentiels liés au minage de crypto

Il y a eu par le passé des exemples où l'environnement cloud public géré par une entreprise a été pris en main par des pirates, qui peuvent très rapidement activer des ressources de calcul supplémentaires pour miner de la crypto. Plus il y a de ressources activées avec le profil de performance le plus élevé (et donc le plus coûteux), plus le pirate a de chances de miner du Bitcoin ou toute autre crypto. Cela s'appelle le ‘Crypto-Jacking’ - selon AWS :

‘Il s'agit d'un type de cybercriminalité qui implique l'utilisation non autorisée d'appareils (ordinateurs en périphérie, smartphones, tablettes, voire serveurs) pour miner de la cryptomonnaie. À mesure que les prix des cryptomonnaies augmentent et que des appareils en périphérie plus puissants dotés de capacités GPU sont utilisés pour exécuter des cas d'usage de Machine Learning en périphérie, la menace de cryptojackers exploitant des vulnérabilités de sécurité sur ces appareils augmente. Lorsque cela se produit, les ressources de calcul en périphérie sont utilisées pour miner de la cryptomonnaie, ce qui entraîne une utilisation accrue du CPU/GPU, une dégradation des performances des applications en périphérie et une augmentation des temps de traitement d'inférence ML en périphérie.’

Il est donc essentiel que toute utilisation de ressources cloud publiques soit correctement conçue en suivant les meilleures pratiques. Celles-ci sont généralement décrites dans une forme de Cadre d'Adoption du Cloud, présentant des recommandations en matière de sécurité, de performance, de surveillance, de résilience et d'opérations. Le responsable informatique doit s'assurer que ces recommandations sont suivies, et qu'une forme de surveillance en temps réel est activée pour identifier et atténuer toute attaque avant que des factures importantes ne soient générées.

##### Manque de connaissance de la technologie utilisée par le Bitcoin

Il existe de nombreuses idées reçues sur la technologie derrière le Bitcoin, ce qui conduit à des questions sur la possibilité qu'il soit piraté, sur l'énergie utilisée, ou s'il sera dépassé par une nouvelle version comme cela s'est souvent produit avec la technologie. En tant que responsable technique, avoir une compréhension de la technologie sous-jacente serait utile pour positionner correctement le Bitcoin en interne et atténuer ces préoccupations.



#### 5.1.2 Du côté positif.

##### Le Bitcoin comme actif de trésorerie

Il existe des avantages financiers potentiels pour une entreprise à inscrire le Bitcoin dans ses livres comme actif de trésorerie.

* Réserve de valeur et protection contre l'inflation
* La confiance décroissante dans les monnaies fiduciaires comme réserve de valeur
* Risque de contrepartie dans le secteur bancaire
* Avantage du premier entrant pour les entreprises qui ajoutent du Bitcoin à leur trésorerie

Bien que les implications financières de cette démarche du point de vue de la comptabilité ne relèvent pas du rôle du responsable informatique, comprendre comment cela pourrait fonctionner et comment le Bitcoin peut être acheté, stocké et sécurisé en fait partie.

Il existe des services sur le marché qui aident à acheter, conserver et proposer des services de prêt sur les actifs stockés. Si ce sujet devient une discussion au sein de l'entreprise, ce qui devrait être le cas, le responsable informatique peut aider à qualifier les éventuels prestataires tiers proposant ces services. Une diligence raisonnable pour s'assurer que le ou les services proposés répondent aux besoins de sécurité, de transparence et de fonctionnalités nécessaires aidera à sélectionner un partenaire fiable.

##### Avantages du minage de Bitcoin

L'utilisation des centres de données ne devrait qu'augmenter à l'avenir, et une grande partie des coûts d'exploitation d'un centre de données consiste à dissiper la chaleur générée. Cela est particulièrement vrai pour les applications utilisant le calcul haute performance, telles que l'IA/ML et le minage de Bitcoin.

Des entreprises de différents secteurs à travers le monde ont identifié comment cette production accrue de chaleur peut devenir un avantage net pour l'entreprise au lieu d'un coût, en utilisant la chaleur générée pour :

* Piscines/Spas
* Centres aquatiques
* Culture de fleurs/légumes dans des serres
* Chauffer les locaux de l'entreprise et les systèmes d'eau chaude

Cela peut être réalisé soit en collaborant avec une entreprise de minage de Bitcoin qui utilise les installations de l'entreprise pour miner du Bitcoin à des fins lucratives et fournit la chaleur pour un usage général, soit

l'entreprise peut effectuer cette fonction elle-même afin de constituer directement une trésorerie en Bitcoin. Cette approche peut également aider une entreprise dans ses initiatives ESG.

Une méthode plus indirecte pour obtenir certains de ces avantages consiste à déplacer les besoins en calcul vers des centres de données qui adoptent cette approche et proposent de l'espace rack ou de l'infrastructure dans le cadre d'un service managé, en répercutant une partie de ces économies de coûts à l'entreprise.

En tant que responsable informatique, rester informé sur ce sujet vous aidera à conseiller l'entreprise dans l'adoption de solutions susceptibles de lui être bénéfiques.

##### Bitcoin et IA

L'utilisation de l'IA et du ML devrait croître considérablement dans les prochaines années. L'intersection entre Bitcoin et l'intelligence artificielle inaugure une nouvelle ère d'innovation numérique, notamment grâce à l'intégration de l'IA avec le Lightning Network de Bitcoin. Cette union est sur le point de révolutionner des aspects d'Internet, des micropaiements aux agents économiques en ligne pilotés par l'IA.

* L'affinage des modèles d'IA est une étape essentielle dans le développement de l'IA – les micropaiements via Lightning permettent aux individus du monde entier d'être rémunérés par tâche en Bitcoin, encourageant ainsi la participation.
* Dans les scénarios où des entités d'IA effectuent des transactions pour des services, le réseau Lightning est un outil indispensable pour les activités économiques pilotées par l'IA où la rapidité est essentielle.
* Une fois le système d'IA développé, les micropaiements pourraient faciliter un modèle de paiement à l'utilisation plus équitable, où les utilisateurs ne paient que pour les ressources d'IA qu'ils consomment.

Pour toute entreprise envisageant l'utilisation de l'IA, que ce soit comme service à acheter ou dans le développement de sa propre solution d'IA, il est important de comprendre comment Bitcoin et Lightning s'intègrent et ajoutent de la valeur à toute solution.

Source :[https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/](https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/)

##### Nouvelles options de paiement en magasin

Toute entreprise qui accepte des paiements pour des services, que ce soit directement en magasin ou en ligne, pourrait bénéficier de l'acceptation des paiements en Bitcoin de la manière suivante :

* Augmentation de la fréquentation et croissance de l'activité en ciblant les clients Bitcoin
* Frais de paiement faibles voire nuls
* Règlement instantané
* Aucun rétrofacturation

D'un point de vue comptable, il existe différentes façons de gérer le Bitcoin reçu, en le conservant dans la trésorerie ou en le convertissant directement en monnaie fiduciaire, ou une combinaison selon l'accord. Selon l'entreprise, il peut y avoir des implications techniques pour y parvenir, telles que de nouveaux terminaux de point de vente ou une intégration avec une solution logicielle pour les paiements en ligne, dont le responsable informatique doit comprendre les implications techniques si cela est retenu comme objectif pour l'entreprise.

##### Réduction des frais de transfert FX mondiaux

Pour les entreprises qui transfèrent de grandes sommes d'argent à l'international, les coûts et la complexité de ces opérations peuvent souvent être un défi. De nouvelles solutions basées sur Bitcoin sont proposées sur le marché, réduisant ces coûts et offrant un règlement plus rapide et immédiat. L'adoption de ces services pourrait potentiellement être bénéfique pour l'entreprise, et comprendre ce marché, les services proposés et travailler avec l'équipe comptable pour mettre en œuvre la meilleure solution nécessite un niveau de connaissance et de compréhension technique que le responsable informatique peut apporter.

##### Avantages pour les employés

La plupart des entreprises cherchent comment offrir des avantages et des incitations à leurs employés pour améliorer le recrutement et la fidélisation. Récemment, plusieurs athlètes professionnels et politiciens de renom ont annoncé qu'ils prenaient tout ou partie de leur salaire en Bitcoin. La possibilité de verser une partie du salaire en Bitcoin comptera pour les employeurs lorsque cela fera la différence dans des recrutements clés, ou lorsque des membres essentiels de l'équipe commenceront à demander cette option ou à chercher des employeurs qui la proposent ailleurs.

* Intégrer l'option d'une rémunération totale ou partielle en Bitcoin donne à une organisation un avantage concurrentiel pour anticiper la tendance. Les solutions de paie en Bitcoin rendent ce processus d'intégration simple.
* Des entreprises comme MicroStrategy cherchent des moyens d'encourager la performance ou même la participation aux réunions avec des micro-paiements basés sur Lightning.

Bien que la décision de mettre en place de tels avantages pour les employés ne relève pas directement du responsable informatique, fournir une compréhension des raisons pour lesquelles cela peut être bénéfique, des solutions disponibles pour y parvenir et des implications techniques de la mise en œuvre peut tout à fait lui incomber. Les directeurs informatiques qui proposent de manière proactive des idées à leurs pairs peuvent démontrer leur valeur stratégique élargie pour l'entreprise.

##### Nouvelles opportunités de marché

Comme l'a déclaré Google, de nombreuses entreprises chercheront à créer de nouvelles sources de revenus basées sur l'écosystème Bitcoin en pleine croissance. Cela peut ouvrir de nouveaux marchés à considérer pour l'entreprise, que le responsable informatique peut jouer un rôle clé dans l'évaluation de leur pertinence, des défis techniques et des opportunités potentielles qu'ils peuvent offrir.



#### 5.1.3 Résumé

On s'attend à ce que l'adoption du Bitcoin se poursuive, devenant de plus en plus importante pour les entreprises au fil du temps, affectant à la fois les stratégies et initiatives commerciales et techniques dans plusieurs domaines. En tant que responsable technique de l'entreprise, le responsable informatique bénéficiera d'une avance sur ces évolutions, en conseillant l'entreprise et en veillant à ce qu'elle tire le meilleur parti de la mise en œuvre de solutions Bitcoin à travers l'organisation.
