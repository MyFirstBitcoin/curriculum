# 7.4 Envoi et réception de transactions Lightning

Avec un portefeuille Lightning, l'utilisation du Bitcoin est rapide, peu coûteuse et confidentielle, ce qui facilite les transactions entre deux personnes. Vous pouvez rapidement envoyer et recevoir des bitcoins pour des dépenses quotidiennes, comme l'achat d'un café.

Voyons quelques exemples concrets d'utilisation du Lightning Network.

###### Exemple 1

Marcia et Eve disposent toutes deux de 5 unités de monnaie. Marcia souhaite envoyer 2 unités à Eve. Le paiement transite par Jeff, qui aide à acheminer le paiement via le Lightning Network. Une fois le paiement effectué, Eve dispose de 7 unités et Marcia de 3.

Jeff facilite l'acheminement du paiement, mais il ne peut pas détourner les fonds. Le Lightning Network utilise la cryptographie pour garantir que seul le destinataire prévu puisse recevoir le paiement. Jeff se contente de faciliter le transit du paiement sur le réseau.

Cela met en évidence l'un des principaux avantages du Lightning Network : les utilisateurs peuvent effectuer des paiements rapidement sans avoir à faire confiance à des intermédiaires tels que les banques.

Les opérateurs de nœuds comme Jeff peuvent également percevoir de modestes commissions pour leur contribution à l'acheminement des paiements. Ce faisant, ils contribuent à préserver la décentralisation et l'efficacité du réseau.

Par rapport aux transactions Bitcoin classiques :

* **Transactions sur la chaîne** se déroulent directement sur la blockchain Bitcoin. Elles sont très sécurisées, mais peuvent s'avérer plus lentes et plus coûteuses.
* **Transactions éclair** se déroulent hors chaîne et permettent d'effectuer des paiements beaucoup plus rapidement et à un coût bien moindre.

C'est pourquoi Lightning est pratique pour les petits paiements quotidiens, tandis que les transactions sur la chaîne sont souvent utilisées pour les virements plus importants ou le stockage à long terme.

###### Exemple 2

Mina adore manger à l'extérieur et passe souvent par son café préféré du quartier. Face à la multitude d'options de paiement disponibles, elle ne sait pas vraiment laquelle choisir. Heureusement, elle s'est un peu renseignée sur le Bitcoin et le Lightning Network. Après avoir passé en revue les différentes possibilités, Mina se rend compte que le paiement via le Lightning Network est la meilleure solution.

Mina souhaite acheter un café, mais payer via une transaction Bitcoin classique peut parfois prendre du temps et entraîner des frais plus élevés. Elle décide donc d'utiliser le Lightning Network.

Le Lightning Network permet d'envoyer des bitcoins instantanément et moyennant des frais très faibles. Il est donc idéal pour les petits achats quotidiens, comme un café.

Pour commencer à utiliser Lightning, Mina télécharge un portefeuille Lightning sur son téléphone. Elle transfère ensuite des bitcoins depuis son portefeuille Bitcoin habituel vers son portefeuille Lightning. Cette étape s'effectue via une transaction Bitcoin classique sur la blockchain. Une fois les fonds transférés dans son portefeuille Lightning, ils peuvent être utilisés sur le réseau Lightning.

Désormais, Mina peut régler sa note au café instantanément grâce à Lightning. Le paiement s'effectue en dehors de la blockchain principale de Bitcoin, ce qui explique pourquoi il est bien plus rapide et moins coûteux qu'une transaction classique sur la chaîne.


| Avantages | Lightning Network | Système bancaire traditionnel |
| --- | --- | --- |
| Vitesse | Rapide | Lent |
| Transparence | Transparent | Opaque |
| Sécurité | Sécurisé | Vulnérable |
| Frais de transaction | Faible | Élevé |
| Inclusion financière | Élevé | Limité |
| Évolutivité | Élevé | Faible |
| Confidentialité | Élevé | Modéré |
| Interopérabilité | Élevé | Faible |
| Conformité réglementaire | Modéré | Élevé |
| Rapport coût-efficacité | Élevé | Modéré |


Les transactions « on-chain » s'effectuent directement sur la blockchain Bitcoin et peuvent prendre plus de temps et entraîner des frais plus élevés. Les transactions « Lightning » s'effectuent hors chaîne, ce qui permet d'effectuer des paiements rapides et peu coûteux tout en continuant à utiliser le bitcoin.


| Visa, Inc. | Bitcoin sur la chaîne de blocs | Lightning Network |
| --- | --- | --- |
| Capacité de 65 000 transactions par seconde. | Capacité de 7 transactions par seconde. | Capacité de plusieurs millions de transactions par seconde. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)


https://mempool.space/graphs/lightning/nodes-channels-map

_Mempool.space Nodes Channels Map_


Voici une carte représentant l'ensemble du Lightning Network. Grâce aux milliers d'exploitants de nœuds Lightning, vous pouvez envoyer des sats à n'importe quel utilisateur disposant d'un portefeuille Bitcoin Lightning, où qu'il se trouve dans le monde. Le paiement sera effectué en quelques secondes et ne coûtera que quelques centimes. **Jetez-y un œil par vous-même !**

#### Activité : Course de relais « éclair »


https://qr.myfirstbitcoin.org/lightning.pdf

_Activity: Lightning_


**Il s'agit d'un exercice pratique dans lequel les étudiants envoient et reçoivent de véritables sats via le Lightning Network.**

###### Points clés

1. L'utilisation d'un portefeuille Lightning vous permettra de gagner en confiance pour recevoir et envoyer de véritables sats.
1. Faites attention aux unités. Certains portefeuilles permettent aux utilisateurs d'envoyer des bitcoins OU des sats (1/100 000 000 de bitcoin).
1. Les paiements Lightning peuvent parfois être bloqués au niveau de l'acheminement, en particulier pour les montants importants. Bien que cela soit possible, ce type d'expérience utilisateur devient de moins en moins fréquent à mesure que le réseau gagne en maturité.

###### Conseil aux étudiants

Vérifiez auprès de votre formateur si et dans quelle mesure les frais de transaction Bitcoin actuels sur la chaîne auront une incidence sur le portefeuille Lightning que vous utilisez.
