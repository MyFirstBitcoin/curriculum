# 8.1 La sécurité grâce à la cryptographie

> Ce que le Bitcoin nous offre, c'est une promesse ferme : le programme s'exécutera exactement comme prévu.  
_Andreas M. Antonopoulos_

#### Cryptographie à clé publique/privée


> **Definition – Définition de la cryptographie**
>
> **Cryptographie** c'est la pratique qui consiste à transformer des informations en un secret que seules les personnes autorisées peuvent consulter.


* **Chiffrement** C'est le processus qui consiste à transformer des informations en un format codé afin que seule une personne disposant de la clé appropriée puisse les lire.
* **Déchiffrement** c'est le processus qui consiste à retransformer ces informations codées en données lisibles.

En cryptographie traditionnelle, deux personnes souhaitant communiquer en toute confidentialité doivent d'abord partager la même clé secrète, à l'instar d'un mot de passe commun. L'une utilise cette clé pour chiffrer le message avant de l'envoyer, tandis que l'autre utilise la même clé pour le déchiffrer et le lire.

Le problème avec ce système, c'est que les deux personnes doivent déjà partager la clé secrète. Si quelqu'un d'autre parvient à se procurer cette clé, il pourra lire tous les messages interceptés.

Le Bitcoin résout ce problème en recourant à une approche différente appelée « cryptographie à clé publique », dans laquelle les utilisateurs n'ont pas besoin de partager leurs clés secrètes au préalable.

La cryptographie à clé publique/privée résout le problème du partage des secrets. Au lieu de partager un mot de passe, chaque personne dispose de deux clés : une clé publique et une clé privée.

* Le **clé publique** peut être partagé avec n'importe qui.
* Le **clé privée** doit toujours rester secret.

Si John souhaite envoyer quelque chose à Arel, il peut utiliser la clé publique d'Arel. Seul Arel peut le déverrouiller à l'aide de sa clé privée. Même si quelqu'un intercepte le message, il ne pourra ni le lire ni l'utiliser sans la clé privée.

Dans le système Bitcoin, ce mécanisme sert à créer des signatures numériques. Une signature numérique prouve que le détenteur d'une clé privée a approuvé une transaction, un peu comme lorsque l'on appose sa signature sur un document. C'est ce qui permet aux transactions Bitcoin d'être sécurisées et vérifiables sans avoir à faire appel à un tiers.

Les transactions en bitcoins consistent à transférer la propriété de bitcoins d'une adresse à une autre.

Le chiffrement sert à garantir que seul le véritable détenteur des bitcoins soit habilité à transférer ses fonds à un tiers. Il permet ainsi de protéger ses avoirs contre les acteurs malveillants.

À titre de mesure de sécurité supplémentaire, chaque transaction Bitcoin est automatiquement dotée d'une signature numérique UNIQUE. Cette signature numérique unique repose sur une technologie inviolable qui permet au réseau de vérifier que c'est bien le véritable propriétaire des bitcoins, et non quelqu'un d'autre, qui les a envoyés.


> **Dark**
>
> Chaque utilisateur dispose de deux clés : une **clé privée**, c'est-à-dire **gardé secret**, et un **clé publique** qui peut être **partagé avec d'autres**. Le **clé privée** sert de pièce d'identité et de preuve de propriété, confirmant : « Cette adresse m'appartient et j'en ai le contrôle. »


###### Comment fonctionne une transaction Bitcoin ?

1. **Création de la transaction**: Un utilisateur lance une transaction Bitcoin en indiquant des informations telles que l'adresse du destinataire et le montant en bitcoins à envoyer.
1. **Génération d'une signature numérique**: L'expéditeur génère un identifiant unique **signature numérique** en utilisant leur **clé privée**. Cette signature est un code unique qui permet de vérifier l'authenticité de la transaction.
1. **Diffusion de l'opération**: La transaction signée est diffusée sur le réseau Bitcoin, indiquant ainsi l'intention de transférer la propriété des bitcoins de l'expéditeur au destinataire.
1. **Vérification sur le réseau**: Les nœuds du réseau Bitcoin reçoivent la transaction et utilisent l'adresse du destinataire **clé publique** pour vérifier l'authenticité de la signature de la transaction. Parallèlement, ils utilisent l'adresse de l'expéditeur **clé publique** pour vérifier le **signature numérique**.
1. **Confirmation sur le réseau Bitcoin**: Si la vérification aboutit, la transaction sera ajoutée au registre, qui constitue un registre sécurisé et transparent de toutes les transactions. Une fois confirmée, la propriété des bitcoins est officiellement transférée de l'expéditeur au destinataire.


> **Callout – Résumé**
>
> Le **signature numérique**, créé à partir des informations de l’expéditeur **clé privée**, prouve que la transaction a été autorisée par le propriétaire du bitcoin. Le réseau Bitcoin peut alors vérifier cette preuve et enregistrer la transaction.


#### Explication du hachage

Ne vous laissez surtout pas intimider par les termes techniques et les concepts mathématiques qui vont suivre. Nous comprenons que tout le monde n’est pas passionné par les maths, mais vous pourriez vous surprendre vous-même en constatant que même les idées les plus complexes peuvent être comprises avec un peu d’effort.


> **Definition – Définition d'une fonction**
>
> A **fonction** c'est comme une machine qui prend des informations et les transforme en quelque chose de nouveau. Les informations que vous fournissez à la fonction sont les **entrée**. Les nouvelles informations générées par la fonction sont les suivantes : **sortie**. Les fonctions aident les ordinateurs à effectuer des tâches et à résoudre des problèmes.


##### Qu'est-ce qu'une fonction ?

Une fonction est un ensemble d'instructions qui prend une entrée et produit une sortie. On peut la comparer à une recette : on suit les étapes en utilisant certains ingrédients, et on obtient toujours un résultat prévisible.

Dans le système Bitcoin, les fonctions servent à traiter et à vérifier les transactions. Lorsqu'un utilisateur envoie des bitcoins, des fonctions cryptographiques permettent de vérifier la validité de la transaction, de s'assurer que l'expéditeur dispose de fonds suffisants et de mettre à jour les soldes dans le grand livre Bitcoin. Une fois vérifiée et ajoutée à un bloc, la transaction est intégrée à l'historique permanent de la blockchain.

##### Qu'est-ce qu'une fonction à sens unique ?

Une fonction à sens unique est un type particulier de fonction qui est facile à calculer dans un sens, mais extrêmement difficile à inverser. Par exemple, mélanger des ingrédients pour préparer un smoothie est facile, mais il est impossible de séparer à nouveau le smoothie pour obtenir les ingrédients d'origine.

La sécurité du Bitcoin repose sur des fonctions à sens unique. Celles-ci sont utilisées dans la cryptographie à clés publiques et privées, permettant ainsi aux utilisateurs de partager une clé publique tout en gardant leur clé privée secrète. Même si la clé publique est visible, il est impossible d'en déduire la clé privée. C'est ce qui garantit la sécurité des transactions Bitcoin.

##### Qu'est-ce qu'une fonction de hachage ?

A **fonction de hachage** C'est comme une machine à coder. Elle reçoit un message et le transforme en code.

###### Comment fonctionne le hachage dans les transactions Bitcoin ?

Dans le système Bitcoin, chaque transaction est convertie en un hachage avant d'être ajoutée à la blockchain. Un hachage est une empreinte numérique unique de la transaction. Si quelqu'un tente de modifier ne serait-ce qu'une infime partie de la transaction, le hachage changera complètement. Cela permet au réseau de détecter facilement toute tentative de falsification.

###### Le rôle du hachage dans la sécurité du Bitcoin

Le hachage contribue à protéger le réseau Bitcoin en rendant les transactions faciles à vérifier et impossibles à modifier discrètement. Chaque transaction disposant d'un hachage unique, le réseau peut rapidement détecter toute altération.

Une fonction de hachage prend des données et les convertit en une chaîne fixe composée de chiffres et de lettres, appelée « hachage ». Une même entrée produira toujours le même hachage, mais la moindre modification de l'entrée donnera lieu à un résultat complètement différent. Cette propriété permet aux ordinateurs de vérifier que les données n'ont pas été modifiées.


> **Definition – Définition du hachage**
>
> **Hachage** C'est un peu comme créer une empreinte digitale pour des données numériques. Il s'agit du processus consistant à transformer un message numérique en un code de longueur fixe, qui sert d'identifiant unique. Tout comme une empreinte digitale permet d'identifier une personne, un hachage permet d'identifier un message numérique.


Le **sortie**, ou « hash », a toujours la même longueur, quelle que soit la longueur de l'information d'origine. Bitcoin utilise plusieurs types spécifiques de fonctions de hachage appelées **SHA-256** et **RIPEMD160**.

En voici quelques exemples :

* Hachage SHA256 de la chaîne de caractères **bonjour tout le monde**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Hachage SHA256 de la chaîne de caractères **Bonjour tout le monde.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Remarquez qu'une petite modification de l'entrée modifie complètement le résultat par rapport au premier.
* Hachage SHA256 du fichier ISO téléchargeable **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Ce fichier d'entrée est très volumineux, mais la sortie reste toujours de longueur fixe.

On peut également comparer le hachage à une partition musicale qui capture l'essence d'un morceau. Tout comme une partition musicale est une représentation unique d'un air, une valeur de hachage est une représentation unique d'une donnée.

En comparant la partition d'un morceau de musique à l'interprétation réelle, un musicien peut déterminer si celle-ci est fidèle à la partition. De la même manière, en comparant la valeur de hachage des données reçues à la valeur de hachage d'origine, on peut déterminer si les données ont été altérées pendant la transmission.

Tout comme une légère variation dans une interprétation musicale peut en modifier la sonorité, la moindre modification apportée aux données d'origine entraînera une valeur de hachage différente. Cela fait du hachage un outil puissant pour garantir l'intégrité et l'authenticité d'une transaction Bitcoin.

Le processus d'encodage du **clé publique** Le hachage est utilisé pour renforcer la sécurité des informations en les convertissant en un format illisible et de longueur fixe. Bitcoin utilise les algorithmes SHA-256 et RIPEMD160 pour générer des adresses publiques. Le résultat obtenu sert d'identifiant unique pour le **clé publique** et contribue à garantir l'intégrité et la sécurité des transactions enregistrées dans le registre. En cryptant les informations de cette manière, il devient plus difficile pour des personnes non autorisées d'accéder aux données et de les manipuler.

##### Propriétés d'une fonction de hachage

* **Déterministe**: Les mêmes ingrédients donnent toujours le même smoothie. De la même manière, les mêmes données produiront toujours le même hachage.
* **Résistance pré-image**: Si vous ne disposez que du smoothie, vous ne pouvez pas déterminer quels fruits ont été utilisés exactement. De même, si vous ne disposez que d'un hachage, vous ne pouvez pas déterminer les données d'origine.
* **Effet d'avalanche**: Il suffit de modifier ne serait-ce qu'un tout petit élément des ingrédients pour obtenir un smoothie complètement différent. En hachage, une modification minime des données produit un hachage complètement différent.
* **Résistance aux chocs**: Il est extrêmement difficile de trouver deux ensembles d'ingrédients différents qui permettent d'obtenir exactement le même smoothie. De la même manière, il est extrêmement improbable que deux données différentes produisent le même hachage.
* **Vérification rapide**: La préparation du smoothie est rapide, et il est facile de vérifier que le résultat correspond bien à un smoothie. Les fonctions de hachage sont rapides à calculer et faciles à vérifier par tout le monde.

#### Activité : Générer un hachage SHA-256


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Vous vous demandez comment fonctionne le hachage ? Scannez le code QR pour générer instantanément un hachage SHA256 à partir d'un mot, d'une phrase ou de n'importe quelle entrée de votre choix. Les fonctions de hachage sont comme des empreintes digitales numériques : elles sont à sens unique, ce qui signifie qu'une fois qu'un élément a été haché, le processus ne peut pas être inversé. Essayez-le et voyez par vous-même !
