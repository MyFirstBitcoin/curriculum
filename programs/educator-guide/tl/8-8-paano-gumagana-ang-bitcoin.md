# 8 - Paano Gumagana ang Bitcoin

Tagal: 90 minuto

Pangunahing Ideya: Ang seguridad ng Bitcoin ay nakasalalay sa mga simpleng ngunit makapangyarihang teknikal na ideya tulad ng mga susi, lagda, hashing, at UTXO, na nagpapahintulot ng pagmamay-ari at beripikasyon nang walang sentral na awtoridad.

#### Mga Layunin sa Pagkatuto

Sa pagtatapos ng araling ito, dapat ay kayang gawin ng mga estudyante ang mga sumusunod:

* Ipaliwanag kung paano nakakatulong ang pampubliko at pribadong susi sa pag-secure ng pagmamay-ari at transaksyon ng Bitcoin.
* Ilarawan kung ano ang digital na lagda at paano nito pinapatunayan na ang isang transaksyon ay inaprubahan ng tamang may-ari.
* Ipaliwanag, sa simpleng paraan, kung ano ang ibig sabihin ng cryptography, encryption, at decryption sa konteksto ng Bitcoin.
* Ibigay ang kahulugan ng hashing at ilarawan kung bakit mahalaga ang mga hash function para sa seguridad at integridad ng datos ng Bitcoin.
* Kilalanin ang mga pangunahing katangian ng isang hash function, tulad ng fixed-length na output, one-way na katangian, at pagiging sensitibo sa maliliit na pagbabago sa input.
* Ipaliwanag ang UTXO model at kung paano ginagastos, tinatanggap, at naibabalik bilang sukli ang bitcoin sa pamamagitan ng mga output ng transaksyon.
* Ilarawan kung paano nakakatulong ang mga node na maiwasan ang double-spending sa pamamagitan ng pag-check kung ang isang output ay nagastos na.

#### Mga Kagamitan at Resources

##### Mga Visual Aid

* Kabanata 8 - Paano Gumagana ang Bitcoin

##### Suportang Aklatan

* Vocabulary Reference Card — Kabanata 8 — Mga Termino: cryptography, hash, UTXO, digital signature, private/public key, merkle tree, blockchain
* Misconceptions Libraries — Kabanata 8 — Tinutukoy: "ang nawalang seed phrase ay maaaring mabawi," "private key = password," "anonymous ang blockchain"
* Technical Explainers & Deep-Dives — Hash functions, public/private keys, UTXO model, Proof of Work security

#### Mga Gawain

* Mga Transaksyon sa Aksyon
* Pag-explore sa Mempool

#### Online na Pagtuturo

* Gamitin ang digital na whiteboard at iguhit nang live ang bawat konsepto sa halip na umasa lang sa paliwanag.
* Ituro ang isang teknikal na ideya sa bawat pagkakataon at mag-pause madalas para sa mga tanong sa pag-check.
* Gumamit ng mga visual para sa mga susi, lagda, hash, at UTXO upang masundan ng mga estudyante ang estruktura.
* Panatilihing konseptwal ang layunin at iwasan ang sobrang lalim sa matematika o jargon.

#### Paghahanda

* Ihanda at i-laminate ang mga diagram: pares ng pampubliko/pribadong susi, digital na lagda, UTXO model, hashing (one-way function).
* I-bookmark ang blockchain explorer at SHA-256 hash calculator; pumili ng 2-3 totoong Bitcoin transaksyon na dadaanan nang sunod-sunod.
* Ihanda ang mga tala sa whiteboard para ipaliwanag ang inputs, outputs, at paano nakukumpirma ang mga transaksyon sa blockchain.

#### Pamamaraan

Ang araling ito ay nagbibigay sa mga estudyante ng unang sulyap sa teknikal na bahagi ng Bitcoin nang hindi nangangailangan ng dating kaalaman sa teknolohiya. Sinusundan na ngayon ng gabay ang parehong pinaikling estruktura ng Diploma, kung saan ang cryptography ay pinagsama sa isang heading at ang UTXO ay pinagsama sa isa pa.

##### 8.0 Panimula, 8 minuto

Magsimula sa pamamagitan ng pagtatakda ng mga inaasahan:

* Ano ang nagpapaseguro sa Bitcoin kung walang sentral na bangko na kumokontrol dito?
* Paano malalaman ng network kung talagang pagmamay-ari ng isang tao ang bitcoin na sinusubukan niyang ipadala?
* Ano talaga ang nangyayari sa likod ng eksena kapag may gumagawa ng Bitcoin transaksyon?

Linawin na ang kabanatang ito ay nakatuon sa mga pangunahing teknikal na pundasyon ng Bitcoin, lalo na ang mga susi, lagda, hashing, at UTXO. Bigyan din ng katiyakan ang mga estudyante na hindi nila kailangang maging inhinyero para maintindihan ang mahalagang lohika. Malinaw na ipinapaliwanag ng kabanata mismo ang puntong ito sa pamamagitan ng paghahambing ng Bitcoin sa internet—maraming tao ang gumagamit nito araw-araw nang hindi lubos na nauunawaan ang bawat layer sa ilalim nito.

##### 8.1 Seguridad sa pamamagitan ng Cryptography, 57 minuto

**Bitcoin bilang isang Ledger na Nakaimbak sa Maraming Kompyuter**

Simulan sa simpleng paglalarawan ng kabanata tungkol sa Bitcoin network:

* Ang Bitcoin ay talaan ng mga transaksyon
* ang talaang iyon ay nakaimbak sa maraming kompyuter na tinatawag na mga node
* ang ledger ay pampubliko at pseudonymous
* ipinapakita nito ang mga address at kasaysayan ng transaksyon, hindi ang personal na detalye ng pagkakakilanlan

Tinutulungan ng seksyong ito ang mga estudyante na balikan ang mga nalalaman na nila mula sa mga naunang kabanata. Ang Bitcoin ay hindi nakabase sa mga nakatagong account sa loob ng bangko. Ito ay nakabase sa isang pinagsasaluhang ledger na maaaring beripikahin ng maraming kalahok. ay lalo nang nakakatulong dito dahil ipinapakita nito ang mga user, wallet, at ang mas malawak na Bitcoin network na konektado sa pampublikong ledger.

**Pampubliko at Pribadong Susi**

Ngayon, lumipat na sa cryptography.

Ipaliwanag na bawat gumagamit ng Bitcoin ay mayroong:

* isang pribadong susi, na kailangang manatiling lihim
* isang pampublikong susi, na maaaring ibahagi

Ipaliwanag ang kanilang layunin sa payak na mga salita:

* ang pribadong susi ang nagpapatunay ng kontrol at nagbibigay pahintulot sa paggastos
* ang pampublikong susi ang tumutulong sa iba na tiyakin na ang transaksyon ay tama ang awtorisasyon

Isang mahalagang punto ng pagtuturo mula sa kabanata ay na ang Bitcoin ay gumagamit ng pampubliko/pribadong key cryptography, hindi ang lumang modelo kung saan kailangang magbahagi muna ng parehong lihim na susi ang dalawang tao. Mahalaga ito dahil nagbibigay-daan ito sa ligtas na beripikasyon nang hindi kailangang ibunyag ng mga gumagamit ang lihim na nagpoprotekta sa kanilang pondo.

Maaari mo itong ipaliwanag ng ganito:

* ang pribadong susi ay parang lihim na patunay na ang bitcoin ay iyo
* ang pampublikong susi ay bahagi ng nagpapahintulot sa network na tiyakin ang iyong awtorisasyon
* kung sino man ang may hawak ng pribadong susi ay may kakayahang gastusin ang bitcoin

Mag-ingat na huwag gawing komplikado ang wika tungkol sa encryption. Ang pinakamahalagang punto para sa mga estudyante ay pagmamay-ari at awtorisasyon.

**Digital Signatures at Awtorisasyon ng Transaksyon**

Ngayon ipaliwanag kung ano ang nangyayari kapag may nagpadala ng bitcoin.

Gamitin ang pagkakasunod-sunod ng kabanata:

* ang gumagamit ay lumilikha ng isang transaksyon
* ang nagpadala ay gumagawa ng digital signature gamit ang kanilang pribadong susi
* ang transaksyon ay ipinapadala sa network
* tinitiyak ng mga node na balido ang lagda
* kapag napatunayan at nakumpirma, naililipat ang pagmamay-ari sa ledger

Ipaliwanag na ang digital signature ay hindi katulad ng simpleng pag-type ng pangalan. Ito ay cryptographic na patunay na ang tunay na may-ari ang nag-awtorisa ng transaksyon. Isa ito sa mga pangunahing mekanismo na nagpapagana sa Bitcoin nang walang sentral na awtoridad na manu-manong nag-aapruba ng mga transaksyon. Kapaki-pakinabang ang diagram dahil ipinapakita nito ang paglagda at beripikasyon nang biswal, pati na rin ang landas ng transaksyon mula sa nagpadala hanggang sa beripikasyon ng network.

Isang magandang pangungusap para sa klase ay:

Ang mga transaksyon sa Bitcoin ay hindi inaaprubahan dahil sinabi ng bangko. Tinatanggap ang mga ito dahil kayang tiyakin ng network ang balidong cryptographic na patunay.

**Hashing at One-Way Functions**

Susunod, ipaliwanag ang hashing.

Simulan sa simple:

* ang isang function ay tumatanggap ng input at gumagawa ng output
* ang one-way function ay madaling patakbuhin sa isang direksyon, ngunit halos imposibleng baliktarin
* ang hash function ay tumatanggap ng datos ng kahit anong laki at ginagawang fixed-length na output na tinatawag na hash

Gamitin ang isa sa mga analohiya ng kabanata, alinman ang pinakamalinaw para sa iyong tagapakinig:

* ang smoothie na analohiya para sa one-way functions
* ang fingerprint na analohiya para sa hashes
* ang musical score na analohiya para sa pag-check kung may nagbago

Ang fingerprint na analohiya ay malamang na pinakamalinaw para sa karamihan ng klase:

* ang hash ay parang digital na fingerprint para sa datos
* kung magbago man kahit kaunti ang input, lubos na nagbabago ang hash
* ito ay tumutulong sa mga computer na suriin ang integridad at matukoy kung may pakikialam

Pagkatapos, ipaliwanag kung bakit mahalaga ang hashing sa Bitcoin:

* ang mga transaksyon ay hinahash
* ginagamit ng network ang hashes upang tumulong sa pagtiyak ng integridad
* kung mabago ang isang transaksyon, nagbabago rin ang hash
* ito ay tumutulong na protektahan ang ledger mula sa hindi napapansing manipulasyon

Napakakapal ng visual sa mga pahina 7 hanggang 10 dito. Ipinapakita ng kabanata ang parehong ideya ng fixed-length output at ang prinsipyo ng "maliit na pagbabago, lubos na magkaibang resulta," na isa sa pinakamahalagang konsepto na dapat maunawaan ng mga estudyante.

**Pangunahing Katangian ng Hash Functions**

Daanan nang mabilis ang mga katangiang binigyang-diin sa kabanata, nang hindi masyadong ginagawang akademiko:

* Deterministiko: ang parehong input ay nagbibigay ng parehong output sa bawat pagkakataon
* One-way / pre-image resistance: hindi mo kayang baliktarin ang proseso sa totoong buhay
* Sensitibo sa pagbabago: kahit maliit na pagbabago sa input ay lilikha ng ibang-ibang output
* Collision resistance: napakahirap makahanap ng dalawang magkaibang input na may parehong output
* Mabilis i-verify: ang function ay episyente patakbuhin at suriin

Hindi kailangang kabisaduhin ng mga estudyante ang bawat termino, ngunit dapat nilang maunawaan ang pangkalahatang punto: nagbibigay ang hashing sa Bitcoin ng maaasahang paraan para kilalanin ang datos at matukoy ang pagbabago.

##### 8.2 Ang UTXO Model, 25 minuto

**Ang UTXO Model**

Ngayon, lumipat tayo sa ikalawang mahalagang bahagi ng kabanata: UTXOs, o Unspent Transaction Outputs.

Ipaliwanag ito sa simpleng paraan gamit ang analogy ng kabanata tungkol sa pera:

* ang bitcoin ay hindi sinusubaybayan na parang balanse ng bank account lang
* sa halip, binubuo ito ng mga pirasong maaaring gastusin na tinatawag na UTXOs
* kapag gumastos ka ng bitcoin, gumagamit ka ng isa o higit pang umiiral na UTXOs bilang inputs
* pagkatapos, may mga bagong UTXOs na nililikha bilang outputs

Gamitin ang halimbawa mula sa kabanata:

* kung mayroon kang 10 BTC na UTXO
* at magpapadala ka ng 6 BTC
* isang bagong 6 BTC na UTXO ang mapupunta sa tatanggap
* isang bagong change UTXO ang babalik sa iyo
* isang maliit na bahagi ay binabayad bilang bayad sa miner

Nakakatulong ito sa mga estudyante na makita na ang Bitcoin ay mas kahalintulad ng paggastos ng pera at pagtanggap ng sukli kaysa sa simpleng pagbabawas ng numero mula sa isang account. Lalo na malakas ang mga diagram dito dahil ipinapakita nila nang biswal kung paano hinahati ang isang UTXO sa recipient output, change output, at fee.

Gawing malinaw ang dalawang pangunahing punto:

* ang balanse ng iyong wallet ay kabuuan ng iyong mga UTXO
* kapag gumastos ka, ang mga lumang UTXO ay nauubos at may mga bagong nalilikha

**Pag-iwas sa Double-Spending**

Tapusin ang nilalaman sa pagpapaliwanag ng isa sa pinakamahalagang implikasyon ng UTXO model.

Kung may magtatangkang gastusin ang parehong output nang dalawang beses, tinatanggihan ng mga node ang pangalawang pagtatangka dahil pinapanatili nila ang ledger at kayang beripikahin kung nagastos na ang UTXO na iyon. Ganito pinipigilan ng Bitcoin ang double-spending nang hindi nangangailangan ng sentralisadong kumpanya ng pagbabayad para magtala. Napakaganda ng halimbawa dito dahil ipinapakita nito kung paano pinagsasama ni Alice ang mga UTXO, nagpapadala ng pondo kay Bob, tumatanggap ng sukli, at naia-update ang ledger sa lahat ng node kapag nakumpirma ang transaksyon.

Isang malinaw na paraan ng pagsasabi nito sa klase ay:

Pinipigilan ng Bitcoin ang double-spending dahil sinusubaybayan ng network kung aling mga output ang hindi pa nagagastos at alin ang nagamit na.

###### Pagwawakas at Pagsusuri ng Pagkaunawa

Tapusin gamit ang ilang mabilis na tanong:

* Ano ang pagkakaiba ng public key at private key?
* Ano ang pinapatunayan ng digital signature?
* Bakit mahalaga ang hashing sa Bitcoin?
* Ano ang mangyayari kung mabago ang isang transaksyon pagkatapos itong ma-hash?
* Ano ang UTXO sa simpleng paliwanag?
* Paano pinipigilan ng network na magastos ng isang tao ang parehong bitcoin nang dalawang beses?

#### Tala para sa Guro

Ang kabanatang ito ay naglalaman ng mas teknikal na wika kaysa sa mga naunang bahagi, kaya bigyang-priyoridad ang kalinawan, analogy, at pag-uulit.

Ang layunin ay hindi gawing developer ang mga estudyante. Ang layunin ay tulungan silang maintindihan kung bakit gumagana ang seguridad ng Bitcoin.

Ang pinakamahalagang punto na dapat bigyang-diin kung kapos sa oras ay:

* private key vs public key
* digital signatures
* ano ang ginagawa ng hashing
* UTXOs bilang mga pirasong maaaring gastusin ng bitcoin
* kung paano naiiwasan ang double-spending

Ang pinaka-kapaki-pakinabang na mga visual sa kabanatang ito ay:

* ang user-wallet-network na diagram
* ang visual ng digital signature
* ang mga halimbawa ng hashing at mga diagram ng fixed-length output sa mga pahina 7 hanggang 10
* ang mga UTXO diagram sa mga pahina 10 hanggang 12

##### Ano ang Magandang Resulta

* Mahalagang ituring ang cryptography bilang pundasyon at hindi misteryo, gumamit ng maraming visual, iwasan ang malalim na matematika, ikonekta sa mga naunang kabanata, at subukin ang pagkaunawa gamit ang mga aplikasyon tulad ng "Kung may magbago ng isang transaksyon, ano ang masisira?"
* Dapat maging matiyaga ang mga guro sa mga estudyanteng nahihirapan, mag-isip nang biswal at iguhit ang lahat, maging tapat sa kung ano ang hindi kailangang maintindihan ng mga estudyante, maging handang magsabi ng "Hindi ko alam pero ganito natin malalaman," at manatiling nakapagpapalakas ng loob sa buong proseso.
* Naiintindihan ng mga estudyante kung bakit hindi maaaring ma-hack ang Bitcoin dahil pinoprotektahan ito ng matematika, nirerespeto ang eleganteng disenyo ng sistema, komportable sa pagiging komplikado kahit hindi alam ang lahat ng detalye, nagkakaroon ng kumpiyansa na magtanong nang walang panghuhusga, at napapansin nilang umangat ang kanilang pagkaunawa sa isang bagay na karamihan ay hindi alam.
* Makakamit ang Learning Outcomes kung maipapaliwanag ng mga estudyante ang mga batayan ng cryptography tulad ng one-way functions at digital signatures nang hindi kailangang magpakadalubhasa sa matematika, naiintindihan ang UTXO model na nagpapakita na coins ang pagmamay-ari mo at hindi account, nakikilala ang hashing bilang pundasyon ng seguridad ng Bitcoin, nauunawaan ang anatomy ng transaksyon kabilang ang signatures at confirmations, naipapaliwanag kung bakit immutable ang Bitcoin, at nakakapagtanong ng mahahalagang tanong tungkol sa mga posibleng atake o kahinaan.

##### Pamamahala ng Oras

Kung kapos sa oras, unahin ang mga sumusunod:

* Pribadong susi vs pampublikong susi
* Digital na lagda
* Ano ang ginagawa ng hashing
* UTXO bilang mga piraso ng bitcoin na maaaring gastusin
* Paano napipigilan ang dobleng paggastos

Kung maaga, maglaan ng oras sa mga sumusunod:

* User-wallet-network na diagram at biswal na modelo ng seguridad
* Biswal ng digital na lagda: detalyadong proseso ng cryptography
* Merkle trees at seguridad ng chain
* Mga advanced na paraan ng pag-atake at kung bakit ito nabibigo

##### Kung Nahihirapan ang mga Estudyante

* Cryptography na nakakatakot → "Araw-araw mo itong ginagamit; ganito rin ang paggamit ng My First Bitcoin."
* Hashing bilang konsepto → Analohiya ng fingerprint; natatangi, hindi mababago nang hindi nagbabago ang hash.
* Digital na lagda → "Pinapatunayan ang awtorisasyon nang hindi isiniwalat ang password."
