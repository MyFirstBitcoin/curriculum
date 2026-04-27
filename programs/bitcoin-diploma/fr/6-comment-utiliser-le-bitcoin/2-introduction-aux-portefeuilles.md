# 6.2 Introduction aux portefeuilles

Contrairement à l'argent physique, les bitcoins ne sont pas réellement contenus dans un portefeuille Bitcoin. À la place, ils existent sur le registre distribué que le réseau Bitcoin vérifie et sécurise en permanence. Alors, comment pouvez-vous posséder des bitcoins ?

Vous êtes propriétaire de vos bitcoins uniquement si vous contrôlez les clés privées qui vous permettent de signer des transactions et de transférer la propriété de vos bitcoins à quelqu'un d'autre. C'est l'acte d'envoyer des bitcoins.

Examinons deux concepts auxquels nous faisons référence lorsque nous utilisons le terme **portefeuille** :

* Une clé privée principale, comme un mot de passe, à partir de laquelle vos clés publiques, semblables à des adresses e-mail, sont générées. Vous pouvez partager votre adresse publique avec d'autres pour recevoir et envoyer des bitcoins, mais vous ne devez jamais partager votre clé privée !
* L'interface mobile ou de bureau utilisée pour interagir avec le réseau Bitcoin, vérifier votre solde de bitcoins, envoyer et recevoir des transactions, et les diffuser sur le réseau. Différents types de portefeuilles, ainsi que leurs avantages et inconvénients, seront décrits dans les prochaines sections.

#### Portefeuilles auto-gérés vs portefeuilles délégués

Avant de détailler les différents types de portefeuilles Bitcoin et leurs caractéristiques, faisons une distinction importante entre les portefeuilles auto-gérés et les portefeuilles délégués. Chaque type a ses propres avantages, risques et niveau de contrôle sur les bitcoins. Auto-géré signifie que l'utilisateur détient les clés privées et contrôle réellement ses bitcoins ; avec un portefeuille délégué, un tiers détient les bitcoins pour l'utilisateur.


| Type | Contrôle | Avantages | Risques |
| --- | --- | --- | --- |
| Auto-géré | L'utilisateur | Contrôle total sur les fonds et les transactions, pas de processus d'approbation ni de gel de compte, aucun contrôle d'entreprise ou gouvernemental, protégé contre la confiscation. | Aucune récupération possible si la phrase de récupération est perdue, toute la responsabilité repose sur l'utilisateur. |
| Délégué | Le prestataire tiers | Récupération facile en cas de perte d'accès, assistance client facilitée. | Les fonds sont connectés à Internet, plus vulnérables au piratage. Le dépositaire peut geler les comptes. |


Dans un portefeuille auto-géré (aussi appelé portefeuille non-déposé), vous êtes le seul à posséder les clés du portefeuille et vous avez un contrôle total sur ce qui entre et sort. À l'inverse, dans un portefeuille délégué, quelqu'un d'autre détient la clé privée, ce qui lui donne un accès complet pour déplacer tous les bitcoins que ce prestataire contrôle en votre nom.

* L'auto-garde, c'est comme être sa propre banque. Les transactions ne sont pas soumises à la surveillance et au contrôle
* L'auto-garde garantit qu'aucun tiers ne peut confisquer vos bitcoins.
* L'auto-garde procure une tranquillité d'esprit en période d'incertitude, car vous savez que vos bitcoins sont en sécurité.

Il est important de choisir le bon type de portefeuille selon les besoins de chacun. Parfois, il est difficile de distinguer si l'on installe un portefeuille auto-géré ou délégué. Ce tableau montre les différences dans le processus d'installation.


| Type | Étape 1 : Choisir | Étape 2 : Installer | Étape 3 : Créer | Étape 4 : Sécuriser |
| --- | --- | --- | --- | --- |
| Auto-géré | Choisir un portefeuille auto-géré | Suivre les instructions du portefeuille | Générer une phrase de récupération | Conserver la phrase de récupération dans un endroit sûr |
| Délégué | Choisir un portefeuille délégué | Suivre les instructions du portefeuille | Créer un compte | N/A |


«**Pas vos clés, pas vos bitcoins** » est un dicton populaire parmi les détenteurs de bitcoins. Il fait référence à l'idée que si vous n'avez pas le contrôle direct des clés privées associées à votre portefeuille Bitcoin, vous ne possédez pas réellement vos bitcoins.

Quiconque accède à vos clés privées possède vos bitcoins. C'est pourquoi il est primordial de les protéger en les gardant à l'abri des regards indiscrets ! Nous verrons plus loin dans le livre quelques moyens de le faire.

Pour la suite, nous ne parlerons que des portefeuilles auto-gérés, où l'utilisateur possède ses clés et a un contrôle total sur ses bitcoins.

Ne vous inquiétez pas si cela vous semble compliqué ou si vous ne comprenez pas tout — c'est un parcours, et vous comprendrez mieux à mesure que vous commencerez à utiliser Bitcoin !

#### Différents types de portefeuilles Bitcoin

L'endroit où votre clé privée est créée et stockée détermine la façon dont nous décrivons les portefeuilles Bitcoin. Si les clés sont sur votre smartphone, il s'agit d'un **portefeuille mobile**. S’ils sont stockés en toute sécurité sur un appareil dédié, il s’agit d’un **portefeuille matériel**.


| Type | Description | Avantages | Inconvénients | Exemple d’utilisateur |
| --- | --- | --- | --- | --- |
| Portefeuille en ligne | Accessible via un navigateur web | Accessible depuis n’importe quel appareil connecté à Internet | Moins sécurisé car il peut être piraté ou compromis | A besoin d’accéder fréquemment à son portefeuille et n’a pas beaucoup de fonds à stocker |
| Portefeuille mobile | Installé sur un appareil mobile | Facile à utiliser | Peut être perdu si l’appareil est volé ou piraté | A besoin de faire des transactions en déplacement et n’a pas beaucoup de fonds à stocker |
| Portefeuille de bureau | Installé sur un ordinateur de bureau | Pratique et accessible de partout | Peut être piraté si l’ordinateur est infecté par un logiciel malveillant | Souhaite stocker une grande quantité de bitcoins et est à l’aise avec l’utilisation d’un ordinateur de bureau |
| Portefeuille matériel | Un appareil physique qui stocke les bitcoins hors ligne | Plus sécurisé que les portefeuilles en ligne et peut être utilisé hors ligne | Les fonds pourraient être irrécupérables | Souhaite stocker une grande quantité de bitcoins et est prêt à payer pour une sécurité accrue |


Comme les clés peuvent être déplacées d’un appareil à un autre, le « statut » de votre portefeuille Bitcoin n’est pas fixe. Par exemple, si je crée mes clés de portefeuille sur un ordinateur et que je les transfère ensuite sur mon téléphone, le « portefeuille de bureau » devient un « portefeuille mobile ».

En matière de stockage de vos bitcoins, il ne s’agit pas seulement de savoir qui contrôle les clés — de nombreux autres risques sont à prendre en compte. C’est pourquoi il est important de trouver une solution de stockage à la fois sûre et pratique. En analysant les compromis des différents types de portefeuilles, vous apprendrez qu’il n’existe pas de portefeuille idéal pour satisfaire tous les besoins.

##### À prendre en compte lors du choix d’un portefeuille

* **Sécurité** : Assurez-vous que le portefeuille dispose de solides mesures de sécurité.
* **Vie privée** : Vérifiez si le portefeuille exige des informations personnelles.
* **Facilité d’utilisation** : Choisissez un portefeuille facile à utiliser et à naviguer.
* **Compatibilité** : Assurez-vous que le portefeuille est compatible avec votre appareil.
* **Frais** : Comparez les frais facturés par différents portefeuilles.
* **Réputation** : Vérifiez la réputation des développeurs pour vous assurer qu’ils sont dignes de confiance.
* **Contrôle** : Certains portefeuilles vous donnent plus de contrôle sur vos clés privées.

##### Open Source vs Source Fermée

Un autre facteur important à garder à l’esprit lors du choix d’un portefeuille Bitcoin est de savoir si l’application ou le logiciel est open source. C’est important car les projets open source permettent à la communauté de revoir le code et de poursuivre le projet si l’équipe arrête de travailler dessus. Tout comme le code de Bitcoin est entièrement ouvert à tous pour être examiné, utilisé et modifié, il en va de même pour le code du portefeuille que vous utilisez pour gérer vos bitcoins.

#### Activité : Discussion et évaluation des portefeuilles Bitcoin

https://bitcoin.org/en/choose-your-wallet

Rendez-vous sur le site suivant : [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Utilisez vos nouvelles connaissances sur les portefeuilles Bitcoin pour choisir celui qui convient le mieux à vos besoins selon les critères que nous avons abordés aujourd'hui.
