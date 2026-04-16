# 3.1 Le développement de TCP/IP

La plupart d'entre nous connaissent les protocoles TCP/IP utilisés aujourd'hui comme fondement d'Internet. Leurs origines remontent à la fin des années 1970, lorsque des scientifiques exploraient des conceptions alternatives à Arpanet – un réseau encore plus ancien conçu par le département de la Défense des États-Unis pour permettre le partage de ressources entre ordinateurs distants. TCP/IP est devenu la norme de protocole pour Arpanet en 1983, ce qui a conduit à son adoption comme modèle dominant de réseau à la fin des années 1990 et à la base de l'internet sur lequel fonctionne Bitcoin aujourd'hui.


| Modèle OSI | TCP/IP |
| --- | --- |
| Application | Application |
| Présentation | Application |
| Session | Application |
| Transport | Transport |
| Réseau | Réseau |
| Liaison de données | Liaison de données |
| Physique | Physique |


Au même moment où le modèle TCP/IP était en cours de développement, un cadre similaire mais plus complet était élaboré par l’Organisation internationale de normalisation (ISO) et l’industrie des télécommunications (CCITT). Le processus de développement de nouveaux protocoles ou de proposition de modifications était lent et lourd comparé à l’approche plus décentralisée utilisée pour TCP/IP, ce qui a conduit à la domination de cette dernière aujourd’hui.

##### Demande de modification

Toute évolution suggérée des protocoles existants ou toute idée de nouveaux protocoles peut être proposée dans le modèle TCP/IP via une **Demande de modification** . Celles-ci passent par un processus d’approbation, géré par l’Internet Engineering Task Force (IETF), et deviennent open source une fois approuvées afin que chacun puisse les implémenter et les adopter. Quelques exemples notables :

* 1969 RFC 1 Documentait comment les paquets seraient envoyés dans l’Arpanet
* 1981 RFC791 a défini le protocole Internet V4 – encore largement utilisé aujourd’hui
* 1982 RFC 821 Protocole simple de transfert de courrier (SMTP)
* 1987 Système de noms de domaine – comment les noms de domaine sont résolus en adresses IP
* 1999 RFC 2616 Protocole de transfert hypertexte – essentiel pour la navigation sur le web


> **Callout**
>
> La **Proposition d'amélioration de Bitcoin** (BIP) suit une approche similaire à celle des RFC, mais se concentre uniquement sur les améliorations de Bitcoin lui-même plutôt que sur le développement de nouveaux protocoles ou de protocoles alternatifs. Bitcoin s’inspire également de ce modèle en couches, et vous verrez des protocoles supplémentaires décrits comme couche deux ou trois.


De la même manière que les couches de base du modèle TCP/IP ont relativement peu changé au cours des dernières décennies, l’innovation ayant lieu dans les couches supérieures, la couche de base de Bitcoin devrait désormais évoluer très lentement, avec des solutions de passage à l’échelle comme Lightning et Liquid qui se développent au-dessus.

Un bon exemple de la difficulté à faire évoluer les protocoles de couche de base au fil du temps est IPv6. L’épuisement attendu de l’espace d’adressage en IPv4 a créé une demande pour un nouveau protocole. Le premier projet de norme a été créé en 1998, mais n’a été ratifié comme norme Internet qu’en 2017. Bien qu’il ait résolu de nombreux problèmes d’IPv4 et soit bien plus pérenne, il a tout de même connu une adoption très lente dans l’industrie aujourd’hui. Pendant ce temps, de nombreux nouveaux protocoles ont été définis dans les couches supérieures pour permettre le multimédia, l’email, etc.

##### Les blocs de construction utilisés par Bitcoin

Cette séparation des problèmes d’interconnexion permet de développer les protocoles indépendamment des couches supérieures et inférieures. Plutôt que de devoir réinventer des solutions pour chaque couche, le réseau Bitcoin peut s’appuyer sur les capacités sous-jacentes du réseau fournies aux couches physique et liaison de données.


| Couche | TCP/IP d'origine |
| --- | --- |
| Application | Utilise le système de noms de domaine (DNS) pour identifier les nœuds voisins. Le port 8333 signale le protocole Bitcoin. |
| Transport | UDP pour les communications FIBRE entre mineurs pour une faible latence. TCP pour les communications P2P entre nœuds. |
| Transport | Routage TOR : permet l’anonymat et la confidentialité. Protocole de diffusion : achemine le trafic sur le réseau. |
| Liaison | Fonctionne sur n’importe quel support (par exemple, Ethernet, Wi-Fi, etc.) |
| Physique | Transmission physique via sans fil, Ethernet ou autres interfaces matérielles. |


##### Bitcoin est un protocole neutre pour transférer de la valeur, comme HTTPS est un protocole pour transférer de l’information

* **HTTPS** : Sites web sécurisés
* **SMTP**: Envoyer des e-mails
* **FTP**: Transférer des fichiers
* **DNS**: Gérer les noms de domaine
* **BTC**: Stocker et transférer de la valeur

Le Bitcoin permet de transporter de la valeur de manière fiable et sans nécessiter de tiers, entre des personnes ou des appareils à travers Internet. On s'attend à ce que cela libère une valeur considérable.
