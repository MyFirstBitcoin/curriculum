# 6.2 Introduction aux portefeuilles

Contrairement à l'argent physique, les bitcoins ne sont pas réellement stockés dans un portefeuille Bitcoin. Ils sont en réalité enregistrés dans le registre distribué que le réseau Bitcoin vérifie et sécurise en permanence. Alors, comment peut-on posséder des bitcoins ?

Vous n'êtes propriétaire de vos bitcoins que si vous contrôlez les clés privées qui vous permettent de signer des transactions et de transférer la propriété de vos bitcoins à quelqu'un d'autre. C'est ce qu'on appelle l'envoi de bitcoins.

Examinons deux concepts auxquels nous faisons référence lorsque nous utilisons ce terme **portefeuille**:

* Une clé privée principale, à l'instar d'un mot de passe, à partir de laquelle sont générées vos clés publiques, comparables à des adresses e-mail. Vous pouvez communiquer votre adresse publique à d'autres personnes pour recevoir et envoyer des bitcoins, mais vous ne devez en aucun cas divulguer votre clé privée !
* L'interface mobile ou de bureau permettant d'interagir avec le réseau Bitcoin, de consulter votre solde en bitcoins, d'envoyer et de recevoir des transactions, puis de les diffuser sur le réseau. Les différentes catégories de portefeuilles, ainsi que leurs avantages et leurs inconvénients, seront présentés dans les sections suivantes.

#### Portefeuilles en gestion autonome vs portefeuilles gérés par un tiers

Avant d’aborder en détail les différents types de portefeuilles Bitcoin et leurs caractéristiques, faisons une distinction importante entre les portefeuilles « auto-gérés » et les portefeuilles « gérés par un tiers ». Chaque type présente ses propres avantages, risques et niveau de contrôle sur les bitcoins. Le terme « auto-géré » signifie que l'utilisateur détient les clés privées et contrôle véritablement ses bitcoins ; avec les portefeuilles gérés par un tiers, c'est un tiers qui détient les bitcoins pour le compte de l'utilisateur.


| Type | Contrôle | Avantages | Risques |
| --- | --- | --- | --- |
| En gestion autonome | L'utilisateur | Contrôle total sur les fonds et les transactions, sans procédure d'autorisation ni gel de compte, sans contrôle d'entreprise ni des pouvoirs publics, à l'abri de toute confiscation. | En cas de perte de la phrase de récupération, aucune récupération n'est possible ; l'entière responsabilité incombe à l'utilisateur. |
| Entretien | Le prestataire tiers | Récupération aisée en cas de perte d'accès, assistance client simplifiée. | Les fonds sont connectés à Internet, ce qui les rend plus vulnérables au piratage. Le dépositaire peut bloquer les comptes. |


Dans un portefeuille auto-géré (également appelé « portefeuille non dépositaire »), vous êtes la seule personne à disposer des clés du portefeuille et vous avez le contrôle total sur les entrées et les sorties. En revanche, dans un portefeuille de garde, c'est une autre personne qui détient la clé privée, ce qui lui donne un accès total pour transférer tous les bitcoins que ce prestataire contrôle en votre nom.

* La gestion autonome, c'est un peu comme si vous étiez votre propre banque. Les transactions ne sont pas soumises à la surveillance ni au contrôle
* La conservation en propre garantit que des tiers ne peuvent pas saisir vos bitcoins.
* La conservation en propre offre une tranquillité d'esprit en période d'incertitude, car vous savez que vos bitcoins sont en sécurité.

Il est important de choisir le type de portefeuille adapté aux besoins de chacun. Il arrive parfois que les utilisateurs aient du mal à déterminer s'ils installent un portefeuille en gestion autonome ou un portefeuille en gestion déléguée. Ce tableau présente les différences entre les deux processus d'installation.


| Type | Étape 1 : Choisissez | Étape 2 : Installation | Étape 3 : Créer | Étape 4 : Sécuriser |
| --- | --- | --- | --- | --- |
| En gestion autonome | Choisissez un portefeuille en gestion autonome | Suivez les instructions fournies avec le portefeuille | Générer une phrase de récupération | Conservez la phrase de récupération dans un endroit sûr |
| Entretien | Choisissez un portefeuille avec service de garde | Suivez les instructions fournies avec le portefeuille | Créer un compte | N/A |


“**Si ce ne sont pas vos clés, ce ne sont pas vos pièces**« » est une expression courante chez les détenteurs de bitcoins. Elle fait référence à l'idée selon laquelle si vous n'avez pas le contrôle direct des clés privées associées à votre portefeuille Bitcoin, vous n'êtes pas véritablement propriétaire de ces bitcoins.

Quiconque a accès à vos clés privées est propriétaire de vos bitcoins. C’est pourquoi il est primordial de les protéger en les gardant à l’abri des regards indiscrets ! Nous verrons plus loin dans cet ouvrage quelques moyens d’y parvenir.

Dans la suite de cet article, nous ne parlerons que des portefeuilles en gestion autonome, dans lesquels l'utilisateur est propriétaire de ses clés et exerce un contrôle total sur ses bitcoins.

Ne t'inquiète pas si cela te semble compliqué ou si tu ne comprends pas tout : c'est un parcours, et tu y verras plus clair au fur et à mesure que tu commenceras à utiliser le Bitcoin !

#### Les différents types de portefeuilles Bitcoin

C'est l'endroit où votre clé privée est créée et stockée qui détermine la manière dont nous décrivons les portefeuilles Bitcoin. Si les clés se trouvent sur votre smartphone, il s'agit d'un **portefeuille mobile**. S'ils sont stockés en toute sécurité sur un appareil dédié, c'est un **portefeuille matériel**.


| Type | Description | Avantages | Inconvénients | Exemple d'utilisateur |
| --- | --- | --- | --- | --- |
| Portefeuille en ligne | Accessible via un navigateur web | Accessible depuis n'importe quel appareil disposant d'une connexion Internet | Moins sûr, car il peut être piraté ou compromis | Doit accéder fréquemment à son portefeuille et ne dispose pas de beaucoup de fonds à y conserver |
| Portefeuille mobile | Installé sur un appareil mobile | Facile à utiliser | Peut être perdu en cas de vol ou de piratage de l'appareil | A besoin d'effectuer des transactions lors de ses déplacements et ne dispose pas de beaucoup de fonds à conserver |
| Portefeuille de bureau | Installé sur un ordinateur de bureau | Pratique et accessible de n'importe où | Il peut être piraté si l'ordinateur est infecté par un logiciel malveillant | Souhaite stocker une grande quantité de bitcoins et est à l'aise avec l'utilisation d'un ordinateur de bureau |
| Portefeuille matériel | Un dispositif physique permettant de stocker des bitcoins hors ligne | Plus sûr que les portefeuilles en ligne et utilisable hors ligne | Les fonds pourraient être irrécupérables | Souhaite stocker une grande quantité de bitcoins et est prêt à payer pour bénéficier d'une sécurité renforcée |


Comme les clés peuvent être transférées d'un appareil à un autre, le « statut » de votre portefeuille Bitcoin n'est pas figé. Par exemple, si je crée les clés de mon portefeuille sur un ordinateur puis que je les transfère ensuite sur mon téléphone, le « portefeuille de bureau » devient un « portefeuille mobile ».

En matière de stockage de vos bitcoins, la question ne se résume pas à savoir qui détient le contrôle des clés : il existe de nombreux autres risques à prendre en compte. C’est pourquoi il est important de trouver une solution de stockage à la fois sécurisée et pratique. En analysant les avantages et les inconvénients des différents types de portefeuilles, vous vous rendrez compte qu'il n'existe pas de portefeuille idéal capable de répondre à tous les besoins.

##### Éléments à prendre en compte lors du choix d'un portefeuille

* **Sécurité**: Assurez-vous que le portefeuille dispose de mesures de sécurité efficaces.
* **Confidentialité**: Vérifiez si le portefeuille électronique demande des informations personnelles.
* **Facilité d'utilisation**: Choisissez un portefeuille facile à utiliser et à parcourir.
* **Compatibilité**: Assurez-vous que le portefeuille est compatible avec votre appareil.
* **Frais**: Comparez les frais pratiqués par différents portefeuilles.
* **Réputation**: Vérifiez la réputation des développeurs pour vous assurer qu'ils sont dignes de confiance.
* **Contrôle**: Certains portefeuilles vous offrent davantage de contrôle sur vos clés privées.

##### Logiciels libres contre logiciels propriétaires

Un autre facteur important à prendre en compte lors du choix d'un portefeuille Bitcoin est de vérifier si l'application ou le logiciel est open source. C'est important car les projets open source permettent à la communauté d'examiner le code et de poursuivre le projet si l'équipe cesse d'y travailler. Tout comme le code de Bitcoin est entièrement accessible à tous pour être examiné, utilisé et modifié, il devrait en être de même pour le code du portefeuille que vous utilisez pour gérer vos bitcoins.

#### Activité : Discussion et évaluation des portefeuilles Bitcoin


https://bitcoin.org/en/choose-your-wallet

_QR Code: Choose your wallet_


Rendez-vous sur le site web suivant : [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Mettez à profit vos nouvelles connaissances sur les portefeuilles Bitcoin pour choisir celui qui correspond le mieux à vos besoins, en vous basant sur les critères dont nous avons parlé aujourd’hui.
