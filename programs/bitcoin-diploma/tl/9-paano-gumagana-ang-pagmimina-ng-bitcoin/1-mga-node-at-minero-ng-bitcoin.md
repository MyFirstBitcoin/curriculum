# 9.1 Mga Node at Minero ng Bitcoin

Maaaring mukhang teknikal ang mga Bitcoin node, ngunit ito ay simpleng software lamang na nagtatago ng kopya ng Bitcoin blockchain sa isang computer. Ang blockchain ay isang pinagsasaluhang talaan ng lahat ng transaksyon sa Bitcoin.

Kapag nagpapatakbo ka ng sarili mong node, ikaw mismo ang nagbeberipika ng mga transaksyon sa Bitcoin sa halip na umasa sa iba. Nagbibigay ito sa iyo ng mas malaking kalayaan at tumutulong na mapanatiling desentralisado ang Bitcoin network.

Maaari mong isipin ang isang Bitcoin node bilang isang digital na traffic officer na may ilang mahahalagang tungkulin.

1. Nagtatago ito ng kopya ng blockchain, na siyang kasaysayan ng lahat ng transaksyon sa Bitcoin.
1. Ang mga node ay kumokonekta sa iba pang mga node sa buong mundo at nagbabahagi ng impormasyon. Isang halimbawa nito ay ang listahan ng mga bagong transaksyon na naghihintay na makumpirma, na tinatawag na mempool.
1. Sinusuri ng mga node na ang bawat transaksyon ay sumusunod sa mga patakaran ng Bitcoin. Kung ang isang transaksyon ay hindi wasto, tinatanggihan ito ng node.

Tumutulong din ang mga node sa mga bagong node na sumali sa network sa pamamagitan ng pagbabahagi ng blockchain sa kanila. Gayunpaman, ang bawat bagong node ay nagsusuri pa rin ng lahat ng patakaran nang mag-isa.

Kahit sino ay maaaring magpatakbo ng node sa pamamagitan ng pag-install ng software tulad ng Bitcoin Core at pag-download ng blockchain. Kapag ito ay na-set up na, patuloy na tumatanggap ang node ng mga bagong block kada humigit-kumulang 10 minuto at sinusuri ang mga ito bago idagdag sa sariling kopya ng blockchain.

Ang pagpapatakbo ng node ay tumutulong gawing mas ligtas at desentralisado ang Bitcoin network, dahil mas maraming tao ang nagsasariling nagbeberipika ng sistema.

#### Ano ang Bitcoin Node?

> Ang layunin ng mining ay hindi ang paglikha ng bagong bitcoin; iyon ay bahagi ng insentibo. Ang mining ang mekanismo kung paano nade-desentralisa ang seguridad ng Bitcoin.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Kinokolekta ng mga miner ang mga hindi pa nakukumpirmang transaksyon, bumubuo ng isang block, at gumagamit ng enerhiya upang makahanap ng susi na magdadagdag at magse-secure ng block.


Nagpapaligsahan ang mga miner na maidagdag ang susunod na block ng mga transaksyon sa blockchain. Para magawa ito, kailangan nilang makahanap ng espesyal na numero na lilikha ng wastong block hash. Maaari mo itong isipin na parang naghahanap ng tamang susi sa bilyun-bilyong posibilidad. Ang unang miner na makahanap ng tamang hash ang nananalo at nagkakaroon ng karapatang idagdag ang kanilang block sa blockchain.

Kapag nakahanap ang isang miner ng wastong hash, ibinabahagi nila ang kanilang block sa network. Mabilis na tinitiyak ng ibang mga miner na tama ang solusyon. Kung tama ito, idinadagdag ang block sa blockchain, na tumutulong panatilihing ligtas ang pampublikong ledger ng Bitcoin.

Kumita ang mga miner ng bitcoin sa dalawang paraan:

* **Block rewards:** Ang mga bagong bitcoin ay nililikha at ibinibigay sa miner na matagumpay na nakapagdagdag ng block sa blockchain.
* **Mga bayad sa transaksyon:** Kapag nagpapadala ng bitcoin ang mga tao, naglalakip sila ng maliit na bayad. Ang miner na nagdagdag ng block ang tumatanggap ng mga bayad mula sa mga transaksyong kasama sa block na iyon.

#### Mga Halving ng Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12.5 BTC | 6.25 BTC | 3.125 BTC |



> **Callout**
>
> Ang gantimpala ng mga miner para sa bawat natapos na block ay nababawasan ng kalahati bawat 210,000 blocks, mga bawat apat na taon.


May nakatakdang pinakamataas na supply ang Bitcoin na 21,000,000 bitcoin, ngunit hindi lahat ay nilikha noong nagsimula ang Bitcoin. Sa halip, unti-unting ipinapakilala ang mga bagong bitcoin sa sirkulasyon sa pamamagitan ng **mining**.

Kapag matagumpay na nadagdag ng mga miner ang bagong block ng mga transaksyon sa Bitcoin network, nakakatanggap sila ng **block reward** na bitcoin. Noong mga unang araw ng Bitcoin, ang gantimpalang ito ay 50 bitcoin bawat block. Ang gantimpalang ito ang nag-udyok sa mga tao na gumamit ng computing power at kuryente upang makatulong sa seguridad ng network.

Mga bawat 210,000 blocks (humigit-kumulang bawat 4 na taon), ang block reward ay nababawasan ng kalahati. Ang pangyayaring ito ay tinatawag na **halving**. Pinapabagal ng halving ang paglikha ng mga bagong bitcoin at tumutulong matiyak na hindi lalampas sa 21 milyon ang kabuuang supply. Sa paglipas ng panahon, nagiging mas kakaunti at mahalaga ang bitcoin.


> **Definition – Circulating supply**
>
> **Ang circulating supply** ay tumutukoy sa kabuuang dami ng isang currency na magagamit. Sa Bitcoin, ang kabuuang circulating supply ay ang bilang ng mga coin na namina at nasa sirkulasyon sa anumang oras.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/f6d523f2e94734fe510bcf760ac287bfb3aca844-292x200.svg)


> **Definition – Iskedyul ng supply ng Bitcoin**
>
> Ang **iskedyul ng supply ng Bitcoin** ay ang nakatakda at pampublikong plano para sa pagpapalabas ng mga bagong bitcoin sa sirkulasyon, na idinisenyo upang mapanatili ang kakulangan ng Bitcoin sa paglipas ng panahon.


Pagkatapos ng bawat halving event, ang gantimpala ng bitcoin na natatanggap ng mga miner para sa pagdagdag ng block ay nababawasan ng kalahati. Binabawasan nito ang bilis ng paglikha ng mga bagong bitcoin.

Patuloy pa ring kumikita ang mga miner mula sa mga bayad sa transaksyon na kasama sa block na kanilang namina. Sa paglipas ng panahon, inaasahang magiging mas malaking bahagi ng kita ng mga miner ang mga bayad na ito.

Ang mga halving ay nakaprograma sa Bitcoin protocol at nangyayari ito nang awtomatiko tuwing apat na taon. Dahil dito, ang iskedyul ng suplay ng Bitcoin ay tiyak at malinaw.

Ipinapakita ng talahanayan ang mga paparating na halving, kabilang ang tinatayang petsa, ang block number kung kailan ito magaganap, ang bagong gantimpala sa bawat block, at ang porsyento ng kabuuang suplay ng bitcoin na namina na.


| Kaganapan | Petsa | Block | Gantimpala | Namina |
| --- | --- | --- | --- | --- |
| Ika-5 Halving | 2028 | 1,050,000 | 1.5625 BTC | 98.44 % |
| Ika-6 Halving | 2032 | 1,260,000 | 0.78125 BTC | 99.22 % |
| Ika-7 Halving | 2036 | 1,470,000 | 0.390625 BTC | 99.61 % |


Habang mas maraming bitcoin ang namimina, patuloy na tumataas ang umiikot na suplay hanggang sa maabot ang pinakamataas na suplay na 21,000,000 bitcoins, na inaasahang mangyayari sa paligid ng taong 2140. Dahil mas kaunti ang nalilikhang bagong bitcoin sa paglipas ng panahon, kung tataas ang demand, maaaring tumaas ang presyo ng Bitcoin. Hinihikayat din nito ang mga miner na patuloy na siguraduhin ang seguridad ng network sa pamamagitan ng pagbibigay ng kanilang computing power.

#### Ano ang isang valid block hash sa Bitcoin?

Sa Bitcoin, ang mga miner ay nag-uunahan upang makahanap ng isang espesyal na code na tinatawag na **block hash**. Ang code na ito ang tumutukoy sa isang block ng mga transaksyon at nagpapahintulot na maidagdag ito sa blockchain.

Ang bawat block ay naglalaman ng impormasyon tungkol sa mga kamakailang transaksyon at kasama rin ang hash ng nakaraang block. Pinagdurugtong nito ang bawat block, na bumubuo ng isang chain mula sa pinakaunang block (ang Genesis Block) hanggang sa pinakabago.

Ang hash ay parang isang **digital na fingerprint** para sa datos sa block. Kung may mababago man sa impormasyon sa block, magbabago rin ang fingerprint. Dahil dito, madali para sa kahit sino na tiyakin na hindi nabago ang kasaysayan ng mga transaksyon sa blockchain at nakakatulong ito upang mapanatiling ligtas ang network.


> **Callout**
>
> Si Satoshi Nakamoto, ang lumikha ng Bitcoin, ang nagmina ng Genesis Block, na nagbukas ng kabuuang 50 bitcoin.


#### Ang Karera sa Pagmina ng Block

Nag-uunahan ang mga miner upang makahanap ng valid block hash. Ang unang miner na makahanap nito ang may karapatang magdagdag ng bagong block sa blockchain at tumanggap ng gantimpala sa bitcoin.

Para maging valid, ang hash ng block ay dapat mas mababa sa isang numerong itinakda ng network na tinatawag na difficulty target. Dahil random ang mga hash, kailangang paulit-ulit na subukan ng mga miner ang iba't ibang input hanggang makahanap sila ng gumagana.

Kung masyadong maraming miner ang nagkokompetensya, masyadong mabilis mahahanap ang mga block. Kung masyadong kaunti naman, masyadong matagal bago makahanap ng block. Para mapanatiling maayos ang sistema, awtomatikong ina-adjust ng Bitcoin ang difficulty tuwing 2,016 blocks (mga dalawang linggo).

Tinitiyak ng adjustment na ito na, sa karaniwan, may nadaragdag na bagong block sa blockchain tuwing 10 minuto.


> **Definition – Kahulugan ng difficulty level**
>
> Ang **difficulty level** sa Bitcoin mining ay sumusukat kung gaano kahirap makahanap ng valid block hash. Ina-adjust ng network ang difficulty tuwing 2,016 blocks (mga dalawang linggo) upang ang mga bagong block ay madagdag sa blockchain tuwing 10 minuto. Kapag mas mataas ang difficulty, mas mahirap para sa mga miner na makahanap ng valid block.


Sa paghahanap ng valid block hash, pinapatunayan ng isang miner na nagawa niya ang kinakailangang trabaho upang maidagdag ang bagong block sa blockchain. Ang prosesong ito ay tinatawag na **Proof of Work** (PoW). Ito ang mekanismo ng seguridad na nagpapahintulot sa Bitcoin na kumpirmahin ang mga transaksyon at magdagdag ng mga bagong block sa blockchain. Ang miner na unang makahanap ng valid hash ay tumatanggap ng gantimpala sa bitcoin, na kinabibilangan ng block reward at mga bayad sa transaksyon mula sa mga transaksyong kasama sa block na iyon.

Tinutulungan ng Proof of Work (PoW) na mapanatiling ligtas ang Bitcoin sa pamamagitan ng paggawa nitong napakamahal para sa sinuman na subukang mandaya o kontrolin ang network. Sa halip, mas kapaki-pakinabang ang sumunod sa mga patakaran.

May apat na pangunahing tungkulin ang mga miner:

1. **Mangolekta ng mga transaksyon**: Pinipili ng mga miner ang mga transaksyong ipinadala sa network at inilalagay ang mga ito sa isang candidate block.
1. **Gawin ang Proof of Work**: Nagkokompetensya ang mga miner upang lutasin ang isang mahirap na matematikal na palaisipan sa pamamagitan ng paghahanap ng valid block hash.
1. **I-broadcast ang block**: Ang unang miner na makahanap ng tamang solusyon ay nagbabahagi ng bagong block sa network.
1. **Kumita ng gantimpala**: Kung tama ang block, idinadagdag ito sa blockchain at ang miner ay tumatanggap ng bagong likhang bitcoin pati na rin ang mga bayad sa transaksyon.

Maraming miners sa buong mundo ang sabay-sabay na sumusubok gumawa ng susunod na block. Kapag may isang miner na nakahanap ng tamang solusyon, sinusuri ng network ang block. Kung tama ang lahat, idinadagdag ito sa blockchain. Ang ibang mga block na kasabay ay tinatanggal. Ang prosesong ito ang nagpapanatili ng pagkakaisa ng network at pumipigil sa dobleng paggastos.

* Ang mga miner ay mga computer na tumutulong magpanatili at mag-update ng ledger ng Bitcoin.
* Kinokolekta nila ang mga transaksyon at pinagsasama-sama sa isang block. Pagkatapos, pinapadaan nila ang data ng block sa isang hashing algorithm upang makagawa ng natatanging code na tinatawag na hash.
* Paulit-ulit na ginagawa ng mga miner ang prosesong ito, naghahanap ng hash na tumutugma sa mga patakaran ng Bitcoin. Ang unang miner na makahanap ng tamang hash ay nakakakuha ng bagong likhang bitcoin bilang gantimpala, at ang kanilang block ay idinadagdag sa blockchain.
* Ang hash ng bawat block ay nag-uugnay din dito sa naunang block. Kung may magtatangkang baguhin ang nakaraang transaksyon, hindi na magtutugma ang mga hash, at tatanggihan ng network ang binagong chain. Ito ang nagpapanatiling ligtas sa ledger ng Bitcoin.
