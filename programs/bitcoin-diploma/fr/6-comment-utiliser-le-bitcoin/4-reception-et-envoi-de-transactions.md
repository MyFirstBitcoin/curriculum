# 6.4 Réception et envoi de transactions

Une transaction Bitcoin est un transfert de propriété de bitcoin vers un nouveau propriétaire. Notez qu’il ne s’agit pas des pièces elles-mêmes qui sont transférées, mais de leur propriété : en d’autres termes, le droit de les dépenser. Chaque fois qu’une transaction est acceptée dans un bloc, tous les nœuds du réseau mettent à jour leur copie locale du registre public pour refléter le changement de propriété. À cet égard, une transaction Bitcoin ressemble davantage à une transaction immobilière (ou autre bien) qu’à une transaction en espèces.

Pour « envoyer » des bitcoins, l’expéditeur signe un message avec sa clé privée, signalant au réseau que le propriétaire légitime du bitcoin a transféré sa propriété au destinataire.

Le bitcoin sera désormais lié à l’adresse du destinataire, lui conférant la propriété du bitcoin, de sorte que seul le nouveau propriétaire pourra les dépenser en utilisant sa clé privée.

De nouvelles transactions Bitcoin sont initiées depuis des portefeuilles partout dans le monde, mais il n’existe aucun processeur de paiement centralisé. À la place, les mineurs se concurrencent pour enregistrer les transactions dans le registre.

Supposons que Jim doive 0,5 BTC à Eliana et soit prêt à la rembourser. Tous deux possèdent des portefeuilles numériques.

1. Eliana partage son adresse avec Jim.
1. Jim utilise son logiciel de portefeuille pour créer la transaction, qui inclut l’adresse d’Eliana, le montant à transférer (0,5 BTC) et des frais pour le mineur. Des frais plus élevés augmentent la probabilité qu’un mineur inclue la transaction dans le prochain bloc.
1. Après avoir signé la transaction, celle-ci est diffusée sur le réseau, où elle est vérifiée par les nœuds. Ils vérifient si Jim dispose de fonds suffisants et s’il est bien le propriétaire légitime des pièces qu’il souhaite dépenser. S’il ne l’est pas, ils rejettent immédiatement la transaction.
1. Une fois la transaction vérifiée, les mineurs choisissent de l’ajouter ou non au prochain bloc, généralement en fonction des frais sélectionnés. Une fois la transaction incluse dans un bloc, elle est ajoutée à la blockchain et les fonds sont transférés à l’adresse d’Eliana.
1. La propriété a été transférée à Eliana. Elle peut désormais utiliser sa clé privée pour dépenser les fonds.

_Il est important de noter qu’une fois la transaction terminée, elle ne peut pas être annulée._


> **Note – Comment fonctionne une transaction Bitcoin**
>
> 1. Quelqu’un demande une transaction
> 1. Transaction diffusée aux ordinateurs P2P (nœuds)
> 1. Les mineurs vérifient la transaction
> 1. Les transactions sont regroupées pour former un bloc de données
> 1. Nouveau bloc ajouté à la blockchain existante
> 1. La transaction est terminée



> **Note – Recevoir des transactions Bitcoin**
>
> Pour recevoir des bitcoins, vous devrez fournir à l’expéditeur une adresse publique Bitcoin. Il s’agit d’une chaîne unique de lettres et de chiffres qui représente votre portefeuille et sert à l’identifier sur le réseau Bitcoin.
>
> Vous pouvez trouver votre adresse publique en ouvrant votre portefeuille Bitcoin et en cherchant une option « Recevoir » ou « Dépôt » de bitcoins.
>
> Vous pouvez ensuite partager votre adresse Bitcoin de plusieurs façons :
>
> 1. **Copier et coller l’adresse** : Vous pouvez copier l’adresse en la sélectionnant puis en appuyant sur « Copier », puis la coller dans un e-mail ou un message.
> 1. **Partager un lien vers votre portefeuille Bitcoin** : Certains portefeuilles Bitcoin vous permettent de créer un lien vers votre portefeuille que vous pouvez partager avec l’expéditeur. Il pourra alors cliquer sur le lien pour accéder à votre portefeuille et envoyer des bitcoins.
> 1. **Partager un code QR** : Si l’expéditeur possède un smartphone avec une application de portefeuille Bitcoin installée, il peut scanner le code QR pour obtenir votre adresse Bitcoin.


Une fois que l’expéditeur a votre adresse, il peut vous envoyer des bitcoins en saisissant votre adresse et le montant qu’il souhaite envoyer. Les bitcoins sont alors envoyés de son portefeuille vers le vôtre.

La transaction est confirmée par le réseau Bitcoin et prend généralement environ 10 minutes. Pour une sécurité accrue, il est recommandé d’attendre deux confirmations, ce qui prend environ 20 minutes.


> **Note – Envoyer des transactions Bitcoin**
>
> Pour envoyer des bitcoins, vous aurez besoin de quelques éléments : un portefeuille Bitcoin, l’adresse publique du destinataire et le montant de bitcoins que vous souhaitez envoyer.
>
> 1. Ouvrez votre portefeuille Bitcoin.
> 1. Accédez au bouton « Envoyer » et collez l’adresse du destinataire dans le champ « À ». Vous pouvez également scanner le code QR si le destinataire en fournit un.
> 1. Saisissez le montant de bitcoins que vous souhaitez envoyer dans le champ « Montant ».
> 1. Vérifiez attentivement l’adresse du destinataire et le montant à envoyer. Rappelez-vous que les transactions sont irréversibles !
> 1. Avant de cliquer sur « Confirmer et envoyer », nous vous recommandons de vérifier une dernière fois les détails de la transaction afin de vous assurer que vous envoyez le bon montant de bitcoins à la bonne adresse.
> 1. Diffusez la transaction et attendez que le réseau confirme la transaction.
>
> Vous savez maintenant comment évaluer, choisir et configurer un portefeuille Bitcoin en auto-garde. L’envoi et la réception de bitcoins sur le réseau Bitcoin sont appelés transactions « on-chain ». Cela signifie que les transactions ont lieu sur le réseau principal Bitcoin et sont enregistrées dans la blockchain.
>
> Les transactions on-chain sont le moyen le plus sûr de transacter avec des bitcoins grâce à la vérification décentralisée fournie par le réseau.
>
> Cependant, les transactions on-chain sont plus lentes et peuvent être nettement plus coûteuses que d’autres options (que nous aborderons dans le Module 7) en raison des frais de minage.


#### Activité : Les transactions en action

https://qr.myfirstbitcoin.org/transactions.pdf

**Il s’agit d’un exercice coopératif simplifiant les rôles de base des personnes impliquées dans une transaction Bitcoin.**

###### Points clés

1. Il existe quatre types de participants dans chaque transaction bitcoin : l’expéditeur, le destinataire, les mineurs et les opérateurs de nœuds.
1. L’expéditeur doit approuver (signer cryptographiquement) le **montant de bitcoins** à envoyer ET l’**adresse spécifique** à laquelle envoyer.
1. Le destinataire doit fournir **une adresse valide** à l'expéditeur ET vérifier que la transaction a bien été confirmée sur la blockchain.
1. Les mineurs s'assurent que tous les critères sont valides avant d'ajouter les transactions aux blocs futurs.
1. Les opérateurs de nœuds vérifient que les blocs minés sont valides avant de mettre à jour leur version de la blockchain (le registre).

###### Astuce pour les étudiants

Alternez entre les quatre rôles pour découvrir ce que fait chaque participant.
