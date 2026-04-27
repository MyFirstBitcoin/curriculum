# 7.4 Envoi et réception de transactions Lightning

Avec un portefeuille Lightning, utiliser Bitcoin est rapide, peu coûteux et privé, ce qui rend les transactions entre deux personnes faciles. Vous pouvez envoyer et recevoir du bitcoin rapidement pour des achats quotidiens comme acheter un café.

Voyons quelques exemples du Lightning Network en action.

###### Exemple 1

Marcia et Eve ont toutes les deux 5 unités de monnaie. Marcia veut envoyer 2 unités à Eve. Le paiement passe par Jeff, qui aide à faire transiter le paiement sur le Lightning Network. Une fois le paiement effectué, Eve a 7 unités et Marcia en a 3.

Jeff aide à acheminer le paiement, mais il ne peut pas voler les fonds. Le Lightning Network utilise la cryptographie pour garantir que seul le destinataire prévu peut recevoir le paiement. Jeff aide simplement le paiement à circuler sur le réseau.

Cela montre un avantage clé du Lightning Network : les gens peuvent envoyer des paiements rapidement sans avoir à faire confiance à des intermédiaires comme les banques.

Les opérateurs de nœuds comme Jeff peuvent aussi gagner de petits frais en aidant à acheminer les paiements. Ce faisant, ils contribuent à maintenir le réseau décentralisé et efficace.

Comparé aux transactions Bitcoin classiques :

* **Les transactions sur la chaîne** se passent directement sur la blockchain Bitcoin. Elles sont très sécurisées mais peuvent être plus lentes et plus coûteuses.
* **Les transactions Lightning** se passent hors chaîne et permettent aux paiements de circuler beaucoup plus rapidement et à un coût bien moindre.

Pour cette raison, Lightning est utile pour les petits paiements quotidiens, tandis que les transactions sur la chaîne sont souvent utilisées pour des transferts plus importants ou le stockage à long terme.

###### Exemple 2

Mina adore manger à l'extérieur et s'arrête souvent dans son café local préféré. Avec autant d'options de paiement différentes, elle ne sait pas laquelle est le meilleur choix. Heureusement, elle a appris un peu sur Bitcoin et le Lightning Network. Après avoir examiné ses options, Mina se rend compte qu'utiliser un moyen de paiement Lightning est la meilleure solution.

Mina veut acheter un café, mais payer avec une transaction Bitcoin classique peut parfois prendre du temps et nécessiter des frais plus élevés. Elle décide donc d'utiliser le Lightning Network.

Le Lightning Network permet d'envoyer du bitcoin instantanément et avec des frais très faibles. Cela le rend idéal pour les petits achats quotidiens comme le café.

Pour commencer à utiliser Lightning, Mina télécharge un portefeuille Lightning sur son téléphone. Elle envoie ensuite du bitcoin depuis son portefeuille Bitcoin classique vers son portefeuille Lightning. Cette étape utilise une transaction Bitcoin normale sur la blockchain. Une fois les fonds dans son portefeuille Lightning, ils peuvent être utilisés sur le Lightning Network.

Maintenant, Mina peut payer le café instantanément grâce à Lightning. Le paiement se fait hors de la blockchain principale de Bitcoin, ce qui explique pourquoi il est beaucoup plus rapide et moins cher qu'une transaction classique sur la chaîne.


| Avantages | Lightning Network | Système bancaire traditionnel |
| --- | --- | --- |
| Vitesse | Rapide | Lent |
| Transparence | Transparent | Opaque |
| Sécurité | Sécurisé | Vulnérable |
| Frais de transaction | Faibles | Élevés |
| Inclusion financière | Élevée | Limitée |
| Scalabilité | Élevée | Faible |
| Confidentialité | Élevée | Modérée |
| Interopérabilité | Élevée | Faible |
| Conformité légale | Modérée | Élevée |
| Rentabilité | Élevé | Modéré |


Les transactions on-chain ont lieu directement sur la blockchain Bitcoin et peuvent prendre plus de temps et entraîner des frais plus élevés. Les transactions Lightning se font hors chaîne, permettant des paiements rapides et à faible coût tout en utilisant le bitcoin.


| Visa, Inc. | Bitcoin On-chain | Réseau Lightning |
| --- | --- | --- |
| Capacité de 65 000 transactions par seconde. | Capacité de 7 transactions par seconde. | Capacité de millions de transactions par seconde. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Voici une carte de l'ensemble du Réseau Lightning. Grâce à des milliers d'opérateurs de nœuds Lightning, vous pouvez envoyer des sats à n'importe quel utilisateur disposant d'un portefeuille Bitcoin Lightning, où qu'il soit dans le monde. Le paiement arrivera en quelques secondes et ne coûtera que quelques centimes.**Essayez par vous-même !**

#### Activité : Relais Lightning

https://qr.myfirstbitcoin.org/lightning.pdf

**Il s'agit d'un exercice pratique où les élèves envoient et reçoivent de vrais sats en utilisant le Réseau Lightning.**

###### Points clés

1. Utiliser un portefeuille Lightning renforcera votre confiance pour recevoir et envoyer de vrais sats.
1. Faites attention aux unités. Certains portefeuilles permettent aux utilisateurs d'envoyer des bitcoins OU des sats (1/100 000 000 d'un bitcoin).
1. Les paiements Lightning peuvent parfois être bloqués lors du routage, surtout pour les paiements importants. Bien que cela soit possible, ce type d'expérience utilisateur devient de moins en moins courant à mesure que le réseau mûrit.

###### Astuce pour les étudiants

Vérifiez auprès de votre instructeur si et comment les frais de transaction Bitcoin on-chain actuels affecteront le portefeuille Lightning spécifique que vous utilisez.
