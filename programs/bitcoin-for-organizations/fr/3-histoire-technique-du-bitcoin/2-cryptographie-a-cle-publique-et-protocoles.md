# 3.2 Cryptographie à clé publique et protocoles

L’Internet d’aujourd’hui, ainsi que la plupart des systèmes informatiques modernes, reposent sur la cryptographie, une méthode permettant de dissimuler l’information afin que seul le destinataire puisse la décoder. Les bases de la cryptographie utilisée pour sécuriser Bitcoin remontent aux années 70.

Le premier problème à résoudre est : comment transmettre un secret partagé sur un canal non sécurisé.

Ce problème a d’abord été étudié par Whitfield Diffie et Martin Hellman.

Le problème : les deux parties – généralement appelées Alice et Bob – souhaitent partager des informations secrètes sur un réseau où d’autres peuvent écouter. Pour cela, ils ont créé le processus d’échange de clés Diffie-Hellman.

Ce secret partagé peut ensuite être utilisé comme valeur de départ pour créer de nombreuses clés symétriques afin de chiffrer et déchiffrer les messages à s’envoyer mutuellement, sans jamais partager la clé elle-même en clair.

Comme la clé privée n’a jamais besoin d’être partagée, et que des clés différentes sont utilisées de chaque côté pour chiffrer et déchiffrer, on parle alors d’un algorithme de chiffrement asymétrique.

Cas d’utilisation :

* Alice signe un message avec la clé publique de Bob – qui est la seule personne capable de le déchiffrer à l’aide de sa clé privée
* Alice signe un message avec sa clé privée – en le déchiffrant avec sa clé publique, n’importe qui peut vérifier que le message a bien été envoyé par Alice, sans connaître sa clé privée
* En combinant ces deux approches avec deux couches de chiffrement, un message peut être envoyé de façon à ce que seul Bob puisse le déchiffrer, et il peut ensuite vérifier que l’expéditeur est bien Alice.

Bien qu’il ne soit pas crédité dans l’article, Ralph Merkle a joué un rôle déterminant dans la résolution de ce qui était jusque-là considéré comme une énigme insoluble : comment établir ou rétablir une communication privée sur un réseau ouvert et potentiellement hostile.

Cette approche, prise isolément, est vulnérable à une attaque par force brute, où un attaquant peut utiliser les nombres partagés pour recréer une clé partagée, à condition d’avoir suffisamment de temps et de ressources. Ce n’est donc pas une solution complète à elle seule.

##### Protocoles pour les systèmes de cryptographie à clé publique

En plus d’avoir contribué au système à clé publique Diffie-Hellman décrit ci-dessus, **Ralph Merkle** a continué à contribuer à ce domaine pendant de nombreuses années, et a joué un rôle clé dans le développement de certains composants essentiels utilisés par Bitcoin.

Une fonction de hachage cryptographique est un algorithme mathématique qui prend des entrées de n’importe quelle taille et effectue des calculs complexes pour retourner une valeur de hachage en bits, généralement représentée par une sortie alphanumérique de longueur fixe en format hexadécimal.

* Les entrées peuvent être de n’importe quelle taille
* La sortie est toujours de longueur fixe et déterministe (la même entrée produit toujours le même hachage)
* Il est facile de vérifier, mais extrêmement difficile d’inverser le processus pour retrouver l’entrée
* Une modification minime des données modifie complètement la sortie

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/4f2c38664dafdbc13d0d3538b0e46f298c85ae93-515x331.svg)

Le hachage est une partie intégrante du protocole Bitcoin. Le SHA-256, utilisé dans Bitcoin, a été créé par la NSA et est un exemple d’algorithme de hachage cryptographique.

* Chaque bloc de la chaîne est haché afin que les données ne puissent pas être modifiées – garantissant ainsi l’intégrité du registre distribué
* Le hachage généré doit répondre aux critères de « preuve de travail » pour être considéré comme un bloc valide
* Les arbres de Merkle – en utilisant des embranchements et des hachages de hachages, les arbres de hachage permettent de vérifier de grands ensembles de données avec un stockage minimal
* Les signatures et clés basées sur le hachage peuvent être utilisées pour les portefeuilles, les adresses et l’autorisation des transactions

La vérification distribuée des états de la blockchain et les modèles de registres append-only résistants à la révision sont rendus possibles par le hachage à sens unique. Les fonctions de hachage offrent une méthode fiable et déterministe pour vérifier les événements sur des registres publics comme Bitcoin, en l’absence d’un modèle de confiance centralisé.

Ces nouvelles capacités dans le domaine de la cryptographie devaient, selon leurs créateurs, inaugurer une nouvelle vague d’innovation dans ce secteur.

##### Cryptographie sur courbes elliptiques

L’une de ces innovations ultérieures est apparue sous la forme de la cryptographie sur courbes elliptiques.

La cryptographie sur courbes elliptiques a été introduite en 1985 par deux scientifiques, N. Koblitz et V. Miller. Ils ont proposé d’utiliser des points définis par des courbes elliptiques au lieu des champs premiers finis, de sorte que l’hypothèse du problème du logarithme discret soit respectée, comme c’est couramment le cas dans le protocole standard d’échange de clés Diffie-Hellman. Les détails de ce fonctionnement dépassent le cadre de cette section, mais, à un niveau élevé, une courbe elliptique est l’ensemble des points qui satisfont une équation mathématique spécifique.

L’équation d’une courbe elliptique ressemble à ceci :

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Cela présente quelques propriétés intéressantes :

* Symétrie horizontale. Tout point de la courbe peut être réfléchi par rapport à l’axe des x et rester sur la même courbe.
* toute droite non verticale coupera la courbe en au plus trois points.
* Des tailles de clés compactes sont essentielles pour un stockage et une transmission efficaces des clés publiques dans la blockchain.

Ces propriétés peuvent être utilisées pour créer des paires de clés d’une manière similaire à l’algorithme Diffie-Hellman. Bitcoin utilise ECDSA, qui signifie « Elliptic Curve Digital Signature Algorithm ». Il s’agit d’un procédé qui utilise une courbe elliptique et un champ fini pour « signer » des données de façon à ce que des tiers puissent vérifier l’authenticité de la signature, tandis que le signataire conserve la capacité exclusive de créer la signature. Avec Bitcoin, les données signées sont la transaction qui transfère la propriété.

La partie « finie » est similaire à l’approche « mod » avec Diffie-Hellman, où le résultat de l’équation est divisé et le reste est utilisé pour s’assurer qu’il reste dans une plage de nombres.
