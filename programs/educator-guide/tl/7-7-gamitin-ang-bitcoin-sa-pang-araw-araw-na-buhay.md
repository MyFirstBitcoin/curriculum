# 7 - Gamitin ang Bitcoin sa Pang-araw-araw na Buhay

Tagal: 90 minuto

Pangunahing Ideya: Ginagawang mas praktikal ng Lightning Network ang Bitcoin para sa araw-araw na bayaran sa pamamagitan ng mas mabilis at mas murang mga transaksyon habang nananatiling pundasyon ang Bitcoin.

#### Mga Layunin sa Pagkatuto

Sa pagtatapos ng araling ito, dapat ay kayang gawin ng mga estudyante ang mga sumusunod:

* Ipaliwanag kung ano ang Lightning Network at kung bakit ito itinayo sa ibabaw ng Bitcoin.
* Ihambing ang on-chain at Lightning na mga transaksyon ayon sa bilis, gastos, at mga kompromiso sa seguridad.
* I-distingguish ang custodial at self-custodial na Lightning wallets, at ipaliwanag kung bakit mahalaga ang self-custody.
* Mag-set up ng Lightning wallet at ilarawan ang papel ng seed phrase sa pag-recover ng wallet.
* Ipakita kung paano gumagalaw ang Lightning payments sa network, kahit hindi direktang konektado ang dalawang user.
* Tukuyin ang mga totoong paraan kung paano magagamit ang Bitcoin sa araw-araw sa pamamagitan ng Lightning, tulad ng kape, grocery, bayad sa tindahan, at lokal na paggastos.
* Ipaliwanag kung paano nakakatulong ang mga tool tulad ng BTCPay Server, BTCMap, at gift cards sa pagpapalawak ng paggamit ng Bitcoin sa aktwal na buhay.
* Ilarawan kung ano ang Bitcoin circular economy at kung bakit ginagawang mas posible ito ng Lightning.

#### Mga Kasangkapan at Resources

##### Mga Visual Aid

* Kabanata 7 - Paggamit ng Bitcoin sa Pang-araw-araw na Buhay

##### Suportang Aklatan

* Vocabulary Reference Card — Mga Termino: Lightning Network, payment channel, routing, Layer 2, circular economy, remittance
* Mga Halimbawa at Kaso sa Tunay na Buhay — El Salvador, Austin circular economy, mga kwento ng pagtanggap ng Lightning ng mga negosyante
* Mga Tsart ng Paghahambing at Reference Sheet — On-Chain vs. Lightning na paghahambing; Paghahambing ng Bayad at Bilis sa iba't ibang paraan ng pagbabayad
* Lightning Network Simplified Explainer — Paano gumagana ang payment channels nang walang jargon; routing; seguridad; mga gamit
* Payment Scenario Walkthroughs — Step-by-step: magpadala sa kaibigan, tumanggap ng bayad, remittance, tumanggap bilang freelancer
* Fee & Speed Comparison Tool — Kailan gagamitin ang Lightning vs. on-chain vs. banking (may mga halimbawa ng gastos)

#### Mga Gawain

* Lightning Relay Race

#### Online na Pagtuturo

* Gumamit ng side-by-side na comparison slide para sa on-chain at Lightning na bayad.
* Magsimula sa isang totoong halimbawa tulad ng kape o remittance para maintindihan ng mga estudyante kung bakit umiiral ang Lightning.
* Gumamit ng simpleng diagram ng routing na may tatlong tao para malinaw ang paliwanag ng network.
* Panatilihing simple ang mechanics ng channel maliban kung may matibay nang pundasyon ang klase.

#### Paghahanda

* I-download ang Lightning wallet at maghanda ng mga screenshot na nagpapakita ng on-chain (mabagal) vs. Lightning (mabilis) na bilis ng transaksyon na magkatabi.
* Mag-research ng 2-3 totoong negosyante o komunidad na gumagamit ng Lightning; i-bookmark ang BTCMap.org bilang reference.
* Maghanda ng on-chain vs. Lightning na comparison chart (bilis, bayad, seguridad, gamit) para ipamahagi.

#### Pamamaraan

Ipinapakita ng araling ito sa mga estudyante kung paano nagiging praktikal ang Bitcoin para sa araw-araw na bayaran sa pamamagitan ng Lightning Network. Ang gabay ay sumusunod na ngayon sa Diploma structure kaya ang mga pangunahing bahagi ng Lightning ay tumutugma sa student guide, habang ang mga paghahambing, tools ng negosyante, at materyal tungkol sa circular economy ay nananatili kung saan sila nararapat.

##### 7.0 Panimula, 8 minuto

Magsimula sa pag-uugnay ng kabanatang ito sa naunang kabanata:

* Kung gumagana ang Bitcoin on-chain, bakit kailangan pa ng isa pang layer?
* Ano ang mangyayari kapag gusto ng mga tao na gumawa ng maraming maliliit na bayad nang mabilis?
* Anong uri ng sistema ng bayad ang mas babagay para sa kape, grocery, o pagbabayad sa kaibigan?

Linawin na ang kabanatang ito ay nakatuon sa paggamit ng Bitcoin sa araw-araw, lalo na kapag mahalaga ang bilis at mababang bayad. Ipaliwanag na ang Lightning ay itinayo sa ibabaw ng Bitcoin, hindi hiwalay dito.

##### 7.1 Ang Lightning Network, 25 minuto

**Ano ang Lightning Network**

Ipaliwanag na ang Lightning Network ay isang sistema ng bayad na itinayo sa ibabaw ng Bitcoin na nagpapahintulot sa mga user na magpadala at tumanggap ng bitcoin nang mabilis at mura. Gumagana ito sa pamamagitan ng paglipat ng maraming maliliit na bayad sa labas ng pangunahing blockchain at tanging ang huling resulta lamang ang isinasara on-chain kalaunan.

Isang kapaki-pakinabang na paraan ng pagpapaliwanag nito ay ang café tab analogy mula sa kabanata:

* sa halip na magbayad ng bawat item isa-isa on-chain
* magbubukas ng channel ang dalawang partido
* ina-update nila ang balanse habang sila ay nagta-transact
* tanging ang huling balanse lamang ang itinatala sa blockchain kapag isinara na ang channel

Dahil dito, mas mabilis at mas mura ang Lightning para sa madalas na maliliit na bayad. Linawin din na ang Lightning payments ay maaaring dumaan sa network, kaya hindi kailangan ng user na may direktang channel sa bawat taong babayaran niya.

**On-chain vs Lightning**

Ngayon, gawing napakalinaw ang pagkakaiba.

On-chain na mga transaksyon

* nangyayari direkta sa Bitcoin blockchain
* karaniwang mas mabagal
* nakadepende sa pagpasok at pagkumpirma sa block
* mas madalas na mas ligtas
* maaaring mas mahal depende sa fees

Lightning na mga transaksyon

* nangyayari sa isang second layer na nakapatong sa Bitcoin
* mas mabilis ang settlement
* karaniwang mas mura ang bayad
* kapaki-pakinabang para sa maliliit at madalas na bayad
* may mga kapalit na trade-off kumpara sa on-chain settlement

Panatilihing simple ang pangunahing punto: mas matibay ang on-chain para sa final settlement, mas malakas ang Lightning para sa bilis at murang pang-araw-araw na gamit. Napakahalaga ng paghahambing dito.

##### 7.2 Iba't Ibang Uri ng Lightning Wallets, 10 minuto

Ipaliwanag na ang Lightning wallet ay gumaganap ng parehong pangunahing tungkulin ng isang Bitcoin wallet, tumatanggap at nagpapadala ng bitcoin, ngunit ito ay dinisenyo para gamitin sa Lightning Network. Pagkatapos, talakayin ang pangunahing pagkakaiba ng mga wallet sa kabanatang ito:

* self-custodial: ang user ang may hawak ng mga susi
* custodial: ibang tao ang may hawak ng mga susi

Linawin ang pangunahing trade-off:

* maaaring mas madali at mas maginhawa ang custodial wallets
* ngunit ang user ay umaasa sa pahintulot at kontrol ng iba
* ang self-custodial wallets ay nagbibigay ng mas malaking pagmamay-ari at kalayaan

Palakasin din ang rekomendasyon ng kabanata na mas piliin ang open-source wallets, dahil ang open-source na mga tool ay maaaring suriin, pagbutihin, at beripikahin ng komunidad.

##### 7.3 Pag-setup ng Bitcoin Lightning Wallet, 10 minuto

Ilakad ang mga estudyante sa pangunahing proseso ng pag-setup:

* i-download ang Lightning wallet
* gumawa ng bagong wallet
* isulat ang recovery phrase
* kumpirmahin ang mga salita sa tamang pagkakasunod-sunod
* magdagdag ng dagdag na seguridad kung pinapayagan ng wallet
* simulan nang gamitin ang wallet

Maging malinaw lalo na tungkol sa seed phrase:

* ito ang nagpapahintulot sa user na mabawi ang access
* kung ito ay mawala, maaaring mawala rin ang access sa pondo
* kung makuha ito ng ibang tao, maaari nilang kontrolin ang pondo

Dapat bigyang-diin ng seksyong ito ang responsibilidad at tamang paghawak, tulad ng sa on-chain na kabanata.

##### 7.4 Pagpapadala at Pagtanggap ng Lightning Transactions, 17 minuto

**Paano Gumagana ang Lightning Transactions sa Praktika**

Gamitin ang halimbawa nina Marcia, Jeff, at Eve para ipaliwanag ang routing. Hindi kailangan ni Marcia ng direktang channel kay Eve. Maaaring dumaan ang kanyang bayad kay Jeff, na konektado sa network, at makarating pa rin kay Eve nang ligtas.

Gawing malinaw ang mga puntong ito:

* Maaaring dumaan ang Lightning payments sa mga tagapamagitan
* ang mga tagapamagitan ay tumutulong mag-route ng bayad
* ang routing process ay hindi nangangahulugang nagtitiwala ang mga user sa bangko o sentralisadong payment processor
* gumagamit ang network ng cryptography para makarating ang bayad sa tamang tatanggap

Nakakatulong ito para maunawaan ng mga estudyante na peer-to-peer pa rin ang Lightning, kahit dumadaan ang bayad sa mas malawak na network. Kung makakatulong, banggitin na nabanggit din sa kabanata na maaaring kumita ng fees ang mga node operator at makatulong palakasin ang network sa pag-route ng bayad.

**Pagpopondo ng Channels at Paulit-ulit na Paggamit ng Lightning**

Ipaliwanag pa ang halimbawa ni Mina:

* Inililipat ni Mina ang bitcoin mula sa kanyang on-chain wallet papunta sa kanyang Lightning wallet
* ito ang nagpopondo sa payment channel
* maaari na siyang gumawa ng paulit-ulit na bayad nang hindi na kailangang buksan muli ang proseso sa bawat pagkakataon
* kapag nagsara ang channel, ang huling balanse ay inaayos pabalik sa on-chain

Ipaliwanag nang malinaw ang isang mahalagang limitasyon: ang mga pondo na naka-lock sa isang aktibong channel ay ginagamit para sa Lightning at hindi malayang magagamit para sa hiwalay na on-chain na paggamit sa parehong oras. Nakakatulong ito sa mga estudyante na maunawaan na makapangyarihan ang Lightning, ngunit may kakaibang istruktura ng pagbabayad ito.

##### 7.5 Pagbili ng Kape at Grocery gamit ang Bitcoin, 20 minuto

**Pang-araw-araw na Gamit**

Lumipat mula sa mekanika papunta sa totoong buhay.

Ipaliwanag na ang Lightning ay lalo nang kapaki-pakinabang para sa:

* pagbili ng kape
* grocery
* pamimili
* pagbabayad sa mga kaibigan
* pang-araw-araw na maliliit na transaksyon

Ang halimbawa ni Mina sa kabanata ay tumutulong ipakita kung bakit mas angkop ang Lightning kaysa sa tradisyonal na mga paraan ng pagbabayad sa maraming sitwasyon: ito ay mabilis, mababa ang bayad, walang hangganan, at abot-kaya kahit sa mga taong walang bank account. Ang talahanayan ng paghahambing at ang diagram ng pagproseso ng bayad ay malalakas na pantulong sa pagtuturo dito, lalo na sa pagpapakita kung gaano karaming tagapamagitan ang mayroon sa tradisyonal na card payments.

**Mga Kasangkapan ng Negosyante at Pag-gastos ng Bitcoin sa Totoong Mundo**

Ngayon, ipaliwanag kung paano maaaring gawing praktikal ng mga negosyo at gumagamit ang Lightning sa araw-araw.

Talakayin ang tatlong pangunahing kasangkapan o paraan sa kabanata:

BTCPay Server

* open-source na payment processor
* pinapayagan ang mga negosyante na tumanggap ng bitcoin nang direkta
* walang middleman na kumokontrol sa pondo
* kapaki-pakinabang para sa online at personal na bayad ng negosyo

BTCMap

* tumutulong sa mga gumagamit na makahanap ng mga negosyante at komunidad na tumatanggap ng bitcoin
* pinapayagan ang mga tao na maghanap sa kanilang lugar
* maaaring i-update ng komunidad

Gift card at voucher

* pansamantalang mga kasangkapan para magastos ang bitcoin kung saan hindi pa direktang tinatanggap
* tumutulong magtulay habang lumalago ang pagtanggap

Mahalaga ang seksyong ito dahil ipinapakita nito sa mga estudyante na ang paggamit ng Bitcoin ay hindi lang teorya. May mga totoong kasangkapan na magagamit ng mga tao ngayon.

**Circular na Ekonomiya at Bitcoin bilang Daluyan ng Palitan**

Tapusin ang pangunahing nilalaman sa pagpapaliwanag na ang circular economy ay isang komunidad kung saan sinusubukan ng mga kalahok na bumili at magbenta sa isa't isa hangga't maaari. Kapag inangkop sa Bitcoin, ibig sabihin nito ay pinipili ng mga negosyante, manggagawa, at gumagamit na magtransaksyon gamit ang bitcoin at suportahan ang isa't isa sa ekonomiya.

Ipaliwanag kung bakit mahalaga ang Lightning dito:

* ang mga bayad ay halos instant
* mababa ang bayad
* nagiging praktikal ang maliliit na bayad
* mas madaling mapanatili ang lokal na kalakalan

Maaari mong banggitin na tinutukoy ng kabanata ang mga halimbawa tulad ng Arnhem at Bitcoin Beach, na nagpapakita na ang circular economies ay hindi haka-haka. Umiiral na sila at patuloy na lumalago. Lalo nang kapaki-pakinabang dito ang visual timeline.

###### Pagwawakas at Pagsusuri ng Pagkaunawa

Tapusin gamit ang ilang mabilis na tanong:

* Bakit itinayo ang Lightning Network?
* Ano ang isang malaking pagkakaiba ng on-chain at Lightning na mga bayad?
* Bakit mahalaga ang self-custody sa isang Lightning wallet?
* Paano makakatanggap ng Lightning payment ang isang tao kahit walang direktang channel sa bawat tao?
* Ano ang Bitcoin circular economy?

#### Tala para sa Guro

Panatilihing malinaw ang pangunahing aral: Ang Bitcoin ang base layer, ang Lightning ay tumutulong gawing mas mabilis at mas mura ang pang-araw-araw na bayad.

Dapat maging praktikal at kongkreto ang kabanatang ito, hindi masyadong teknikal.

Bigyang prayoridad ang pag-unawa kaysa sa malalim na mekanika ng channel.

Ang pinakamahalagang punto na dapat bigyang prayoridad, kung kapos sa oras, ay:

* ano ang Lightning
* mga kompromiso sa pagitan ng on-chain at Lightning
* pag-aalaga at pag-setup ng wallet
* mga totoong bayad sa totoong buhay
* mga paikot na ekonomiya

Ang pinaka-kapaki-pakinabang na mga visual sa kabanatang ito ay:

* ang paghahambing ng on-chain at Lightning
* ang mga pagkakaiba ng wallet
* ang routing na halimbawa kina Marcia, Jeff, at Eve
* ang talahanayan ng paghahambing at tsart ng kapasidad
* ang tradisyonal na diagram ng pagproseso ng bayad
* ang timeline ng paikot na ekonomiya

##### Ano ang Magandang Itsura

* Mahalagang magsimula sa sakit na punto na "Ang Bitcoin ay tumatagal ng 10 minuto at nagkakahalaga ng ₱100," ipaliwanag ang Lightning bilang mabilis na daan sa ibabaw ng Bitcoin, gumamit ng totoong halimbawa mula sa mga negosyante at remittance corridors, at gumawa ng mga decision tree kung kailan gagamitin ang on-chain kumpara sa Lightning.
* Dapat maging praktikal ang mga guro tungkol sa kung ano talaga ang nalulutas ng Lightning, magbahagi ng mga kwento mula sa aktwal na paggamit ng Bitcoin, maging malinaw sa mga partikular na kompromiso, at manatiling realistiko sa pag-ampon habang nananatiling masigasig sa mga posibilidad.
* Nakikita ng mga estudyante ang aktwal na paggana ng Bitcoin para sa totoong bayad sa totoong lugar, nauunawaan na mahalaga ang bilis at gastos sa mga bayad, naiisip ang paikot na ekonomiya kung saan nananatili ang Bitcoin sa lokal, nakikilala na ang Lightning ≠ Bitcoin (magkaibang gamit para sa magkaibang layunin), at nagiging mausisa tungkol sa mga sistemang pang-ekonomiya na nakabatay sa mga bayad gamit ang Bitcoin.
* Makakamit ang mga Layunin sa Pagkatuto kung maipapaliwanag ng mga estudyante ang Lightning Network bilang layer sa ibabaw ng Bitcoin, nauunawaan ang mga pangunahing konsepto ng payment channels at routing, nakikita ang mga totoong gamit ng Lightning payments, naihahambing ang on-chain at Lightning para sa iba't ibang sitwasyon, nauunawaan ang konsepto ng paikot na ekonomiya, at nakikilala ang mga partikular na kompromiso ng bawat paraan.

##### Pamamahala ng Oras

Kung kulang ang oras, bigyang-priyoridad ang:

* Ano ang Lightning
* Mga kompromiso ng On-chain at Lightning
* Totoong bayad sa totoong buhay
* Paikot na ekonomiya

Kung may sobra pang oras, maglaan ng panahon sa:

* Mekaniks ng payment channel at routing
* Kasangkapan sa paghahambing ng bayad at bilis
* Mga pag-aaral ng kaso ng paikot na ekonomiya sa El Salvador at Austin
* Mga walkthrough ng praktikal na Lightning payment scenario

##### Kung Nahihirapan ang mga Estudyante

* Bakit umiiral ang Lightning → Ihambing: 10 min/₱100 vs. ilang segundo/barya.
* Payment channels → Analohiya ng utang sa kape; magsettle muna sa loob bago sa Bitcoin.
* Bakit mahalaga sa buong mundo → "Paano kung walang bangko pero may Bitcoin?"
