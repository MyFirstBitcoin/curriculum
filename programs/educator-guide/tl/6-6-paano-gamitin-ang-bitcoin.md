# 6 - Paano Gamitin ang Bitcoin

Tagal: 90 minuto

Pangunahing Ideya: Ang paggamit ng Bitcoin on-chain ay nagtuturo sa mga estudyante kung paano gumagana ang pagmamay-ari, sariling kustodiya, at beripikasyon sa aktwal na buhay, ginagawang praktikal na aksyon sa pananalapi ang teorya.

#### Mga Layunin sa Pagkatuto

Sa pagtatapos ng araling ito, dapat ay kaya ng mga estudyante na:

* Tukuyin ang mga karaniwang paraan ng pagkuha at pagpapalitan ng bitcoin, kabilang ang peer-to-peer at mga sentralisadong paraan ng palitan.
* Ipaliwanag ang pagkakaiba ng self-custodial at custodial na mga wallet, at kung bakit mahalaga ang sariling kustodiya sa Bitcoin.
* Ilarawan ang layunin ng private keys, public addresses, seed phrases, at mga interface ng wallet.
* Ihambing ang iba't ibang uri ng wallet at suriin ang kanilang mga kalakasan at kahinaan batay sa seguridad, kaginhawaan, privacy, at kontrol.
* Mag-set up ng mobile Bitcoin wallet at ipaliwanag ang pangunahing proseso ng pag-recover.
* Ipakita kung paano tumanggap at magpadala ng on-chain na bitcoin transaction.

Ipatupad ang prinsipyo ng "Don't Trust, Verify" sa pagpili ng wallet, mga transaksyon, at mas malawak na paggamit ng Bitcoin.

#### Mga Kagamitan at Resources

##### Mga Visual Aid

* Kabanata 6 - Paano Gamitin ang Bitcoin

##### Support Library

* Vocabulary Reference Card — Kabanata 6 — Mga Termino: wallet, private key, public address, seed phrase, custodial, self-custodial, UTXO, transaction fee
* Mga Tsart ng Paghahambing at Reference Sheet — Paghahambing ng mga uri ng wallet (custodial, mobile, hardware, papel)
* Mga Teknikal na Paliwanag at Malalimang Talakayan — Public/private keys, UTXO model, transaction confirmation
* Malalimang Talakayan sa Seguridad ng Private Key — Seed phrases, key derivation, mga paraan ng backup, mga uri ng atake
* Gabay sa Anatomy ng Transaksyon — Hakbang-hakbang na halimbawa kung paano gumagana ang isang Bitcoin transaction
* Checklist ng Pinakamahusay na Praktis sa Seguridad — Bago magsimula, paggawa ng wallet, pagtanggap, pagpapadala, pag-iwas sa phishing

#### Mga Aktibidad

* Mga Transaksyon sa Aksyon
* Lightning Relay Race
* Pag-explore sa Mempool

#### Online na Pagtuturo

* Gawing malinaw mula sa simula kung ang mga estudyante ay nanonood lamang ng demo o sila mismo ang magse-set up ng wallet.
* Gumamit ng malalaki at madaling basahing screenshot para sa bawat hakbang ng pag-setup ng wallet.
* Mag-pause pagkatapos ng bawat hakbang at tanungin ang mga estudyante na kumpirmahin ang kanilang pagkaunawa sa chat bago magpatuloy.
* Magbigay ng direktang babala bago ang seksyon ng seed phrase at paalalahanan ang mga estudyante na huwag kailanman magbahagi ng sensitibong impormasyon online.

#### Paghahanda

* I-download at subukan ang isang mobile wallet app (Blue Wallet o Muun); maghanda ng mga screenshot ng mahahalagang hakbang sa pag-setup.
* Maghanda ng gabay sa pag-setup ng wallet (download → create → backup seed → receive) bilang reference.
* Siguraduhing gumagana ang network/WiFi; maghanda ng demo address at QR code na ipapakita.

#### Pamamaraan

Ang araling ito ay lilipat mula sa teorya patungo sa direktang praktis. Ngayon ay tumutugma na ito sa estruktura ng Diploma kung saan ang acquisition, wallets, setup, transaksyon, at beripikasyon ay lumalabas sa parehong pangunahing mga heading tulad ng sa student guide. Ang karagdagang suporta sa pagtuturo ay nananatiling naka-nest sa loob ng mga seksyong iyon.

##### 6.0 Panimula, 8 minuto

Simulan sa pamamagitan ng pag-uugnay ng kabanatang ito sa naunang kabanata:

* Kung ang Bitcoin ay pera, paano nga ba ito nakukuha at nagagamit ng mga tao?
* Ano ang ibig sabihin ng tunay na pagkontrol sa iyong bitcoin?
* Bakit iba ang paggamit ng Bitcoin kumpara sa paggamit ng bank app?

Linawin na ang kabanatang ito ay tungkol sa praktikal na paggamit. Hindi na lang natututo ang mga estudyante kung ano ang Bitcoin, natututo na silang direktang makipag-ugnayan dito.

##### 6.1 Pagkuha at Pagpapalitan ng Bitcoin, 12 minuto

Ipaliwanag na maaaring makuha ng mga tao ang bitcoin sa iba't ibang paraan, kabilang ang:

* pagkakaroon ng bayad sa bitcoin
* pagmimina ng bitcoin
* pagpapalit ng fiat para sa bitcoin nang personal
* pagpapalit ng fiat para sa bitcoin online

Pagkatapos, ituon ang pansin sa dalawang pangunahing paraan ng pagkuha na tinalakay sa kabanata:

* peer-to-peer, nang personal
* peer-to-peer, online
* sentralisadong palitan

Gawing malinaw ang mga kompromiso.

Para sa P2P nang personal, bigyang-diin ang direktang palitan nang walang bangko o tagapamagitan, ngunit banggitin din ang mga praktikal na panganib ng pakikipagkita sa mga tao para sa palitan ng pera.

Para sa P2P online, ipaliwanag ang escrow sa simpleng paraan, bilang isang paraan upang mabawasan ang panganib sa kabilang panig habang pinapayagan pa rin ang direktang palitan sa pagitan ng mga tao.

Para sa sentralisadong palitan, gawing malinaw na ito ay maginhawa, ngunit nangangailangan ito ng pagtitiwala sa isang kumpanya, madalas na pagbabahagi ng personal na impormasyon, at iniiwan ang pondo sa kontrol ng ikatlong partido hanggang ito ay ma-withdraw. Magandang pagkakataon ito upang bigyang-diin na kadalasan, ang kaginhawaan ay may kapalit sa privacy at kalayaan.

##### 6.2 Panimula sa Bitcoin Wallets, 35 minuto

**Ano ba Talaga ang Bitcoin Wallet**

Linawin agad ang isang karaniwang maling akala: ang bitcoin ay hindi nakaimbak sa loob ng wallet app na parang pisikal na pera sa bag.  
Ang bitcoin ay umiiral sa ledger na pinapanatili ng network. Ang kinokontrol ng user ay ang kakayahang gastusin ito gamit ang mga private key.

Pagkatapos, ipaliwanag ang dalawang bagay na kadalasang tinutukoy ng mga tao kapag sinabing "wallet":

* ang sistema ng private key, kung saan nagmumula ang mga address
* ang app o interface na ginagamit upang makipag-ugnayan sa network

Gamitin ang email analogy ng kabanata kung makakatulong:

* public address = parang email address na maaari mong ibahagi
* private key = parang password na kailangan mong protektahan

Maging napakalinaw dito: kung sino ang may hawak ng private keys, siya ang may kontrol sa bitcoin. Ito ang pangunahing konsepto na dapat maunawaan ng mga estudyante.

**Self-Custodial vs Custodial Wallets**

Isa ito sa pinakamahalagang bahagi ng kabanata.

Ipaliwanag nang malinaw ang pagkakaiba:

* Self-custodial wallet: ang user ang may kontrol sa private keys
* Custodial wallet: isang ikatlong partido ang may kontrol sa private keys para sa user

Pagkatapos, talakayin ang mga kompromiso:

Self-custodial

* buong kontrol sa pondo
* walang kailangang aprubadong proseso
* proteksyon laban sa biglaang kumpiskasyon
* mas malaking responsibilidad
* walang madaling paraan ng pagbawi kung mawala ang seed phrase

Custodial

* mas madaling pagbawi at suporta
* mas simple para sa mga baguhan
* mas lantad sa pag-freeze ng account, pag-hack, at kontrol ng ikatlong partido
* hindi tunay na hawak ng user ang bitcoin

Ito ang tamang sandali upang bigyang-diin ang pariralang ito:

"Not your keys, not your coins."

Dapat umalis ang mga estudyante sa seksyong ito na hindi lang alam ang slogan, kundi nauunawaan kung ano talaga ang ibig sabihin nito sa praktika.

**Iba't Ibang Uri ng Wallet at Paano Pumili**

Ipakilala ang mga uri ng wallet na tinalakay sa kabanata:

* online wallet
* mobile wallet
* desktop wallet
* hardware wallet
* paper wallet

Huwag ituring na may perpektong wallet. Sa halip, ipaliwanag na bawat isa ay may kompromiso sa pagitan ng:

* seguridad
* privacy
* kaginhawaan
* compatibility
* bayarin
* kontrol
* reputasyon

Ipaliwanag din nang malinaw na inirerekomenda naming bigyang-pansin kung ang wallet software ay open-source, dahil ang mga open-source na tool ay maaaring suriin, i-audit, at ipagpatuloy ng komunidad. Direktang konektado ito sa prinsipyo ng beripikasyon sa Bitcoin.

##### 6.3 Pagse-set up ng Mobile Bitcoin Wallet, 10 minuto

Lakarin ang mga estudyante sa pangunahing proseso na ipinakita sa kabanata:

* i-download ang wallet
* gumawa ng bagong wallet
* bumuo at isulat ang recovery phrase
* kumpirmahin ang recovery phrase
* magdagdag ng dagdag na seguridad kung mayroon
* buksan ang wallet at hanapin ang receive function

Gawing napakalinaw ang babala tungkol sa seed phrase:

* kung mawala ang seed phrase, maaaring mawala ang access sa pondo
* kung may ibang makakuha ng seed phrase, maaari nilang kunin ang pondo

Kung ginagawa ito ng mga estudyante nang aktwal, dapat huminto ang guro sa bawat hakbang at tiyaking nauunawaan ng lahat ang kanilang ginagawa. Kung mas konseptwal ang klase, maaaring ipaliwanag ang seksyong ito bilang walkthrough sa halip na gawin nang live. Ang recovery option na ipinakita sa kabanata ay kapaki-pakinabang din para ipaliwanag na maaaring ma-restore ang wallets kung tama ang pagkaka-backup ng seed phrase.

##### 6.4 Pagtanggap at Pagpapadala ng Transaksyon, 17 minuto

**Pagtanggap at Pagpapadala ng On-chain na Transaksyon**

Ngayon, ipaliwanag kung paano gumagana ang on-chain na mga transaksyon.

Para tumanggap ng bitcoin:

* buksan ang wallet
* i-tap ang receive o deposit
* kopyahin ang address, ibahagi ang link, o ipakita ang QR code

Para magpadala ng bitcoin:

* buksan ang wallet
* i-paste o i-scan ang address ng tatanggap
* ilagay ang halaga
* dobleng suriin ang lahat ng detalye
* i-broadcast ang transaksyon
* maghintay ng kumpirmasyon

Gawing malinaw ang mga pangunahing puntong ito:

* ang transaksyon ay naglilipat ng pagmamay-ari, hindi pisikal na barya
* ang mga transaksyon ay hindi na mababawi
* tinitiyak ng mga node ang bisa
* isinusama ng mga miner ang mga transaksyon sa mga block
* ang mga bayarin ay nakakaapekto sa prayoridad ng kumpirmasyon
* ang mga on-chain na transaksyon ay karaniwang ligtas, ngunit mas mabagal at madalas na mas mahal kaysa sa mga Lightning na transaksyon

Ang diagram ng daloy ng transaksyon sa kabanata ay lalo nang kapaki-pakinabang dito, dahil tumutulong ito sa mga estudyante na mailarawan ang landas mula sa wallet request hanggang sa network confirmation.

**Mga Transaksyon sa Aksyon at Role-Based na Pagsasanay**

Gamitin ang estruktura ng kooperatibong ehersisyo mula sa kabanata upang palalimin ang pag-unawa. Ipaliwanag ang apat na papel na kasangkot:

* nagpapadala
* tatanggap
* miner
* operator ng node

Isang simpleng paraan sa klase ay magtalaga ng mga papel at lakarin ang isang transaksyon, hakbang-hakbang. Nakakatulong ito sa mga estudyante na makita na ang Bitcoin transaksyon ay hindi mahika, ito ay isang koordinadong proseso na may kasamang pag-apruba, beripikasyon, pagsama sa block, at pag-update ng ledger.

Ang layunin dito ay hindi teknikal na lalim. Ito ay upang matulungan ang mga estudyante na maunawaan kung sino ang gumagawa ng ano sa isang transaksyon at kung bakit mahalaga ang beripikasyon.

##### 6.5 Huwag Magtiwala, Mag-Beripika, 8 minuto

Ipaliwanag na ito ay naaangkop sa:

* mga wallet
* mga exchange
* mga app
* mga detalye ng transaksyon
* mga pahayag tungkol sa "madaling kita"
* mga proyektong nagpapanggap na parang Bitcoin

Ipaliwanag nang malinaw na ang Bitcoin ay nangangailangan ng kritikal na pag-iisip mula sa mga gumagamit, beripikasyon ng kanilang ginagamit, at pag-iwas sa bulag na pagtitiwala. Ipaliwanag din kung bakit mahalaga ang open-source na mga tool sa kontekstong ito: nagbibigay ito ng kakayahan para sa independiyenteng beripikasyon.

###### Pagwawakas at Pagsusuri ng Pagkaunawa

Tapusin gamit ang ilang mabilis na tanong:

* Ano ang pagkakaiba ng custodial at self-custodial na wallet?
* Bakit napakahalaga ng seed phrase?
* Ano ang nangyayari kapag nagpadala ka ng on-chain na transaksyon?
* Bakit mas mabagal ang mga on-chain na transaksyon kumpara sa ibang Bitcoin payments?
* Ano ang ibig sabihin ng "Don't Trust, Verify" sa aktwal na paggamit?

#### Tala para sa Guro

Ang kabanatang ito ay napaka-praktikal, kaya bigyang-priyoridad ang kalinawan, kaligtasan, at pag-uulit.

Hindi kailangang matutunan ng mga estudyante ang lahat ng uri ng wallet sa isang klase. Ang mga pangunahing layunin ay:

* pag-unawa sa mga pangunahing kaalaman ng wallet
* pag-unawa sa self-custody
* pagkatuto ng pangunahing daloy ng transaksyon
* pag-aangkin ng responsable at mapanuring pananaw sa beripikasyon

Maging ekstra-ingat kapag tinatalakay ang seed phrase at pag-setup ng wallet. Dapat umalis ang mga estudyante na nauunawaan na hindi ito maliliit na detalye, kundi ito ang pundasyon ng pagmamay-ari ng Bitcoin.

Ang pinaka-kapaki-pakinabang na visual at aktibidad sa kabanatang ito ay:

* ang paghahambing ng self-custodial at custodial
* ang talahanayan ng trade-off ng mga uri ng wallet
* ang step-by-step na ehersisyo sa pag-setup ng wallet
* ang diagram ng daloy ng transaksyon
* ang aktibidad ng transaksyon batay sa papel

##### Ano ang Magandang Resulta

* Mahalagang aktwal na mag-setup ng wallet ang mga estudyante o manood ng maingat na demo, gawing sentro ang seed phrase gamit ang "Itong 12 salita ANG iyong Bitcoin," subukan ang mga senaryo tulad ng "Ano ang mangyayari kung mawala ang iyong telepono?", at magsanay ng pagkilala sa phishing.
* Ang mga guro ay dapat maging hands-on na gabay na may karanasan na dito, maging maingat sa seguridad nang hindi paranoid, at maging tapat tungkol sa antas ng hirap at pagkatutong kailangan.
* Nararamdaman ng mga estudyante na natutunan nila ang isang tunay na kasanayan na magagamit nila, nauunawaan na ang seed phrase ay totoo at mahalaga at hindi lang abstract, nararamdaman nilang kaya nilang maghawak ng sarili nilang Bitcoin, at nauunawaan na ang desentralisasyon ay nangangailangan ng personal na responsibilidad.
* Makakamit ang Learning Outcomes kung kayang mag-setup ng wallet ng mga estudyante at nauunawaan ang pagkakaiba ng public at private keys, nauunawaan ang mga trade-off ng custody sa pagitan ng custodial at self-custody wallets, maipaliwanag kung paano gumagana ang isang transaksyon kabilang ang inputs, outputs, at fees, maipakita ang kaalaman sa seguridad kabilang ang proteksyon ng seed phrase, at makapagtanong ng mapanuring tanong tungkol sa pagmamay-ari at kontrol.

##### Pamamahala ng Oras

Kung kapos sa oras, bigyang-priyoridad ang:

* Pag-unawa sa mga pangunahing kaalaman ng wallet
* Pag-unawa sa self-custody
* Pagkatuto ng pangunahing daloy ng transaksyon
* Pag-aangkin ng responsable at mapanuring pananaw sa beripikasyon

Kung may sobra sa oras, maglaan ng panahon sa:

* Talahanayan ng paghahambing ng self-custodial at custodial
* Talahanayan ng trade-off ng mga uri ng wallet
* Step-by-step na ehersisyo sa pag-setup ng wallet na may live demo
* Diagram ng daloy ng transaksyon na may kalkulasyon ng fee
* Mga advanced na kasanayan sa seguridad at konsiderasyon sa hardware wallet

##### Kung Nahihirapan ang mga Estudyante

* Seed phrase bilang "totoo" → "Ang pariralang ito ANG iyong bitcoin; walang customer service."
* Public vs. private keys → Analohiya sa email (address vs. password).
* Bakit mahirap → "Ikaw ang may kontrol; ikaw ang responsable." Kilalanin ang trade-off.
