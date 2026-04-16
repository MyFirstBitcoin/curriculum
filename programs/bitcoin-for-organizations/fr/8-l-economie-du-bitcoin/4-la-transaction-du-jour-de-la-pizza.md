# 8.4 La transaction du jour de la pizza

Jusqu'à présent, ce module s'est concentré sur l'utilisation de la nature ouverte du registre Bitcoin pour compiler des métriques utiles à partir de données de transactions agrégées. Cependant, il est possible d'utiliser les données du registre et les explorateurs de blocs pour examiner des transactions réelles et retracer le mouvement des fonds au sein du réseau.

Chaque année, le 22 mai, la communauté Bitcoin rend hommage à Laszlo Hanyecz, qui est devenu la première personne connue à utiliser des bitcoins pour acheter des biens physiques. Le 18 mai 2010, Hanyecz a annoncé sur un forum de Bitcointalk.org qu'il cherchait une pizza et était prêt à payer en BTC. Il a offert 10 000 BTC à toute personne acceptant de conclure la transaction. Il a attendu plusieurs jours, jusqu'à ce que Jeremy Sturdivant, un étudiant de 19 ans, accepte et lui envoie deux grandes pizzas.

La **Journée de la Pizza** peut être consultée par n'importe qui et possède l'identifiant de transaction suivant :

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

En saisissant cet identifiant de transaction dans [mempool.space](https://mempool.space) révèle les informations suivantes :

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Date et heure de la transaction : 22 mai 2010

Frais de transaction réseau : 99 000 000 sats (à l'époque cela équivalait à moins d'1 centime US. En mai 2025, cela représente 95 072,67 $)

Hauteur du bloc : 57 043

Nombre de confirmations : 838 645 (c'est le nombre de blocs ajoutés au registre après cette transaction)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Nombre d'entrées de transaction : 131

Nombre de sorties de transaction : 1

En cliquant sur la clé publique de sortie (se terminant par `XaxFyQ`) que l'on sait appartenir à Jeremy Sturdivant, qui a reçu 10 000 BTC pour deux pizzas, on découvre les informations suivantes :

Cette adresse a actuellement un solde de 0,00257879 BTC et il semble qu'elle ait été impliquée dans 14 transactions, la plus récente datant du 13 décembre 2024.



#### 8.4.1 Activité : Discussion de groupe

1. Décrivez les avantages (par exemple, audit, responsabilité) ou les risques (par exemple, préoccupations relatives à la vie privée) pour les particuliers ou les entreprises utilisant un système de transaction aussi transparent et ouvert.
1. Comment ce type de transparence financière pourrait-il affecter des secteurs comme la charité, les marchés publics, les transferts de fonds ou les forces de l'ordre ?
1. Les systèmes bancaires traditionnels devraient-ils offrir un niveau de visibilité similaire ? Seront-ils contraints de le faire par le marché ?
