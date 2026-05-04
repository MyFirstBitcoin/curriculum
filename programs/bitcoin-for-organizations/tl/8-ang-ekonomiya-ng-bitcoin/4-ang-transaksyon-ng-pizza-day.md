# 8.4 Ang Transaksyon ng Pizza Day

Sa ngayon, nakatuon ang modyul na ito sa paggamit ng bukas na katangian ng Bitcoin ledger upang makabuo ng kapaki-pakinabang na mga sukatan mula sa pinagsama-samang datos ng transaksyon. Gayunpaman, posible ring gamitin ang datos ng ledger at block explorers upang suriin ang mga totoong transaksyon at subaybayan ang galaw ng pondo sa loob ng network.

Tuwing ika-22 ng Mayo bawat taon, kinikilala ng komunidad ng Bitcoin si Laszlo Hanyecz, na naging unang tao na naitalang gumamit ng bitcoin upang bumili ng pisikal na produkto. Noong ika-18 ng Mayo 2010, inanunsyo ni Hanyecz sa isang forum ng Bitcointalk.org na naghahanap siya ng pizza at handang magbayad gamit ang BTC. Nag-alok siya ng 10,000 BTC sa sinumang handang pumasok sa transaksyon. Naghintay siya ng ilang araw, hanggang sa pumayag ang 19-anyos na estudyanteng si Jericho at nagpadala ng dalawang malaking pizza.

Ang **Pizza Day** na transaksyon ay maaaring makita ng kahit sino at may sumusunod na transaction ID:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Kapag inilagay ang transaction ID na ito sa [mempool.space](https://mempool.space) ay makikita ang mga sumusunod:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Petsa at oras ng transaksyon: 22 Mayo 2010

Bayad sa network transaction: 99,000,000 sats (noong panahong iyon ay mas mababa pa sa 1 sentimo ng US. Noong Mayo 2025, ito ay katumbas ng ₱5,500,000.00)

Block Height: 57,043

Bilang ng mga Kumpirmasyon: 838,645 (ito ang bilang ng mga block na nadagdag sa ledger pagkatapos ng transaksyong ito)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Bilang ng Transaction Inputs: 131

Bilang ng Transaction Outputs: 1

Kapag kinlik ang output public key (nagtatapos sa `XaxFyQ`) na alam nating pagmamay-ari ni Jericho na tumanggap ng 10,000 BTC para sa dalawang pizza, makikita ang mga sumusunod:

Ang address na ito ay kasalukuyang may balanse na 0.00257879 BTC at lumalabas na ito ay nasangkot na sa 14 na transaksyon, ang pinakahuli ay noong ika-13 ng Disyembre 2024.



#### 8.4.1 Gawain: Talakayan ng Grupo

1. Ilarawan ang mga benepisyo (hal. auditing, pananagutan) o mga panganib (hal. isyu sa privacy) para sa mga indibidwal o negosyo na gumagamit ng ganitong transparent at bukas na sistema ng transaksyon.
1. Paano maaaring makaapekto ang ganitong uri ng pinansyal na transparency sa mga industriya tulad ng kawanggawa, pagbili ng pamahalaan, remittance o pagpapatupad ng batas?
1. Dapat bang mag-alok ang mga tradisyonal na sistema ng pagbabangko ng katulad na antas ng visibility? Mapipilitan ba silang gawin ito dahil sa merkado?
