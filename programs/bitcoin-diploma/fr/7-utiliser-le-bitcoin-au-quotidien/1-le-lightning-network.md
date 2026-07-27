# 7.1 Le Lightning Network

Le Lightning Network est un système de paiement qui permet aux utilisateurs d'envoyer et de recevoir des bitcoins rapidement et à moindre coût. Il fonctionne grâce à la création d’un portefeuille partagé dans lequel les deux parties stockent une partie de leurs bitcoins. Elles peuvent alors effectuer un nombre illimité de transactions entre elles sans avoir à enregistrer chacune d’entre elles sur la blockchain principale. Ce faisant, elles évitent d’avoir à vérifier et à inclure chaque transaction dans un bloc, ce qui rend le processus à la fois rapide et économique. Grâce à ces frais réduits, le Lightning Network peut être utilisé pour de petits paiements qui ne sont pas toujours viables sur la chaîne principale. Une fois que les parties décident de mettre fin à leur collaboration, seul le solde final est enregistré sur la blockchain.

Imaginez une journée de travail dans un café. Comme vous comptez rester un moment, vous ouvrez un compte et payez d’avance au lieu de régler chaque commande au fur et à mesure. À la fin de la journée, vous passez en revue le compte avec le propriétaire pour régler la note. Si votre dépôt est supérieur à ce que vous avez dépensé, on vous rembourse la différence ; si vous avez dépensé plus, vous payez ce qu’il vous reste à régler.

Ce système peut s'étendre pour inclure davantage de participants. Par exemple, lors d'une de vos visites au café, vous venez accompagné d'un ami que le barman ne connaît pas et pour lequel il ne peut pas ouvrir de compte. Vous proposez à vos amis d’utiliser votre compte ouvert pour régler leurs dépenses, et vous convenez qu’ils vous rembourseront en privé. Imaginez maintenant des milliers de personnes faisant la même chose simultanément, permettant ainsi à d’autres d’utiliser des comptes ouverts existants pour entrer en contact avec encore plus de personnes — cela démontre que le Lightning Network fonctionne !

Avec Lightning, vous pouvez effectuer des paiements à n'importe qui sur le réseau, et pas seulement à la personne avec laquelle vous partagez un compte commun — à condition qu'un chemin entre les deux parties puisse être trouvé. Votre paiement peut circuler à travers le réseau jusqu'à ce qu'il atteigne sa destination, même si vous ne disposez pas d'un canal ouvert directement avec le destinataire.

Voyons quelle est la différence entre les transactions « on-chain » et « off-chain ».

##### Transactions sur la chaîne

Il s'agit de transactions qui s'effectuent directement sur la blockchain Bitcoin. Leur confirmation prend environ 10 minutes, et les frais dépendent de la taille de la transaction, exprimée en octets virtuels. Elles sont plus sûres mais plus lentes, car elles nécessitent le consensus du réseau.

##### Transactions sur le Lightning Network

Ces transactions s'effectuent sur un réseau distinct, construit par-dessus la blockchain Bitcoin. Elles sont réglées plus rapidement et entraînent des frais moins élevés. Elles sont couramment utilisées lorsque des critères tels que la rapidité et le coût des transactions revêtent une importance particulière. Par rapport aux transactions sur la chaîne, elles sont moins sécurisées.


|  | Réseau Bitcoin | Lightning Network |
| --- | --- | --- |
| Définition | Un réseau numérique décentralisé qui utilise la cryptographie pour sécuriser les transactions financières. | Un protocole de paiement de deuxième couche fonctionnant sur la blockchain Bitcoin, permettant des transactions plus rapides et moins coûteuses. |
| Avantages | Décentralisé et sécurisé. Pas de rétrofacturation ni de fraude. Utilisation possible sous pseudonyme. Accepté dans le monde entier. | Des transactions plus rapides et moins coûteuses. Une évolutivité accrue. Les transactions hors chaîne n'encombrent pas la blockchain. |
| Inconvénients | Temps de traitement longs. Frais élevés pour certains types de transactions. Complexe pour les débutants. | Peut nécessiter une relation de confiance avec les opérateurs de canaux. Nécessite une transaction sur la chaîne pour ouvrir et fermer les canaux. |
