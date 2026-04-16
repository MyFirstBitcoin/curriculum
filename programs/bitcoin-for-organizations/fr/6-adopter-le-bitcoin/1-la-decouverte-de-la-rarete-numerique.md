# 6.1 La découverte de la rareté numérique

> Avec Bitcoin, une nouvelle forme de marchandise a été découverte… une sorte de marchandise numérique, générée par des ordinateurs et en partie conçue pour les ordinateurs. L’humanité a une histoire d’inventions majeures. Dans les livres d’histoire écrits à l’avenir, Bitcoin sera répertorié comme l’une d’entre elles.  
_Prof. Dr. Philipp Sander_



#### 6.1.0 La rareté en économie

Dans le domaine de l’économie, il est bien compris que la rareté est un principe clé qui détermine la valeur. Les biens et services qui connaissent une demande importante deviennent plus précieux si l’offre est limitée au point que la demande ne peut être facilement satisfaite. De plus, la rareté alimente la concurrence et constitue un moteur de la découverte des prix sur le marché. Sur un marché de concurrence libre, équitable et ouverte, les prix devraient s’établir au point où l’offre et la demande se rencontrent.

Les ressources qui connaissent une forte demande peuvent être considérées comme plus précieuses si elles sont finies ou plus difficiles à acquérir. Cela peut stimuler une demande accrue pour cette ressource, les acteurs du marché cherchant à en sécuriser l’accès. Cette dynamique peut être observée avec les ressources naturelles telles que les métaux précieux, le pétrole ou les « matières premières douces » comme les denrées alimentaires. La rareté, par conséquent, sous-tend la prise de décision économique, l’allocation des ressources et le coût d’opportunité. Dans un monde de ressources illimitées, tout serait également accessible et de très faible valeur. À l’inverse, la rareté confère de la valeur et favorise le commerce, l’investissement et l’innovation, car elle oblige les sociétés à gérer efficacement des ressources limitées.



#### 6.1.1 Le défi de la rareté numérique

Le défi de la rareté numérique réside dans la facilité avec laquelle l’information numérique peut être copiée et distribuée. L’information numérique est intrinsèquement plus difficile à sécuriser que l’information physique car, contrairement aux biens physiques - dont certains

possèdent naturellement une rareté en raison de contraintes matérielles - les éléments numériques tels que les fichiers musicaux, les documents ou les images peuvent être dupliqués à l’infini à un coût pratiquement nul.

Traditionnellement, la reproductibilité des données numériques signifiait que ces actifs ne pouvaient pas avoir une valeur économique similaire à celle des biens physiques, car ils manquaient de toute forme de rareté imposable. Pour la monnaie numérique, cela pose un problème particulièrement important, caractérisé comme le problème de la « double dépense », où une unité numérique unique (par exemple un jeton ou une devise) pourrait être copiée et dépensée plusieurs fois, la dévalorisant ainsi. Si la double dépense d’une monnaie est possible, cela la dévalue en la rendant indiscernable de fonds contrefaits ou frauduleux.

Traditionnellement, les institutions financières centralisées comme les banques atténuent ce risque en maintenant un registre qui vérifie chaque transaction et déduit les soldes en conséquence, garantissant qu’une fois l’argent dépensé, il ne peut pas être réutilisé par le même titulaire de compte. Cependant, cette approche nécessite une autorité centrale de confiance ou un « oracle » pour gérer et vérifier les transactions, ce qui impose une dépendance et un point de contrôle unique. Disposer d’un oracle centralisé d’information rend les actifs numériques vulnérables à la manipulation et à la censure.

Pour un système décentralisé et minimisant la confiance comme Bitcoin, où aucune autorité centrale n’existe pour superviser les transactions, empêcher la double dépense est un défi monumental. Sans mécanisme pour garantir l’unicité de chaque transaction, Bitcoin serait vulnérable à l’exploitation, le rendant impraticable comme réserve de valeur et moyen d’échange fiable. Bitcoin résout le problème de la double dépense grâce à un registre décentralisé, où les transactions sont confirmées simultanément par des milliers de participants au réseau. Ce mécanisme permet à Bitcoin de maintenir un enregistrement immuable de chaque transaction, garantissant que chaque pièce ne peut être dépensée qu’une seule fois.

Cette solution génère une rareté numérique sans dépendre d’un contrôle centralisé. Bitcoin introduit la première solution réussie à la rareté numérique, ouvrant la voie à un écosystème d’actifs numériques rares et minimisant la confiance, d’une manière auparavant jugée impossible.



#### 6.1.2 Imposer la rareté numérique avec Bitcoin

> Nous proposons une solution au problème de la double dépense en utilisant un serveur d’horodatage distribué de pair à pair pour générer une preuve computationnelle de l’ordre chronologique des transactions. Le système est sécurisé tant que les nœuds honnêtes contrôlent collectivement plus de puissance CPU que tout groupe coopérant de nœuds attaquants.  
_Satoshi Nakamoto_

Satoshi Nakamoto a créé Bitcoin comme une solution d’ingénierie aux problèmes associés à la monnaie fiduciaire. Cependant, cette solution nécessitait que Satoshi découvre un moyen d’imposer une rareté numérique absolue. Pour y parvenir, Satoshi a développé un protocole de communication open-source qui fonctionne sur un réseau décentralisé d’ordinateurs ou de nœuds. Chacun de ces nœuds détient une copie localement vérifiable d’un registre immuable, la soi-disant blockchain ou timechain. Le protocole Bitcoin définit les règles et le réseau décentralisé vérifie indépendamment les transactions, en respectant les mêmes règles sans nécessiter d’autorité centrale.

La rareté de Bitcoin contribue à son rôle de réserve de valeur. Tout comme l’or, Bitcoin est précieux non seulement en raison de son offre limitée mais aussi à cause de l’effort nécessaire pour « miner » ou produire de nouvelles pièces. Le minage de Bitcoin (le processus qui maintient le registre et émet de nouvelles pièces) est un processus coûteux et énergivore qui reflète l’acte physique d’extraire des minéraux de la terre. Cette « preuve de travail » numérique impose une contrainte de production qui rapproche Bitcoin des matières premières tangibles, lui conférant des propriétés de durabilité et de vérifiabilité que les biens numériques traditionnels n’ont pas. La difficulté intégrée et le taux décroissant d’émission de nouvelles pièces via des « halvings » périodiques créent une structure économique où l’offre de Bitcoin devient de plus en plus rare au fil du temps, augmentant son attrait comme réserve de valeur à long terme.

##### Comment la rareté numérique est-elle imposée ?

La solution de Bitcoin au problème de la double dépense réside dans son utilisation d’un registre décentralisé et publiquement consultable. Le registre Bitcoin peut être considéré comme une base de données immuable qui enregistre chaque transaction dans une chaîne séquentielle de lots horodatés, appelés blocs. Chaque bloc est strictement chronologique et contient des transactions qui ont été vérifiées et acceptées par les participants du réseau. Chaque bloc est relié au précédent, créant un enregistrement permanent distribué sur des milliers de nœuds à travers le monde. En stockant et partageant ce registre sur un réseau décentralisé, Bitcoin élimine le besoin d’une autorité centrale pour confirmer les transactions. Lorsqu’une transaction Bitcoin a lieu, les nœuds du réseau la valident indépendamment, garantissant que chaque pièce n’est dépensée qu’une seule fois. Ce registre partagé rend également extrêmement difficile pour des attaquants de pirater le réseau ou de modifier des transactions passées, car tout changement nécessiterait l’approbation de la majorité des participants au réseau.

Le mécanisme de Preuve de Travail (Proof-of-Work, PoW) de Bitcoin renforce encore la protection contre la double dépense en exigeant que les mineurs résolvent un problème cryptographique pour avoir la permission de valider de nouvelles transactions et de créer un nouveau bloc. Ce processus, appelé minage, demande de la puissance de calcul et ajoute un niveau de difficulté et de coût à la modification du registre. Chaque bloc ajouté au registre doit contenir un lien cryptographique avec le bloc précédent, ce qui solidifie l’intégrité de la chaîne et empêche toute falsification.

Le rôle d’un nœud est de stocker la copie la plus récente du registre, qui contient l’historique complet des transactions. Les nœuds maintiennent l’honnêteté des mineurs puisqu’ils vérifient qu’aucune double dépense n’a eu lieu et, surtout, que toutes les pièces ont été créées conformément au calendrier d’émission de Bitcoin. Tout utilisateur de Bitcoin peut exécuter un nœud et vérifier la propriété de ses pièces sans avoir à faire confiance à un tiers. Il n’est pas nécessaire d’avoir des autorités pour résoudre les litiges dans Bitcoin car toute transaction incluse dans un bloc est objectivement valide.

##### Comment un attaquant pourrait-il contrôler le réseau Bitcoin ?

Si un attaquant voulait modifier une transaction passée pour réussir une attaque de double dépense, il devrait refaire la Preuve de Travail pour ce bloc et tous les blocs suivants, en concurrence avec la puissance de calcul combinée de l’ensemble du réseau. Ce mécanisme de sécurité garantit que, si quelqu’un tente une double dépense, il doit contrôler plus de 50 % de la puissance de minage du réseau pour réussir. C’est ce qu’on appelle une attaque à 51 %.

Au début de Bitcoin, lorsqu’il était possible pour des participants individuels de créer ou miner de nouveaux blocs à l’aide de matériel informatique généralement disponible, il était au moins théoriquement possible de déployer suffisamment de puissance de calcul pour réussir une attaque à 51 %. Aujourd’hui, la puissance de calcul combinée du réseau Proof-of-Work dépasse 700 ExaHash/s. Cela signifie qu’au total, les ordinateurs de minage effectuent plus de 700 quintillions de hachages (calculs cryptographiques) chaque seconde. Nous avons atteint un point où le coût et la coordination immenses nécessaires pour réécrire le registre et réussir une attaque à 51 % rendent la double dépense irréalisable en pratique.

##### Confirmations et réorganisations

Une autre couche de protection (parfois négligée) provient du processus de confirmation des transactions de Bitcoin. Lorsqu’une transaction est d’abord diffusée, elle est considérée comme non confirmée et collectée dans le « mempool » en attendant son inclusion dans un bloc et sa validation par les mineurs. Une fois qu’une transaction est ajoutée à un bloc, elle est considérée comme « confirmée ». Chaque bloc ajouté par la suite compte comme une confirmation supplémentaire pour la transaction. Bien qu’une transaction soit considérée comme officielle après une seule confirmation, elle n’est pas considérée comme définitive tant que d’autres confirmations ne sont pas ajoutées.

Pour une sécurité totale, les utilisateurs de Bitcoin attendent souvent plusieurs confirmations (généralement six), car chaque bloc supplémentaire ajouté à la blockchain sécurise davantage la transaction, réduisant considérablement la probabilité d’une tentative de double dépense réussie. Ce processus de confirmation établit une fenêtre temporelle pendant laquelle les transactions sont finalisées.

##### Pourquoi attendre six confirmations ?

Les utilisateurs de Bitcoin attendent des confirmations supplémentaires car il est possible que le bloc de transactions le plus récent soit retiré de la chaîne de blocs, s’il ne fait plus partie de la chaîne la plus longue. Il est important de noter que le minage est une compétition entre de très grands pools de puissance de calcul. Il est donc possible que deux mineurs concurrents trouvent une solution cryptographique valide et que des blocs distincts soient ajoutés à la chaîne presque simultanément. Si cela se produit, la chaîne est essentiellement divisée. Les mineurs continueront à tenter d’ajouter des blocs à chaque branche de la chaîne. Cependant, une fois le bloc suivant miné, la chaîne la plus longue1 (définie comme la chaîne ayant le plus de preuve de travail investie) est celle qui prévaut et le bloc sur la chaîne la plus courte est « orphelin » et devient invalide. Toutes les transactions du bloc orphelin sont renvoyées dans le mempool pour être incluses dans un bloc valide ultérieur. Ce processus s’appelle une réorganisation ou, simplement, un « reorg ».

Un acteur malveillant, tentant une double dépense, doit prendre le contrôle du réseau suffisamment longtemps pour « réorganiser » la chaîne. Comme nous l’avons vu ci-dessus, obtenir le contrôle total nécessite une quantité énorme de puissance de calcul, mais que se passerait-il si une grande opération de minage - qui contrôlerait hypothétiquement un peu plus d’un tiers de toute la puissance de calcul du réseau - tentait une double dépense de pièces ?

Examinons un exemple :

Prenons, par exemple, que la puissance totale de minage du réseau Bitcoin soit de 550 ExaHash/s. Rogue Inc, qui contrôle 200 ExaHash/s, effectue un important achat immobilier et prévoit de payer en Bitcoin. Cependant, Rogue envisage également de tenter une double dépense des mêmes pièces. Le vendeur indique à Rogue qu'il attendra six confirmations avant de remettre les titres de propriété. Pour réussir une attaque de double dépense, Rogue doit construire en secret une branche alternative de la chaîne, en minant une chaîne plus longue contenant la transaction de double dépense. Une fois que le vendeur a vu six confirmations contenant sa transaction et a remis l'actif, Rogue doit alors publier tous les blocs qu'il a minés dans une nouvelle branche, faisant ainsi de celle-ci la chaîne la plus longue. Quelle est la probabilité que cela réussisse ?

À tout moment, la probabilité que Rogue mine le prochain bloc est de 200/550 = 0,36. Même si Rogue est le plus grand pool de minage, la probabilité que les mineurs honnêtes trouvent le prochain bloc est de 1 - 0,36 = 0,64. Les blocs devraient donc être minés beaucoup plus rapidement sur la chaîne honnête. Mais supposons que Rogue ait de la chance, mine un bloc et le garde secret. Il tente alors d’en miner un autre sur cette branche secrète. Cependant, la chaîne honnête mine ensuite un bloc et prend de l’avance en en minant un autre, avant que Rogue ne mine son deuxième bloc.

Rogue abandonne alors. Pourquoi ?


| Blocs à rattraper | 1 % | 10 % | 36 % (Rogue) | 51 % |
| --- | --- | --- | --- | --- |
| 1 | 0,010101 | 0,111111 | 0,562500 | 1,0 |
| 2 | 0,010102 | 0,012346 | 0,316406 | 1,0 |
| 3 | 1,0e-06 | 0,001372 | 0,177919 | 1,0 |
| 4 | 1,0e-08 | 0,000152 | 0,100113 | 1,0 |
| 5 | 1,0e-10 | 0,000017 | 0,056314 | 1,0 |
| 6 | 1,0e-12 | 1,9e-06 | 0,031676 | 1,0 |


**Source** : D'après un tableau de Grokking Bitcoin par Kalle Rosenbaum

Rogue se rend compte qu'il ne dispose pas d'assez de puissance de calcul pour réussir la double dépense, malgré le fait qu'il contrôle 36 % du taux de hachage du Bitcoin. Pour réussir, il doit miner quatre blocs supplémentaires pour dépasser la chaîne honnête. Malgré sa puissance de calcul considérable et le contrôle de 36 % du réseau, les chances de succès de Rogue ne sont que de 0,100113.


> **Info – La théorie des jeux entre en scène**
>
> Les chances de succès de Rogue sont très faibles, mais cela empire encore. Chaque minute où il continue d’essayer, Rogue consomme une quantité énorme d’électricité. Tout cela aura été vain. De plus, pour chaque bloc qu’il ne mine pas honnêtement, Rogue renonce à la récompense de bloc, actuellement de 3,125 pièces par bloc, d’une valeur supérieure à 300 000 $ actuellement.
>
> La raison principale de l’échec de Rogue est que le vendeur du bien immobilier a exigé six confirmations. Plus le nombre de confirmations requises est élevé, plus il est difficile pour les mineurs malhonnêtes de construire des chaînes alternatives de blocs. En effet, pour une transaction très importante, un vendeur peut exiger davantage de confirmations. Par exemple, dix confirmations (ce qui devrait prendre environ 100 minutes) réduiraient les chances de succès de Rogue à seulement 0,003.
>
> De cette manière, la théorie des jeux autour du minage garantit que tous sont incités à agir honnêtement et à ne pas gaspiller de ressources informatiques ou à renoncer aux récompenses de bloc. De plus, il est dans l’intérêt de tous les mineurs que le réseau Bitcoin soit sécurisé et fiable. Cela garantit que leur énorme investissement en puissance de calcul est protégé. Si le réseau est attaqué avec succès, la valeur de marché des pièces chutera considérablement car la confiance dans le réseau sera diminuée.




#### 6.1.3 La centralisation du minage est-elle une menace ?

Comme on le voit dans le tableau ci-dessus, la centralisation du minage peut constituer une menace potentielle pour la protection contre la double dépense de Bitcoin, car elle augmente la probabilité d'une attaque à 51 % – un scénario dans lequel un seul mineur ou un groupe de mineurs contrôle plus de la moitié de la puissance de calcul du réseau. Si cela devait se produire, l'entité contrôlante pourrait théoriquement modifier les transactions récentes ou tenter une double dépense en réécrivant le registre, lui permettant ainsi de dépenser les mêmes pièces plusieurs fois.

Une telle situation sape l'intégrité du réseau Bitcoin en accordant une influence disproportionnée sur la validation des transactions à quelques acteurs. Cependant, bien que théoriquement possible, mener une attaque à 51 % resterait extrêmement complexe et coûteux, nécessitant d'immenses ressources informatiques, de l'électricité et de la coordination, ce qui dépasserait probablement les avantages potentiels d'une tentative de double dépense.

Il existe des garde-fous qui aident à limiter les risques de centralisation du minage. Les pools de minage, par exemple, permettent aux petits mineurs de combiner leurs ressources et de partager les récompenses de bloc, réduisant ainsi la domination d'une seule entité. Bien que ce soit un moyen utile pour les petits mineurs de participer au réseau, il existe un risque que l'entité contrôlant le pool se comporte mal et tente d'attaquer le réseau. Cependant, la transparence du registre Bitcoin signifie également que toute concentration de puissance de minage est visible, alertant la communauté sur les risques potentiels et permettant la mise en place de contre-mesures. Les mineurs sont très conscients que toute attaque contre le réseau Bitcoin risque de nuire gravement à sa proposition de valeur, il est donc très simple pour les petits mineurs de changer de pool afin d'éviter que leur puissance de minage ne soit utilisée à des fins malveillantes. Bien que le risque ne soit pas nul, la nature ouverte et distribuée de l'écosystème Bitcoin, combinée au coût élevé d'une attaque, fait de la centralisation du minage une menace plus théorique qu'imminente, car maintenir un tel contrôle sur de longues périodes serait financièrement non viable pour tout attaquant.



#### 6.1.4 L'impact plus large de la rareté numérique

Le Bitcoin a transformé notre façon de concevoir la rareté dans le domaine numérique. En effet, les biens numériques – tels que les logiciels, les fichiers musicaux, les livres électroniques et les contenus en ligne – possèdent des caractéristiques qui les distinguent des biens physiques : ils peuvent être reproduits à un coût négligeable et partagés instantanément. Contrairement aux objets physiques, qui sont soumis à des contraintes matérielles comme les coûts de production et les limites de stockage, les biens numériques existent sous forme de données pouvant être dupliquées à l’infini sans aucune dégradation de qualité. Cela signifie que, tandis que les biens physiques sont intrinsèquement rares en raison de ces contraintes matérielles, les biens numériques ont traditionnellement été abondants, dépourvus de tout mécanisme intégré pour limiter leur offre.

Il est important de noter que les biens numériques sont non rivaux. Cela signifie que la consommation d’un bien numérique par une personne ne diminue pas la disponibilité de ce bien pour les autres. Par exemple, lorsqu’une chanson est téléchargée, elle peut être copiée et distribuée un nombre illimité de fois sans perdre de son utilité. Historiquement, cette abondance pose un défi pour la création de valeur, car le modèle économique traditionnel de l’offre et de la demande est bouleversé lorsque l’offre est, du moins en théorie, illimitée. Pour y répondre, la gestion des droits numériques (DRM) et d’autres mesures de rareté artificielle ont tenté de restreindre l’accès. Cependant, ces mécanismes peuvent être contournés et délèguent la confiance à des autorités centralisées. L’innovation du Bitcoin réside dans la manière dont il aborde ce problème de façon native, en devenant le premier actif numérique à intégrer la rareté grâce à une technologie décentralisée, sans dépendre de ces limitations traditionnelles.

Le Bitcoin joue un rôle transformateur dans l’établissement de la rareté numérique en introduisant un protocole qui impose une offre finie. Une limite de 21 millions de pièces est inscrite dans le protocole et cette limite ne peut être modifiée sans le consensus du réseau, c’est-à-dire l’ensemble des milliers de participants répartis dans le monde entier qui font fonctionner des nœuds Bitcoin. De cette manière, le Bitcoin a créé un actif qui imite la nature finie des matières premières physiques, comme l’or, tout en existant entièrement dans le domaine numérique. Le plafond d’émission est fondamental pour la proposition de valeur du Bitcoin et est maintenu par une combinaison de cryptographie, de mécanismes de consensus et de code source ouvert et transparent. Cela garantit que tous les participants du réseau respectent les mêmes règles, tout en étant motivés par l’incitation économique clé d’assurer que l’offre de pièces soit absolument et de manière vérifiable finie.

En résolvant le problème de la double dépense, le Bitcoin empêche l’inflation ou la duplication de l’actif, un défi qui a longtemps entravé les précédentes tentatives de monnaie numérique. Au sein du Bitcoin, aucune autorité unique ne contrôle l’offre, ce qui le rend immunisé contre la manipulation centrale telle qu’on la voit dans le système monétaire fiduciaire, comme l’impression arbitraire de monnaie ou la dévaluation. Cette innovation permet au Bitcoin de servir de réserve de valeur et de protection contre l’inflation, lui permettant d’occuper une position unique semblable à celle de « l’or numérique » – une ressource numérique rare à la valeur vérifiable.



#### 6.1.5 Conclusion

En conclusion, il est de plus en plus reconnu que l’innovation du Bitcoin en matière de rareté numérique a redéfini le concept de monnaie. Cependant, il est parfois négligé que le Bitcoin a également transformé le paysage numérique en résolvant le problème de longue date de la création de rareté dans un monde numérique intrinsèquement abondant. Le Bitcoin a effectivement introduit une nouvelle catégorie d’actif numérique qui reflète les qualités des matières premières physiques.

Cette avancée démontre qu’un système décentralisé peut établir la rareté, l’immutabilité et la valeur indépendamment de toute autorité centrale. De plus, cela pourrait avoir des usages au-delà de la monnaie, puisqu’il a inspiré tout un domaine de recherche et de développement autour de cette technologie.

En regardant vers l’avenir, le modèle de rareté numérique du Bitcoin façonne le futur de la monnaie et du stockage de valeur. À mesure que les préoccupations liées à l’inflation et les questions sur la gestion de la monnaie fiduciaire deviennent plus largement reconnues, l’offre fixe du Bitcoin le rend de plus en plus attractif comme protection contre l’instabilité financière traditionnelle.

En fin de compte, la découverte par le Bitcoin de la rareté numérique pourrait marquer le début d’un changement de paradigme, où les actifs numériques dotés d’une rareté reconnue et d’une confiance vérifiable sont reconnus comme des composantes précieuses de l’économie moderne, établissant ainsi une base pour l’avenir de la finance décentralisée et de la propriété numérique. Cela a des implications majeures pour le domaine de l’économie – le Bitcoin a fourni le modèle de la façon dont la rareté et la valeur peuvent exister sous forme numérique.

> Au-delà de la rareté numérique, le Bitcoin est également le premier exemple de rareté absolue, la seule marchandise liquide (numérique ou physique) avec une quantité fixe qui ne peut pas être augmentée de façon concevable. Jusqu’à l’invention du Bitcoin, la rareté était toujours relative, jamais absolue.  
_Saifedean Ammous_



###### Notes

1. La chaîne la plus longue est acceptée par les nœuds Bitcoin comme la version la plus valide du registre, car elle est définie comme la chaîne ayant nécessité le plus d’effort (ou la plus grande preuve de travail) pour être construite. Plus d’informations ici : [https://learnmeabitcoin.com/technical/blockchain/longest-chain/](https://learnmeabitcoin.com/technical/blockchain/longest-chain/)
