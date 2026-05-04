# 2.4 Walang nagaganap na inobasyon sa Bitcoin

> Ang paglikha ng isang libong gubat ay nagmumula sa isang buto ng ensina.   
_Ralph Waldo Emerson_

Madalas subukan ng mga kritiko na sabihing 'luma' o 'patay' na teknolohiya ang Bitcoin dahil hindi ito madalas baguhin ang base layer protocol kumpara sa ibang mga blockchain. Hindi nito isinasaalang-alang ang mga dahilan kung bakit dahan-dahan ang pagtanggap ng mga pagbabago sa Bitcoin at ang dami ng inobasyon na nangyayari upang mapalawak ang network sa mas mataas na mga layer, tulad ng Lightning Network. Hindi rin nito kinikilala na marami sa ating pinaka-flexible at matibay na teknolohiya ay hindi rin mabilis magbago sa base layer.

Halimbawa, wala ring inobasyon na nangyayari sa Transmission Control Protocol (TCP), na siyang pundasyon ng internet. Unang nilikha ang TCP noong 1974. Huling na-update ang TCP noong 1982. Ginagawa nito ang kailangan nitong gawin. Hindi ito perpekto, at may mga debate kung kailangan bang i-upgrade ang IPv4 para suportahan ang mga susunod na pag-unlad ng internet. Gayunpaman, ang sabihing walang inobasyon sa internet mula 1982 ay isang kahanga-hangang pahayag. Lahat ng inobasyon ay nangyari 'sa ibabaw' ng TCP, hindi 'sa loob' nito.

Ang napakaraming inobasyon na nangyayari ay hindi 'sa loob' ng Bitcoin kundi 'sa ibabaw' ng Bitcoin. Darating ang panahon na maaaring wala nang inobasyon 'sa loob' ng Bitcoin, at ito ay dapat maging layunin at hindi batikos, dahil ito ay magiging repleksyon kung gaano na ito kahalaga sa pagsuporta sa pandaigdigang ekonomiya sa pagbibigay ng pundasyon para sa global, neutral, at walang hadlang na matatag na pera. Pera na matatag hindi lang sa ekonomiyang aspeto na may takdang suplay at hindi nababagong ledger, kundi matatag din sa teknolohikal na aspeto dahil hindi ito nagbabago at ang tumatakbo ay may taon ng tuloy-tuloy na operasyon. Naabot na ng Bitcoin ang 100% uptime sa nakaraang 10 taon.

Gayunpaman, magiging problema kung walang inobasyon na nangyayari 'sa ibabaw' ng Bitcoin. Tingnan natin ito sa nakaraang 10 taon:



#### 'Sa loob' ng Bitcoin

Naipatupad ang Segregated Witness (SegWit) noong 2017 upang maprotektahan laban sa transaction malleability at upang madagdagan ang kapasidad ng block. Ang SegWit ay naging mahalagang hakbang para gumana nang mahusay ang lightning at ilang side chains.

Naipatupad ang Taproot noong 2021 upang payagan ang batching at pag-validate ng maraming lagda sa pamamagitan ng pagsasama ng Schnorr signatures, pagpapakilala ng scripting language para sa mas komplikadong functionality, at pagtaas ng privacy at censorship resistance ng mga transaksyon.



#### 'Sa ibabaw' ng Bitcoin

##### Liquid Sidechain

Naipatupad ang Liquid sidechain noong 2018. Ang Liquid, tulad ng ibang sidechains, ay isang hiwalay na blockchain ledger na konektado sa pangunahing Bitcoin blockchain, ayon sa itinakdang mga patakaran. Sapat na flexible ang mga patakarang ito upang payagan ang Liquid chain na mag-develop at magdagdag ng mga disenyo at scalability enhancements sa paglipas ng panahon. Gayunpaman, ang koneksyon sa Bitcoin blockchain ay tinitiyak na ang kabuuang 21 milyong supply cap ng bitcoin ay pareho sa parehong chain.

Ang asset sa Liquid, L-BTC, ay two-way pegged sa bitcoin sa main chain. May mga trade off sa gastos, bilis, privacy at seguridad na ginagawang angkop ang L-BTC para sa ilang aplikasyon. Ang gastos, bilis at privacy ay lahat napapabuti sa L-BTC, kapalit ng paglalagay ng tiwala sa mga organisasyon na bumubuo sa Liquid Federation, na may kontrol sa isang 11 sa 15 multisig na proseso para mag-peg in at peg out ng L-BTC sa bitcoin at kabaliktaran.

##### Lightning Network

Naipatupad ang Lightning network noong 2018. Ang Lightning ay dinisenyo bilang peer to peer payments network sa anyo ng graph ng mga node na konektado sa pamamagitan ng mga channel; hindi ito isang blockchain. Ang bitcoin ay nilalock ng isang node runner sa main blockchain upang magamit ito sa Lightning Network, na tinitiyak na 'totoong' bitcoin lang ang ginagamit. Maaaring magbukas ng liquidity channels ang mga node sa isa't isa gamit ang multisig smart contracts. Ang mga bayad ay naghahanap ng ruta sa network mula pinagmulan hanggang destinasyon, na ino-optimize ang gastos laban sa pangangailangan na may sapat na liquidity sa tamang direksyon sa bawat hakbang ng ruta. Malaki ang pinapabuti ng Lightning Network sa gastos, bilis at privacy kapalit ng kaunting pagkawala ng seguridad (o dagdag na tiwala na kailangan) at pagtaas ng komplikasyon. Gayunpaman, ito ay para sa mataas na volume, mababang halaga ng araw-araw na bayad, kaya't itinuturing itong makatarungang trade off para sa milyun-milyong transaksyon araw-araw (source: River, 2023).

##### Chaumian eCash Mints

Maaaring ituring ang Fedimints bilang isang lightning network na limitado sa komunidad. Dinisenyo ito upang gamitin ang likas na tiwala na umiiral sa ilang mga komunidad (hal. pamilya, baryo, grupo ng magkakaibigan) kapalit ng pagpapasimple ng komplikasyon at pagpapahusay ng privacy para sa mga gumagamit. Ito ay mga modular, open source na protocol para sa pag-iingat at pag-transact ng bitcoin sa konteksto ng komunidad. Interoperable ito sa mismong Lightning Network.

**Cashu** ay isang bearer token na maaaring itago sa isang device tulad ng mobile phone; ang disenyo ay layuning tularan ang mga benepisyo ng pisikal na pera ngunit sa digital na anyo. Ang Cashu ay isang halimbawa ng Chaumian eCash na nakabatay sa Bitcoin at nagpapataas ng privacy at censorship resistance at nagpapababa ng komplikasyon kapalit ng pagtitiwala sa eCash mint na ginagamit. Ang mga Cashu mint ay naglalabas ng eCash tokens, na kumakatawan sa bitcoin, na maaaring gastusin ng mga gumagamit nang hindi ibinubunyag ang kanilang pagkakakilanlan. Ang Cashu ay interoperable sa Lightning Network.

Malamang na marami pang layer 2 na aplikasyon ang itatayo sa hinaharap, at marami pang layer 3 na aplikasyon ang itatayo naman sa ibabaw ng bawat isa sa mga iyon.

Bilang halimbawa ng napakaraming aplikasyon na ginagawa sa ibabaw ng Lightning, narito ang isang bahagi mula sa Lightning Network Research Report ng River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
