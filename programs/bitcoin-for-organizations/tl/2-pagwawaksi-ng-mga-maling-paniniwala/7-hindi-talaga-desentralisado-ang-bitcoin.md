# 2.7 Hindi talaga desentralisado ang Bitcoin.

> Ang pagiging komplikado ng crypto ay nagmumula sa mga pagsubok na gawing desentralisado ito—sa pamamagitan ng pamamahagi ng kapangyarihan at pamamahala sa sistema, teoretikal na hindi na kailangan ng pinagkakatiwalaang tagapamagitan tulad ng mga institusyong pinansyal. Iyan ang batayan ng orihinal na Bitcoin white paper, na nag-alok ng solusyong kriptograpiko na layuning payagan ang mga bayad na maipadala nang hindi dumadaan sa anumang institusyong pinansyal o iba pang pinagkakatiwalaang tagapamagitan. Gayunpaman, naging sentralisado agad ang Bitcoin at ngayon ay umaasa na sa isang maliit na grupo ng mga software developer at mining pool upang gumana  
_International Monetary Fund_

Tulad ng ipinapakita ng sipi sa itaas mula sa isang medyo bagong post ng International Monetary Fund, patuloy na iginigiit ng mainstream na industriya ng pananalapi na hindi desentralisado ang Bitcoin, at nalilito rin nila ang Bitcoin sa iba pang crypto asset.

##### Panimula

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/d59c22e7081b19509449fdbcb642dbd365707640-161x167.svg)

Ang desentralisasyon ay isang mahalagang aspeto ng Bitcoin. Ang kakayahang mapanatili ang mga patakaran ng protocol tulad ng kakulangan at distribusyon nang walang sentral na awtoridad ay tinitiyak na maaari itong magsilbing pera na walang hadlang para sa isang pandaigdigang lipunan.

Tulad ng nabanggit ni Satoshi sa kanyang online na pakikipag-ugnayan, ang mga desentralisadong serbisyo tulad ng BitTorrent ay 'nakakatagal' laban sa mga pagsupil ng Gobyerno, kumpara sa mga serbisyong may kilalang may-ari at sentralisadong mga server. Malinaw na nag-aalala siya tungkol sa posibleng panganib na isara o maapektuhan ng Gobyerno o iba pang interes ang Bitcoin.

Sa kontekstong ito, interesado tayo sa desentralisasyon ng:

* Ang pag-develop at pamamahala ng code na nagpapatakbo ng protocol; sino ang pinapayagang magbago ng mga patakaran?
* Ang mining function na lumilikha ng mga bagong block ayon sa mga patakaran at nagva-validate laban sa double-spend
* Ang mga node na nagva-validate ng mga transaksyon para sa bisa at nagtatago ng kopya ng blockchain

##### Mga Developer

Ang Bitcoin ay isang open-source na protocol na malayang maaaring tingnan, i-download, kopyahin o suhestiyunan ng sinuman ng mga pagbabago. Makikita ito sa isang GitHub library, at ang source code ay inilunsad noong 2009 ni Satoshi Nakamoto. Malaya ang sinuman na i-download ang code at magpatakbo ng node, na karamihan ay gumagamit ng orihinal na Bitcoin Core software, na na-update sa paglipas ng panahon.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Pinagmulan: https://river.com/learn/what-is-bitcoin-core/_

Ang pag-develop ng Bitcoin Core ay sumusunod sa pinakamahusay na praktis ng open source development. Sa anumang oras, maaaring may iba't ibang developer na sumusulat o nagrerepaso ng mga pagbabago sa code. Kailangan nilang pakinggan ang mga saloobin ng mga node operator at miner, pati na rin ang user base bago gumawa ng anumang kritikal na pagbabago sa code, na rerepasuhin at pagkakasunduan gaya ng ipinapakita sa flowchart sa itaas bago maisama sa code.

Ang mga patakaran ng Bitcoin ay naka-encode sa Bitcoin Core software na ito, na tumatakbo sa bawat node. Maaaring magmungkahi ng pagbabago sa mga patakaran ang sinuman – ang mga patakaran ay code, ngunit hindi ito_basta_code lang, ito ay_napagkasunduang_code. Kapag binago nang mag-isa, ang bagong code ay hindi na bahagi ng consensus at hindi na bahagi ng Bitcoin. Ang pagbabago ng anuman sa Bitcoin at manatili sa consensus ay mahirap. Ang mga mungkahing pagbabago sa code ay nahahati sa tatlong kategorya:

* Sa loob ng umiiral na mga patakaran: Maliit na upgrade tulad ng pagwawasto ng spelling, mas magandang UI o data management ay maaaring pumasok sa kategoryang ito at medyo madali lang makakuha ng pag-apruba.
* Pagdaragdag ng bagong patakaran na nagdadagdag ng mga restriksyon sa mga umiiral na patakaran – tulad ng pagbawas ng block size. Ito ay tinatawag na 'soft fork'. Ang mga node na piniling hindi ipatupad ang pagbabago sa code at manatili sa lumang bersyon ay maaari pa ring makibahagi sa network.
* Pagdaragdag ng bagong patakaran na sumasalungat sa kasalukuyang mga patakaran, halimbawa ay pagtaas ng block size. Ang mga node na hindi mag-upgrade sa bagong code ay ituturing na invalid ang block na nilikha sa mas malaking sukat. Ito ay tinatawag na 'hard fork' at magdudulot ng paghahati ng chain sa pagitan ng mga node na nagpapatakbo ng orihinal at bagong code at lilikha ng bagong coin. Nangyari na ito dati ngunit hindi nagtagumpay sa pangmatagalan ang bagong coin dahil pinili ng karamihan ng mga node na manatili sa orihinal na code.

Samakatuwid, hindi maaaring baguhin ng isang partido o grupo ng tao ang Bitcoin code nang mag-isa nang hindi nakakakuha ng consensus agreement, kung hindi ay nanganganib silang magkaroon ng chain split at paglikha ng bagong coin na sumusunod sa ibang patakaran.

##### Pagmimina

Ang mining function ay nagva-validate ng mga transaksyon tulad ng ibang node sa network, ngunit ito ay gagastos ng enerhiya na kailangan upang lumikha ng bagong block na tumutugma sa consensus rules sa code. Kapag nagtagumpay, makakakuha ang miner ng gantimpala sa anyo ng transaction fees at Bitcoin rewards (sa oras ng pagsulat, 3.125 coins bawat block).

Karaniwan, ang pagmimina ay isinasagawa ng mga mining 'pool' kung saan pinagsasama-sama ng mga tao ang kanilang mining power o hash rate upang tumaas ang tsansa na makapagmina ng block at magbahagi ng gantimpala. May panganib na ang isa o higit pang mining pool ay magsanib upang makamit ang 51% na dominasyon sa pagmimina at sa gayon ay mapaboran ang kanilang sarili sa network validation protocol upang mag-double spend ng coins. Mangangailangan ito ng napakalaking resources at gastos, at madaling makalipat ang mga indibidwal na miner sa ibang mining pool anumang oras. Malamang na babagsak din ang halaga ng bitcoin kung mangyari ang ganitong atake, dahil magiging malinaw na naapektuhan ang integridad ng network. Kailangan ding agad na ipalit ng umaatake ang anumang bitcoin na nakuha sa fiat bago bumaba ang halaga. Mas lalo nitong pinapahirap na magtagal ang atake, kaya mas kapaki-pakinabang para sa miner o pool operator na sumunod sa mga patakaran at subukang magmina ng valid na blocks.

Mahalaga rin ang heograpikal na distribusyon ng mining function upang maiwasan, halimbawa, ang gobyerno na sakupin o ipasara ang mining capacity. Halimbawa, ang kamakailang pagbabawal ng China sa pagmimina ay nagpakita ng kakayahan ng Bitcoin na mag-adapt at mabuhay sa kabila ng interbensyon ng gobyerno, mabilis na nakaangkop at nakabawi mula sa pagkawala ng hash power.

##### Mga Node

Hindi tulad ng pagmimina, na nangangailangan ng malaking puhunan upang epektibong makipagkumpitensya sa pagmina ng mga bagong block, o pag-develop ng code na nangangailangan ng kasanayan sa programming, ang pagpapatakbo ng node ay isang bagay na kayang gawin ng sinumang interesado na tumulong mapanatili ang desentralisasyon ng Bitcoin.

Ang mga node ay nagpapatakbo ng Bitcoin Core software at nagpapatupad ng mga patakaran na nakapaloob sa code upang matiyak na hindi nandaraya ang mga miner, halimbawa sa pamamagitan ng paglalaan ng mas mataas na block reward kaysa pinapayagan. Pinapatupad din nila ang 21 milyong supply cap, na mahalaga upang mapanatili ang kakulangan ng Bitcoin. Para mapatigil ng gobyerno o masamang aktor ang Bitcoin, kailangan nilang sirain ang bawat kopya ng blockchain, na kasalukuyang tumatakbo sa libu-libong node na nakakalat sa buong mundo—isang halos imposibleng gawain.

##### Mga Tao

Isa pang aspeto ng posibleng sentralisasyon ay ang mga tao. Bawat ibang 'alt-coin' ay may pinuno—isang taong maaaring pilitin na magtaguyod ng mga pagbabagong hindi pabor sa Bitcoin. Nanatili si Satoshi Nakamoto nang sapat na matagal upang matiyak na nasa tamang landas ang Bitcoin bago tuluyang mawala, iniwan ito sa kamay ng iba upang paunlarin at iangkop ang software.

Paano naman ang mga may hawak ng malaking halaga ng Bitcoin? Ang mga unang namuhunan, na hindi pa nawala ang kanilang mga coin, ay siguradong napakayaman na ngayon. Mahalaga na tandaan na maaaring totoo ito, ngunit hindi ito nagbibigay sa kanila ng mas malaking impluwensya sa sistema kaysa sa iba, hindi tulad ng mga 'proof of stake' na coin kung saan ang mga naunang yumaman sa coin na iyon ay may kalamangan sa paggawa ng desisyon at distribusyon ng mga susunod na coin. Ito ay nagdudulot o magdudulot ng sentralisasyon sa paglipas ng panahon.

##### Konklusyon

Ano ang mga posibleng banta na kayang bawasan ng desentralisasyon?

* Pagpapasara o pagbabawal ng gobyerno sa Bitcoin
* Hindi kanais-nais na pagbabago sa code na pumapabor sa isang grupo ng interes sa Bitcoin, hal. pagtaas ng block reward
* Pamimilit ng gobyerno o masamang aktor sa protocol upang impluwensyahan ang direksyon ng protocol
* Kakayahan ng isang grupo ng mga miner na sakupin ang network at mag-'double-spend' ng Bitcoin – isang 51% na atake

Tulad ng nakikita natin, ang kombinasyon ng mga node, code developer at miner, pati na rin ang paggamit ng 'proof of work' na mekanismo, ay nagdedesentralisa sa Bitcoin sa sapat na antas kung saan ang mga posibleng banta na ito ay hindi itinuturing na malaking alalahanin. Kailangang patuloy na bantayan ng komunidad ang sitwasyon upang matiyak na mananatili itong ganito.
