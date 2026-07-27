# 6.4 Réception et envoi de transactions

Une transaction Bitcoin correspond à un transfert de propriété de bitcoins vers un nouveau propriétaire. Il convient de noter que ce ne sont pas les bitcoins eux-mêmes qui sont transférés, mais leur propriété : en d’autres termes, le droit de les dépenser. Chaque fois qu’une transaction est intégrée dans un bloc, tous les nœuds du réseau mettent à jour leur copie locale du registre public afin de refléter ce changement de propriété. À cet égard, une transaction Bitcoin s’apparente davantage à une transaction immobilière (ou à une autre transaction portant sur des biens) qu’à une transaction en espèces.

Pour « envoyer » des bitcoins, l'expéditeur signe un message avec sa clé privée, indiquant ainsi au réseau que le propriétaire légitime des bitcoins en a transféré la propriété au destinataire.

Le bitcoin sera désormais associé à l'adresse du destinataire, ce qui lui confère la propriété de ce bitcoin, de sorte que seul le nouveau propriétaire pourra le dépenser à l'aide de sa clé privée.

Les nouvelles transactions Bitcoin sont initiées à partir de portefeuilles situés partout dans le monde, mais il n'existe pas de système central de traitement des paiements. À la place, les mineurs se font concurrence pour enregistrer les transactions dans le registre.

Imaginons que Jim doive 0,5 BTC à Eliana et qu'il soit prêt à la rembourser. Tous deux possèdent un portefeuille numérique.

1. Eliana donne son adresse à Jim.
1. Jim utilise son logiciel de portefeuille pour créer la transaction, qui comprend l'adresse d'Eliana, le montant à transférer (0,5 BTC) et des frais destinés au mineur. Plus les frais sont élevés, plus il y a de chances qu'un mineur inclue la transaction dans le bloc suivant.
1. Une fois la transaction signée, elle est diffusée sur le réseau, où elle est vérifiée par les nœuds. Ceux-ci vérifient si Jim dispose de fonds suffisants et s'il est bien le propriétaire légitime des pièces qu'il souhaite dépenser. Si ce n'est pas le cas, ils rejettent immédiatement la transaction.
1. Une fois la transaction vérifiée, les mineurs décident s'ils souhaitent l'ajouter au bloc suivant, généralement en fonction des frais indiqués. Une fois que la transaction est intégrée à un bloc, elle est ajoutée à la blockchain et les fonds sont transférés vers l'adresse d'Eliana.
1. La propriété a été transférée à Eliana. Elle peut désormais utiliser sa clé privée pour disposer de ces fonds.

_Il est important de noter qu'une fois la transaction effectuée, elle ne peut plus être annulée._

###### Comment fonctionne une transaction Bitcoin ?

1. La transaction est diffusée sur le réseau
1. Les mineurs regroupent les transactions dans un bloc
1. Le bloc est ajouté à la blockchain
1. La transaction est confirmée


> **Light – Réception de transactions en bitcoins**
>
> Pour recevoir des bitcoins, vous devrez fournir à l'expéditeur une adresse publique Bitcoin. Il s'agit d'une chaîne unique de lettres et de chiffres qui correspond à votre portefeuille et qui sert à l'identifier sur le réseau Bitcoin.
>
> Pour trouver votre adresse publique, ouvrez votre portefeuille Bitcoin et recherchez l'option « Recevoir » ou « Déposer » des bitcoins.
>
> Vous pouvez ensuite communiquer votre adresse Bitcoin de plusieurs façons :
>
> 1. **Copiez et collez l'adresse**: Vous pouvez copier l'adresse en la sélectionnant puis en cliquant sur « Copier », avant de la coller dans un e-mail ou un message.
> 1. **Partagez le lien vers votre portefeuille Bitcoin**: Certains portefeuilles Bitcoin vous permettent de créer un lien vers votre portefeuille que vous pouvez partager avec l'expéditeur. Celui-ci peut alors cliquer sur ce lien pour accéder à votre portefeuille et vous envoyer des bitcoins.
> 1. **Partager un code QR**: Si l'expéditeur dispose d'un smartphone sur lequel est installée une application de portefeuille Bitcoin, il peut scanner le code QR pour obtenir votre adresse Bitcoin.


Une fois que l'expéditeur dispose de votre adresse, il peut vous envoyer des bitcoins en saisissant votre adresse et le montant qu'il souhaite vous envoyer. Les bitcoins sont alors transférés de son portefeuille vers le vôtre.

La transaction est validée par le réseau Bitcoin, ce qui prend généralement environ 10 minutes. Pour plus de sécurité, il est recommandé d'attendre deux confirmations, ce qui prend environ 20 minutes.


> **Light – Envoi de transactions Bitcoin**
>
> Pour envoyer des bitcoins, vous aurez besoin de plusieurs éléments : un portefeuille Bitcoin, l'adresse publique du destinataire et le montant en bitcoins que vous souhaitez envoyer.
>
> 1. Ouvrez votre portefeuille Bitcoin.
> 1. Cliquez sur le bouton « Envoyer » et collez l'adresse du destinataire dans le champ « À ». Vous pouvez également scanner le code QR si le destinataire en fournit un.
> 1. Saisissez le montant en bitcoins que vous souhaitez envoyer dans le champ « Montant ».
> 1. Vérifiez bien l'adresse du destinataire et le montant à envoyer. N'oubliez pas que les transactions sont irréversibles !
> 1. Avant de cliquer sur « Confirmer et envoyer », nous vous recommandons de vérifier une dernière fois les détails de la transaction afin de vous assurer que vous envoyez bien le montant correct de bitcoins à la bonne adresse.
> 1. Diffusez la transaction et attendez que le réseau la confirme.
>
> Vous savez désormais comment évaluer, choisir et configurer un portefeuille Bitcoin en gestion autonome. L'envoi et la réception de bitcoins sur le réseau Bitcoin sont appelés « transactions on-chain ». En effet, ces transactions ont lieu sur le réseau principal de Bitcoin et sont enregistrées dans la blockchain.
>
> Les transactions sur la chaîne constituent le moyen le plus sûr d'effectuer des transactions en bitcoins grâce à la vérification décentralisée assurée par le réseau.
>
> Cependant, les transactions sur la chaîne sont plus lentes et peuvent s'avérer nettement plus coûteuses que d'autres options (que nous aborderons dans le module 7) en raison des frais de minage.


#### Activité : Les transactions en pratique


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Il s'agit d'un exercice collaboratif visant à simplifier les rôles fondamentaux des personnes impliquées dans une transaction Bitcoin.**

###### Points clés

1. Chaque transaction Bitcoin implique quatre types d'acteurs : l'expéditeur, le destinataire, les mineurs et les opérateurs de nœuds.
1. L'expéditeur doit valider (signer cryptographiquement) le **montant en bitcoins** pour envoyer ET le **adresse précise** à qui l'envoyer.
1. Le destinataire doit fournir un **adresse valide** à l'expéditeur ET vérifier que la transaction a bien été validée sur la blockchain.
1. Les mineurs s'assurent que tous les critères sont respectés avant d'ajouter des transactions aux futurs blocs.
1. Les opérateurs de nœuds vérifient que les blocs minés sont valides avant de mettre à jour leur version de la blockchain (le registre).

###### Conseil aux étudiants

Alternez entre les quatre rôles afin de découvrir ce que fait chaque participant.
