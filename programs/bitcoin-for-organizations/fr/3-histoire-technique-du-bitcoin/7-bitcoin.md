# 3.7 Bitcoin

Après de nombreuses années et tentatives infructueuses, les Cypherpunks avaient pour la plupart commencé à perdre de l'intérêt pour l'idée d'une monnaie numérique sans autorisation, lorsque Adam Back a reçu un e-mail contenant un lien vers un brouillon de livre blanc intitulé « monnaie électronique sans tiers de confiance » provenant d'une personne anonyme se faisant appeler Satoshi Nakamoto.

Pour récapituler à ce stade, nous avons au moins les idées suivantes :

* Signatures cryptographiques pouvant offrir un certain niveau de confidentialité et d'anonymat
* Concept d'une monnaie non adossée (B-Money)
* Propositions (mais sans moyen) pour limiter l'émission de nouvelle monnaie
* Pièces numériques dont la propriété était attribuée par des clés publiques (B-Money) et pouvant être transférées par signature et réattribuées en fonction de l'adresse du destinataire (RPOW et Hashcash)
* Tous les nœuds maintiennent une copie d'un registre totalement distribué (B-Money) (rejeté à l'époque comme impraticable)
* Protocole d'horodatage – utilisant le hachage d'arbre de Merkle pour fournir une chronologie mathématiquement prouvable des événements, difficile à falsifier si tous les utilisateurs conservent les mêmes enregistrements
* Preuve de travail pour lier un effort réel au système (mais en utilisant le hachage lui-même comme monnaie)
* Réseaux totalement décentralisés où tous les pairs sont égaux et peuvent rejoindre ou quitter le réseau à tout moment (BitTorrent)
* Concept de lier de nouveaux hachages aux hachages précédents (Bit Gold et horodatage)

Ce qui manquait à cette époque comprenait :

* Une solution viable au problème des « généraux byzantins »
* Une méthode pour limiter la quantité de monnaie en circulation malgré l'amélioration continue du matériel
* Un système d'incitations pour encourager la participation (problème de la poule et de l'œuf)

L'autre grande différence entre les tentatives récentes et Bitcoin était que Satoshi travaillait sur le code depuis un certain temps dans le véritable esprit originel des « Cypherpunks écrivent du code » avant de l'annoncer sur les listes de diffusion, contrairement à Bit Gold et B-Money qui étaient davantage conceptuels.

Quelle a été l'innovation qui a distingué Bitcoin des tentatives précédentes de monnaie électronique ?

La preuve de travail serait utilisée comme mécanisme de consensus et comme moyen d'assurer la sécurité et l'immutabilité : au lieu d'utiliser le hachage comme forme de monnaie, il serait utilisé par un nouveau processus conceptuel appelé minage, où un nœud regrouperait un ensemble de transactions, ajouterait un nombre aléatoire puis appliquerait le hachage au « bloc » de données. Un bloc valide répondant à l'exigence de hachage serait alors annoncé au réseau. Ces blocs seraient liés entre eux en utilisant le hachage du bloc précédent dans chacun, et la plus longue chaîne de blocs serait utilisée en cas d'égalité où différents nœuds valideraient et annonceraient différents blocs en même temps, créant ainsi des divisions de chaîne. La preuve de travail est devenue le mécanisme distribué de départage pour résoudre le problème des généraux byzantins.

Ces mineurs recevaient également une incitation à fournir la puissance de calcul nécessaire pour effectuer la preuve de travail en se voyant attribuer de nouveaux bitcoins pour chaque bloc. Le montant de Bitcoin attribué est également programmé pour diminuer environ tous les 4 ans jusqu'à ce que tous les bitcoins aient été créés, établissant ainsi une limite stricte au nombre total de bitcoins qui seront jamais en circulation à 21 millions.

L'idée la plus originale était la manière dont il a résolu la question de la création monétaire à mesure que le matériel s'améliore et que plus de puissance peut être appliquée au réseau. Les horodatages d'un nombre défini de blocs (2016) seraient moyennés, et s'ils étaient créés trop rapidement, le hachage nécessaire pour créer un nouveau bloc serait rendu plus difficile, et s'ils étaient créés trop lentement, il serait rendu plus facile. Cela a été intégré dans le protocole décentralisé exécuté par tous les nœuds, de sorte que tout mineur l'ignorant dépenserait de l'énergie pour miner un bloc sans aucun bénéfice, car il serait rejeté par le reste du réseau. Cet ajustement garantit que la création de nouveaux blocs reste conforme au calendrier prévu d'émission, et incite les mineurs à « respecter les règles ».

####   
Résumé

De nombreux éléments du puzzle nécessaires à la construction d'un système de monnaie électronique pair à pair décentralisé basé sur des principes monétaires sains étaient en place avant que Satoshi ne publie son livre blanc et peu après la sortie initiale du code.

> La nature de Bitcoin est telle qu'une fois la version 0.1 publiée, la conception de base était gravée dans le marbre pour le reste de sa durée de vie  
_Satoshi Nakamoto_

Bien que de nombreuses idées d'amélioration (BIP) aient été proposées et adoptées, Bitcoin fonctionne en arrière-plan depuis 2009 en suivant le protocole conçu dans la version initiale et avec à peine la moindre perturbation. Toutes les améliorations ont été réalisées tout en permettant la rétrocompatibilité avec toutes les versions précédentes.



##### Notes

1. Pour une explication du problème des généraux byzantins - voir [https://fr.wikipedia.org/wiki/Probl%C3%A8me_des_g%C3%A9n%C3%A9raux_byzantins](https://en.wikipedia.org/wiki/Byzantine_fault)
