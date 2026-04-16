# 3.0 Introduction

> **Info – Résumé du livre blanc sur le Bitcoin**
>
> **Une version purement pair-à-pair de la monnaie électronique** permettrait d’envoyer des paiements en ligne directement d’une partie à une autre sans passer par une institution financière. **Les signatures numériques fournissent une partie de la solution**, mais les principaux avantages sont perdus si un **tiers de confiance** est toujours nécessaire pour empêcher la double dépense. Nous proposons une solution au problème de la double dépense en utilisant un **réseau pair-à-pair**. Le **réseau horodate les transactions** en les hachant dans une chaîne continue de **preuve de travail basée sur le hachage,** formant un registre qui ne peut pas être modifié sans refaire la **preuve de travail**. La chaîne la plus longue sert non seulement de preuve de la séquence des événements observés, mais aussi de preuve qu’elle provient du plus grand pool de puissance de calcul. Tant qu’une majorité de la puissance de calcul est contrôlée par des nœuds qui ne coopèrent pas pour attaquer le réseau, ils généreront la chaîne la plus longue et dépasseront les attaquants. **Le réseau lui-même nécessite une structure minimale. Les messages sont diffusés selon le principe du meilleur effort, et les nœuds peuvent quitter et rejoindre le réseau à leur guise**, acceptant la chaîne de preuve de travail la plus longue comme preuve de ce qui s’est passé pendant leur absence.


Le Bitcoin n’est pas apparu dans le vide, mais s’est appuyé sur le travail de nombreux chercheurs des décennies précédentes. Ce module explorera les fondations de l’internet sur lesquelles Bitcoin s’appuie, ainsi que la recherche et le développement reconnus dans le livre blanc.

Dans les années 70, un groupe d’individus a observé comment le gouvernement américain, en particulier, tentait de restreindre l’accès à la cryptographie, et s’est efforcé de faire en sorte que cette technologie soit accessible à tous afin de protéger la vie privée en ligne. Certains de ces pionniers s’intéressaient également aux avantages potentiels d’un système monétaire numérique « sain » qui pourrait servir à stocker et échanger de la valeur sur l’internet émergent. Friedrich Hayek – un contributeur majeur à l’école autrichienne d’économie – avait imaginé à quoi ressemblerait une monnaie idéale fondée sur la concurrence du marché libre bien avant l’ère d’internet, mais avait jugé cela techniquement et politiquement irréalisable. Outre la vie privée numérique, ce groupe, qui deviendra les Cypherpunks, a tenté de concrétiser la vision de Hayek pour une monnaie numérique, mais ces tentatives avaient échoué jusqu’à ce que Satoshi publie ses idées sur la liste de diffusion.

* Protocole TCP/IP (1976)
* Protocoles pour les systèmes de cryptographie à clé publique - Ralph Merkle (1980)
* Digicash - David Chaum (1989)
* Horodatage numérique (années 90)
* Hashcash - Adam Back (1997)
* BitTorrent - Bram Cohen (2001)
* POW réutilisable - Hal Finney (2004)
* Livre blanc Bitcoin - Satoshi Nakamoto (2008)

Une influence majeure sur le développement de Bitcoin fut l’émergence du mouvement Cypherpunk dans les années 1990. Ils ont développé plusieurs technologies cryptographiques, dont la cryptographie à clé publique, permettant aux utilisateurs de communiquer et partager des informations de manière sécurisée et privée. Beaucoup des développements décrits ici et les personnes impliquées faisaient partie de ce groupe.

Le besoin d’une monnaie numérique a également été identifié et plusieurs tentatives ont été faites pour la créer, mais elles présentaient des limites qui les ont empêchées de réussir. Le génie de Satoshi Nakamoto a été de rassembler ces capacités et, avec quelques innovations personnelles, de s’appuyer dessus pour créer le protocole Bitcoin utilisé aujourd’hui. Dans les prochaines sections, nous explorerons certains de ces développements et expliquerons comment ils ont contribué à la conception de Bitcoin. Nous discuterons également des pièces manquantes du puzzle que Satoshi a réussi à résoudre.
