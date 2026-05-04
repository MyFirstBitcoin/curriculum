# 9 - Paano Gumagana ang Pagmimina ng Bitcoin

Tagal: 90 minuto

Pangunahing Ideya: Ang pagmimina ng Bitcoin at pag-validate ng node ay magkasamang nagtutulungan upang tiyakin ang seguridad ng network, kumpirmahin ang mga transaksyon, at ipatupad ang mga patakaran ng sistema sa pamamagitan ng Proof of Work.

#### Mga Layunin sa Pagkatuto

Sa pagtatapos ng araling ito, dapat ay kayang gawin ng mga estudyante ang mga sumusunod:

* Ipaliwanag ang pagkakaiba ng papel ng mga Bitcoin node at ng papel ng mga Bitcoin miner.
* Ilarawan kung paano nagva-validate ng mga transaksyon ang mga node, nagbabahagi ng impormasyon, at tumutulong magpatupad ng mga patakaran ng Bitcoin.
* Ipaliwanag ang ginagawa ng mga miner, kabilang ang pagpili ng mga transaksyon, paggawa ng candidate blocks, at ang pakikipagpaligsahan upang makahanap ng valid na block hash.
* Ibigay ang kahulugan ng mempool at ipaliwanag kung bakit ito parang waiting room para sa mga hindi pa nakukumpirmang transaksyon.
* Ilarawan kung paano naaapektuhan ng transaction fees ang pagpili ng mga miner at ang bilis ng pagkumpirma.
* Ipaliwanag ang Proof of Work bilang mekanismo na nagsisiguro sa Bitcoin sa pamamagitan ng pagpapamahal ng mga pag-atake.
* Ilarawan kung paano nakakatulong ang difficulty adjustment upang mapanatili ang average na block time na humigit-kumulang 10 minuto.
* Ilakad ang buong siklo ng buhay ng isang Bitcoin transaksyon, mula sa paggawa at pag-sign hanggang sa pagkumpirma sa isang block.

#### Mga Kasangkapan at Sanggunian

##### Mga Visual Aid

* Kabanata 9 - Paano Gumagana ang Pagmimina ng Bitcoin?

##### Suportang Aklatan

* Vocabulary Reference Card — Kabanata 9 — Mga Termino: pagmimina, Proof of Work, hash puzzle, difficulty adjustment, block reward, mempool, 51% attack
* Misconceptions Libraries — Kabanata 9 — Tinutugunan: "gumagawa ng Bitcoin mula sa wala ang mga miner," "kontrolado ng mga miner ang Bitcoin," "mas maraming pagmimina = mas hindi ligtas"
* Mga Tsart ng Paghahambing at Reference Sheet — Ekonomiya ng pagmimina: kita, gastos, pag-align ng insentibo; difficulty adjustment
* Mga Teknikal na Paliwanag at Malalalim na Talakayan — Seguridad ng Proof of Work; bakit mahal ang pag-atake; 51% threshold

#### Mga Gawain

* Paggalugad sa Mempool
* Mga Transaksyon sa Aksyon

#### Online na Pagtuturo

* Gumamit ng isang malinaw na diagram ng daloy ng transaksyon mula sa pag-sign ng wallet hanggang sa pagkumpirma.
* Panatilihing malinaw na magkaiba ang mga node at miner sa screen sa buong aralin.
* Gamitin ang mempool.space o screenshot nito upang ipakita ang mga hindi pa nakukumpirmang transaksyon at pressure sa fees.
* Huminto pagkatapos ng bawat yugto ng proseso ng pagmimina at magtanong ng isang maikling tanong sa pag-unawa.

#### Paghahanda

* Maghanda ng diagram ng proseso ng pagmimina (mempool → pagpili ng transaksyon → paggawa ng block → difficulty adjustment) para ipakita.
* I-bookmark ang mempool.space o blockchain.com mining page; maghanda ng mga screenshot ng kasalukuyang mining stats at difficulty adjustments.
* Gumawa ng visual na paliwanag ng Proof of Work bilang mekanismo ng seguridad; ipakita ang difficulty adjustment sa nakaraang 3-6 buwan.

#### Pamamaraan

Ang araling ito ay masusing tumitingin kung paano gumagalaw ang mga Bitcoin transaksyon sa network at nagiging bahagi ng blockchain. Sinusundan na nito ngayon ang Diploma structure nang direkta kaya ang mga pangunahing seksyon ay naka-align sa student guide habang pinananatili pa rin ang mas malawak na paliwanag para sa guro sa bawat seksyon.

##### 9.0 Panimula, 8 minuto

Simulan sa pag-uugnay ng kabanatang ito sa naunang kabanata:

* Kung ang isang user ay nag-sign ng transaksyon gamit ang private key, ano ang susunod na mangyayari?
* Sino ang nagche-check kung valid ang transaksyong iyon?
* Paano ito nadaragdag sa blockchain?
* Bakit kailangan ng Bitcoin ng parehong node at miner?

Linawin na ipapaliwanag ng kabanatang ito kung paano pinoproseso ng network ang mga transaksyon sa aktwal at kung paano pinananatiling ligtas ng pagmimina ang sistema kahit walang sentral na awtoridad.

##### 9.1 Mga Bitcoin Node at Miner, 47 minuto

**Node at Miner, Magkaibang Papel**

Simulan sa malinaw na paghihiwalay ng dalawang papel.

Mga Bitcoin node:

* nag-iingat ng kopya ng blockchain
* nagsusuri kung sumusunod sa mga patakaran ang mga transaksyon
* nagbabahagi ng impormasyon sa ibang mga node
* tumutulong sa mga wallet at iba pang software na makakuha ng data mula sa blockchain
* maaaring tumanggi sa mga hindi valid na transaksyon o block

Inilalarawan ng kabanata ang mga node bilang mga tagapagbantay ng beripikasyon, at pinalalawak ito gamit ang analohiyang "digital traffic officer." Nakakatulong ito dahil ipinapakita nito ang mga node bilang mga tagasuri at tagapag-ugnay, hindi mga pinuno. Pinatitibay din ng diagram na maraming node ang nagtatago ng mga kopya ng ledger sa buong mundo.

Mga Bitcoin miner:

* nangongolekta ng mga balidong transaksyon
* nagbubuo ng mga kandidatong block
* nagpapaligsahan upang makahanap ng balidong block hash
* nagpapadala ng balidong block kapag nanalo sila
* tumatanggap ng gantimpala sa block at bayad sa transaksyon

Isang mahalagang punto ng pagtuturo mula sa kabanata ay ang layunin ng mining ay hindi lang basta lumikha ng bagong bitcoin, kundi upang idesentralisa ang seguridad ng Bitcoin. Ang bagong bitcoin ay insentibo, habang ang mismong proseso ng mining ang nagsisilbing mekanismo ng seguridad.

**Ano Talaga ang Ginagawa ng mga Node**

Palawakin ang seksyon ng node gamit ang listahan ng mga tungkulin ng node mula sa kabanata:

* Tagapagbantay ng beripikasyon: sinusuri nila na ang mga transaksyon at block ay sumusunod sa mga patakaran
* Sentro ng komunikasyon: nag-uugnayan sila sa isa't isa at nagbabahagi ng datos ng transaksyon
* Tagasuri ng kalidad: tinatanggihan nila ang maling impormasyon
* Tagapagbigay-impormasyon ng blockchain: nagbibigay sila ng datos sa ibang software tulad ng mga wallet
* Tagatanggap ng bagong node: tinutulungan nila ang mga bagong node na makuha ang blockchain, habang ang bawat bagong node ay nagsusuri pa rin ng datos nang mag-isa

Magandang pagkakataon ito upang bigyang-diin na ang pagpapatakbo ng node ay nagbibigay ng mas malaking kalayaan sa gumagamit. Sa halip na umasa lang sa mga panlabas na serbisyo para malaman ang estado ng network, maaari nilang beripikahin ito mismo. Malinaw na ipinapaliwanag ito ng kabanata, kabilang ang pagbanggit sa Bitcoin Core bilang isang implementasyon na maaaring patakbuhin ng mga gumagamit.

**Ano Talaga ang Ginagawa ng mga Miner**

Ngayon, ipaliwanag ang mining nang mas maingat.

Mga miner:

* nangongolekta ng mga napatunayan ngunit hindi pa nakukumpirmang transaksyon
* pinagsasama-sama ang mga ito sa isang kandidatong block
* paulit-ulit na hinahash ang datos ng block habang naghahanap ng balidong block hash
* ipinapadala ang nanalong block sa network
* kumukuha ng gantimpala kung tinanggap ang block

Gamitin ang analohiyang "malaking dayami ng mga susi" mula sa kabanata kung makakatulong. Nagbibigay ito ng konkretong larawan sa mga estudyante tungkol sa karera ng mining. Ang pangunahing ideya ay hindi na ang mga miner ay nagsosolve ng kapaki-pakinabang na math problem sa karaniwang kahulugan, kundi pinapatunayan nila na gumastos sila ng totoong enerhiya at computation upang mapanatiling ligtas ang sistema.

Ito rin ang tamang pagkakataon upang ipaliwanag ang gantimpala ng mga miner:

* gantimpala sa block: bagong nilikhang bitcoin
* bayad sa transaksyon: mga bayad na idinagdag sa mga transaksyon na nais ng mga gumagamit na makumpirma

Linawin na kadalasang inuuna ng mga miner ang mga transaksyon na may mas mataas na bayad, dahil pinapataas nito ang kanilang gantimpala. Ipinapaliwanag din ng kabanata ang mga halving dito, kaya maaari mong banggitin na ang gantimpala sa block ay nababawasan tuwing 210,000 block, mga bawat apat na taon, ayon sa pampublikong iskedyul ng suplay ng Bitcoin. Ang mga pahina 5 at 6 ay naglalaman ng iskedyul ng suplay at talahanayan ng susunod na halving, na makakatulong upang palakasin ang predictable na paglabas ng Bitcoin.

**Balidong Block Hash, Proof of Work, at Pag-aadjust ng Hirap**

Ang seksyong ito ang sentro ng kabanata.

Ipaliwanag na ang mga miner ay naghahanap ng balidong block hash, ibig sabihin, isang block hash na pumapasa sa target ng network. Ipinapaliwanag ito ng kabanata bilang paghahanap ng numerong mas mababa sa target na itinakda ng network.

Pagkatapos, ipaliwanag nang malinaw ang Proof of Work:

* kailangang magsagawa ng paulit-ulit na computational work ang mga miner
* ang unang makahanap ng balidong hash ay nagpapatunay na ginawa nila ang trabahong iyon
* ginagawa nitong magastos ang pagsubok na baguhin o atakihin ang ledger
* saka tinitingnan at bineberipika ng mga node ang block bago ito tanggapin

Isang malakas na linyang pampagtuturo ay:

Pinoprotektahan ng Proof of Work ang Bitcoin sa pamamagitan ng paggawa na magastos ang panlilinlang at madali ang beripikasyon.

Ipaliwanag din ang pag-aadjust ng hirap:

* inaadjust ng network ang hirap ng mining tuwing 2,016 block
* nangyayari ito mga bawat dalawang linggo
* ang layunin ay mapanatili ang average na oras ng block na malapit sa 10 minuto
* kung mas maraming hash power ang sumali sa network, tumataas ang hirap
* kung mas kaunti ang hash power, bumababa ang hirap

Ipinapaliwanag ng mga pahina 7 at 8 ang prosesong ito at ipinapakita kung paano ang mas mahirap na target ay nangangailangan ng mas maraming trabaho. Nakakatulong ito sa mga estudyante na maunawaan na ang timing ng Bitcoin ay hindi kinokontrol ng isang sentral na awtoridad kundi ng mga patakaran ng protocol na awtomatikong tumutugon sa kondisyon ng network.

##### 9.2 Ano ang Mempool?, 15 minuto

Ngayon, lumipat sa mempool.

Ipaliwanag na ang mempool ay ang waiting room para sa mga balido ngunit hindi pa nakukumpirmang transaksyon. Kapag nag-broadcast ang isang gumagamit ng transaksyon, unang bineberipika ito ng mga node. Kung ito ay balido, idinadagdag nila ito sa kanilang mempool at ibinabahagi sa ibang mga node. Pagkatapos, maaaring pumili ang mga miner mula sa mga naghihintay na transaksyon na iyon kapag bumubuo ng block. Ipinapaliwanag ng mga pahina 10 at 11 ang prosesong ito nang direkta.

Mahalagang mga puntong dapat bigyang-diin:

* ang mempool ay hindi ang blockchain
* ang mga transaksyon doon ay hindi pa nakukumpirma
* bawat node ay may sariling mempool
* walang iisang unibersal na mempool
* ang mga transaksyong may mas mataas na bayad ay mas malamang mapili agad

Ipinaliwanag din sa kabanatang ito ang mga karaniwang dahilan kung bakit maaaring manatiling hindi kumpirmado ang isang transaksyon nang matagal:

* mababang bayad
* siksikan ang network
* pagsubok na mag-double spend
* mali o kulang ang datos
* maling anyo ng transaksyon

Kung makakatulong, banggitin ang aktibidad gamit ang mempool.space bilang praktikal na paraan para makita ang mga hindi pa kumpirmadong transaksyon at mga rate ng bayad. Ipaliwanag din na ang mempool.space ay isa lamang explorer, hindi ang mismong mempool.

##### 9.3 Paano Gumagana ang Bitcoin Transactions, 20 minuto

Ngayon, pagsamahin ang lahat gamit ang sunud-sunod na proseso ng kabanata.

Isang malinaw na bersyon para sa klase ay:



1. Pinipili ng nagpadala ang isang UTXO at gumagawa ng transaksyon
1. Idinadagdag ng nagpadala ang address ng tatanggap at ang bayad
1. Nilalagdaan ng nagpadala ang transaksyon gamit ang kanilang private key
1. Ibinobroadcast ang transaksyon sa network
1. Sini-check ng mga node at idinadagdag sa kanilang mempools
1. Pinipili ito ng mga miner para sa candidate block
1. Nagpapaligsahan ang mga miner sa pamamagitan ng Proof of Work
1. Isang miner ang nakakahanap ng valid na block hash at ibinobroadcast ang block
1. Sini-check ng mga node ang block at idinadagdag ito sa blockchain
1. Nakakatanggap ng mga kumpirmasyon ang transaksyon habang nadaragdagan ang mga block
1. Gawing malinaw ang huling punto:
1. kapag naisama na ang transaksyon sa isang valid na block, ito ay kumpirmado na
1. hindi na magagamit ang mga nagastos na input
1. ang tumanggap ay may kontrol na sa mga bagong UTXO na nilikha ng transaksyong iyon

Lalo na kapaki-pakinabang ang summary diagram dito dahil ipinapakita nito nang biswal ang buong proseso mula sa pag-sign ng wallet hanggang sa pagsama ng miner, pag-validate ng node, at pagkalat ng block.

###### Pagwawakas at Pagsusuri ng Pagkaunawa

Tapusin gamit ang ilang mabilis na tanong:

* Ano ang pagkakaiba ng node at miner?
* Ano ang mempool?
* Bakit may mga transaksyong mas mabilis makumpirma kaysa sa iba?
* Ano ang pinapatunayan ng Proof of Work?
* Bakit ina-adjust ng Bitcoin ang hirap ng pagmimina?
* Ano ang mga pangunahing hakbang mula sa pagpapadala ng transaksyon hanggang sa pagtanggap ng kumpirmasyon?

#### Tala para sa Guro

Panatilihing malinaw ang pangunahing daloy ng pagtuturo: nagbe-verify ang mga node, naglalaban ang mga miner, ang Proof of Work ang nagsisiguro, at ang mempool ang nagtatago ng mga valid na transaksyon hanggang makumpirma ang mga ito.

Maaaring maging teknikal ang kabanatang ito, kaya gumamit ng mga analohiya at diagram nang madalas.

Iwasang ipaliwanag ang mining na parang "lumilikha ng bitcoin mula sa wala." Linawin na ang reward ay insentibo, habang ang proseso ng pagmimina ang nagsisiguro sa network.

Ang pinakamahalagang punto na dapat bigyang-priyoridad kung kapos sa oras ay:



1. Mga tungkulin ng node at miner
1. Mempool bilang waiting room
1. Proof of Work
1. Pag-aadjust ng hirap
1. Daloy ng transaksyon mula pag-sign hanggang kumpirmasyon

##### Ano ang Magandang Itsura

* Mahalagang agad linawin na Miners ≠ Nodes, ipakita ang mining bilang gawaing pang-ekonomiya na may totoong gastos sa hardware at kuryente, gamitin ang difficulty adjustment at Proof of Work para ipaliwanag ang mekanismo ng seguridad, at subukin ang pagkaunawa gamit ang mga scenario tungkol sa pagbabago sa network.
* Dapat gumamit ang mga guro ng totoong mga numero upang maging makatotohanan ang mga talakayan, maging malinaw at paulit-ulit sa pagpapaliwanag ng pagkakaiba ng Miners at Nodes, maging realistiko tungkol sa mga isyu ng sentralisasyon sa mining pools, at igalang ang tunay na kasalimuotan ng prosesong ito.
* Naiintindihan ng mga estudyante na ang mining ay ginagawa ng matatalinong tao na gumagawa ng komplikadong trabaho dahil kumikita sila ng Bitcoin, kinikilala na ang mga insentibo ang nagtutulak ng tapat na kilos dahil nakasalalay ang kita ng mga miner sa tagumpay ng Bitcoin, nakikita na ang sistema ay nag-aayos ng sarili sa pamamagitan ng awtomatikong pag-aadjust ng difficulty, nauunawaan na ang mining ay isang tunay na negosyo at hindi kawanggawa, at pinahahalagahan na ang seguridad ng Bitcoin ay may totoong gastos sa kuryente at pera.
* Makakamit ang mga Layunin sa Pagkatuto kung kayang makilala ng mga estudyante ang mga miner na lumilikha ng mga block mula sa mga node na nagva-validate nito, nauunawaan ang Proof of Work bilang mekanismo ng seguridad na nagpapamahal ng husto sa mga atake, kinikilala na ang difficulty adjustment ang nagpapanatili ng block time sa humigit-kumulang 10 minuto, nauunawaan ang mga insentibo ng mga miner sa block rewards at fees, maipaliwanag kung bakit hindi gumagana ang 51% attack, at makita ang mining bilang isang gawaing pang-ekonomiya na may tunay na gastos at benepisyo.

##### Pamamahala ng Oras

Kung kapos sa oras, unahin ang:

* Mga papel ng node at miner (ang mahalagang pagkakaiba)
* Mempool bilang waiting room
* Mekanismo ng Proof of Work
* Difficulty adjustment (nag-aayos ang sistema ng sarili nito)
* Daloy ng transaksyon mula sa pag-sign hanggang sa kumpirmasyon

Kung maaga, maglaan ng oras sa:

* Ekonomiya ng mining at mga detalye ng hardware
* Dynamics ng mining pool at mga isyu ng sentralisasyon
* Mga senaryo ng 51% attack at kung bakit ito nabibigo sa matematika
* Pangmatagalang seguridad sa pamamagitan ng pagkaka-align ng mga insentibo

##### Kung Nahihirapan ang mga Estudyante

* Miners vs. nodes (kalituhan) → "Nodes ang nagva-validate, miners ang nagpo-propose; mga referee vs. mga manlalaro."
* Proof of Work nakakaaksaya → "Mahal ang seguridad para maiwasan ang mga atake; ginagawa nitong walang saysay ang mga ito."
* Difficulty adjustment → "Mas maraming miner = mas mabilis ang mga block = tumataas ang difficulty; parang humihinga ang sistema."
