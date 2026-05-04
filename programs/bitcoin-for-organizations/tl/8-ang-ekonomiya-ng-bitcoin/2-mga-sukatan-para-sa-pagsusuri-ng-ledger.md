# 8.2 Mga Sukatan para sa Pagsusuri ng Ledger

Dahil ang transparency ng Bitcoin ay kakaiba kumpara sa tradisyonal na mga sistemang pinansyal — kung saan karamihan ng daloy ng pera ay nangyayari sa likod ng mga saradong pinto ng mga institusyon — nagbubukas ito ng malawak na larangan ng on-chain analytics, kung saan ang datos sa antas ng network ay nagiging lente para maunawaan ang kilos ng mga gumagamit, daloy ng pera, at mga pangmatagalang uso. Ang mga metrikang ito ay makakatulong sagutin ang mga partikular na tanong, tulad ng kung gaano kaaktibo ang paggamit ng network, kung ang mga coin ay iniipon o ibinibenta, at kung ang network ay nagiging mas ligtas.

Ang pag-unawa sa mga metrikang ito ay kapaki-pakinabang hindi lang para sa mga gumagamit ng Bitcoin, kundi pati na rin sa mga mananaliksik o gumagawa ng polisiya na naghahanap ng pananaw sa natatanging transparent na sistemang pinansyal na ito.

Ang seksyong ito ay naglalaman ng ilang karaniwang ginagamit na metrika para sa pagsusuri ng aktibidad sa Bitcoin na pinagsama sa mga sub-kategorya. Hindi ito isang kumpletong listahan. Bisitahin ang [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) para sa mas kumpletong listahan at mga paliwanag.



#### 8.2.1 Mga Metrika ng Address

Ang mga metrika ng address ay kapaki-pakinabang na subaybayan sa paglipas ng panahon dahil ipinapakita nito ang antas ng aktibidad sa Bitcoin network. Halimbawa, habang mas tinatanggap ang Bitcoin, tumataas ang bilang ng mga aktibong address. Maaari pa natin itong suriin sa pamamagitan ng pagtukoy ng bilang ng mga address na may hawak na tinakdang minimum na halaga ng Bitcoin, halimbawa 0.1 BTC, sa loob ng isang partikular na panahon, tulad ng isang taon. Bagama't nagbibigay ito ng pananaw sa paglaganap ng Bitcoin sa paglipas ng panahon, hindi ito perpekto dahil maaaring magmay-ari ang isang tao ng maraming Bitcoin address. Sa kabilang banda, ang mga exchange o ETF ay maaaring lumitaw bilang iisang entidad kahit na humahawak ng pondo para sa maraming tao.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Mga Address na Nagho-Hodl ng Bitcoin > X BTC kada Taon. Pinagmulan: Bitcoin Magazine Pro._

Sa pamamagitan ng paghahambing ng mga address sa kasalukuyang presyo ng BTC sa merkado, posible nating makita ang porsyento ng kabuuang Bitcoin address na may kita. Pinapayagan tayo nitong subaybayan ang sentimyento ng merkado dahil makikita natin kung anong bahagi ng merkado ang nagho-hold ng BTC na may kita o lugi.

Halimbawa, ang **Porsyento ng Hindi Pa Natatanggap na Kita** na tsart sa ibaba ay nagpapakita ng proporsyon ng lahat ng ledger address na may hindi pa natatanggap na kita na sinusukat sa US dollars. Tandaan na, dahil ang tsart sa ibaba ay kinuha malapit sa all-time high ng Bitcoin, ang porsyento ng mga address na nagpapakita ng hindi pa natatanggap na kita ay halos isang daang porsyento. Makikita rin natin na ang matagal na panahon ng Porsyento ng Hindi Pa Natatanggap na Kita na mas mababa sa isang standard deviation mula sa mean ay hindi karaniwan. Kaya, ang pagbaba sa linyang ito ay maaaring magpahiwatig ng magandang pagkakataon para sa mga mamimili.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Porsyento ng Hindi Pa Natatanggap na Kita. Pinagmulan: checkonchain.com_



#### 8.2.2 Mga On-Chain Indicator

Ang mga on-chain indicator ay kapaki-pakinabang dahil nagbibigay ito ng pananaw sa kilos ng network, lampas sa ipinapakita ng presyo at address metrics lamang. Tinutulungan nito ang mga analyst na maunawaan ang mga kilos at sentimyento ng iba't ibang uri ng kalahok, tulad ng mga pangmatagalang holder kumpara sa mga panandaliang trader, sa pamamagitan ng pagsubaybay kung paano hinahawakan, inililipat, o binibigyang-halaga ang mga coin sa paglipas ng panahon. Ang mga indicator na ito ay umaasa sa transparent na katangian ng ledger upang ipakita ang mga nakatagong dinamika ng merkado tulad ng pag-iipon, pamamahagi, o kahit paniniwala ng mga mamumuhunan. Ginagawa nitong partikular na kapaki-pakinabang ang mga ito para matukoy ang mga estruktural na uso, suriin kung ang merkado ay sobra o kulang ang halaga, at asahan ang mga turning point sa isang market cycle.

Halimbawa, sa pamamagitan ng pagsusuri sa halaga ng BTC na hawak mula noong huli itong nailipat, maaari nating matukoy kung ang merkado ay nasa ilalim ng stress (tulad ng maaaring mangyari sa isang malaking cycle low). Ang metrikang ito ay tinatawag na **Realised Price** at nagbibigay sa atin ng 'average cost basis' ng lahat ng BTC na umiikot. Kung ang presyo sa merkado ay bumaba sa ilalim ng Realised Price, ipinapakita nito na sa kabuuan, karamihan ng mga address ay nagho-hold ng papel na lugi.

Sa pamamagitan ng karagdagang pag-grupo ng datos ng ledger sa mga age band, maaari nating ipakita kung paano gumagalaw ang dami ng BTC sa pagitan ng mga address sa paglipas ng panahon, na lumilikha ng mga wave-like na pattern sa isang tsart na tinatawag na **HODL waves**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL Waves. Pinagmulan: Bitcoin Magazine Pro._

Ipinapakita ng HODL waves kung ano ang ginagawa ng mga pangmatagalan, panggitnang panahon, at panandaliang holder sa kanilang BTC. Halimbawa, sa tsart sa itaas, ang mga panandaliang holder ay ipinapakita sa pula at kahel at makikita natin ang mga pagtaas ng aktibidad habang ang grupong ito ay nagmamadaling bumili malapit sa tuktok ng merkado. Sa kabilang dulo, makikita natin na ang mga tunay na pangmatagalang holder (sa lila at asul) ay patuloy na tumataas ang kabuuang bahagi sa network, na nagpapahiwatig ng mataas na paniniwala sa mga grupong ito. Hindi perpekto ang tsart dahil maaaring lumipat ang ilang coin mula sa luma patungo sa bagong address na kontrolado pa rin ng parehong gumagamit. Gayunpaman, nagbibigay ito ng kawili-wiling pananaw sa paniniwala ng mga pangmatagalang holder.

Isa pang paraan ng pagsusuri sa 'smart money' ng mga pangmatagalang holder ay ang pagtingin sa **Coin Days Destroyed** (CDD). Ang konsepto ng 'Coin Days' ay produkto ng bilang ng BTC na pinarami sa bilang ng araw mula nang huling nailipat ang mga coin. Halimbawa, ang 5 BTC na hindi gumalaw sa loob ng 100 araw ay may 500 coin days at ang 10 BTC na hindi gumalaw sa loob ng 10 araw ay may 100 coin days. Sa ganitong paraan, binibigyan natin ng dagdag na bigat ang mga coin na mas matagal na hawak. Kapag nailipat ang mga coin na iyon, ang coin days ay 'nasisira'. Ipinapakita ng indicator na ito ang pagtaas ng CDD sa mga panahon ng makabuluhang galaw ng presyo, na nagbibigay sa mga analyst ng paraan upang paghiwalayin ang karaniwang aktibidad ng merkado mula sa makabuluhang pagbabago sa sentimyento ng mga pangmatagalang holder.

Isa pang metrika na maaaring makatulong matukoy kung ang merkado ay kulang o sobra ang halaga ng BTC ay ang Market-Value to Realised Value o **MVRV**. Ito ay simpleng kinukwenta bilang ratio ng Market Value (bilang ng BTC na umiikot na pinarami sa presyo sa merkado) na hinati sa Realised Value (ang kabuuan ng lahat ng BTC mula nang huli silang nailipat). Ang mataas na MVRV ay nagpapahiwatig na mas maraming coin ang may kita (karaniwang nakikita malapit sa tuktok ng merkado) at ang mababang MVRV ay nagpapahiwatig na maraming coin ang hawak na lugi (nakikita malapit sa ilalim ng merkado).



#### 8.2.3 Mga Metrika ng Pagmimina

Ang mga metrika ng pagmimina ay kapaki-pakinabang para maunawaan ang seguridad, insentibong pang-ekonomiya, at pangkalahatang kalusugan ng Bitcoin network. Ang mga metrika tulad ng hashrate, kita ng minero, difficulty, at fee ratios ay nagpapakita kung gaano kalaking computational power ang nagse-secure ng blockchain at kung gaano kabuti ang kabayaran sa mga minero para sa kanilang aktibidad.

Ang **Hashrate** ng Bitcoin network ay marahil ang pinaka-karaniwang tinutukoy na indicator ng kalusugan ng network at lakas ng seguridad. Dahil ang proseso ng pagmimina ang nagse-secure ng network at nagkukumpirma na ang mga transaksyon sa ledger ay balido, mas mataas ang antas ng computing (o hashing) power, mas mahirap para sa isang masamang aktor na mapabagsak at atakihin ang network.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Pinagmulan: Bitcoin Magazine Pro._

Ipinapakita ng tsart sa itaas na, noong Mayo 2025, ang kabuuang computing power ng network ay nasa humigit-kumulang 900 TeraHash/s (900 Trilyong cryptographic na 'hash' na kalkulasyon bawat segundo). Kung tumataas ang hashrate, ipinapakita nito na ang network ay nagiging mas ligtas, na nagbibigay ng kapanatagan sa mga gumagamit.

Ang Puell Multiple (na nilikha ni David Puell) ay tumitingin sa market cycle mula sa pananaw ng mga minero at ng kanilang kita. Kinukwenta ang metrika sa pamamagitan ng paghati ng araw-araw na paglabas ng BTC (sa USD) sa 365-araw na moving average ng halaga ng araw-araw na paglabas. Tinutulungan ng metrika na ito na matukoy ang mga panahon ng stress o ginhawa ng mga minero. Sa kasaysayan, ang multiple na higit sa 3 ay nauuna sa pagbaba ng market value ng BTC, dahil nagpapahiwatig ito na ang mga minero ay lubos na kumikita. Ang halaga na mas mababa sa 0.5 ay nagpapahiwatig ng stress at sa kasaysayan ay nagpakita ng mga ilalim ng merkado para sa halaga ng BTC.
