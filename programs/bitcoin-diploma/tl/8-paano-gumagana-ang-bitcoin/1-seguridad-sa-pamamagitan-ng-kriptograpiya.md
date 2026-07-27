# 8.1 Seguridad sa pamamagitan ng Kriptograpiya

> Ang ibinibigay sa atin ng Bitcoin ay isang matibay na pangako: ang programa ay tatakbo nang eksakto ayon sa itinakda.  
_Andreas M. Antonopoulos_

#### Kryptograpiya ng Pampubliko/Pribadong Susi


> **Definition – Kahulugan ng Kryptograpiya**
>
> **Kryptograpiya** ay ang pagsasanay ng paggawa ng impormasyon bilang isang lihim na tanging ang tamang tao lamang ang makakabasa.


* **Pag-eenkripto** ay ang proseso ng paggawa ng impormasyon bilang isang naka-kodigong anyo upang tanging ang may tamang susi lamang ang makakabasa nito.
* **Pagde-dekripto** ay ang proseso ng pagbabalik ng naka-kodigong impormasyon sa anyong nababasa.

Sa tradisyonal na kryptograpiya, ang dalawang tao na gustong mag-usap nang pribado ay kailangang magbahagi muna ng parehong lihim na susi, na parang password na pareho nilang alam. Ginagamit ng isa ang susi na ito para i-encrypt ang mensahe bago ipadala, at ginagamit ng isa pa ang parehong susi para i-decrypt at basahin ito.

Ang problema sa sistemang ito ay pareho nilang kailangang alam na ang lihim na susi. Kapag may ibang nakakuha ng susi, maaari nilang mabasa ang anumang mensaheng nasabat.

Nilulutas ng Bitcoin ang problemang ito gamit ang ibang paraan na tinatawag na pampublikong-susi na kryptograpiya, kung saan hindi na kailangang magbahagi ng lihim na susi ang mga gumagamit bago mag-usap.

Nilulutas ng pampubliko/pribadong susi na kryptograpiya ang problema ng pagbabahagi ng mga lihim. Sa halip na magbahagi ng password, bawat tao ay may dalawang susi: isang pampublikong susi at isang pribadong susi.

* Ang **pampublikong susi** ay maaaring ibahagi sa kahit sino.
* Ang **pribadong susi** ay kailangang laging itago bilang lihim.

Kung gusto ni Juan na magpadala ng mensahe kay Arel, maaari niyang gamitin ang pampublikong susi ni Arel. Tanging si Arel lamang ang makakabukas nito gamit ang kanyang pribadong susi. Kahit masabat ang mensahe, hindi ito mababasa o magagamit nang walang pribadong susi.

Sa Bitcoin, ginagamit ang sistemang ito upang lumikha ng digital na lagda. Ang digital na lagda ay nagpapatunay na ang may-ari ng pribadong susi ang nag-apruba ng transaksyon, katulad ng paglagda ng iyong pangalan sa isang dokumento. Ito ang dahilan kung bakit ligtas at mapapatunayan ang mga transaksyon sa Bitcoin nang hindi kailangang magtiwala sa ikatlong partido.

Ang mga transaksyon sa Bitcoin ay kinabibilangan ng paglilipat ng pagmamay-ari ng bitcoin mula sa isang address papunta sa iba.

Ginagamit ang pag-eenkripto upang matiyak na tanging ang tunay na may hawak ng bitcoin lamang ang may awtoridad na magpadala ng kanilang pera sa iba. Tinitiyak nito na ang kanilang ari-arian ay protektado laban sa masasamang loob.

Bilang karagdagang proteksyon, bawat transaksyon sa Bitcoin ay awtomatikong nagkakaroon ng NATATANGING digital na lagda. Ang natatanging digital na lagdang ito ay pinapagana ng teknolohiyang hindi maaaring pakialaman na tumutulong sa network na mapatunayan na ang tunay na may-ari ng bitcoin, at hindi iba, ang siyang nagpadala nito.


> **Dark**
>
> Bawat gumagamit ay may dalawang susi: isang **pribadong susi**, na **itinago bilang lihim**, at isang **pampublikong susi** na maaaring **ibahagi sa iba**. Ang **pribadong susi** ay nagsisilbing anyo ng pagkakakilanlan at patunay ng pagmamay-ari, na nagpapatunay: “Sa akin ang address na ito at ako ang may kontrol dito.”


###### Paano Gumagana ang Isang Transaksyon sa Bitcoin

1. **Paglikha ng Transaksyon**: Ang isang gumagamit ay nagsisimula ng transaksyon sa Bitcoin sa pamamagitan ng pagtukoy ng mga detalye tulad ng address ng tatanggap at halaga ng bitcoin na ipapadala.
1. **Pagbuo ng Digital na Lagda**: Ang nagpadala ay bumubuo ng natatanging **digital na lagda** gamit ang kanyang **pribadong susi**. Ang lagdang ito ay isang natatanging code na nagpapatunay ng pagiging totoo ng transaksyon.
1. **Pagpapadala ng Transaksyon**: Ang nilagdaang transaksyon ay ipinapadala sa Bitcoin network, na nagpapahiwatig ng layunin na ilipat ang pagmamay-ari ng bitcoin mula sa nagpadala papunta sa tatanggap.
1. **Pagpapatunay sa Network**: Tinatanggap ng mga node sa Bitcoin network ang transaksyon at ginagamit ang pampublikong susi ng tatanggap upang tiyakin ang pagiging totoo ng lagda ng transaksyon. Kasabay nito, ginagamit nila ang pampublikong susi ng nagpadala **pampublikong susi** upang tiyakin ang **digital na lagda**.
1. **Kumpirmasyon sa Bitcoin network**: Kapag matagumpay ang beripikasyon, ang transaksyon ay idaragdag sa ledger, na nagsisilbing ligtas at transparent na talaan ng lahat ng transaksyon. Kapag nakumpirma na, opisyal nang nailipat ang pagmamay-ari ng bitcoin mula sa nagpadala papunta sa tumanggap.


> **Callout – Buod**
>
> Ang **digital na lagda**, na nilikha gamit ang pribadong susi ng nagpadala **pribadong susi**, ay nagpapatunay na ang transaksyon ay inaprubahan ng may-ari ng bitcoin. Maari nang beripikahin ng Bitcoin network ang patunay na ito at itala ang transaksyon.


#### Paliwanag sa Hashing

Huwag kang matakot sa mga teknikal na termino at matematikal na konsepto na susunod. Naiintindihan naming hindi lahat ay mahilig sa matematika, pero baka magulat ka na kahit ang pinakamahirap na ideya ay kayang maintindihan basta may kaunting pagsisikap.


> **Definition – Depinisyon ng isang function**
>
> Ang isang **function** ay parang makina na tumatanggap ng impormasyon at ginagawang bago ito. Ang impormasyong ibinibigay mo sa function ay ang **input**. Ang bagong impormasyong nililikha ng function ay ang **output**. Tinutulungan ng mga function ang mga computer na gawin ang mga gawain at lutasin ang mga problema.


##### Ano ang function?

Ang function ay isang set ng mga tagubilin na tumatanggap ng input at gumagawa ng output. Maaari mo itong ituring na parang recipe: sundin mo ang mga hakbang gamit ang mga partikular na sangkap, at palaging pareho ang kalalabasan.

Sa Bitcoin, ginagamit ang mga function upang iproseso at beripikahin ang mga transaksyon. Kapag may nagpadala ng bitcoin, tumutulong ang mga cryptographic function na tiyakin na tama ang transaksyon, kumpirmahin na sapat ang pondo ng nagpadala, at i-update ang balanse sa Bitcoin ledger. Kapag napatunayan at naidagdag sa isang block, ang transaksyon ay nagiging bahagi ng permanenteng talaan sa blockchain.

##### Ano ang one-way function?

Ang one-way function ay isang espesyal na uri ng function na madaling gawin sa isang direksyon ngunit napakahirap baliktarin. Halimbawa, madali ang paghalo ng mga sangkap para gawing smoothie, pero hindi mo na kayang ibalik ang smoothie sa orihinal nitong mga sangkap.

Ang seguridad ng Bitcoin ay nakasalalay sa mga one-way function. Ginagamit ang mga ito sa pampubliko at pribadong key cryptography, na nagpapahintulot sa mga tao na ibahagi ang pampublikong susi habang nananatiling lihim ang kanilang pribadong susi. Kahit nakikita ang pampublikong susi, imposibleng makuha mula rito ang pribadong susi. Ito ang dahilan kung bakit ligtas ang mga transaksyon sa Bitcoin.

##### Ano ang hash function?

Ang isang **hash function** ay parang makina ng lihim na code. Tumatanggap ito ng mensahe at ginagawang code.

###### Paano Gumagana ang Hashing sa mga Transaksyon ng Bitcoin

Sa Bitcoin, bawat transaksyon ay ginagawang hash bago ito idagdag sa blockchain. Ang hash ay natatanging digital na fingerprint ng transaksyon. Kapag may nagtangkang baguhin kahit maliit na bahagi ng transaksyon, magbabago nang buo ang hash. Dahil dito, madaling matukoy ng network kung may nangyaring pakikialam.

###### Ang Papel ng Hashing sa Seguridad ng Bitcoin

Tumutulong ang hashing na protektahan ang Bitcoin network sa pamamagitan ng pagpapadali ng beripikasyon ng mga transaksyon at paggawa nitong imposibleng baguhin nang palihim. Dahil bawat transaksyon ay may natatanging hash, mabilis na natutukoy ng network kung may binago.

Ang hash function ay kumukuha ng data at ginagawang isang tiyak na haba ng mga numero at letra na tinatawag na hash. Ang parehong input ay palaging magbubunga ng parehong hash, ngunit kahit maliit na pagbabago sa input ay magreresulta sa ibang-iba na resulta. Dahil dito, madaling matiyak ng mga computer na hindi nabago ang data.


> **Definition – Depinisyon ng Hashing**
>
> **Hashing** ay parang paggawa ng fingerprint para sa digital na datos. Ito ang proseso ng pagkuha ng digital na mensahe at paggawa nito ng code na may tiyak na haba, na nagsisilbing natatanging pagkakakilanlan. Gaya ng fingerprint na nakikilala ang tao, ang hash ay nakikilala ang digital na mensahe.


Ang **output**, o hash, ay palaging may parehong haba, kahit gaano kahaba ang orihinal na impormasyon. Gumagamit ang Bitcoin ng ilang partikular na uri ng hash function na tinatawag na **SHA-256** at **RIPEMD160**.

Narito ang ilang halimbawa:

* SHA256 hash ng string **kamusta mundo**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256 hash ng string na **kamusta mundo.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Mapapansin mo na kahit maliit na pagbabago sa input ay lubos na binabago ang output kumpara sa nauna
* SHA256 hash ng mada-download na iso file **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Malaki ang input na ito ngunit ang output ay nananatiling pareho ang haba

Maaari mo ring isipin ang hashing na parang isang musical score na kumakatawan sa diwa ng isang piraso ng musika. Tulad ng musical score na natatanging representasyon ng isang tugtugin, ang hash value ay natatanging representasyon ng isang datos.

Sa paghahambing ng score ng isang piraso ng musika sa aktwal na pagganap, malalaman ng musikero kung tama ang pagkakatugtog. Sa parehong paraan, sa paghahambing ng hash value ng natanggap na datos sa orihinal na hash value, malalaman kung nabago ang datos habang ipinapadala.

Tulad ng kahit kaunting paglihis sa isang musikal na pagganap ay maaaring magpabago sa tunog nito, kahit maliit na pagbabago sa orihinal na datos ay magreresulta sa ibang hash value. Ginagawa nitong makapangyarihang kasangkapan ang hashing para tiyakin ang integridad at pagiging totoo ng isang Bitcoin transaksyon.

Ang proseso ng pag-encode ng **public key** sa pamamagitan ng hashing ay ginagamit upang mapabuti ang seguridad ng impormasyon sa pamamagitan ng paggawa nito bilang isang fixed-length na hindi nababasang format. Ginagamit ng Bitcoin ang SHA-256 at RIPEMD160 na mga algorithm upang makagawa ng mga pampublikong address. Ang resulta ay nagsisilbing natatanging pagkakakilanlan para sa **public key** at tumutulong upang tiyakin ang integridad at seguridad ng mga transaksyon na naka-imbak sa ledger. Sa pag-e-encrypt ng impormasyon sa ganitong paraan, mas mahirap para sa mga hindi awtorisadong tao na ma-access at manipulahin ang datos.

##### Mga Katangian ng Hashing Function

* **Deterministiko**: Ang parehong mga sangkap ay laging gumagawa ng parehong smoothie. Sa parehong paraan, ang parehong datos ay laging magbibigay ng parehong hash.
* **Pre-image resistance**: Kung smoothie lang ang meron ka, hindi mo malalaman ang eksaktong prutas na ginamit. Sa parehong paraan, kung hash lang ang meron ka, hindi mo matutukoy ang orihinal na datos.
* **Avalanche effect**: Kahit maliit na pagbabago sa mga sangkap ay lilikha ng ibang smoothie. Sa hashing, kahit napakaliit na pagbabago sa datos ay magbubunga ng ibang hash.
* **Collision resistance**: Napakahirap makahanap ng dalawang magkaibang set ng sangkap na magbibigay ng eksaktong parehong smoothie. Sa parehong paraan, napakabihira na dalawang magkaibang datos ay magbigay ng parehong hash.
* **Mabilis i-verify**: Mabilis gawin ang smoothie, at madali ring makita na ito ay smoothie. Ang hash functions ay mabilis kwentahin at madaling i-verify ng kahit sino.

#### Gawain: Gumawa ng SHA 256 Hash


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Nais mo bang malaman kung paano gumagana ang hashing? I-scan ang QR code para agad makagawa ng SHA256 hash mula sa kahit anong salita, pangungusap, o input na gusto mo. Ang hash functions ay parang digital na fingerprint: one-way ito, ibig sabihin kapag na-hash na, hindi na ito mababalik. Subukan mo at tingnan mo mismo!
