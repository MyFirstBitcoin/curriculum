# 7.1 Le Réseau Lightning

Le Lightning Network est un système de paiement qui permet aux utilisateurs d’envoyer et de recevoir des bitcoins rapidement et à moindre coût. Il fonctionne en mettant en place un portefeuille partagé où les deux parties déposent une partie de leurs bitcoins. Elles peuvent ensuite effectuer un nombre illimité de transactions entre elles sans avoir besoin d’enregistrer chacune d’elles sur la blockchain principale. Ce faisant, elles évitent la nécessité de vérifier et d’inclure chaque transaction dans un bloc, ce qui rend le processus à la fois rapide et économique. Les frais réduits signifient que le Lightning Network peut être utilisé pour de petits paiements qui ne sont pas toujours viables sur la chaîne principale. Une fois que les parties décident de mettre fin à leur collaboration, seul le solde final est enregistré sur la blockchain.

Imaginez une journée de travail dans un café. Prévoyant de rester un moment, vous ouvrez une note et payez à l’avance au lieu de régler chaque commande séparément. À la fin de la journée, vous et le propriétaire vérifiez la note pour régler l’addition. Si votre dépôt dépasse ce que vous avez dépensé, vous récupérez la différence ; si vous avez dépensé plus, vous payez ce que vous devez encore.

Ce système peut s’étendre pour inclure plus de participants. Par exemple, lors d’une de vos visites au café, vous venez avec un ami que le barman ne connaît pas et à qui il ne peut pas ouvrir de note. Vous proposez à votre ami d’utiliser votre note existante pour couvrir ses dépenses, et vous convenez qu’il vous remboursera en privé. Imaginez maintenant des milliers de personnes faisant la même chose en même temps, permettant à d’autres d’utiliser des notes existantes pour se connecter avec encore plus d’individus — c’est ainsi que fonctionne le Lightning Network !

Avec Lightning, vous pouvez effectuer des paiements à n’importe qui sur le réseau, pas seulement à la personne avec qui vous partagez une note directe — à condition qu’un chemin entre les deux parties puisse être trouvé. Votre paiement peut parcourir le réseau jusqu’à atteindre sa destination, même si vous n’avez pas de canal ouvert directement avec le destinataire.

Voyons la différence entre les transactions sur chaîne et hors chaîne.

##### Transactions sur chaîne

Ce sont des transactions qui ont lieu directement sur la blockchain Bitcoin. Elles prennent environ 10 minutes pour être confirmées, et les frais dépendent de la taille de la transaction en octets virtuels. Elles sont plus sécurisées mais plus lentes, car elles nécessitent le consensus du réseau.

##### Transactions sur le Lightning Network

Ces transactions ont lieu sur un réseau séparé construit au-dessus de la blockchain Bitcoin. Elles se règlent plus rapidement et avec des frais plus faibles. Elles sont couramment utilisées lorsque la rapidité et le coût des transactions sont des critères importants. Comparées aux transactions sur chaîne, elles sont moins sécurisées.


|  | Réseau Bitcoin | Lightning Network |
| --- | --- | --- |
| Définition | Un réseau numérique décentralisé qui utilise la cryptographie pour sécuriser les transactions financières. | Un protocole de paiement de seconde couche qui fonctionne au-dessus de la blockchain Bitcoin, permettant des transactions plus rapides et moins coûteuses. |
| Avantages | Décentralisé et sécurisé. Pas de rétrofacturation ni de fraude. Peut être utilisé de manière pseudonyme. Acceptation mondiale. | Transactions plus rapides et moins chères. Scalabilité accrue. Les transactions hors chaîne ne saturent pas la blockchain. |
| Inconvénients | Temps de transaction lents. Frais élevés pour certains types de transactions. Complexe pour les débutants. | Peut nécessiter de faire confiance aux opérateurs de canaux. Nécessite une transaction sur chaîne pour ouvrir et fermer les canaux. |
