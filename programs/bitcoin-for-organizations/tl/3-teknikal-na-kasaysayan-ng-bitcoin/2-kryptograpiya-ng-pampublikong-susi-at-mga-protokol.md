# 3.2 Kryptograpiya ng Pampublikong Susi at mga Protokol

Ang Internet ngayon, at karamihan sa mga makabagong sistema ng kompyuter, ay umaasa sa kriptograpiya, isang paraan ng pagtatago ng impormasyon upang tanging ang tumatanggap lamang ang makaka-decode nito. Ang mga pundasyon ng kriptograpiyang ginagamit upang gawing ligtas ang Bitcoin ay maaaring masundan pabalik noong dekada 70.

Ang unang isyung kailangang lutasin ay – paano magpadala ng lihim na impormasyon sa isang hindi ligtas na daluyan.

Ito ay unang pinag-aralan nina Whitfield Diffie at Martin Hellman.

Ang problema: ang dalawang panig – na karaniwang tinutukoy bilang Alice at Bob – ay nais magbahagi ng lihim na impormasyon sa isang network kung saan maaaring may nakikinig. Upang magawa ito, nilikha nila ang Diffie-Hellman key exchange process.

Ang lihim na ito ay maaaring gamitin bilang panimulang halaga upang lumikha ng maraming symmetric keys para i-encrypt at i-decrypt ang mga mensaheng ipapadala sa isa’t isa nang hindi kailangang ibahagi ang mismong key sa publiko.

Dahil ang private key ay hindi kailangang ibahagi, at magkaibang keys ang ginagamit sa bawat dulo para mag-encrypt at mag-decrypt, ito ay tinatawag na asymmetric encryption algorithm.

Mga halimbawa ng paggamit:

* Nilagdaan ni Alice ang isang mensahe gamit ang pampublikong susi ni Bob – siya lamang ang makaka-decrypt nito gamit ang kanyang private key
* Nilagdaan ni Alice ang isang mensahe gamit ang kanyang private key – sa pamamagitan ng pag-decrypt gamit ang kanyang pampublikong susi, kahit sino ay maaaring magpatunay na si Alice ang nagpadala ng mensahe, nang hindi nalalaman ang kanyang private key
* Sa pagsasama ng dalawang pamamaraang ito na may dalawang layer ng encryption, maaaring magpadala ng mensahe na naka-encrypt upang tanging si Bob lamang ang makaka-decrypt, at maaari niyang mapatunayan na si Alice nga ang nagpadala

Bagaman hindi nabanggit sa papel, si Ralph Merkle ay mahalaga sa pagtulong na lutasin ang itinuturing noon na imposibleng palaisipan – kung paano magtatag o magpanumbalik ng pribadong komunikasyon sa isang bukas at posibleng mapanganib na network.

Ang pamamaraang ito ay madaling atakihin gamit ang brute force, kung saan maaaring kunin ng isang umaatake ang mga pinagsaluhang numero at muling likhain ang shared key kalaunan kung may sapat na oras at resources, kaya hindi ito ang kumpletong sagot sa sarili nito.

##### Mga Protokol para sa Public Key Cryptosystems

Bukod sa ambag niya sa Diffie-Hellman public-key system na nabanggit sa itaas, **Ralph Merkle** ay patuloy na nag-ambag sa larangang ito sa loob ng maraming taon, at naging mahalaga sa pagbuo ng ilang mahahalagang bahagi na ginagamit ng Bitcoin.

Ang cryptographic hash function ay isang matematikal na algorithm na tumatanggap ng input na anumang laki at nagsasagawa ng komplikadong kalkulasyon upang magbalik ng hash value sa bits, na karaniwang kinakatawan ng isang fixed-length na alphanumeric output gamit ang hexadecimal format.

* Maaaring anumang laki ang input
* Ang output ay laging may tiyak na haba at deterministiko (parehong input ay laging magbubunga ng parehong hash)
* Madaling beripikahin ngunit napakahirap baliktarin ang proseso upang matukoy ang input
* Ang maliit na pagbabago sa datos ay lubos na magbabago sa output

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/a5725f0a95ec8a7eb4a4fadfac1de5d51b4d4421-515x331.svg)

Ang hashing ay mahalagang bahagi ng Bitcoin protocol. Ang SHA-256, na ginagamit sa Bitcoin, ay nilikha ng NSA at halimbawa ng cryptographic hashing algorithm.

* Bawat bloke sa chain ay hinahash upang hindi mabago ang datos – tinitiyak ang integridad ng distributed ledger
* Ang hash na nabuo ay kailangang tumugma sa ‘Proof of work’ na pamantayan upang maituring na valid na block
* Merkle trees – sa paggamit ng branching at hashes ng hashes, ang hash trees ay nagbibigay-daan sa beripikasyon ng malalaking datasets na may kaunting storage
* Ang Hash based Signatures at Keys ay maaaring gamitin para sa mga wallet, address at awtorisasyon ng mga transaksyon

Ang distributed verification ng blockchain states at append-only ledger models na hindi madaling baguhin ay posible dahil sa one-way hashing. Ang hash functions ay nagbibigay ng maaasahan at deterministikong paraan upang beripikahin ang mga pangyayari sa pampublikong ledger tulad ng Bitcoin kahit walang sentralisadong modelo ng pagtitiwala.

Ang mga bagong kakayahang ito sa larangan ng kriptograpiya ay inaasahan ng mga lumikha nito na magdadala ng bagong alon ng inobasyon sa larangang ito.

##### Elliptic curve cryptography

Isa sa mga sumunod na inobasyon ay dumating sa anyo ng elliptic curve cryptography.

Ang elliptic curve cryptography ay ipinakilala noong 1985 ng dalawang siyentipiko, N. Koblitz at V. Miller. Iminungkahi nila ang ideya ng paggamit ng mga puntong tinutukoy ng elliptic curves sa halip na finite prime fields upang mapanatili ang Discrete Logarithm problem assumption, gaya ng karaniwang ginagamit sa standard na Diffie-Hellman key exchange protocol. Ang mga detalye kung paano ito gumagana ay lampas sa saklaw ng seksyong ito, ngunit sa pangkalahatan, ang elliptic curve ay ang hanay ng mga puntong tumutugon sa isang partikular na matematikal na ekwasyon.

Ang ekwasyon para sa isang elliptic curve ay ganito ang itsura:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

May ilang kapaki-pakinabang na katangian ito:

* Horizontal na simetriya. Anumang punto sa curve ay maaaring i-reflect sa x axis at mananatili pa ring bahagi ng parehong curve.
* anumang hindi patayong linya ay tatama sa curve sa hindi hihigit sa tatlong lugar.
* Ang compact na laki ng key ay mahalaga para sa episyenteng pag-iimbak at pagpapadala ng public keys sa blockchain.

Ang mga katangiang ito ay maaaring gamitin upang lumikha ng key pairs na katulad ng sa Diffie-Hellman algorithm. Ang Bitcoin ay gumagamit ng ECDSA, na pinaikli ng Elliptic Curve Digital Signature Algorithm. Isa itong proseso na gumagamit ng elliptic curve at finite field upang 'pumirma' ng datos sa paraang maaaring mapatunayan ng iba ang pagiging totoo ng lagda habang ang pumirma lamang ang may kakayahang lumikha ng lagda. Sa bitcoin, ang datos na nilalagdaan ay ang transaksyong nagpapasa ng pagmamay-ari.

Ang ‘finite’ na bahagi ay katulad ng ‘mod’ na paraan sa Diffie-Hellman, kung saan ang output ng ekwasyon ay hinahati at ang natitirang bahagi ay ginagamit upang matiyak na pasok ito sa saklaw ng mga numero.
