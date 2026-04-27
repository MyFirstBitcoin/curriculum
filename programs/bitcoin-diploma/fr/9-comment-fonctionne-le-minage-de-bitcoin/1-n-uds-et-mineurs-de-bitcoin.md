# 9.1 Nœuds et mineurs de Bitcoin

Les nœuds Bitcoin peuvent sembler techniques, mais il s'agit simplement de logiciels qui conservent une copie de la blockchain Bitcoin sur un ordinateur. La blockchain est un registre partagé de toutes les transactions Bitcoin.

Lorsque vous faites fonctionner votre propre nœud, vous vérifiez vous-même les transactions Bitcoin au lieu de faire confiance à quelqu'un d'autre. Cela vous donne plus d'indépendance et contribue à maintenir le réseau Bitcoin décentralisé.

Vous pouvez considérer un nœud Bitcoin comme un agent de circulation numérique avec quelques missions importantes.

1. Il conserve une copie de la blockchain, qui est l'historique de toutes les transactions Bitcoin.
1. Les nœuds se connectent à d'autres nœuds dans le monde entier et partagent des informations. Un exemple est la liste des nouvelles transactions en attente de confirmation, appelée le mempool.
1. Les nœuds vérifient que chaque transaction respecte les règles de Bitcoin. Si une transaction est invalide, le nœud la rejette.

Les nœuds aident aussi les nouveaux nœuds à rejoindre le réseau en partageant la blockchain avec eux. Cependant, chaque nouveau nœud vérifie tout de même toutes les règles de manière indépendante.

N'importe qui peut faire fonctionner un nœud en installant un logiciel comme Bitcoin Core et en téléchargeant la blockchain. Une fois installé, le nœud continue de recevoir de nouveaux blocs environ toutes les 10 minutes et les vérifie avant de les ajouter à sa copie de la blockchain.

Faire fonctionner un nœud contribue à rendre le réseau Bitcoin plus sûr et plus décentralisé, car davantage de personnes vérifient le système de manière indépendante.

#### Qu'est-ce qu'un nœud Bitcoin ?

> Le but du minage n'est pas la création de nouveaux bitcoin ; c'est le système d'incitation. Le minage est le mécanisme par lequel la sécurité de Bitcoin est décentralisée.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Les mineurs collectent les transactions non confirmées, forment un bloc et utilisent de l'énergie pour trouver une clé qui ajoute et sécurise le bloc.


Les mineurs sont en compétition pour ajouter le prochain bloc de transactions à la blockchain. Pour cela, ils doivent trouver un nombre spécial qui crée un hash de bloc valide. Vous pouvez imaginer cela comme chercher la bonne clé parmi des milliards de possibilités. Le premier mineur à trouver le bon hash remporte la course et gagne le droit d'ajouter son bloc à la blockchain.

Lorsqu'un mineur trouve un hash valide, il partage son bloc avec le réseau. Les autres mineurs vérifient rapidement que la solution est correcte. Si c'est le cas, le bloc est ajouté à la blockchain, ce qui contribue à sécuriser le registre public de Bitcoin.

Les mineurs gagnent des bitcoin de deux façons :

* **Récompenses de bloc :** De nouveaux bitcoin sont créés et attribués au mineur qui ajoute avec succès un bloc à la blockchain.
* **Frais de transaction :** Lorsque des personnes envoient des bitcoin, elles incluent un petit frais. Le mineur qui ajoute le bloc reçoit les frais des transactions incluses dans ce bloc.

#### Halvings de Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Les récompenses des mineurs pour compléter un bloc sont divisées par deux tous les 210 000 blocs, soit environ tous les quatre ans.


Bitcoin a une offre maximale fixe de 21 000 000 bitcoin, mais ils n'ont pas tous été créés au lancement de Bitcoin. Au lieu de cela, de nouveaux bitcoin sont progressivement introduits en circulation grâce au **minage**.

Lorsque les mineurs ajoutent avec succès un nouveau bloc de transactions au réseau Bitcoin, ils reçoivent une **récompense de bloc** en bitcoin. Au début de Bitcoin, cette récompense était de 50 bitcoin par bloc. Cette récompense encourageait les gens à utiliser de la puissance de calcul et de l'électricité pour aider à sécuriser le réseau.

Environ tous les 210 000 blocs (soit tous les 4 ans), la récompense de bloc est divisée par deux. Cet événement s'appelle le **halving**. Le halving ralentit la création de nouveaux bitcoin et permet de s'assurer que l'offre totale ne dépassera jamais 21 millions. Avec le temps, cela rend le bitcoin de plus en plus rare.


> **Definition – Offre en circulation**
>
> **L'offre en circulation** désigne la quantité totale disponible d'une monnaie. Pour Bitcoin, l'offre en circulation totale correspond au nombre de pièces qui ont été minées et sont en circulation à un moment donné.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/5818173fa028d96ef4803d468ead76ed00be68a2-292x200.svg)


> **Definition – Calendrier d'émission de Bitcoin**
>
> Le **calendrier d'émission de Bitcoin** est le plan prédéfini et public pour la mise en circulation de nouveaux bitcoin, conçu pour maintenir la rareté de Bitcoin au fil du temps.


Après chaque événement de halving, la récompense en bitcoin que les mineurs reçoivent pour l'ajout d'un bloc est divisée par deux. Cela réduit le rythme de création de nouveaux bitcoin.

Les mineurs continuent de gagner des frais de transaction provenant des transactions incluses dans le bloc qu'ils minent. Avec le temps, ces frais devraient devenir une part plus importante des revenus des mineurs.

Les halvings sont intégrés dans le protocole Bitcoin et se produisent automatiquement environ tous les quatre ans. Grâce à cela, le calendrier d’émission de Bitcoin est prévisible et transparent.

Le tableau présente les prochains halvings, avec la date approximative, le numéro du bloc concerné, la nouvelle récompense par bloc et le pourcentage du total de bitcoins qui auront été minés.


| Événement | Date | Bloc | Récompense | Miné |
| --- | --- | --- | --- | --- |
| 5ᵉ Halving | 2028 | 1 050 000 | 1,5625 BTC | 98,44 % |
| 6ᵉ Halving | 2032 | 1 260 000 | 0,78125 BTC | 99,22 % |
| 7ᵉ Halving | 2036 | 1 470 000 | 0,390625 BTC | 99,61 % |


À mesure que de nouveaux bitcoins sont minés, la quantité en circulation continue d’augmenter jusqu’à atteindre le maximum de 21 000 000 bitcoins, prévu vers l’an 2140. Comme de moins en moins de nouveaux bitcoins sont créés avec le temps, si la demande augmente, le prix de Bitcoin peut monter. Cela encourage aussi les mineurs à continuer de sécuriser le réseau en apportant leur puissance de calcul.

#### Qu’est-ce qu’un hash de bloc valide dans Bitcoin ?

Dans Bitcoin, les mineurs sont en compétition pour trouver un code spécial appelé **hash de bloc**. Ce code identifie un bloc de transactions et permet de l’ajouter à la blockchain.

Chaque bloc contient des informations sur les transactions récentes et inclut aussi le hash du bloc précédent. Cela relie tous les blocs entre eux, formant une chaîne depuis le tout premier bloc (le Bloc Genesis) jusqu’au plus récent.

Un hash fonctionne comme une **empreinte digitale numérique** pour les données du bloc. Si une information du bloc était modifiée, l’empreinte changerait aussi. Cela permet à chacun de vérifier facilement que l’historique des transactions de la blockchain n’a pas été modifié et contribue à la sécurité du réseau.


> **Callout**
>
> Satoshi Nakamoto, le créateur de Bitcoin, a miné le Bloc Genesis, ce qui a débloqué un total de 50 bitcoins.


#### La course au minage d’un bloc

Les mineurs sont en compétition pour trouver un hash de bloc valide. Le premier mineur à en trouver un peut ajouter le nouveau bloc à la blockchain et reçoit une récompense en bitcoin.

Pour être valide, le hash du bloc doit être inférieur à un nombre fixé par le réseau, appelé la cible de difficulté. Comme les hashes sont aléatoires, les mineurs doivent essayer de nombreuses entrées différentes jusqu’à en trouver une qui fonctionne.

Si trop de mineurs participent, les blocs seraient trouvés trop rapidement. S’il y en a trop peu, les blocs prendraient trop de temps à être trouvés. Pour que le système fonctionne de façon régulière, Bitcoin ajuste automatiquement la difficulté tous les 2 016 blocs (environ toutes les deux semaines).

Cet ajustement garantit qu’en moyenne, un nouveau bloc est ajouté à la blockchain toutes les 10 minutes environ.


> **Definition – Définition du niveau de difficulté**
>
> Le **niveau de difficulté** dans le minage de Bitcoin mesure la difficulté à trouver un hash de bloc valide. Le réseau ajuste cette difficulté tous les 2 016 blocs (environ toutes les deux semaines) afin que de nouveaux blocs soient ajoutés à la blockchain environ toutes les 10 minutes. Plus la difficulté est élevée, plus il est difficile pour les mineurs de trouver un bloc valide.


En trouvant un hash de bloc valide, un mineur prouve qu’il a effectué le travail nécessaire pour ajouter un nouveau bloc à la blockchain. Ce processus s’appelle la **Preuve de Travail** (PoW). C’est le mécanisme de sécurité qui permet à Bitcoin de valider les transactions et d’ajouter de nouveaux blocs à la blockchain. Le mineur qui trouve le hash valide en premier gagne une récompense en bitcoin, qui comprend la récompense de bloc et les frais de transaction des transactions incluses dans ce bloc.

La Preuve de Travail (PoW) contribue à la sécurité de Bitcoin en rendant extrêmement coûteux toute tentative de triche ou de prise de contrôle du réseau. Il est donc bien plus rentable de suivre les règles.

Les mineurs jouent quatre rôles principaux :

1. **Collecter les transactions** : Les mineurs sélectionnent les transactions envoyées au réseau et les placent dans un bloc candidat.
1. **Effectuer la Preuve de Travail** : Les mineurs sont en compétition pour résoudre une énigme mathématique difficile en trouvant un hash de bloc valide.
1. **Diffuser le bloc** : Le premier mineur à trouver une solution valide partage le nouveau bloc avec le réseau.
1. **Gagner des récompenses** : Si le bloc est valide, il est ajouté à la blockchain et le mineur reçoit des bitcoin nouvellement créés ainsi que les frais de transaction.

De nombreux mineurs à travers le monde essaient de créer le prochain bloc en même temps. Lorsqu’un mineur trouve une solution valide, le réseau vérifie le bloc. Si tout est correct, il est ajouté à la blockchain. Les autres blocs concurrents sont écartés. Ce processus permet au réseau de rester synchronisé et empêche la double dépense.

* Les mineurs sont des ordinateurs qui aident à maintenir et à mettre à jour le registre de My First Bitcoin.
* Ils collectent les transactions et les regroupent dans un bloc. Ensuite, ils font passer les données du bloc dans un algorithme de hachage pour créer un code unique appelé hash.
* Les mineurs répètent ce processus de nombreuses fois, à la recherche d’un hash qui respecte les règles de My First Bitcoin. Le premier mineur à trouver un hash valide reçoit des bitcoin nouvellement créés en récompense, et son bloc est ajouté à la blockchain.
* Le hash de chaque bloc le relie également au bloc précédent. Si quelqu’un essayait de modifier une transaction passée, les hash ne correspondraient plus et le réseau rejetterait la chaîne modifiée. C’est ce qui garantit la sécurité du registre de My First Bitcoin.
