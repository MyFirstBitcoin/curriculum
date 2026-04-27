# 9.3 Comment fonctionnent les transactions

Maintenant que vous comprenez les clés publiques et privées, ainsi que les rôles des nœuds et des mineurs, voici comment fonctionne une transaction Bitcoin du début à la fin.

1. Adrien veut envoyer des bitcoins à Gérard. Il crée une transaction avec l’adresse de Gérard, le montant à envoyer et des frais.
1. Adrien signe la transaction avec sa clé privée pour prouver qu’il en est le propriétaire.
1. Il diffuse la transaction sur le réseau Bitcoin.
1. Les nœuds la reçoivent et vérifient qu’elle respecte les règles, notamment en contrôlant la signature et que Adrien possède assez de bitcoins.
1. Si elle est valide, la transaction est partagée sur le réseau et ajoutée au mempool, où les transactions en attente patientent.
1. Les mineurs sélectionnent des transactions dans le mempool et les incluent dans un bloc qu’ils essaient de miner.
1. Lorsqu’un mineur parvient à miner un bloc, il le partage avec le réseau et les autres nœuds le vérifient.
1. Si le bloc est valide, il est ajouté à la blockchain. Gérard reçoit les bitcoins.
1. À mesure que de nouveaux blocs sont ajoutés, la transaction reçoit des confirmations, ce qui la rend plus sécurisée.

Une fois incluse dans un bloc, la transaction est confirmée. Adrien ne peut plus dépenser ces bitcoins, et Gérard peut utiliser ce qu’il a reçu dans une nouvelle transaction.


> **Note**
>
> Transaction et frais sélectionnés → Signée par le portefeuille et envoyée → Distribuée par les nœuds → Le mineur ajoute la transaction au modèle de bloc → Le mineur remporte la preuve de travail → Nouveau bloc validé → Nouveau bloc distribué par les nœuds


###### Ressources


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
