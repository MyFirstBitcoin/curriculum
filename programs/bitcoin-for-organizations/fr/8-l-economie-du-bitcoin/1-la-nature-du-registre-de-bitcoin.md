# 8.1 La nature du registre de Bitcoin

Le registre des transactions de Bitcoin (égallement appelé timechain ou blockchain) est un enregistrement public, horodaté, de chaque transaction valide ayant jamais eu lieu sur le réseau. Dans le système financier traditionnel, les transactions internes ne sont visibles que par les participants autorisés, tels que les banques, les régulateurs ou des opérateurs de données comme SWIFT, BACS ou SEPA. L'accès aux données de paiement dans les systèmes traditionnels peut être très restreint et coûteux.

En revanche, sur le réseau Bitcoin, toute personne disposant d'une connexion Internet peut consulter chaque transaction, de la plus grande valeur jusqu'au Satoshi individuel. Les participants peuvent suivre l'offre totale de bitcoins en temps réel, surveiller l'activité des adresses et des portefeuilles, et consulter les récompenses des mineurs ainsi que le comportement des frais. Bien que l'activité visible sur le registre soit liée à des adresses de clés publiques et non à des identités individuelles, il est possible d'agréger de grands ensembles de données sur les comportements de dépense, permettant à chacun de compiler et d'étudier l'activité économique en temps réel. À mesure que le réseau se développe et devient plus accepté comme source de vérité économique, nous pourrions voir une moindre dépendance envers les organismes gouvernementaux et les prestataires tiers pour la production d'analyses statistiques et de rapports sur les comportements de dépense.



#### 8.1.1 Nœuds et explorateurs de blocs

Toute personne souhaitant vérifier de manière indépendante le registre Bitcoin et accéder à ses données devrait exécuter un nœud complet. Le nœud complet est souvent décrit comme la manière la plus fondamentale de participer à l'économie Bitcoin et de la vérifier. Il est disponible mondialement en tant que logiciel open-source qui, une fois exécuté, télécharge et valide l'intégralité du registre Bitcoin depuis le « Bloc Genesis », publié en janvier 2009, jusqu'à aujourd'hui. Il contribue également à la sécurité du réseau Bitcoin en aidant à vérifier les nouvelles transactions ajoutées au registre. En accédant au registre Bitcoin de cette manière, le nœud complet sert de source de vérité pour les chercheurs et les auditeurs du réseau. Et, pour les utilisateurs de Bitcoin, le nœud complet agit comme une passerelle « auto-souveraine » vers l'information transactionnelle de l'économie Bitcoin, car il améliore la confidentialité et la sécurité en supprimant la dépendance aux services tiers.

Alors que les nœuds complets téléchargent les données brutes, les explorateurs de blocs tels que mempool.space ou blockstream.info offrent une interface visuelle pour rechercher et interpréter l'activité du registre. L'explorateur de blocs permet de suivre des transactions individuelles et de consulter les soldes et historiques des portefeuilles. Il affiche également des métriques sur l'activité des mineurs, telles que les récompenses de blocs et les données sur les frais de transaction.

Ensemble, les nœuds complets et les explorateurs de blocs sont les outils qui rendent la transparence du réseau Bitcoin exploitable.



#### 8.1.2 Activité : Explorer le registre Bitcoin

1. Ouvrez [mempool.space](https://mempool.space) et explorez la page d'accueil.
  * Quel est le dernier numéro de bloc (block height) ?
  * Quel est le montant actuel des frais de transaction (Priorité basse, moyenne et haute) ?
  * Combien de transactions attendent dans le mempool pour le prochain bloc ?
1. Accédez au dernier bloc du registre.
  * Combien de transactions ont été incluses ?
  * Nommez le mineur du bloc.
  * Quelle était la récompense du bloc ?
1. Accédez à une transaction dans le bloc.
  * Combien d'entrées et de sorties la transaction possède-t-elle ?
  * Quelle est la valeur de la transaction en BTC et en USD ?

Discutez des différences entre la façon dont l'argent circule dans le système traditionnel et la manière dont une entreprise ou un gouvernement utilise ce type de transparence.
