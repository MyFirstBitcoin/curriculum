# 3.1 Ang pagbuo ng TCP/IP

Karamihan sa atin ay pamilyar sa mga protocol ng TCP/IP na ginagamit ngayon bilang pundasyon ng internet. Ang pinagmulan nito ay nagsimula pa noong huling bahagi ng dekada 70 nang ang mga siyentipiko ay nagsasaliksik ng mga alternatibong disenyo sa Arpanet – isang mas naunang network na nilikha ng Kagawaran ng Tanggulan ng Estados Unidos upang pahintulutan ang pagbabahagi ng mga mapagkukunan sa pagitan ng mga malalayong computer. Naging pamantayang protocol ng Arpanet ang TCP/IP noong 1983, na nagresulta sa pagiging pangunahing modelo ng networking pagdating ng dekada 90 at naging pundasyon ng internet na ginagamit ng Bitcoin ngayon.


| Modelo ng OSI | TCP/IP |
| --- | --- |
| Aplikasyon | Aplikasyon |
| Presentasyon | Aplikasyon |
| Sesyon | Aplikasyon |
| Transportasyon | Transportasyon |
| Network | Network |
| Data Link | Data Link |
| Pisikal | Pisikal |


Kasabay ng pagbuo ng modelo ng TCP/IP, isang katulad ngunit mas malawak na balangkas ang binubuo ng International Standards Organisation (ISO) at ng industriya ng Telecoms (CCITT). Ang proseso ng pagbuo ng mga bagong protocol o pagsasagawa ng mga pagbabago ay mabagal at mahirap ikumpara sa mas desentralisadong paraan ng pagbuo ng TCP/IP, dahilan kung bakit nanaig ang huli hanggang ngayon.

##### Request for Change

Anumang mungkahing pag-unlad sa mga umiiral na protocol o ideya para sa mga bago ay maaaring ipanukala sa modelo ng TCP/IP sa pamamagitan ng isang **Request for Change** na proseso. Dumadaan ito sa isang proseso ng pag-apruba, na pinamamahalaan ng Internet Engineering Task Force (IETF), at nagiging open source kapag naaprubahan upang malayang magamit at tanggapin ng sinuman. Ilan sa mga halimbawa:

* 1969 RFC 1 Dokumentado kung paano ipapadala ang mga packet sa Arpanet
* 1981 RFC791 nagtakda ng Internet protocol V4 – malawak pa ring ginagamit ngayon
* 1982 RFC 821 Simple Mail Transfer Protocol
* 1987 Domain Name System – kung paano tinutukoy ang mga domain name sa IP address
* 1999 RDC 2616 Hypertext Transfer Protocol – mahalaga para sa pag-browse sa web


> **Callout**
>
> Ang **Bitcoin Improvement Proposal** (BIP) ay sumusunod sa katulad na paraan ng RFC, ngunit nakatuon lamang sa mga pagpapabuti sa Bitcoin mismo sa halip na pagbuo ng mga bagong protocol. Hango rin sa modelong ito ang Bitcoin, at makikita mo ang mga karagdagang protocol na tinutukoy bilang layer dalawa o tatlo.


Katulad ng base layers ng TCP/IP model na bihirang magbago sa mga nakaraang dekada, at ang mga inobasyon ay nangyayari sa mas mataas na layer, inaasahan ding mabagal ang pagbabago sa base layer ng Bitcoin sa ngayon, at ang mga solusyon sa scaling tulad ng Lightning at Liquid ay nangyayari sa itaas nito.

Isang magandang halimbawa kung paano nagiging mahirap baguhin ang mga base layer protocol sa paglipas ng panahon ay ang IPv6. Ang inaasahang pagkaubos ng address space sa IPv4 ay lumikha ng pangangailangan para sa bagong protocol. Ang unang draft standard ay nilikha noong 1998, ngunit naaprubahan lamang bilang internet standard noong 2017. Bagamat nalutas nito ang maraming problema ng IPv4 at mas handa para sa hinaharap, mabagal pa rin ang pagtanggap nito sa industriya ngayon. Sa panahong ito, maraming bagong protocol ang nailarawan sa mas mataas na layer para sa multimedia, email, atbp.

##### Ang mga Pundasyon na Ginagamit ng Bitcoin

Ang pagkakahiwalay ng mga problema ng interconnectivity ay nagpapahintulot na ang mga protocol ay ma-develop nang hiwalay mula sa mga layer sa itaas at ibaba nito. Sa halip na muling imbentuhin ang mga solusyon para sa bawat layer, ang network ng Bitcoin ay maaaring umasa sa mga kakayahan ng network na ibinibigay ng physical at data link layers.


| Layer | Orihinal na TCP/IP |
| --- | --- |
| Aplikasyon | Gumagamit ng Domain Name System (DNS) upang tukuyin ang mga kalapit na node. Ang Port 8333 ay nagsesenyas ng Bitcoin protocol. |
| Transportasyon | UDP para sa FIBRE comms sa pagitan ng mga minero para sa mababang latency. TCP para sa P2P na komunikasyon sa pagitan ng mga node. |
| Transportasyon | TOR Routing: Nagbibigay ng anonymity at privacy. Broadcast Protocol: Nagpapadala ng trapiko sa buong network. |
| Link | Gumagana sa anumang medium (hal., Ethernet, Wi-Fi, atbp.) |
| Pisikal | Pisikal na transmisyon sa pamamagitan ng wireless, Ethernet, o iba pang hardware interface. |


##### Ang Bitcoin ay isang neutral na protocol para maglipat ng halaga tulad ng HTTPS na isang protocol para maglipat ng impormasyon

* **HTTPS**: Secure na mga Website
* **SMTP**: Magpadala ng mga Email
* **FTP**: Maglipat ng mga file
* **DNS**: Pamahalaan ang mga pangalan ng domain
* **BTC**: Mag-imbak at maglipat ng halaga

Pinapahintulutan ng Bitcoin na mailipat ang halaga nang maaasahan at hindi nangangailangan ng ikatlong partido sa pagitan ng mga tao o mga device sa Internet. Inaasahan na magbubukas ito ng napakalaking halaga.
