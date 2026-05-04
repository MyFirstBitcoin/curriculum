# 3.4 Hashcash

Ang Hashcash ay nilikha ni Adam Back, isa pang maagang innovator sa larangang ito. Malaki ang interes ni Adam sa malayang pamilihan at privacy sa internet, at nadiskubre niya ang Cypherpunks mailing list na kanyang sinalihan at naging aktibong kalahok.

Interesado siya nang husto sa digital na pera, at nagbigay siya ng ilang suhestiyon kung paano maaaring mas magtulungan ang grupo sa DigiCash kasama si Chaum, ngunit hindi ito nagbunga. Pagkatapos, inilipat niya ang kanyang atensyon sa isa pang lumalabas na problema – spam sa email. Gusto nilang mga Cypherpunks na makahanap ng solusyon sa spam, kung saan napakadaling gumawa at magpadala ng libu-libong email na bumabara sa mga network. Ang kanyang makabagong solusyon ay nakabatay sa hashing – ang kakayahan ng cryptography na gawing natatangi at random na string ng tiyak na haba ang anumang datos, upang lumikha ng katumbas ng digital na 'selyo' na kailangang idagdag sa email para ito ay tanggapin at maipadala sa network. Maliit na gastos para sa totoong email, ngunit hadlang para sa spammer.

Ang pangunahing inobasyon na nilikha ng Hashcash ay ang pag-uugnay ng totoong yaman—computational power—sa isang digital na network. Habang ang mga digital na yaman noon ay maaaring ulit-ulitin nang walang hanggan, ang bilang ng 'hashcash' na nalilikha ay nililimitahan ng kung gaano karaming enerhiya ang handang ilaan ng mga tao rito.

Bagamat natugunan ng solusyon ang ilan sa mga pamantayan na pinaniniwalaan ni Adam na kailangan sa isang digital cash system; ito ay anonymous, matibay at trustless, ang bawat hashcash ay hindi maaaring gamitin muli at hindi tunay na kakaunti. Nagmungkahi siya ng ibang paraan upang matugunan ang mga isyung ito gamit ang mga panlabas na third party.

##### BitGold

Pinagyaman ni Nick Szabo ang konsepto ng Hashcash at proof of work upang magmungkahi ng alternatibong solusyon, na inilarawan niya sa isang mailing list isang taon matapos mailathala ang Hashcash, noong 1998.

Habang papalapit sa solusyon, marami pa ring hamon ang panukalang ito.

* Sino ang magpapatakbo ng Registry ng pagmamay-ari ng hash at paano sila mapagkakatiwalaan?
* Ang hashing ay karaniwang bumababa ang halaga sa paglipas ng panahon, isang hamon din para sa HashCash.

Dahil ang mga magkakaugnay na hash ay may time-stamp, iminungkahi niya ang isang uri ng historical tracking ng hirap ng hashing noon; ang mas naunang hash ay mangangailangan ng mas mataas na processing cost kaysa sa mas huli dahil bumaba na ang gastos. Sa kasamaang palad, ibig sabihin nito ay hindi magiging 'fungible' ang mga hash, ibig sabihin ay hindi pantay-pantay ang halaga, na itinuturing na mahalagang katangian ng digital na pera. Upang makatulong na maresolba ito, iminungkahi ni Nick ang isang uri ng 'free banking' na gagana sa ibabaw ng BitGold na maaaring magtipon ng iba't ibang grupo ng hash na pareho ang halaga.

##### B-Money

Hindi nagtagal matapos ang panukala ng Bit Gold, nagmungkahi si Wei Dai ng katulad na solusyon. Nakagawa na siya ng ilang iba pang mga tool para sa mga Cypherpunks, at may sarili siyang mga ideya tungkol sa digital na pera.

Kawangis ng Bit Gold ang kanyang panukala dahil gumagamit ito ng digital signatures upang maglipat ng pera, at ang mga tala ng transaksyon ay itatala sa isang ledger, na naglalaman ng mga public key at halaga ng currency units na nakatalaga sa bawat isa. Tulad ng sa Bit-Gold, itinuturing na butas sa seguridad ang mga pinagkakatiwalaang third party, at ang paniniwala ay hindi dapat umasa ang isang electronic cash system sa iisang entidad upang subaybayan ang balanse, transaksyon o upang maiwasan ang double spend.

Nagmungkahi si Wei-Dai ng ilang solusyon sa mga isyung ito, isa na rito ay imbes na isang sentral na entidad(ies) ang magpanatili ng ledger, LAHAT ng nodes ay magtatago ng kopya. Kung lahat ng user ay susuriin ang sarili nilang ledger at ang bisa ng bawat transaksyon, basta't lahat ng nodes ay napapanahon, mananatiling magkatugma ang mga ledger sa buong network. Ang ganitong kalawak na distributed na sistema ay mahirap dayain.

Napansin ni Wei Dai na hindi nito nalulutas ang Byzantine generals problem (1), dahil madaling mawalan ng synchronisation ang mga node o magsinungaling lang. Nagmungkahi siya ng alternatibong paraan tulad ng pagkakaroon ng subset ng 'pinagkakatiwalaang' mga server na magpapanatili ng ledger, at paglikha ng mga insentibong pinansyal upang mapanatiling tapat ang mga server na ito.

Para sa patakarang pananalapi, iminungkahi niyang i-peg ang purchasing power ng B-Money sa isang uri ng panlabas na consumer price index. Gusto niyang ang parehong halaga ng B-Money ay makabili ng pantay na bahagi ng index sa paglipas ng panahon, upang magkaroon ng kaunting price stability. Kaya, sinuman ay maaaring lumikha ng bagong currency units sa pamamagitan ng pagbibigay ng valid na hash, ngunit maaaring magbago ang hirap ng paglikha ng hash batay sa gastos ng CPU at price index, upang ang bawat unit ay maging 'immutable'.
