# 6 - Comment utiliser le Bitcoin

Durée : 90 minutes

Idée principale : Utiliser Bitcoin sur la blockchain enseigne aux étudiants comment fonctionnent la propriété, l’auto-garde et la vérification en pratique, transformant la théorie en action financière concrète.

#### Objectifs d'apprentissage

À la fin de cette leçon, les étudiants devraient être capables de :

* Identifier les moyens courants d’acquérir et d’échanger du bitcoin, y compris les méthodes de pair à pair et via des plateformes centralisées.
* Expliquer la différence entre les portefeuilles auto-gérés et les portefeuilles dépositaires, et pourquoi l’auto-garde est importante dans Bitcoin.
* Décrire le rôle des clés privées, des adresses publiques, des phrases de récupération (seed phrase) et des interfaces de portefeuille.
* Comparer différents types de portefeuilles et évaluer leurs compromis en termes de sécurité, de commodité, de confidentialité et de contrôle.
* Configurer un portefeuille Bitcoin mobile et expliquer le processus de récupération de base.
* Démontrer comment recevoir et envoyer une transaction bitcoin sur la blockchain.

Appliquer le principe « Ne faites pas confiance, vérifiez » au choix du portefeuille, aux transactions et à l’utilisation plus large de Bitcoin.

#### Outils & Ressources

##### Supports visuels

* Chapitre 6 - Comment utiliser Bitcoin

##### Bibliothèque de soutien

* Carte de référence du vocabulaire — Chapitre 6 — Termes : portefeuille, clé privée, adresse publique, phrase de récupération, dépositaire, auto-garde, UTXO, frais de transaction
* Tableaux comparatifs & fiches de référence — Comparaison des types de portefeuilles (dépositaire, mobile, matériel, papier)
* Explications techniques & approfondissements — Clés publiques/privées, modèle UTXO, confirmation des transactions
* Approfondissement sur la sécurité des clés privées — Phrases de récupération, dérivation de clés, méthodes de sauvegarde, vecteurs d’attaque
* Guide de l’anatomie d’une transaction — Exemple étape par étape du fonctionnement d’une transaction Bitcoin
* Liste de vérification des meilleures pratiques de sécurité — Avant de commencer, création du portefeuille, réception, envoi, prévention du phishing

#### Activités

* Transactions en action
* Course de relais Lightning
* Explorer le mempool

#### Enseignement en ligne

* Précisez dès le début si les étudiants regardent une démonstration ou s’ils configurent eux-mêmes un portefeuille.
* Utilisez de grandes captures d’écran lisibles pour chaque étape de la configuration du portefeuille.
* Faites une pause après chaque étape et demandez aux étudiants de confirmer leur compréhension dans le chat avant de continuer.
* Donnez un avertissement direct avant la section sur la phrase de récupération et rappelez aux étudiants de ne jamais partager d’informations sensibles en ligne.

#### Préparation

* Téléchargez et testez une application de portefeuille mobile (Blue Wallet ou Muun) ; préparez des captures d’écran des étapes clés de la configuration.
* Préparez un guide de configuration du portefeuille (téléchargement → création → sauvegarde de la phrase de récupération → réception) pour référence.
* Assurez-vous que le réseau/WiFi fonctionne ; préparez une adresse de démonstration et un QR code à montrer.

#### Procédure

Cette leçon passe de la théorie à la pratique directe. Elle correspond désormais directement à la structure du Diplôme afin que l’acquisition, les portefeuilles, la configuration, les transactions et la vérification apparaissent sous les mêmes rubriques principales que le guide de l’étudiant. Le soutien pédagogique supplémentaire reste intégré dans ces sections.

##### 6.0 Introduction, 8 minutes

Commencez par relier ce chapitre au précédent :

* Si Bitcoin est de l’argent, comment les gens l’obtiennent-ils et l’utilisent-ils réellement ?
* Que signifie vraiment contrôler son bitcoin ?
* Pourquoi utiliser Bitcoin est-il différent d’utiliser une application bancaire ?

Précisez que ce chapitre porte sur l’utilisation pratique. Les étudiants n’apprennent plus seulement ce qu’est Bitcoin, ils apprennent à interagir directement avec lui.

##### 6.1 Acquérir et échanger du Bitcoin, 12 minutes

Expliquez que l’on peut acquérir du bitcoin de différentes manières, notamment :

* être payé en bitcoin
* miner du bitcoin
* échanger des monnaies fiduciaires contre du bitcoin en personne
* échanger des monnaies fiduciaires contre du bitcoin en ligne

Concentrez-vous ensuite sur les deux principales méthodes d’acquisition abordées dans le chapitre :

* de pair à pair, en personne
* pair-à-pair, en ligne
* plateformes d’échange centralisées

Rendez les compromis clairs.

Pour le pair-à-pair en personne, insistez sur l’échange direct sans banque ni intermédiaire, mais mentionnez aussi les risques pratiques de rencontrer des personnes pour des échanges en espèces.

Pour le pair-à-pair en ligne, expliquez l’escrow (tiers de confiance) en termes simples, comme un moyen de réduire le risque de contrepartie tout en permettant un échange direct entre pairs.

Pour les plateformes d’échange centralisées, précisez qu’elles sont pratiques, mais qu’elles exigent des utilisateurs qu’ils fassent confiance à une entreprise, partagent souvent des informations personnelles, et laissent leurs fonds sous le contrôle d’un tiers jusqu’au retrait. C’est le bon moment pour rappeler que la commodité s’accompagne souvent de compromis en matière de vie privée et de souveraineté.

##### 6.2 Introduction aux portefeuilles Bitcoin, 35 minutes

**Ce qu’est réellement un portefeuille Bitcoin**

Clarifiez tout de suite une idée reçue : le bitcoin n’est pas stocké dans l’application portefeuille comme de l’argent liquide dans un sac.  
Le bitcoin existe sur le registre maintenu par le réseau. Ce que l’utilisateur contrôle, c’est la capacité de le dépenser via les clés privées.

Expliquez ensuite les deux choses que les gens entendent souvent par « portefeuille » :

* le système de clés privées, à partir duquel les adresses sont générées
* l’application ou l’interface utilisée pour interagir avec le réseau

Utilisez l’analogie de l’email du chapitre si cela aide :

* adresse publique = comme une adresse email que vous pouvez partager
* clé privée = comme un mot de passe que vous devez protéger

Soyez très clair ici : celui qui contrôle les clés privées contrôle le bitcoin. C’est le concept fondamental que les étudiants doivent comprendre.

**Portefeuilles en auto-garde vs portefeuilles en garde**

C’est l’une des parties les plus importantes du chapitre.

Expliquez clairement la distinction :

* Portefeuille en auto-garde : l’utilisateur contrôle les clés privées
* Portefeuille en garde : un tiers contrôle les clés privées au nom de l’utilisateur

Présentez ensuite les compromis :

Auto-garde

* contrôle total des fonds
* aucun processus d’approbation
* protection contre la confiscation arbitraire
* plus grande responsabilité
* pas de récupération facile si la phrase de récupération est perdue

Garde

* récupération et assistance plus faciles
* plus simple pour les débutants
* plus exposé aux gels de compte, piratages et contrôle par des tiers
* l’utilisateur ne détient pas réellement le bitcoin

C’est le bon moment pour insister sur la phrase :

« Pas vos clés, pas vos bitcoins. »

Les étudiants doivent quitter cette section en comprenant non seulement le slogan, mais aussi ce qu’il signifie concrètement.

**Différents types de portefeuilles et comment en choisir un**

Présentez les types de portefeuilles abordés dans le chapitre :

* portefeuille en ligne
* portefeuille mobile
* portefeuille de bureau
* portefeuille matériel
* portefeuille papier

Ne présentez aucun comme parfait. Expliquez plutôt que chacun implique des compromis entre :

* sécurité
* confidentialité
* commodité
* compatibilité
* frais
* contrôle
* réputation

Précisez également que nous recommandons de prêter attention au fait que le logiciel de portefeuille soit open source, car les outils open source peuvent être examinés, audités et maintenus par la communauté. Cela se rattache directement au principe de vérification dans Bitcoin.

##### 6.3 Configuration d’un portefeuille Bitcoin mobile, 10 minutes

Guide les élèves à travers le processus de base présenté dans le chapitre :

* télécharger le portefeuille
* créer un nouveau portefeuille
* générer et noter la phrase de récupération
* confirmer la phrase de récupération
* ajouter une sécurité supplémentaire si disponible
* ouvrir le portefeuille et trouver la fonction de réception

Rendez l’avertissement concernant la phrase de récupération très explicite :

* si la phrase de récupération est perdue, l’accès aux fonds peut être perdu
* si quelqu’un d’autre obtient la phrase de récupération, il peut prendre les fonds

Si les élèves réalisent cette activité de manière pratique, l’enseignant doit faire une pause à chaque étape et vérifier que tout le monde comprend ce qu’il fait. Si la classe est plus conceptuelle, cette section peut être expliquée comme une démonstration plutôt que réalisée en direct. L’option de récupération présentée dans le chapitre est également utile pour expliquer que les portefeuilles peuvent être restaurés si la phrase de récupération a été correctement sauvegardée.

##### 6.4 Recevoir et envoyer des transactions, 17 minutes

**Recevoir et envoyer des transactions sur la blockchain**

Expliquez maintenant comment fonctionnent les transactions sur la blockchain.

Pour recevoir des bitcoins :

* ouvrir le portefeuille
* appuyer sur recevoir ou déposer
* copier l’adresse, partager le lien ou montrer le code QR

Pour envoyer des bitcoins :

* ouvrir le portefeuille
* coller ou scanner l’adresse du destinataire
* saisir le montant
* vérifier tous les détails
* diffuser la transaction
* attendre la confirmation

Rendez ces points clés clairs :

* la transaction transfère la propriété, pas des pièces physiques
* les transactions sont irréversibles
* les nœuds vérifient la validité
* les mineurs incluent les transactions dans les blocs
* les frais influencent la priorité de confirmation
* les transactions sur la blockchain sont généralement sûres, mais plus lentes et souvent plus coûteuses que les transactions Lightning

Le schéma du flux de transaction dans le chapitre est particulièrement utile ici, car il aide les élèves à visualiser le chemin allant de la demande du portefeuille à la confirmation sur le réseau.

**Transactions en action et pratique par rôle**

Utilisez la structure d’exercice coopératif du chapitre pour renforcer la compréhension. Expliquez les quatre rôles impliqués :

* expéditeur
* destinataire
* mineur
* opérateur de nœud

Une approche simple en classe consiste à attribuer des rôles et à parcourir une transaction étape par étape. Cela aide les élèves à voir qu’une transaction Bitcoin n’est pas magique, c’est un processus coordonné impliquant approbation, vérification, inclusion dans un bloc et mise à jour du registre.

L’objectif ici n’est pas la profondeur technique. Il s’agit d’aider les élèves à comprendre qui fait quoi dans une transaction et pourquoi la vérification est importante.

##### 6.5 Ne faites pas confiance, vérifiez, 8 minutes

Expliquez que cela s’applique à :

* portefeuilles
* plateformes d’échange
* applications
* détails des transactions
* affirmations sur des « profits faciles »
* projets prétendant être comme Bitcoin

Expliquez clairement que Bitcoin exige des utilisateurs qu'ils réfléchissent de manière critique, vérifient ce qu'ils utilisent et évitent la confiance aveugle. Expliquez également pourquoi les outils open source sont importants dans ce contexte : ils rendent possible la vérification indépendante.

###### Conclusion et vérification de la compréhension

Terminez avec quelques questions rapides :

* Quelle est la différence entre un portefeuille dépositaire et un portefeuille en auto-garde ?
* Pourquoi la phrase de récupération (seed phrase) est-elle si importante ?
* Que se passe-t-il lorsque vous envoyez une transaction sur la blockchain ?
* Pourquoi les transactions sur la blockchain sont-elles plus lentes que certains autres paiements Bitcoin ?
* Que signifie « Ne faites pas confiance, vérifiez » en pratique ?

#### Notes pour l’enseignant

Ce chapitre est très pratique, donc privilégiez la clarté, la sécurité et la répétition.

Les élèves n'ont pas besoin de maîtriser chaque type de portefeuille en un seul cours. Les objectifs principaux sont :

* comprendre les bases des portefeuilles
* comprendre l’auto-garde
* apprendre le déroulement de base d’une transaction
* adopter un état d’esprit de vérification responsable

Soyez particulièrement vigilant lors de la discussion sur les phrases de récupération et la configuration des portefeuilles. Les élèves doivent repartir en comprenant que ce ne sont pas de petits détails, mais la base de la possession de Bitcoin.

Les visuels et activités les plus utiles dans ce chapitre sont :

* la comparaison entre auto-garde et garde par un tiers
* le tableau des compromis entre types de portefeuilles
* l’exercice de configuration de portefeuille étape par étape
* le schéma du déroulement d’une transaction
* l’activité de transaction basée sur les rôles

##### À quoi ressemble un bon résultat

* Il est important que les élèves configurent réellement un portefeuille ou assistent à une démonstration attentive, que la phrase de récupération soit placée au centre avec « Ces 12 mots SONT votre Bitcoin », qu’on teste des scénarios comme « Que se passe-t-il si vous perdez votre téléphone ? », et qu’on s’entraîne à reconnaître le phishing.
* Les enseignants doivent être des guides pratiques qui ont déjà fait cela, être attentifs à la sécurité sans paranoïa, et être honnêtes sur la difficulté et l’apprentissage nécessaires.
* Les élèves sentent qu’ils ont acquis une compétence réelle qu’ils peuvent utiliser, comprennent que la phrase de récupération est concrète et importante plutôt qu’abstraite, se sentent capables de détenir leur propre Bitcoin, et comprennent que la décentralisation implique une responsabilité personnelle.
* Les objectifs d’apprentissage sont atteints si les élèves savent configurer un portefeuille et comprennent la différence entre clés publiques et privées, comprennent les compromis de garde entre portefeuilles dépositaires et auto-garde, expliquent le fonctionnement d’une transaction (entrées, sorties, frais), démontrent une conscience de la sécurité (protection de la phrase de récupération), et posent des questions critiques sur la propriété et le contrôle.

##### Gestion du temps

Si le temps est limité, privilégiez :

* Comprendre les bases des portefeuilles
* Comprendre l’auto-garde
* Apprendre le déroulement de base d’une transaction
* Adopter un état d’esprit de vérification responsable

Si vous êtes en avance, prenez le temps de :

* Tableau comparatif auto-garde vs garde par un tiers
* Tableau des compromis entre types de portefeuilles
* Exercice de configuration de portefeuille étape par étape avec démonstration en direct
* Schéma du déroulement d’une transaction avec calcul des frais
* Pratiques de sécurité avancées et considérations sur les portefeuilles matériels

##### Si les élèves rencontrent des difficultés

* Phrases de récupération comme « réelles » → « Cette phrase EST votre bitcoin ; pas de service client. »
* Clés publiques vs privées → Analogie avec l’email (adresse vs mot de passe).
* Pourquoi c’est difficile → « Vous en avez le contrôle ; vous en êtes responsable. » Reconnaître le compromis.
