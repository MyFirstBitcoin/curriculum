# 2.3 Le Bitcoin est trop lent pour être une monnaie mondiale.

> Les visionnaires imaginent un avenir où les travailleurs télétravaillent, où les bibliothèques sont interactives et les salles de classe multimédias. Ils parlent de réunions municipales électroniques et de communautés virtuelles… La vérité, c’est qu’aucune base de données en ligne ne remplacera votre journal quotidien, aucun CD-ROM ne pourra remplacer un enseignant compétent et aucun réseau informatique ne changera la façon dont fonctionne le gouvernement.  
_Clifford Stroll_

17 ans plus tard, Newsweek a cessé sa publication imprimée et est devenue exclusivement disponible en ligne. Imaginez vivre en 1974, lorsque le protocole de contrôle de transmission (TCP) a été créé pour la première fois.

Personne n’avait prévu le smartphone, avec toutes ses applications, dans votre main. Personne n’avait imaginé le système de navigation par satellite dans votre voiture.

Internet n’est pas apparu d’un seul coup, mais plutôt progressivement, comme une évolution de protocoles et de couches. Ces évolutions se sont appuyées sur TCP, mais ne l’ont principalement pas modifié.

> Ainsi, alors que j’envisage la transition vers les plateformes de communication du futur, je constate que la beauté des protocoles Internet réside dans la séparation des couches entre le service et la technologie.  
_Michael K Powell_



##### Comparer l’évolution du Bitcoin à celle d’Internet

TCP était nécessaire mais pas suffisant pour l’émergence de tout le reste sur Internet. L’évolution du Bitcoin semble suivre une trajectoire similaire. Les systèmes ouverts semblent être plus résilients et réussir davantage lorsqu’ils sont développés en couches, même s’il peut s’écouler beaucoup de temps entre la pose des premiers blocs de construction et l’adoption généralisée. Les solutions tout-en-un ne semblent pas aussi efficaces dans les systèmes ouverts que celles construites en couches sur des protocoles. De la même manière que personne n’a eu besoin de reconstruire Internet parce que les films ne pouvaient pas être diffusés en streaming via TCP, il est probable qu’il en sera de même pour Bitcoin.

Il existe déjà un certain nombre de protocoles de couche 2 reposant sur Bitcoin, et de nombreuses applications reposant sur ces protocoles de couche 2 (voir la section 201.4 pour plus de détails à ce sujet).

Plutôt que de se concentrer sur ce que le bitcoin et le réseau Bitcoin ne peuvent pas faire aujourd’hui, pensez à ce qui peut déjà être fait aujourd’hui, et comparez cela à ce qui était possible il y a 10 ans. Faites cet exercice avec Internet de 1985 à 1995, puis observez à quelle vitesse Internet s’est développé au cours des 30 années suivantes et les applications qui sont devenues possibles. Utilisez cette perspective pour projeter Bitcoin dans l’avenir et imaginez à quoi il pourrait ressembler dans seulement 10 ans, ou 30 si votre imagination peut aller aussi loin.



##### Comparer Bitcoin avec le système monétaire mondial existant

L’affirmation centrale selon laquelle Bitcoin est trop lent pour être une monnaie mondiale est sans doute vraie si l’on se limite à la couche de base de Bitcoin. Il est également vrai que la couche de base de nos systèmes monétaires actuels est trop lente pour être une monnaie mondiale, si une restriction similaire signifiait qu’aucune infrastructure de paiement n’était construite dessus par les banques privées et les services de paiement comme Visa et Mastercard. Notre système actuel est construit en couches, donc on peut s’attendre à ce que l’avenir ressemble à cela. Certains compromis de conception, comme entre la confiance, la rapidité et le coût, peuvent se retrouver dans les systèmes qui fournissent les mêmes solutions, même s’ils sont conçus pour déplacer différents jetons de valeur.

Certaines des couches 2 existantes sur Bitcoin répondent directement à la question de la rapidité, par exemple Liquid et le Lightning Network (voir la section 201.4 pour plus de détails). Liquid est plus rapide et moins cher que la blockchain Bitcoin, et le Lightning Network est encore plus rapide et moins cher que Liquid. Une prolifération de couches 2, chacune avec des compromis différents, est à prévoir et est saine.

Il y aura probablement davantage de couches 2 et 3 et une explosion d’applications qui les utiliseront, tout comme cela s’est produit avec l’évolution d’Internet.



##### Motivation

Lorsque cette critique est formulée, il vaut la peine de se demander si le critique n’a pas d’autres motivations. Par exemple, ont-ils un nouveau projet blockchain ou un projet différent ? Cela peut être analogue à essayer de vendre un meilleur protocole de contrôle de transmission.

Le trilemme de l’évolutivité, ou de la blockchain, a été soulevé pour la première fois par Vitalik Buterin en 2017. Il affirme qu’il y a toujours un compromis dans la conception d’une blockchain entre les propriétés de décentralisation, de sécurité et d’évolutivité. Toute personne qui critique Bitcoin en disant qu’il est trop lent et qu’elle a une solution plus rapide dans une blockchain de couche 1 sacrifie une partie de la sécurité ou de la décentralisation pour y parvenir. Bien qu’un tel compromis puisse avoir du sens pour une blockchain conçue pour d’autres usages, l’ordre de priorité pour une monnaie mondiale doit être :


> **Note**
>
> * **Décentralisation**
>   * Permet de supprimer les parties de confiance
> * **Sécurité**
>   * Empêche les acteurs malveillants de falsifier les transactions ou le registre
> * **Évolutivité**
>   * Permet au système de s’adapter économiquement en nombre d’utilisateurs et en rapidité


Les deux premières caractéristiques créent l’environnement pour une émission sans émetteurs, des paiements sans intermédiaires et une garde sans gestionnaires.

Bitcoin fait le bon compromis entre les trois caractéristiques de conception de la blockchain, étant donné que son cas d’utilisation cible est celui de monnaie mondiale, et il atténue les compromis d’évolutivité et de rapidité grâce aux couches.

> Satoshi a découvert comment protéger l’intégrité de la monnaie numérique sans parties de confiance – pas besoin d’émetteurs, d’intermédiaires ou de gestionnaires.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
