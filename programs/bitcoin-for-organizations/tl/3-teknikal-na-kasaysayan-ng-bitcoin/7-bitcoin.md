# 3.7 Bitcoin

Pagkatapos ng maraming taon at mga nabigong pagtatangka, karamihan sa mga Cypherpunk ay nagsimula nang mawalan ng interes sa ideya ng isang digital na pera na walang pahintulot, nang makatanggap si Adam Back ng isang email na may kalakip na draft ng white paper na tinatawag na ‘electronic cash without a third party’ mula sa isang hindi kilalang tao na nagpakilalang si Satoshi Nakamoto.

Upang balikan sa puntong ito, mayroon na tayong mga ideya ng:

* Mga cryptographic signature na maaaring magbigay ng antas ng privacy at anonymity
* Konsepto ng isang perang walang suporta (B-Money)
* Mga panukala (ngunit walang paraan) para limitahan ang paglabas ng bagong pera
* Mga digital na barya na ang pagmamay-ari ay itinatakda gamit ang public keys (B-Money) at maaaring ilipat sa pamamagitan ng pagpirma at muling itatalaga batay sa address ng tatanggap (RPOW at Hashcash)
* Lahat ng node ay nagpapanatili ng kopya ng isang ganap na distributed ledger (B-Money) (itinuring noon na hindi praktikal)
* Time-stamping protocol– gamit ang Merkle tree hashing upang magbigay ng matematikal na mapapatunayang pagkakasunod-sunod ng mga pangyayari na mahirap dayain kung lahat ng user ay may parehong talaan
* Proof of work upang itali ang tunay na pagsisikap sa sistema (ngunit ginagamit ang hash mismo bilang pera)
* Ganap na desentralisadong mga network kung saan lahat ng peer ay pantay at maaaring pumasok o umalis sa network (BitTorrent)
* Konsepto ng pag-uugnay ng mga bagong hash sa mga naunang hash (Bit Gold at time-stamping)

Ang mga kulang noong panahong iyon ay kinabibilangan ng:

* Isang mabisang solusyon upang lutasin ang ‘Byzantine generals’ problem
* Isang paraan upang limitahan ang dami ng pera sa sirkulasyon kahit patuloy ang pag-unlad ng hardware
* Incentive scheme para sa mga tao na lumahok (chicken and egg issue)

Ang isa pang malaking pagkakaiba ng mga kamakailang pagtatangka at Bitcoin ay si Satoshi ay matagal nang nagtatrabaho sa code sa tunay na diwa ng ‘Cypherpunks write code’ bago ito inanunsyo sa mga mailing list, hindi tulad ng Bit Gold at B-Money na mas konseptwal lamang.

Ano ang inobasyon na nagbukod sa Bitcoin mula sa mga naunang pagtatangka sa electronic cash?

Ang proof of work ay gagamitin bilang consensus mechanism at paraan ng pagbibigay ng seguridad at hindi mababago: Sa halip na gamitin ang hash bilang anyo ng pera, ito ay gagamitin sa isang bagong konseptwal na proseso na tinatawag na mining, kung saan ang isang node ay magbubuo ng isang batch ng mga transaksyon, magdadagdag ng random na numero at pagkatapos ay ia-apply ang hashing sa ‘block’ ng data. Ang isang valid na block na tumutugon sa hash requirement ay iaanunsyo sa network. Ang mga block na ito ay magkakaugnay gamit ang hash ng naunang block sa bawat isa, at ang pinakamahabang blockchain ang gagamitin kung may tie-breaker kung saan iba't ibang node ang magva-validate at mag-aanunsyo ng iba't ibang block nang sabay upang lumikha ng chain splits. Ang proof of work ang naging distributed tie-breaker upang lutasin ang Byzantine generals problem.

Ang mga miner na ito ay binigyan din ng insentibo upang maglaan ng CPU na kailangan para sa proof-of-work sa pamamagitan ng paglalaan sa kanila ng bagong bitcoin para sa bawat block. Ang dami ng Bitcoin na kanilang natatanggap ay naka-programa ring bumaba tuwing humigit-kumulang bawat 4 na taon hanggang sa malikha na ang lahat ng Bitcoin, na nagtatakda ng matigas na limitasyon sa kabuuang Bitcoin na kailanman ay iikot sa 21M.

Ang pinaka-orihinal na ideya ay ang paraan kung paano niya nilutas ang isyu kung gaano karaming pera ang malilikha habang gumaganda ang hardware at mas maraming kapangyarihan ang naiaambag sa network. Ang mga timestamp ng isang takdang bilang ng mga block (2016) ay kukunin ang average, at kung masyadong mabilis silang nalilikha, ang hash na kailangan upang makalikha ng bagong block ay gagawing mas mahirap, kung masyadong mabagal ay gagawing mas madali. Ito ay nakapaloob sa desentralisadong protocol na pinapatakbo ng lahat ng node kaya anumang miner na hindi susunod dito ay magsasayang ng enerhiya sa pag-mine ng block na walang benepisyo dahil ito ay tatanggihan ng natitirang bahagi ng network. Tinitiyak ng adjustment na ito na ang paglikha ng mga bagong block ay nananatili sa planadong iskedyul ng paglalabas, at nagbibigay ng insentibo sa mga miner na ‘sumunod sa mga patakaran’.

####   
Buod

Marami sa mga piraso ng puzzle kung paano bumuo ng isang desentralisadong peer to peer electronic cash system na nakabatay sa mga prinsipyo ng sound money ay naroon na bago inilabas ni Satoshi ang kanyang whitepaper at agad pagkatapos ng paunang paglabas ng code.

> Ang likas na katangian ng Bitcoin ay ganoon na kapag nailabas na ang version 0.1, ang pangunahing disenyo ay nakatakda na para sa buong buhay nito  
_Satoshi Nakamoto_

Bagaman maraming ideya para sa mga pagpapabuti (BIPs) ang iminungkahi at tinanggap, tahimik na gumagana ang Bitcoin mula pa noong 2009 na sinusunod ang protocol na idinisenyo sa paunang paglabas at halos walang abala. Lahat ng pagpapabuti ay ginawa habang pinananatili ang backward compatibility sa lahat ng naunang bersyon.



##### Mga Tala

1. Para sa paliwanag ng Byzantine Generals problem - tingnan ang [https://en.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
