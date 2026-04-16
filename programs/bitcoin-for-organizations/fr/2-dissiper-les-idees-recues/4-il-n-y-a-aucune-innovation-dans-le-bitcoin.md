# 2.4 Il n’y a aucune innovation dans le Bitcoin.

> La création de mille forêts est contenue dans un seul gland.   
_Ralph Waldo Emerson_

Les critiques tentent souvent de prétendre que Bitcoin est une technologie « ancienne » ou « morte » parce qu’il ne modifie pas la couche de base du protocole aussi fréquemment que les blockchains concurrentes. Cette affirmation ignore à la fois les raisons pour lesquelles les changements sur Bitcoin sont adoptés lentement et la quantité d’innovation qui a lieu pour faire évoluer le réseau sur des couches supérieures, comme le Lightning Network. Elle ignore également que nombre de nos technologies les plus flexibles et durables ne se développent pas non plus rapidement à la couche de base.

Par exemple, il n’y a également aucune innovation en cours dans le protocole de contrôle de transmission (TCP), qui sous-tend l’internet. TCP a été créé pour la première fois en 1974. La dernière mise à jour de TCP date de 1982. Il fait ce qu’il doit faire. Ce n’est pas parfait, et il existe des débats sur la nécessité de mettre à niveau IPv4 pour soutenir les développements futurs d’internet. Cependant, affirmer qu’il n’y a eu aucune innovation sur internet depuis 1982 serait une affirmation remarquable. Toute cette innovation s’est faite « sur » TCP, plutôt qu’« en » TCP.

La grande majorité de l’innovation qui a lieu ne se fait pas « dans » Bitcoin mais « sur » Bitcoin. Un jour, il n’y aura probablement plus d’innovation « dans » Bitcoin, et cela devrait être un objectif et non une critique, car ce sera le reflet de son caractère fondamental dans le soutien de l’économie mondiale en fournissant les bases d’une monnaie saine, globale, neutre et sans autorisation. Une monnaie saine à la fois au sens économique, avec une offre fixe et un registre immuable, mais aussi au sens technologique car elle ne change pas et ce qui fonctionne a bénéficié d’années de disponibilité ininterrompue. Bitcoin a déjà atteint 100 % de disponibilité au cours des 10 dernières années.

Cependant, il serait préoccupant qu’aucune innovation n’ait lieu « sur » Bitcoin. Jetons un œil à cela au cours des 10 dernières années :



#### « Dans » Bitcoin

Segregated Witness (SegWit) a été mis en œuvre en 2017 pour protéger contre la malléabilité des transactions et augmenter la capacité des blocs. SegWit était également un prérequis nécessaire pour que le Lightning Network et certaines chaînes latérales fonctionnent efficacement.

Taproot a été mis en œuvre en 2021 pour permettre le regroupement et la validation de plusieurs signatures en incorporant les signatures Schnorr, introduisant un langage de script pour permettre des fonctionnalités plus complexes et augmentant la confidentialité et la résistance à la censure des transactions.



#### « Sur » Bitcoin

##### Chaîne latérale Liquid

La chaîne latérale Liquid a été mise en œuvre en 2018. Liquid, comme d’autres chaînes latérales, est un registre blockchain séparé qui est lié à la blockchain principale de Bitcoin, selon un ensemble de règles prédéfinies. Ces règles sont suffisamment flexibles pour permettre à la chaîne Liquid de se développer et d’intégrer des améliorations de conception et de scalabilité au fil du temps. Cependant, le lien avec la blockchain Bitcoin garantit que le plafond total de 21 millions de bitcoins est cohérent sur les deux chaînes.

L’actif sur Liquid, L-BTC, est ancré à double sens au bitcoin sur la chaîne principale. Il existe des compromis en termes de coût, de rapidité, de confidentialité et de sécurité qui rendent L-BTC idéal pour certaines applications. Le coût, la rapidité et la confidentialité sont tous améliorés avec L-BTC, au prix d’une certaine confiance accordée aux organisations composant la Fédération Liquid, qui contrôlent ensemble un processus multisignature 11 sur 15 pour ancrer et désancrer L-BTC vers bitcoin et inversement.

##### Lightning Network

Le Lightning Network a été mis en œuvre en 2018. Lightning est conçu pour être un réseau de paiements pair à pair sous la forme d’un graphe de nœuds connectés via des canaux ; ce n’est pas une blockchain. Le bitcoin est verrouillé par un opérateur de nœud sur la blockchain principale afin de le rendre disponible pour une utilisation sur le Lightning Network, ce qui garantit que seul du « vrai » bitcoin est utilisé. Les nœuds peuvent ensuite ouvrir des canaux de liquidité via des contrats intelligents multisignatures entre eux. Les paiements trouvent des routes à travers le réseau de la source à la destination, en optimisant le coût tout en exigeant qu’il y ait suffisamment de liquidité dans la bonne direction à chaque étape du parcours. Le Lightning Network améliore considérablement le coût, la rapidité et la confidentialité en échange d’une perte de sécurité (ou d’une augmentation de la confiance requise) et d’une complexité accrue. Cependant, il est destiné aux paiements quotidiens de faible valeur et de grand volume, ce qui est considéré comme un compromis très raisonnable pour ses millions de transactions quotidiennes (source : River, 2023).

##### Chaumian eCash Mints

Les Fedimints peuvent être considérés comme un réseau Lightning limité à une communauté. Ils sont conçus pour tirer parti de la confiance inhérente qui existe au sein de certaines communautés (par exemple, familles, villages, groupes d’amis) en échange d’une simplification de la complexité et d’une amélioration de la confidentialité pour les utilisateurs. Ce sont des protocoles modulaires et open source pour la garde et la transaction de bitcoins dans un contexte communautaire. Ils sont interopérables avec le Lightning Network lui-même.

**Cashu** est un jeton au porteur qui peut être stocké sur un appareil tel qu’un téléphone mobile ; la conception vise à reproduire les avantages de l’argent liquide physique mais sous forme numérique. Cashu est un exemple de Chaumian eCash construit sur Bitcoin et augmente la confidentialité et la résistance à la censure tout en réduisant la complexité, en échange de la confiance accordée à la « mint » eCash utilisée. Les mints Cashu émettent des jetons eCash, représentant du bitcoin, qui peuvent être dépensés par les utilisateurs sans révéler leur identité. Cashu est interopérable avec le Lightning Network.

Il est probable que de nombreuses autres applications de couche 2 seront développées à l’avenir, avec de nombreuses applications de couche 3 construites à leur tour au-dessus de chacune d’elles.

À titre d’exemple du nombre incroyable d’applications construites sur Lightning, voici un extrait d’un rapport de recherche sur le Lightning Network par River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
