# 6.2 Panimula sa mga Wallet

Hindi tulad ng pisikal na pera, ang bitcoin ay hindi talaga nakaimbak sa isang Bitcoin wallet. Sa halip, ito ay nasa distributed ledger na palaging sinusuri at pinoprotektahan ng Bitcoin network. Kaya, paano mo pagmamay-ari ang bitcoin?

May pagmamay-ari ka lamang ng iyong bitcoin kung ikaw ang may kontrol sa mga private key na nagbibigay-daan sa iyong mag-sign ng mga transaksyon at ilipat ang pagmamay-ari ng iyong bitcoin sa iba. Ito ang mismong proseso ng pagpapadala ng bitcoin.

Tingnan natin ang dalawang konsepto na tinutukoy natin kapag ginagamit ang salitang **wallet**:

* Isang master private key, na parang password, kung saan nagmumula ang iyong mga public key, na parang mga email address. Maaari mong ibahagi ang iyong public address sa iba para makatanggap at makapagpadala ng bitcoin, ngunit huwag kailanman ibahagi ang iyong private key!
* Ang mobile o desktop interface na ginagamit upang makipag-ugnayan sa Bitcoin network, tingnan ang iyong bitcoin balance, magpadala at tumanggap ng mga transaksyon, at i-broadcast ang mga ito sa network. Iba't ibang uri ng wallet, kasama ang kanilang mga benepisyo at kapalit, ay ilalarawan sa mga susunod na seksyon.

#### Self-Custodial vs Custodial Wallets

Bago talakayin ang iba't ibang uri ng Bitcoin wallet at ang kanilang mga katangian, mahalagang malaman ang pagkakaiba ng self-custodial at custodial wallets. Bawat uri ay may sariling benepisyo, panganib, at antas ng kontrol sa bitcoin. Ang self-custodial ay nangangahulugang ang user ang may hawak ng private keys at tunay na may kontrol sa kanilang bitcoin; sa custodial wallets, isang third party ang may hawak ng bitcoin para sa user.


| Uri | Kontrol | Mga Benepisyo | Mga Panganib |
| --- | --- | --- | --- |
| Self-Custodial | Ang user | Kumpletong kontrol sa pondo at mga transaksyon, walang approval process o pag-freeze ng account, walang kontrol ng kumpanya o gobyerno, protektado laban sa kumpiskasyon. | Walang recovery kung mawala ang recovery phrase, buong responsibilidad ay nasa user. |
| Custodial | Ang third-party provider | Madaling recovery kung mawala ang access, mas madaling customer support. | Ang pondo ay konektado sa Internet, mas madaling ma-hack. Maaaring i-freeze ng custodian ang mga account. |


Sa isang self-custodial wallet (tinatawag ding non-custodial wallet), ikaw lang ang may hawak ng mga susi ng wallet at ikaw ang may buong kontrol sa lahat ng papasok at palabas. Sa kabilang banda, sa custodial wallet, ibang tao ang may hawak ng private key, kaya't sila ang may buong access na ilipat ang anumang bitcoin na hawak ng provider para sa iyo.

* Ang self-custody ay parang ikaw mismo ang iyong bangko. Ang mga transaksyon ay hindi dumadaan sa pagsusuri at kontrol
* Tinitiyak ng self-custody na hindi makukuha ng ibang tao ang iyong bitcoin.
* Nagbibigay ng kapanatagan ang self-custody sa panahon ng kawalang-katiyakan, dahil alam mong ligtas ang iyong bitcoin.

Mahalagang pumili ng tamang uri ng wallet para sa pangangailangan ng bawat isa. Minsan, nahihirapan ang mga tao na malaman kung self-custodial o custodial wallet ba ang kanilang ini-install. Ipinapakita ng talahanayang ito ang mga pagkakaiba sa proseso ng pag-install.


| Uri | Hakbang 1: Pumili | Hakbang 2: I-install | Hakbang 3: Gumawa | Hakbang 4: Siguraduhin |
| --- | --- | --- | --- | --- |
| Self-Custodial | Pumili ng self-custodial wallet | Sundin ang mga tagubilin ng wallet | Gumawa ng recovery phrase | Itago ang recovery phrase sa ligtas na lugar |
| Custodial | Pumili ng custodial wallet | Sundin ang mga tagubilin ng wallet | Gumawa ng account | N/A |


“**Not your keys, not your coins**” ay isang tanyag na kasabihan sa mga may hawak ng bitcoin. Tumutukoy ito sa ideya na kung wala kang direktang kontrol sa private keys na konektado sa iyong Bitcoin wallet, wala kang tunay na pagmamay-ari sa mga coin.

Kung sino man ang may access sa iyong private keys, siya ang may pagmamay-ari ng iyong bitcoin. Kaya napakahalaga na protektahan ang mga ito at ilayo sa mga mapanuring mata! Tatalakayin natin ang ilang paraan kung paano mo ito magagawa sa mga susunod na bahagi ng aklat.

Sa mga susunod na bahagi, tatalakayin natin ang tungkol lamang sa self-custodial wallets, kung saan ang user ang may hawak ng kanilang mga susi at may ganap na kontrol sa kanilang bitcoin.

Huwag mag-alala kung tila komplikado o hindi mo agad maintindihan ang lahat — ito ay isang paglalakbay, at mas mauunawaan mo ito habang ginagamit mo ang Bitcoin!

#### Iba't Ibang Uri ng Bitcoin Wallet

Kung saan nilikha at iniimbak ang iyong private key ang nagtatakda kung paano natin inilalarawan ang Bitcoin wallets. Kung ang mga susi ay nasa iyong smartphone, ito ay isang **mobile wallet**. Kung ito ay nakaimbak nang ligtas sa isang dedikadong aparato, ito ay isang **hardware wallet**.


| Uri | Paglalarawan | Mga Kalamangan | Mga Kahinaan | Halimbawa ng Gumagamit |
| --- | --- | --- | --- | --- |
| Online Wallet | Ina-access gamit ang web browser | Maaaring ma-access mula sa kahit anong device na may internet connection | Mas hindi ligtas dahil maaaring ma-hack o makompromiso | Kailangang madalas gamitin ang wallet at hindi nag-iimbak ng malaking halaga |
| Mobile Wallet | Ini-install sa mobile device | Madaling gamitin | Maaaring mawala kung manakaw o ma-hack ang device | Kailangang mag-transaksyon habang naglalakbay at hindi nag-iimbak ng malaking halaga |
| Desktop Wallet | Ini-install sa desktop computer | Maginhawa at maaaring ma-access kahit saan | Maaaring ma-hack kung may malware ang computer | Nais mag-imbak ng malaking halaga ng bitcoin at komportable gumamit ng desktop computer |
| Hardware Wallet | Isang pisikal na aparato na nag-iimbak ng bitcoin offline | Mas ligtas kaysa online wallets at maaaring gamitin offline | Maaaring hindi na mabawi ang pondo | Nais mag-imbak ng malaking halaga ng bitcoin at handang magbayad para sa dagdag na seguridad |


Dahil maaaring ilipat ang mga key mula sa isang device papunta sa iba, ang “status” ng iyong Bitcoin wallet ay hindi permanente. Halimbawa, kung nilikha ko ang wallet keys sa computer at inilipat ko ito sa aking telepono, ang “desktop wallet” ay nagiging “mobile wallet.”

Pagdating sa pag-iimbak ng iyong bitcoin, hindi lang ito tungkol sa kung sino ang may kontrol sa mga key — marami pang ibang panganib na dapat isaalang-alang. Kaya mahalagang makahanap ng storage solution na parehong ligtas at maginhawa. Kapag inaral mo ang mga trade-off ng iba't ibang uri ng wallet, matututuhan mong walang perpektong wallet na makakatugon sa lahat ng pangangailangan.

##### Mga dapat isaalang-alang sa pagpili ng wallet

* **Seguridad**: Siguraduhing may matibay na security measures ang wallet.
* **Pribasiya**: Isaalang-alang kung nangangailangan ng personal na impormasyon ang wallet.
* **Dali ng paggamit**: Pumili ng wallet na madaling gamitin at i-navigate.
* **Kompatibilidad**: Siguraduhing compatible ang wallet sa iyong device.
* **Mga Bayarin**: Ihambing ang mga bayad na sinisingil ng iba't ibang wallet.
* **Reputasyon**: Suriin ang reputasyon ng mga developer upang matiyak na sila ay mapagkakatiwalaan.
* **Kontrol**: May mga wallet na nagbibigay ng mas malaking kontrol sa iyong private keys.

##### Open Source vs Closed Source

Isa pang mahalagang bagay na dapat tandaan sa pagpili ng Bitcoin wallet ay kung ang application o software ay open-source. Mahalaga ito dahil ang open-source na proyekto ay nagpapahintulot sa komunidad na suriin ang code at ipagpatuloy ang proyekto kung titigil ang team sa paggawa nito. Katulad ng code ng Bitcoin na bukas para sa lahat upang suriin, gamitin, at baguhin, ganoon din dapat ang code ng wallet na gagamitin mo para pamahalaan ang iyong bitcoin.

#### Gawain: Talakayan at pagsusuri ng mga Bitcoin wallet

https://bitcoin.org/en/choose-your-wallet

Pumunta sa sumusunod na website: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Gamitin ang bago mong kaalaman tungkol sa mga Bitcoin wallet upang piliin ang pinakaangkop para sa iyong pangangailangan batay sa mga pamantayang tinalakay natin ngayon.
