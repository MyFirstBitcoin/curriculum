# 3.4 Hashcash

Hashcash a été créé par Adam Back, un autre des premiers innovateurs dans ce domaine. Adam avait un vif intérêt pour les marchés libres et la vie privée sur Internet, et il a découvert la liste de diffusion des Cypherpunks, qu'il a rejointe et dont il est devenu un membre actif.

Il s'intéressait beaucoup à la monnaie numérique et a proposé quelques idées sur la façon dont le groupe pourrait potentiellement collaborer plus étroitement avec Chaum sur DigiCash, mais cela n'a mené à rien. Il a alors porté son attention sur un autre problème émergent : le spam par e-mail. Lui et les autres Cypherpunks voulaient trouver une solution au problème du spam, où il était trivial pour les spammeurs de créer et d'envoyer des milliers d'e-mails qui encombraient les réseaux. Sa solution innovante était basée sur le hachage – la capacité, grâce à la cryptographie, de transformer n'importe quelle donnée en une chaîne unique et aléatoire d'une longueur spécifique, afin de créer l'équivalent d'un « timbre » numérique devant être ajouté à l'e-mail pour qu'il soit considéré comme valide et transmis sur le réseau. Un coût négligeable pour un e-mail authentique, mais prohibitif pour un spammeur.

L'innovation clé apportée par Hashcash a été de lier des ressources du monde réel – la puissance de calcul – à un réseau numérique. Alors que les ressources numériques pouvaient jusqu'alors être reproduites sans limite, le nombre de « hashcash » créés était limité par la quantité d'énergie que les gens étaient prêts à y investir.

Bien que la solution remplissait certains des critères qu'Adam jugeait nécessaires pour un système de monnaie numérique ; elle était anonyme, résiliente et sans confiance, chaque hashcash n'était pas réutilisable et n'était pas vraiment rare. Il a suggéré d'autres moyens de résoudre ces problèmes en utilisant des tiers externes.

##### BitGold

Nick Szabo s'est appuyé sur le concept de Hashcash et la preuve de travail pour proposer une solution alternative, qu'il a décrite sur une liste de diffusion un an après la publication de Hashcash, en 1998.

Bien que cette proposition se rapproche d'une solution, elle présentait encore plusieurs défis.

* Qui gérerait le registre de propriété des hash et comment leur faire confiance ?
* Le hachage deviendrait généralement moins coûteux avec le temps, un défi également pour HashCash.

Comme les hash liés seraient horodatés, il a proposé une forme de suivi historique de la difficulté du hachage à un moment donné ; un hash plus ancien nécessiterait plus de puissance de calcul qu'un hash plus récent, car les coûts auraient diminué. Malheureusement, cela signifiait que les hash ne seraient pas « fongibles », c'est-à-dire de valeur égale, ce qui est considéré comme une caractéristique clé de la monnaie numérique. Pour aider à résoudre ce problème, Nick a suggéré une forme de « banque libre » fonctionnant au-dessus de BitGold, qui pourrait agréger différents groupes de hash qui seraient alors valorisés de la même manière.

##### B-Money

Peu de temps après la proposition de Bit Gold, Wei Dai a proposé une solution similaire. Il avait déjà développé plusieurs autres outils pour les Cypherpunks et avait ses propres idées sur la monnaie numérique.

Sa proposition ressemblait à Bit Gold en ce qu'elle utilisait des signatures numériques pour transférer de l'argent, et les enregistrements des transactions seraient stockés sur un registre, contenant des clés publiques et le montant d'unités monétaires attribuées à chacune. Comme pour Bit-Gold, les tiers de confiance étaient considérés comme des failles de sécurité, et l'on pensait qu'un système de monnaie électronique ne devait pas dépendre d'une seule entité pour suivre les soldes, les transactions ou empêcher la double dépense.

Wei-Dai a proposé plusieurs solutions à ces problèmes, dont l'une était qu'au lieu qu'une entité centrale (ou plusieurs) maintienne le registre, TOUS les nœuds en conserveraient une copie. Si tous les utilisateurs vérifiaient leur propre registre et la validité de chaque transaction, tant que tous les nœuds restent à jour, les registres devraient rester synchronisés sur le réseau. Ce système hautement distribué serait difficile à corrompre.

Wei Dai a reconnu que cela ne résolvait pas le problème des généraux byzantins (1), car les nœuds pouvaient facilement perdre la synchronisation ou simplement mentir. Il a suggéré d'autres méthodes, comme avoir un sous-ensemble de serveurs « de confiance » qui maintiennent le registre, et créer des incitations financières pour que ces serveurs restent honnêtes.

Pour la politique monétaire, il a proposé d'indexer le pouvoir d'achat du B-Money sur une sorte d'indice des prix à la consommation externe. Il voulait que la même quantité de B-Money puisse acheter une part égale de l'indice au fil du temps, assurant ainsi une certaine stabilité des prix. Ainsi, n'importe qui pouvait générer de nouvelles unités monétaires en fournissant un hash valide, mais la difficulté de générer un hash pouvait évoluer dans le temps en fonction des coûts CPU et de l'indice des prix, de sorte que chaque unité serait « immuable ».
