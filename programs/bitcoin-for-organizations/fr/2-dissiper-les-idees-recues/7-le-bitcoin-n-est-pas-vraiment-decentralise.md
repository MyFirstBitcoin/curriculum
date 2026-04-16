# 2.7 Le Bitcoin n'est pas vraiment décentralisé.

> La complexité des cryptomonnaies découle des tentatives de décentralisation—en répartissant le pouvoir et la gouvernance dans le système, il n’y a théoriquement plus besoin d’intermédiaires de confiance comme les institutions financières. Tel était le principe du livre blanc initial du Bitcoin, qui proposait une solution cryptographique permettant d’effectuer des paiements sans impliquer d’institution financière ou autre intermédiaire de confiance. Cependant, le Bitcoin est devenu centralisé très rapidement et dépend aujourd’hui d’un petit groupe de développeurs de logiciels et de pools de minage pour fonctionner  
_Fonds monétaire international_

Comme le montre la citation ci-dessus, tirée d’un article assez récent du Fonds monétaire international, l’industrie financière traditionnelle continue d’affirmer que le Bitcoin n’est pas décentralisé, tout en confondant le Bitcoin avec d’autres crypto-actifs.

##### Introduction

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/3333a336188df0e3d1412285a0a963cc3302e308-161x167.svg)

La décentralisation est un aspect essentiel du Bitcoin. La capacité à maintenir les règles du protocole telles que la rareté et la distribution sans autorité centrale garantit qu’il peut servir de monnaie sans permission pour une société mondiale.

Comme Satoshi l’a noté dans sa correspondance en ligne, des services décentralisés comme BitTorrent « tenaient bon » face aux répressions gouvernementales, contrairement aux services avec propriétaire(s) identifié(s) et serveurs centralisés. Il était manifestement préoccupé par le risque potentiel que des gouvernements ou d’autres intérêts ferment ou affectent négativement le Bitcoin.

Dans ce contexte, nous nous intéressons à la décentralisation de :

* Le développement et la gestion du code exécutant le protocole ; qui est autorisé à changer les règles ?
* La fonction de minage qui crée de nouveaux blocs conformément aux règles et valide contre la double dépense
* Les nœuds qui valident la validité des transactions et conservent une copie de la blockchain

##### Développeurs

Bitcoin est un protocole open source que tout le monde est libre de consulter, télécharger, copier ou proposer des modifications. Il est disponible dans une bibliothèque GitHub, le code source ayant été lancé à l’origine en 2009 par Satoshi Nakamoto. Chacun est libre de télécharger le code et d’exécuter un nœud, dont la majorité utilise le logiciel original Bitcoin Core, qui a été mis à jour au fil du temps.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Source : https://river.com/learn/what-is-bitcoin-core/_

Le développement de Bitcoin Core suit les meilleures pratiques du développement open source. À tout moment, il peut y avoir un nombre quelconque de développeurs écrivant ou révisant des modifications du code. Ils doivent écouter les préoccupations des opérateurs de nœuds et des mineurs, ainsi que de la base d’utilisateurs, avant d’apporter tout changement critique au code, qui sera examiné et approuvé comme indiqué dans le schéma ci-dessus avant d’être intégré au code.

Les règles du Bitcoin sont ensuite codées dans ce logiciel Bitcoin Core, qui s’exécute sur chaque nœud. N’importe qui peut proposer une modification des règles – les règles sont du code, mais elles ne sont pas_juste_ du code, elles sont_du code approuvé_ . Si elles sont modifiées unilatéralement, le nouveau code ne fait plus partie du consensus et ne fait plus partie du Bitcoin. Modifier quelque chose dans Bitcoin tout en restant dans le consensus est délicat. Les modifications proposées au code entrent dans l’une des trois catégories suivantes :

* Dans le cadre des règles existantes : Des mises à jour mineures telles que des corrections orthographiques, une interface utilisateur améliorée ou une meilleure gestion des données peuvent entrer dans cette catégorie et sont relativement faciles à faire approuver.
* Ajout d’une nouvelle règle qui ajoute des restrictions aux règles – comme la réduction de la taille des blocs. Cela s’appelle un « soft fork ». Les nœuds qui choisissent de ne pas appliquer la modification du code et de rester sur l’ancienne version pourront toujours participer au réseau.
* Ajout d’une nouvelle règle qui enfreint les règles actuelles, par exemple une augmentation de la taille des blocs. Les nœuds qui ne mettent pas à jour leur code rejetteront un bloc créé dans la taille supérieure comme invalide. Cela s’appelle un « hard fork » et créera une scission de la chaîne entre les nœuds exécutant l’ancien et le nouveau code, créant ainsi une nouvelle monnaie. Cela s’est déjà produit, mais n’a jamais conduit à un succès durable pour la nouvelle monnaie, car la majorité des nœuds ont choisi de conserver le code original.

Ainsi, une seule partie ou un groupe de personnes ne peut pas modifier unilatéralement le code du Bitcoin sans obtenir un accord de consensus, sous peine de provoquer une scission de la chaîne et la création d’une nouvelle monnaie suivant un ensemble de règles différent.

##### Minage

La fonction de minage valide les transactions comme tout autre nœud du réseau, mais elle dépense ensuite l’énergie nécessaire pour créer un nouveau bloc conforme aux règles de consensus du code. En cas de succès, le mineur obtient des récompenses sous forme de frais de transaction et de récompenses en Bitcoin (au moment de la rédaction, 3,125 pièces par bloc).

Le minage est généralement effectué par des « pools » de minage où les personnes regroupent leur puissance de calcul ou taux de hachage pour augmenter leurs chances de miner un bloc et de partager les récompenses. Il existe un risque qu’un ou plusieurs de ces pools de minage s’associent pour atteindre une domination de 51 % du minage et, en substance, passer outre le protocole de validation du réseau en leur faveur pour effectuer une double dépense. Cela nécessiterait d’énormes ressources à un coût très élevé, et les mineurs individuels peuvent très facilement changer de pool de minage à tout moment. Une telle attaque ferait probablement aussi s’effondrer la valeur du bitcoin, puisqu’il serait évident que l’intégrité du réseau a été compromise. Un attaquant devrait donc convertir rapidement tout bitcoin obtenu en monnaie fiduciaire avant que la valeur ne s’érode. Cela rendrait encore plus difficile de maintenir une attaque sur une longue période, et il est donc plus rentable pour un mineur ou un opérateur de pool de respecter les règles et de tenter de miner des blocs valides.

La répartition géographique de la fonction de minage est également importante pour éviter, par exemple, que des gouvernements prennent le contrôle de la capacité de minage ou la ferment. Par exemple, une récente interdiction du minage par la Chine a démontré la capacité du Bitcoin à s’adapter et à survivre à une telle intervention gouvernementale, en s’adaptant et en se remettant rapidement de la perte de puissance de hachage qui en a résulté.

##### Nœuds

Contrairement au minage, qui nécessite un investissement financier important pour être compétitif dans la course au minage de nouveaux blocs, ou au développement du code qui demande une expertise en programmation, faire tourner un nœud est quelque chose que toute personne intéressée à contribuer à la décentralisation du Bitcoin peut faire.

Les nœuds exécutent le logiciel Bitcoin Core et appliquent les règles incluses dans le code pour s’assurer que les mineurs ne trichent pas, par exemple en s’attribuant une récompense de bloc supérieure à ce qui est autorisé. Ils appliquent également le plafond d’approvisionnement de 21 millions, ce qui est essentiel pour maintenir la rareté du Bitcoin. Pour qu’un gouvernement ou un acteur malveillant arrête le Bitcoin, il faudrait détruire chaque copie de la blockchain, actuellement exécutée sur des milliers de nœuds répartis dans le monde entier, une tâche quasiment impossible.

##### Personnes

Un autre aspect de la centralisation potentielle concerne les personnes. Toutes les autres « alt-coins » ont un leader – quelqu’un qui pourrait potentiellement être contraint de défendre des changements qui ne sont pas dans l’intérêt du Bitcoin. Satoshi Nakamoto est resté assez longtemps pour s’assurer que le Bitcoin était sur la voie du succès avant de disparaître définitivement, laissant à d’autres le soin d’améliorer et d’adapter le logiciel.

Qu’en est-il des détenteurs de grandes quantités de Bitcoin ? Les premiers investisseurs, qui ont conservé leurs pièces et ne les ont pas perdues, sont aujourd’hui extrêmement riches. Il est important de noter que cela peut effectivement être le cas, mais cela ne leur donne pas plus d’influence sur le système que n’importe qui d’autre, contrairement aux monnaies « proof of stake » où les premiers adoptants, déjà riches dans cette monnaie, bénéficient d’avantages dans la prise de décision et la distribution des futures pièces. Cela a ou aura inévitablement pour conséquence une centralisation au fil du temps.

##### Conclusion

Quelles sont les menaces potentielles que la décentralisation peut tenter de limiter ?

* Un gouvernement qui ferme ou interdit le Bitcoin
* Des modifications indésirables du code qui favorisent un ensemble d’intérêts dans le Bitcoin, par exemple l’augmentation de la récompense de bloc
* La coercition du protocole par un gouvernement ou des acteurs malveillants pour influencer la direction du protocole
* La possibilité pour un pool de mineurs de prendre le contrôle du réseau et de « double-dépenser » du Bitcoin – une attaque à 51 %

Comme nous pouvons le voir, la combinaison des nœuds, des développeurs de code et des mineurs, ainsi que l’utilisation du mécanisme de « preuve de travail », décentralise le Bitcoin à un niveau suffisant pour que ces menaces potentielles ne soient pas considérées comme très préoccupantes. La communauté devra continuer à surveiller la situation pour s’assurer que cela reste le cas.
