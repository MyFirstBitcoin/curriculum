# 8.1 Ang Kalikasan ng Ledger ng Bitcoin

Ang ledger ng mga transaksyon ng Bitcoin (kilala rin bilang timechain o blockchain) ay isang pampublikong talaan na may time-stamp ng bawat balidong transaksyon na naganap kailanman sa network. Sa lumang sistema ng pananalapi, ang mga internal na transaksyon ay makikita lamang ng mga awtorisadong kalahok, gaya ng mga bangko, regulator, o mga operator ng datos tulad ng SWIFT, BACS, o SEPA. Ang pag-access sa datos ng bayad sa tradisyonal na mga sistema ay maaaring lubhang limitado at magastos.

Sa kabilang banda, sa loob ng Bitcoin network, kahit sino na may koneksyon sa internet ay maaaring makita ang bawat transaksyon mula sa pinakamalaking halaga hanggang sa bawat indibidwal na Satoshi. Maaaring subaybayan ng mga kalahok ang kabuuang suplay ng bitcoin sa real-time, bantayan ang aktibidad ng mga address at wallet, at makita ang mga gantimpala ng mga minero at kilos ng bayad. Bagaman ang nakikitang aktibidad sa ledger ay naka-link sa mga pampublikong address ng susi at hindi sa mga indibidwal na pagkakakilanlan, posible pa ring pagsama-samahin ang malalaking datos tungkol sa gawi ng paggastos, na nagpapahintulot sa lahat na magtipon at magsaliksik ng aktibidad ng ekonomiya sa real-time. Habang lumalaki ang network at mas tinatanggap bilang pinagmumulan ng katotohanang pang-ekonomiya, maaaring mabawasan ang pag-asa sa mga ahensya ng gobyerno at mga third-party na tagapagbigay para sa paggawa ng estadistika at ulat ng gawi ng paggastos.



#### 8.1.1 Mga Node at Block Explorer

Ang sinumang nais na malayang beripikahin ang ledger ng Bitcoin at ma-access ang datos nito ay dapat magpatakbo ng full node. Ang full node ay madalas na inilalarawan bilang pinaka-pundamental na paraan upang makilahok at mag-verify sa ekonomiya ng Bitcoin. Ito ay pandaigdigang available bilang open-source na software na, kapag pinatakbo, ay ida-download at ibe-beripika ang buong ledger ng Bitcoin mula sa 'Genesis Block', na nailathala noong Enero 2009, hanggang sa kasalukuyan. Sinusuportahan din nito ang seguridad ng Bitcoin network sa pagtulong na beripikahin ang mga bagong transaksyong idinadagdag sa ledger. Sa pag-access ng ledger ng Bitcoin sa ganitong paraan, ang full node ay nagsisilbing pinagmumulan ng katotohanan para sa mga mananaliksik at auditor ng network. At, para sa mga gumagamit ng Bitcoin, ang full node ay nagsisilbing 'self-sovereign' na gateway sa impormasyong transaksyonal ng ekonomiya ng Bitcoin dahil pinapalakas nito ang privacy at seguridad sa pagtanggal ng pag-asa sa mga third-party na serbisyo.

Habang ang mga full node ay nagda-download ng raw na datos, ang mga block explorer tulad ng mempool.space o blockstream.info ay nag-aalok ng visual na interface upang hanapin at bigyang-kahulugan ang aktibidad sa ledger. Pinapayagan ng block explorer na masubaybayan ang mga indibidwal na transaksyon at makita ang balanse at kasaysayan ng mga wallet. Ipinapakita rin nito ang mga sukatan ng aktibidad ng minero tulad ng mga gantimpala sa block at datos ng bayad sa transaksyon.

Sama-sama, ang mga full node at block explorer ang mga kasangkapan na nagpapagamit ng transparency ng Bitcoin network.



#### 8.1.2 Gawain: Paggalugad sa Ledger ng Bitcoin

1. Buksan ang [mempool.space](https://mempool.space) at galugarin ang homepage.
  * Ano ang pinakabagong block height?
  * Ano ang kasalukuyang bayad sa transaksyon (Mababa, Katamtaman, at Mataas na Prayoridad)?
  * Ilan ang mga transaksyong naghihintay sa mempool para sa susunod na block?
1. I-access ang pinakabagong block sa ledger.
  * Ilan ang mga transaksyong naisama?
  * Sino ang minero ng block?
  * Ano ang gantimpala sa block?
1. I-access ang isang transaksyon sa block.
  * Ilan ang input at output ng transaksyon?
  * Ano ang halaga ng transaksyon sa BTC at USD?

Talakayin ang mga pagkakaiba kung paano gumagalaw ang pera sa lumang sistema at kung paano ginagamit ng negosyo o gobyerno ang ganitong uri ng transparency.
