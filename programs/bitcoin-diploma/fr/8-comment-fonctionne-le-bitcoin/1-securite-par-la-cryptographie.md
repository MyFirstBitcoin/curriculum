# 8.1 Sécurité par la cryptographie

> Ce que Bitcoin nous offre, c'est une promesse ferme : le programme s'exécutera exactement comme spécifié.  
_Andreas M. Antonopoulos_

#### Cryptographie à clé publique/privée


> **Definition – Définition de la cryptographie**
>
> **Cryptographie** est la pratique qui consiste à transformer des informations en un secret que seules les bonnes personnes peuvent lire.


* **Chiffrement** est le processus qui consiste à transformer des informations en une forme codée afin que seule une personne possédant la clé correcte puisse les lire.
* **Déchiffrement** est le processus qui consiste à transformer ces informations codées en quelque chose de lisible.

Dans la cryptographie traditionnelle, deux personnes qui souhaitent communiquer en privé doivent d'abord partager la même clé secrète, similaire à un mot de passe partagé. Une personne utilise cette clé pour chiffrer le message avant de l'envoyer, et l'autre personne utilise la même clé pour le déchiffrer et le lire.

Le problème avec ce système est que les deux personnes doivent déjà partager la clé secrète. Si quelqu'un d'autre accède à cette clé, il peut lire tous les messages interceptés.

Bitcoin résout ce problème en utilisant une approche différente appelée cryptographie à clé publique, où les utilisateurs n'ont pas besoin de partager des clés secrètes à l'avance.

La cryptographie à clé publique/privée résout le problème du partage des secrets. Au lieu de partager un mot de passe, chaque personne possède deux clés : une clé publique et une clé privée.

* La **clé publique** peut être partagée avec n'importe qui.
* La **clé privée** doit toujours rester secrète.

Si John veut envoyer quelque chose à Arel, il peut utiliser la clé publique d'Arel. Seul Arel peut la déverrouiller en utilisant sa clé privée. Même si quelqu'un intercepte le message, il ne pourra pas le lire ou l'utiliser sans la clé privée.

Dans Bitcoin, ce système est utilisé pour créer des signatures numériques. Une signature numérique prouve que le propriétaire d'une clé privée a approuvé une transaction, comme lorsque vous signez votre nom sur un document. C'est ce qui permet aux transactions Bitcoin d'être sécurisées et vérifiables sans avoir à faire confiance à un tiers.


> **Info**
>
> Chaque utilisateur possède deux clés : une **clé privée**, qui est **gardée secrète**, et une **clé publique** qui peut être **partagée avec d'autres**.
>
> La **clé privée** sert de forme d'identification et de preuve de propriété, confirmant : « Cette adresse m'appartient et j'en ai le contrôle. »
>
> **Signatures numériques** sont créées pour identifier des transactions uniques.


Les transactions Bitcoin impliquent le transfert de propriété de bitcoins d'une adresse à une autre.

Le chiffrement est utilisé pour garantir que seul le véritable détenteur du bitcoin a l'autorité d'envoyer son argent à quelqu'un d'autre. Il garantit que sa propriété est protégée contre les acteurs malveillants.

Comme mesure de protection supplémentaire, chaque transaction Bitcoin reçoit automatiquement une signature numérique UNIQUE. Cette signature numérique unique est alimentée par une technologie inviolable qui aide le réseau à vérifier que le véritable propriétaire du bitcoin, et non quelqu'un d'autre, les a envoyés.

###### Comment fonctionne une transaction Bitcoin

1. **Création de la transaction** : Un utilisateur initie une transaction Bitcoin en spécifiant des détails tels que l'adresse du destinataire et le montant de bitcoin à envoyer.
1. **Génération de la signature numérique** : L'expéditeur génère une **signature numérique** unique en utilisant sa **clé privée**. Cette signature est un code unique qui vérifie l'authenticité de la transaction.
1. **Diffusion de la transaction** : La transaction signée est diffusée sur le réseau Bitcoin, indiquant l'intention de transférer la propriété du bitcoin de l'expéditeur au destinataire.
1. **Vérification sur le réseau**: Les nœuds du réseau Bitcoin reçoivent la transaction et utilisent la **clé publique** du destinataire pour vérifier l’authenticité de la signature de la transaction. Simultanément, ils utilisent la **clé publique** de l’expéditeur pour vérifier la **signature numérique**.
1. **Confirmation sur le réseau Bitcoin**: Si la vérification est réussie, la transaction sera ajoutée au registre, qui sert de dossier sécurisé et transparent de toutes les transactions. Une fois confirmée, la propriété du bitcoin est officiellement transférée de l’expéditeur au destinataire.


> **Callout – Résumé**
>
> La **signature numérique**, créée avec la **clé privée** de l’expéditeur, prouve que la transaction a été autorisée par le propriétaire du bitcoin.
>
> Le réseau Bitcoin peut alors vérifier cette preuve et enregistrer la transaction.


#### Explication du hachage

Ne soyez pas intimidé par les termes techniques et les concepts mathématiques à venir. Nous comprenons que tout le monde n’est pas passionné de mathématiques, mais vous pourriez vous surprendre et voir que même les idées les plus complexes peuvent être comprises avec un peu d’effort.


> **Definition – Définition d’une fonction**
>
> Une **fonction** est comme une machine qui prend des informations et les transforme en quelque chose de nouveau. Les informations que vous donnez à la fonction sont l’**entrée**. La nouvelle information créée par la fonction est la **sortie**. Les fonctions aident les ordinateurs à effectuer des tâches et à résoudre des problèmes.


##### Qu’est-ce qu’une fonction ?

Une fonction est un ensemble d’instructions qui prend une entrée et produit une sortie. Vous pouvez la comparer à une recette : vous suivez les étapes avec certains ingrédients, et vous obtenez toujours un résultat prévisible.

Dans Bitcoin, les fonctions sont utilisées pour traiter et vérifier les transactions. Lorsqu’une personne envoie des bitcoins, des fonctions cryptographiques permettent de vérifier que la transaction est valide, de confirmer que l’expéditeur dispose de fonds suffisants et de mettre à jour les soldes sur le registre Bitcoin. Une fois vérifiée et ajoutée à un bloc, la transaction fait partie de l’enregistrement permanent sur la blockchain.

##### Qu’est-ce qu’une fonction à sens unique ?

Une fonction à sens unique est un type spécial de fonction qui est facile à calculer dans un sens mais extrêmement difficile à inverser. Par exemple, mixer des ingrédients pour faire un smoothie est facile, mais il est impossible de séparer le smoothie pour retrouver les ingrédients d’origine.

La sécurité de Bitcoin repose sur les fonctions à sens unique. Elles sont utilisées dans la cryptographie à clé publique et privée, permettant aux gens de partager une clé publique tout en gardant leur clé privée secrète. Même si la clé publique est visible, il est impossible d’en déduire la clé privée. C’est ce qui rend les transactions Bitcoin sécurisées.

##### Qu’est-ce qu’une fonction de hachage ?

Une **fonction de hachage** est comme une machine à code secret. Elle prend un message et le transforme en un code.

###### Comment fonctionne le hachage dans les transactions Bitcoin

Dans Bitcoin, chaque transaction est transformée en un hachage avant d’être ajoutée à la blockchain. Un hachage est une empreinte digitale unique de la transaction. Si quelqu’un essaie de modifier ne serait-ce qu’une petite partie de la transaction, le hachage changera complètement. Cela permet au réseau de détecter facilement toute tentative de falsification.

###### Le rôle du hachage dans la sécurité de Bitcoin

Le hachage aide à protéger le réseau Bitcoin en rendant les transactions faciles à vérifier et impossibles à modifier discrètement. Parce que chaque transaction a son propre hachage unique, le réseau peut rapidement détecter si quelque chose a été modifié.

Une fonction de hachage prend des données et les convertit en une chaîne fixe de chiffres et de lettres appelée hachage. La même entrée produira toujours le même hachage, mais même un minuscule changement dans l’entrée créera un résultat complètement différent. Cette propriété permet aux ordinateurs de vérifier que les données n’ont pas été modifiées.


> **Definition – Définition du hachage**
>
> **Le hachage** est comme créer une empreinte digitale pour des données numériques. C’est le processus qui consiste à prendre un message numérique et à le transformer en un code de longueur fixe, qui sert d’identifiant unique. Tout comme une empreinte digitale peut identifier une personne, un hachage peut identifier un message numérique.


La **sortie**, ou hachage, a toujours la même longueur, quelle que soit la taille de l’information d’origine. Bitcoin utilise quelques types spécifiques de fonction de hachage appelés **SHA-256** et **RIPEMD160**.

Voici quelques exemples ci-dessous :

* SHA256 du texte **hello world**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256 du texte **hello world.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Remarquez qu’un petit changement dans l’entrée modifie complètement la sortie par rapport au premier exemple
* SHA256 du fichier iso téléchargeable **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Cette entrée est un fichier volumineux, mais la sortie reste toujours de la même longueur fixe

Vous pouvez aussi comparer le hachage à une partition musicale qui capture l’essence d’un morceau de musique. Tout comme une partition est une représentation unique d’un air, une valeur de hachage est une représentation unique d’une donnée.

En comparant la partition d’un morceau avec l’interprétation réelle, un musicien peut déterminer si l’exécution est fidèle. De la même manière, en comparant la valeur de hachage des données reçues avec la valeur de hachage originale, on peut savoir si les données ont été modifiées pendant la transmission.

De même qu’une légère variation dans une interprétation musicale peut la rendre différente, même le plus petit changement dans les données originales produira une valeur de hachage différente. Cela fait du hachage un outil puissant pour garantir l’intégrité et l’authenticité d’une transaction Bitcoin.

Le processus de codage de la **clé publique** par hachage est utilisé pour renforcer la sécurité de l’information en la convertissant en un format illisible de longueur fixe. Bitcoin utilise les algorithmes SHA-256 et RIPEMD160 pour produire les adresses publiques. Le résultat sert d’identifiant unique pour la **clé publique** et contribue à garantir l’intégrité et la sécurité des transactions enregistrées dans le registre. En chiffrant l’information de cette manière, il devient plus difficile pour des personnes non autorisées d’accéder aux données et de les manipuler.

##### Propriétés d’une fonction de hachage

* **Déterministe** : Les mêmes ingrédients produisent toujours le même smoothie. De la même façon, les mêmes données produiront toujours le même hachage.
* **Résistance à la préimage** : Si vous n’avez que le smoothie, vous ne pouvez pas retrouver exactement quels fruits ont été utilisés. De même, si vous n’avez qu’un hachage, vous ne pouvez pas retrouver les données originales.
* **Effet avalanche** : Changer ne serait-ce qu’une toute petite partie des ingrédients donne un smoothie complètement différent. En hachage, une très petite modification des données produit un hachage totalement différent.
* **Résistance aux collisions** : Il est extrêmement difficile de trouver deux ensembles d’ingrédients différents qui produisent exactement le même smoothie. De la même façon, il est extrêmement improbable que deux données différentes produisent le même hachage.
* **Rapide à vérifier** : Faire le smoothie est rapide, et il est facile de vérifier que le résultat est bien un smoothie. Les fonctions de hachage sont rapides à calculer et faciles à vérifier pour tout le monde.

#### Activité : Générer un hachage SHA 256

https://tools.keycdn.com/sha256-online-generator

Curieux de savoir comment fonctionne le hachage ? Scannez le code QR pour générer instantanément un hachage SHA256 à partir de n’importe quel mot, phrase ou entrée de votre choix. Les fonctions de hachage sont comme des empreintes digitales numériques : elles sont à sens unique, ce qui signifie qu’une fois quelque chose haché, il est impossible de revenir en arrière. Essayez et voyez par vous-même !
