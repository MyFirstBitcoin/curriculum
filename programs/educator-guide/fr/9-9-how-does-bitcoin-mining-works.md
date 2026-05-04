# 9 - How Does Bitcoin Mining Works

Durée : 90 minutes

Idée principale : Le minage de Bitcoin et la validation par les nœuds travaillent ensemble pour sécuriser le réseau, confirmer les transactions et faire respecter les règles du système grâce à la Preuve de Travail.

#### Objectifs d'apprentissage

À la fin de cette leçon, les élèves devraient être capables de :

* Expliquer la différence entre le rôle des nœuds Bitcoin et celui des mineurs Bitcoin.
* Décrire comment les nœuds valident les transactions, partagent l'information et contribuent à faire respecter les règles de Bitcoin.
* Expliquer ce que font les mineurs, y compris la sélection des transactions, la construction de blocs candidats et la compétition pour trouver un hachage de bloc valide.
* Définir le mempool et expliquer pourquoi il fonctionne comme une salle d'attente pour les transactions non confirmées.
* Décrire comment les frais de transaction influencent la sélection par les mineurs et la rapidité de confirmation.
* Expliquer la Preuve de Travail comme le mécanisme qui sécurise Bitcoin en rendant les attaques coûteuses.
* Décrire comment l'ajustement de la difficulté aide à maintenir un temps moyen de bloc d'environ 10 minutes.
* Parcourir le cycle de vie complet d'une transaction Bitcoin, de sa création et signature à sa confirmation dans un bloc.

#### Outils et ressources

##### Aides visuelles

* Chapitre 9 - Comment fonctionne le minage de Bitcoin ?

##### Bibliothèque de soutien

* Carte de référence du vocabulaire — Chapitre 9 — Termes : minage, Preuve de Travail, énigme de hachage, ajustement de la difficulté, récompense de bloc, mempool, attaque à 51 %
* Bibliothèques de malentendus — Chapitre 9 — À traiter : « les mineurs créent du Bitcoin à partir de rien », « les mineurs contrôlent Bitcoin », « plus de minage = moins de sécurité »
* Tableaux comparatifs et fiches de référence — Économie du minage : revenus, coûts, alignement des incitations ; ajustement de la difficulté
* Explications techniques et analyses approfondies — Sécurité de la Preuve de Travail ; pourquoi attaquer est coûteux ; seuil de 51 %

#### Activités

* Explorer le mempool
* Transactions en action

#### Enseignement en ligne

* Utiliser un schéma clair du flux de transaction, de la signature par le portefeuille à la confirmation.
* Garder les nœuds et les mineurs visuellement séparés à l'écran tout au long de la leçon.
* Utiliser mempool.space ou une capture d'écran de celui-ci pour montrer les transactions non confirmées et la pression sur les frais.
* Faire une pause après chaque étape du processus de minage et poser une courte question de compréhension.

#### Préparation

* Préparer un schéma du processus de minage (mempool → sélection des transactions → création de bloc → ajustement de la difficulté) à afficher.
* Mettre en favori mempool.space ou la page de minage de blockchain.com ; préparer des captures d'écran des statistiques de minage actuelles et des ajustements de difficulté.
* Créer une explication visuelle de la Preuve de Travail comme mécanisme de sécurité ; montrer l'ajustement de la difficulté sur les 3 à 6 derniers mois.

#### Procédure

Cette leçon examine de plus près comment les transactions Bitcoin circulent dans le réseau et deviennent partie intégrante de la blockchain. Elle suit désormais directement la structure du Diplôme afin que les principales sections s'alignent avec le guide de l'étudiant tout en préservant l'explication complète pour l'enseignant dans chaque section.

##### 9.0 Introduction, 8 minutes

Commencez par relier ce chapitre au précédent :

* Si un utilisateur signe une transaction avec une clé privée, que se passe-t-il ensuite ?
* Qui vérifie si cette transaction est valide ?
* Comment est-elle ajoutée à la blockchain ?
* Pourquoi Bitcoin a-t-il besoin à la fois de nœuds et de mineurs ?

Précisez que ce chapitre explique comment le réseau traite les transactions en pratique et comment le minage sécurise le système sans autorité centrale.

##### 9.1 Nœuds et mineurs Bitcoin, 47 minutes

**Nœuds et mineurs, rôles différents**

Commencez par bien distinguer les deux rôles.

Nœuds Bitcoin :

* conservent une copie de la blockchain
* vérifient si les transactions respectent les règles
* partagent l'information avec d'autres nœuds
* aident les portefeuilles et autres logiciels à accéder aux données de la blockchain
* peuvent rejeter les transactions ou blocs invalides

Le chapitre décrit les nœuds comme des gardiens de la validation, et développe cette idée avec l’analogie de « l’agent de circulation numérique ». Cela est utile car cela montre les nœuds comme des vérificateurs et des coordinateurs, et non comme des dirigeants. Le schéma renforce également le fait que de nombreux nœuds conservent des copies du registre à travers le monde.

Mineurs de Bitcoin :

* rassemblent les transactions valides
* assemblent des blocs candidats
* sont en compétition pour trouver un hachage de bloc valide
* diffusent les blocs valides lorsqu’ils gagnent
* reçoivent la récompense de bloc et les frais de transaction

Un point clé d’enseignement du chapitre est que le but du minage n’est pas simplement de créer de nouveaux bitcoins, mais de décentraliser la sécurité de Bitcoin. Les nouveaux bitcoins sont l’incitation, tandis que le processus de minage lui-même est le mécanisme de sécurité.

**Ce que font réellement les nœuds**

Développez la section sur les nœuds avec la liste des fonctions des nœuds du chapitre :

* Gardiens de la validation : ils vérifient que les transactions et les blocs respectent les règles
* Centre de communication : ils se connectent entre eux et partagent les données de transaction
* Contrôleur de qualité : ils rejettent les informations invalides
* Informateur de la blockchain : ils fournissent des données à d’autres logiciels comme les portefeuilles
* Accueillant des nouveaux nœuds : ils aident les nouveaux nœuds à obtenir la blockchain, tandis que chaque nouveau nœud vérifie toujours les données de manière indépendante

C’est un bon moment pour souligner que faire tourner un nœud donne à l’utilisateur plus d’indépendance. Au lieu de dépendre entièrement de services extérieurs pour connaître l’état du réseau, il peut le vérifier lui-même. le souligne clairement, y compris la mention de Bitcoin Core comme une des implémentations que les utilisateurs peuvent faire tourner.

**Ce que font réellement les mineurs**

Expliquez maintenant le minage plus en détail.

Les mineurs :

* collectent les transactions vérifiées mais non confirmées
* les regroupent dans un bloc candidat
* hachent à répétition les données du bloc en cherchant un hachage de bloc valide
* diffusent le bloc gagnant au réseau
* gagnent des récompenses si le bloc est accepté

Utilisez l’analogie du chapitre sur « l’immense botte de clés » si cela aide. Cela donne aux étudiants une image concrète de la course au minage. L’idée principale n’est pas que les mineurs résolvent un problème mathématique utile au sens ordinaire, mais qu’ils prouvent qu’ils ont dépensé de l’énergie et de la puissance de calcul réelles pour sécuriser le système.

C’est aussi le bon moment pour expliquer les récompenses des mineurs :

* récompense de bloc : nouveaux bitcoins émis
* frais de transaction : frais attachés aux transactions que les utilisateurs veulent faire confirmer

Précisez que les mineurs privilégient généralement les transactions avec des frais plus élevés, car cela augmente leur récompense. Le chapitre explique aussi les halvings ici, donc vous pouvez noter brièvement que la récompense de bloc diminue tous les 210 000 blocs, soit environ tous les quatre ans, selon le calendrier public d’émission de Bitcoin. Les pages 5 et 6 incluent le calendrier d’émission et le tableau des prochains halvings, ce qui peut aider à renforcer la prévisibilité de l’émission de Bitcoin.

**Hachage de bloc valide, Preuve de travail et Ajustement de la difficulté**

Cette section est le cœur du chapitre.

Expliquez que les mineurs cherchent un hachage de bloc valide, c’est-à-dire un hachage de bloc qui respecte la cible du réseau. Le chapitre explique cela comme le fait de trouver un nombre inférieur à la cible fixée par le réseau.

Expliquez ensuite clairement la Preuve de travail :

* les mineurs doivent effectuer des calculs répétés
* le premier à trouver un hachage valide prouve qu’il a fait ce travail
* cela rend coûteux de réécrire ou d’attaquer le registre
* les nœuds vérifient ensuite le bloc avant de l’accepter

Une phrase forte pour l’enseignement est :

La Preuve de travail sécurise Bitcoin en rendant la malhonnêteté coûteuse et la vérification facile.

Expliquez aussi l’ajustement de la difficulté :

* le réseau ajuste la difficulté du minage tous les 2 016 blocs
* cela se produit environ toutes les deux semaines
* l’objectif est de maintenir le temps moyen entre les blocs proche de 10 minutes
* si plus de puissance de calcul rejoint le réseau, la difficulté augmente
* si moins de puissance de calcul est présente, la difficulté diminue

Les pages 7 et 8 expliquent ce processus et montrent comment des cibles plus difficiles exigent plus de travail. Cela aide les étudiants à comprendre que le rythme de Bitcoin n’est pas contrôlé par une autorité centrale mais par des règles du protocole qui réagissent automatiquement aux conditions du réseau.

##### 9.2 Qu’est-ce que le mempool ?, 15 minutes

Passez maintenant au mempool.

Expliquez que le mempool est la salle d’attente pour les transactions valides mais non confirmées. Lorsqu’un utilisateur diffuse une transaction, les nœuds la vérifient d’abord. Si elle est valide, ils l’ajoutent à leur mempool et la partagent avec d’autres nœuds. Ensuite, les mineurs peuvent sélectionner parmi ces transactions en attente lors de la construction d’un bloc. Les pages 10 et 11 expliquent ce processus directement.

Points importants à souligner :

* le mempool n'est pas la blockchain
* les transactions qui s'y trouvent ne sont pas encore confirmées
* chaque nœud maintient son propre mempool
* il n'existe pas un mempool universel unique
* les transactions avec des frais plus élevés ont plus de chances d'être sélectionnées rapidement

Le chapitre explique également les raisons courantes pour lesquelles une transaction peut rester non confirmée pendant longtemps :

* frais faibles
* congestion du réseau
* tentative de double dépense
* données incorrectes ou incomplètes
* transaction mal formée

Si cela est utile, mentionnez l'activité avec mempool.space comme moyen pratique de visualiser les transactions non confirmées et les taux de frais. Précisez également que mempool.space n'est qu'un explorateur parmi d'autres, et non le mempool lui-même.

##### 9.3 Comment fonctionnent les transactions Bitcoin, 20 minutes

Rassemblez maintenant tous les éléments en utilisant la séquence étape par étape du chapitre.

Une version claire pour la classe est :



1. L'expéditeur sélectionne un UTXO et crée une transaction
1. L'expéditeur ajoute l'adresse du destinataire et les frais
1. L'expéditeur signe la transaction avec sa clé privée
1. La transaction est diffusée sur le réseau
1. Les nœuds la vérifient et l'ajoutent à leur mempool
1. Les mineurs la sélectionnent pour un bloc candidat
1. Les mineurs se concurrencent via la Preuve de Travail
1. Un mineur trouve un hash de bloc valide et diffuse le bloc
1. Les nœuds vérifient le bloc et l'ajoutent à la blockchain
1. La transaction reçoit des confirmations à mesure que de nouveaux blocs sont ajoutés
1. Rendez le point final explicite :
1. une fois que la transaction est incluse dans un bloc valide, elle est confirmée
1. les entrées dépensées ne sont plus utilisables
1. le destinataire contrôle désormais les nouveaux UTXO créés par cette transaction

Le schéma récapitulatif est particulièrement utile ici car il relie visuellement l'ensemble du processus, de la signature du portefeuille à l'inclusion par le mineur, à la validation par les nœuds et à la distribution du bloc.

###### Conclusion et vérification de la compréhension

Terminez par quelques questions rapides :

* Quelle est la différence entre un nœud et un mineur ?
* Qu'est-ce que le mempool ?
* Pourquoi certaines transactions sont-elles confirmées plus rapidement que d'autres ?
* Que prouve la Preuve de Travail ?
* Pourquoi Bitcoin ajuste-t-il la difficulté du minage ?
* Quelles sont les principales étapes entre l'envoi d'une transaction et la réception de la confirmation ?

#### Notes pour l'enseignant

Gardez le fil conducteur principal clair : les nœuds vérifient, les mineurs se concurrencent, la Preuve de Travail sécurise, et le mempool conserve les transactions valides jusqu'à leur confirmation.

Ce chapitre peut sembler technique, alors utilisez souvent des analogies et des schémas.

Évitez de présenter le minage comme la « création de bitcoin à partir de rien ». Soyez précis : la récompense est l'incitation, tandis que le processus de minage sécurise le réseau.

Les points les plus importants à privilégier, si le temps manque, sont :



1. Rôles de nœud vs mineur
1. Mempool comme salle d'attente
1. Preuve de Travail
1. Ajustement de la difficulté
1. Flux de transaction de la signature à la confirmation

##### À quoi ressemble un bon résultat

* Il est important de clarifier immédiatement que Mineurs ≠ Nœuds, de montrer le minage comme une activité économique avec de vrais coûts matériels et dépenses d'électricité, d'utiliser l'ajustement de la difficulté et la Preuve de Travail pour expliquer le mécanisme de sécurité, et de tester la compréhension avec des scénarios sur les changements du réseau.
* Les éducateurs doivent utiliser des chiffres réels pour ancrer les discussions, être d'une clarté absolue et répétitive sur la distinction entre Mineurs et Nœuds, être réalistes quant aux préoccupations de centralisation liées aux pools de minage, et respecter la véritable sophistication impliquée.
* Les étudiants comprennent que le minage implique des personnes intelligentes effectuant un travail complexe car elles gagnent du Bitcoin, reconnaissent que les incitations motivent un comportement honnête puisque les profits des mineurs dépendent du succès de Bitcoin, voient le système s'autoréguler grâce à l'ajustement automatique de la difficulté, comprennent que le minage est une véritable entreprise et non de la charité, et apprécient que la sécurité de Bitcoin coûte réellement de l'électricité et de l'argent.
* Les résultats d'apprentissage doivent être atteints si les étudiants peuvent distinguer les mineurs qui créent les blocs des nœuds qui les valident, comprendre la Preuve de Travail comme un mécanisme de sécurité qui rend les attaques exponentiellement coûteuses, reconnaître que l'ajustement de la difficulté maintient le temps de bloc à environ 10 minutes, comprendre les incitations des mineurs autour des récompenses de bloc et des frais, expliquer pourquoi une attaque à 51% échoue, et voir le minage comme une activité économique avec de vrais coûts et bénéfices.

##### Gestion du temps

Si le temps est limité, priorisez :

* Rôles de nœud vs mineur (la distinction essentielle)
* Mempool comme salle d'attente
* Mécanisme de Preuve de Travail
* Ajustement de la difficulté (système autorégulateur)
* Flux de transaction de la signature à la confirmation

Si vous êtes en avance, prenez le temps sur :

* Économie du minage et spécificités du matériel
* Dynamiques des pools de minage et préoccupations de centralisation
* Scénarios d'attaque à 51% et pourquoi ils échouent mathématiquement
* Sécurité à long terme grâce à l'alignement des incitations

##### Si les étudiants ont des difficultés

* Mineurs vs. nœuds (confusion) → « Les nœuds valident, les mineurs proposent ; arbitres vs joueurs. »
* Preuve de Travail gaspilleuse → « Une sécurité coûteuse empêche les attaques ; les rend inutiles. »
* Ajustement de la difficulté → « Plus de mineurs = blocs plus rapides = difficulté augmente ; le système respire. »
