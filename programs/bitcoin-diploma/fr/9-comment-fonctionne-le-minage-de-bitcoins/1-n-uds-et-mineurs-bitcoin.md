# 9.1 Nœuds et mineurs Bitcoin

Qu'est-ce qu'un nœud Bitcoin ?  
Le terme « nœud Bitcoin » peut sembler technique, mais il s'agit simplement d'un logiciel qui conserve une copie de la blockchain Bitcoin sur un ordinateur. La blockchain est un registre partagé de toutes les transactions Bitcoin.

Lorsque vous exploitez votre propre nœud, vous vérifiez vous-même les transactions Bitcoin au lieu de vous fier à quelqu'un d'autre. Cela vous offre davantage d'indépendance et contribue à préserver la décentralisation du réseau Bitcoin.

On peut comparer un nœud Bitcoin à un agent de circulation numérique chargé de plusieurs missions importantes.

1. Il conserve une copie de la blockchain, qui retrace l'historique de toutes les transactions en bitcoins.
1. Les nœuds se connectent à d'autres nœuds partout dans le monde et échangent des informations. Citons par exemple la liste des nouvelles transactions en attente de confirmation, appelée « mempool ».
1. Les nœuds vérifient que chaque transaction respecte les règles de Bitcoin. Si une transaction n'est pas valide, le nœud la rejette.

Les nœuds aident également les nouveaux nœuds à rejoindre le réseau en partageant la blockchain avec eux. Cependant, chaque nouveau nœud vérifie tout de même toutes les règles de manière indépendante.

Tout le monde peut faire fonctionner un nœud en installant un logiciel tel que Bitcoin Core et en téléchargeant la blockchain. Une fois configuré, le nœud continue de recevoir de nouveaux blocs toutes les 10 minutes environ et les vérifie avant de les ajouter à sa copie de la blockchain.

L'exploitation d'un nœud contribue à renforcer la sécurité et la décentralisation du réseau Bitcoin, car davantage de personnes vérifient le système de manière indépendante.

#### Qu'est-ce qu'un mineur de bitcoins ?

> Le but du minage n'est pas la création de nouveaux bitcoins ; il s'agit là du système d'incitation. Le minage est le mécanisme grâce auquel la sécurité du Bitcoin est décentralisée.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Les mineurs collectent les transactions non confirmées, forment un bloc et utilisent de l'énergie pour trouver une clé qui permet d'ajouter ce bloc et de le sécuriser.


Les mineurs rivalisent pour ajouter le prochain bloc de transactions à la blockchain. Pour ce faire, ils doivent trouver un nombre spécifique permettant de générer un hachage de bloc valide. On peut comparer cela à la recherche de la bonne clé parmi des milliards de possibilités. Le premier mineur à trouver le bon hachage remporte la course et obtient le droit d'ajouter son bloc à la blockchain.

Lorsqu'un mineur trouve un hachage valide, il partage son bloc avec le réseau. Les autres mineurs vérifient rapidement que la solution est correcte. Si c'est le cas, le bloc est ajouté à la blockchain, ce qui contribue à assurer la sécurité du registre public de Bitcoin.

Les mineurs gagnent des bitcoins de deux façons :

* **Récompenses par bloc :** De nouveaux bitcoins sont créés et attribués au mineur qui parvient à ajouter un bloc à la blockchain.
* **Frais de transaction :** Lorsque les utilisateurs envoient des bitcoins, ils versent des frais minimes. Le mineur qui ajoute le bloc perçoit les frais liés aux transactions incluses dans ce bloc.

#### Réductions de moitié du Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Les récompenses versées aux mineurs pour la validation d'un bloc sont divisées par deux tous les 210 000 blocs, soit environ tous les quatre ans.


Le bitcoin a un plafond d'émission fixé à 21 000 000 bitcoins, mais ceux-ci n'ont pas tous été créés dès le lancement du bitcoin. En effet, de nouveaux bitcoins sont progressivement mis en circulation par le biais de **exploitation minière**.

Lorsque les mineurs parviennent à ajouter un nouveau bloc de transactions au réseau Bitcoin, ils reçoivent une **récompense par bloc** en bitcoins. Aux débuts du Bitcoin, cette récompense s'élevait à 50 bitcoins par bloc. Cette récompense incitait les utilisateurs à mettre à disposition leur puissance de calcul et leur électricité pour contribuer à la sécurité du réseau.

Tous les 210 000 blocs (soit environ tous les 4 ans), la récompense par bloc est divisée par deux. Cet événement s'appelle le **réduction de moitié**. La réduction de moitié ralentit la création de nouveaux bitcoins et contribue à garantir que l'offre totale ne dépassera jamais 21 millions. Au fil du temps, cela rend le bitcoin de plus en plus rare.


> **Definition – Offre en circulation**
>
> **Offre en circulation** désigne la quantité totale disponible d'une monnaie. Dans le cas du Bitcoin, l'offre totale en circulation correspond au nombre de pièces qui ont été minées et qui sont en circulation à un moment donné.



<!-- micrographic: bitcoin-supply-schedule -->



> **Definition – Calendrier de mise en circulation du Bitcoin**
>
> Le **Calendrier de mise en circulation du Bitcoin** Il s'agit du plan prédéfini et rendu public régissant la mise en circulation de nouveaux bitcoins, conçu pour préserver la rareté du bitcoin au fil du temps.


Après chaque « halving », la récompense en bitcoins que reçoivent les mineurs pour l'ajout d'un bloc est divisée par deux. Cela réduit le rythme de création de nouveaux bitcoins.

Les mineurs perçoivent toujours des frais de transaction sur les opérations incluses dans le bloc qu’ils minent. À terme, ces frais devraient représenter une part plus importante des revenus des mineurs.

Les « halvings » sont intégrés au protocole Bitcoin et se produisent automatiquement tous les quatre ans environ. De ce fait, le calendrier d'émission des bitcoins est prévisible et transparent.

Le tableau présente les prochaines réductions de moitié, en indiquant notamment la date approximative, le numéro de bloc auquel elles auront lieu, la nouvelle récompense par bloc, ainsi que le pourcentage de l'offre totale de bitcoins qui aura été minée.


| Événement | Date | Bloc | Récompense | Extrait |
| --- | --- | --- | --- | --- |
| 5e réduction de moitié | 2028 | 1 050 000 | 1,5625 BTC | 98,44 % |
| 6e réduction de moitié | 2032 | 1 260 000 | 0,78125 BTC | 99,22 % |
| 7e halving | 2036 | 1 470 000 | 0,390625 BTC | 99,61 % |


À mesure que de nouveaux bitcoins sont minés, l'offre en circulation ne cesse d'augmenter jusqu'à ce que l'offre maximale de 21 000 000 de bitcoins soit atteinte, ce qui devrait se produire vers l'an 2140. Étant donné que le nombre de nouveaux bitcoins créés diminue avec le temps, si la demande augmente, le cours du bitcoin peut s'apprécier. Cela incite également les mineurs à continuer de sécuriser le réseau en mettant à disposition leur puissance de calcul.

#### Qu'est-ce qu'un hachage de bloc valide dans Bitcoin ?

Les mineurs rivalisent pour trouver un code spécial appelé « **hachage de bloc**. Ce code identifie un bloc de transactions et permet de l'ajouter à la blockchain.

Chaque bloc contient des informations sur les transactions récentes et comprend également le hachage du bloc précédent. Cela permet de relier tous les blocs entre eux, formant ainsi une chaîne qui va du tout premier bloc (le bloc Genesis) au plus récent.

Un hachage fonctionne comme un **empreinte numérique** pour les données contenues dans le bloc. Si une information quelconque du bloc venait à être modifiée, l'empreinte numérique changerait également. Cela permet à quiconque de vérifier facilement que l'historique des transactions de la blockchain n'a pas été altéré et contribue à assurer la sécurité du réseau.


> **Callout**
>
> Satoshi Nakamoto, le créateur du Bitcoin, a miné le bloc Genesis, ce qui a permis de débloquer un total de 50 bitcoins.


#### La course à l'extraction d'un bloc

Les mineurs rivalisent pour trouver un hachage de bloc valide. Le premier mineur à en trouver un peut ajouter le nouveau bloc à la blockchain et reçoit une récompense en bitcoins.

Pour être valide, le hachage du bloc doit être inférieur à une valeur définie par le réseau, appelée « objectif de difficulté ». Les hachages étant aléatoires, les mineurs doivent tester différentes entrées jusqu’à ce qu’ils trouvent celle qui fonctionne.

Si le nombre de mineurs en concurrence est trop élevé, les blocs seraient trouvés trop rapidement. Si le nombre de mineurs participants est trop faible, la recherche des blocs prendrait trop de temps. Afin d'assurer le bon fonctionnement du système, Bitcoin ajuste automatiquement la difficulté tous les 2 016 blocs (soit environ toutes les deux semaines).

Cet ajustement garantit qu'en moyenne, un nouveau bloc est ajouté à la blockchain toutes les 10 minutes environ.


> **Definition – Définition du niveau de difficulté**
>
> Le **niveau de difficulté** Dans le minage de Bitcoin, la difficulté mesure le niveau de complexité requis pour trouver un hachage de bloc valide. Le réseau ajuste cette difficulté tous les 2 016 blocs (soit environ toutes les deux semaines) afin que de nouveaux blocs soient ajoutés à la blockchain toutes les 10 minutes environ. Plus la difficulté est élevée, plus il est difficile pour les mineurs de trouver un bloc valide.


En trouvant un hachage de bloc valide, un mineur prouve qu’il a effectué le travail nécessaire pour ajouter un nouveau bloc à la blockchain. Ce processus s’appelle **Preuve de travail** (PoW). Il s'agit du mécanisme de sécurité qui permet à Bitcoin de valider les transactions et d'ajouter de nouveaux blocs à la blockchain. Le mineur qui trouve en premier le hachage valide reçoit une récompense en bitcoins, qui comprend la récompense du bloc et les frais de transaction liés aux transactions incluses dans ce bloc.

La preuve de travail (PoW) contribue à la sécurité du Bitcoin en rendant extrêmement coûteuse toute tentative de tricherie ou de prise de contrôle du réseau. Il est en effet bien plus rentable de respecter les règles.

Les mineurs remplissent quatre rôles principaux :

1. **Collecter les transactions**: Les mineurs sélectionnent les transactions qui ont été envoyées au réseau et les intègrent dans un bloc candidat.
1. **Effectuer une preuve de travail**: Les mineurs s'affrontent pour résoudre une énigme mathématique complexe en trouvant un hachage de bloc valide.
1. **Diffuser le bloc**: Le premier mineur à trouver une solution valide diffuse le nouveau bloc sur le réseau.
1. **Gagnez des récompenses**: Si le bloc est valide, il est ajouté à la blockchain et le mineur reçoit des bitcoins nouvellement créés ainsi que les frais de transaction.

De nombreux mineurs à travers le monde tentent simultanément de créer le bloc suivant. Lorsqu’un mineur trouve une solution valide, le réseau vérifie le bloc. Si tout est correct, celui-ci est ajouté à la blockchain. Les autres blocs concurrents sont rejetés. Ce processus garantit la cohérence du réseau et empêche les doubles dépenses.

* Les « mineurs » sont des ordinateurs qui contribuent à la maintenance et à la mise à jour du registre Bitcoin.
* Ils collectent les transactions et les regroupent dans un bloc. Ils soumettent ensuite les données de ce bloc à un algorithme de hachage afin de générer un code unique appelé « hachage ».
* Les mineurs répètent ce processus à de nombreuses reprises, à la recherche d'un hachage conforme aux règles du Bitcoin. Le premier mineur à trouver un hachage valide reçoit en récompense des bitcoins nouvellement créés, et son bloc est ajouté à la blockchain.
* Le hachage de chaque bloc établit également un lien avec le bloc précédent. Si quelqu’un tentait de modifier une transaction antérieure, les hachages ne correspondraient plus, et le réseau rejetterait la chaîne altérée. C’est ce qui garantit la sécurité du registre de Bitcoin.
