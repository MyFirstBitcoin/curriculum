# 7.1 Ang Lightning Network

Ang Lightning Network ay isang sistema ng pagbabayad na nagpapahintulot sa mga gumagamit na magpadala at tumanggap ng bitcoin nang mabilis at mura. Gumagana ito sa pamamagitan ng pag-set up ng isang pinagsasaluhang wallet kung saan parehong naglalagay ng bitcoin ang dalawang partido. Pagkatapos, maaari silang magsagawa ng walang limitasyong transaksyon sa isa’t isa nang hindi kailangang irekord ang bawat isa sa pangunahing blockchain. Sa ganitong paraan, naiiwasan nila ang pangangailangang beripikahin at isama ang bawat transaksyon sa isang block, kaya’t nagiging mabilis at matipid ang proseso. Dahil mababa ang bayad, maaaring gamitin ang Lightning Network para sa maliliit na bayad na hindi laging praktikal sa on-chain. Kapag nagpasya ang dalawang partido na tapusin ang kanilang ugnayan, tanging ang huling balanse lamang ang itinatala sa blockchain.

Isipin mong nagtatrabaho ka sa isang araw sa isang kapihan. Dahil balak mong magtagal, nagbukas ka ng tab at nagbayad nang pauna imbes na magbayad sa bawat order. Sa pagtatapos ng araw, ikaw at ang may-ari ay titingnan ang tab para ayusin ang bayarin. Kung mas malaki ang deposito mo kaysa sa nagastos mo, ibabalik sa iyo ang sukli; kung mas malaki ang nagastos mo, babayaran mo ang natitirang utang.

Maaaring palawakin ang sistemang ito para isama ang mas maraming kalahok. Halimbawa, sa isa sa mga pagbisita mo sa kapihan, may kasama kang kaibigan na hindi kilala ng bartender at hindi makapagbukas ng tab. Inalok mo sa kaibigan mo na gamitin ang tab mo para sa kanilang gastos, at nagkasundo kayong babayaran ka nila nang pribado. Isipin mo na libu-libong tao ang gumagawa ng ganito nang sabay-sabay, na nagpapahintulot sa iba na gamitin ang mga umiiral na tab para kumonekta sa mas marami pang tao — ganito gumagana ang Lightning Network!

Sa Lightning, maaari kang magpadala ng bayad sa kahit sino sa network, hindi lang sa taong may direktang tab ka — basta’t may ruta na nag-uugnay sa inyo. Maaaring dumaan ang bayad mo sa network hanggang makarating ito sa destinasyon, kahit wala kang bukas na channel direkta sa tatanggap.

Tingnan natin ang pagkakaiba ng on-chain at off-chain na mga transaksyon.

##### On-Chain na mga Transaksyon

Ito ang mga transaksyong nangyayari direkta sa Bitcoin blockchain. Karaniwang tumatagal ng mga 10 minuto bago makumpirma, at ang bayad ay nakadepende sa laki ng transaksyon sa virtual bytes. Mas ligtas ito ngunit mas mabagal, dahil nangangailangan ng konsensus ng buong network.

##### Mga Transaksyon sa Lightning Network

Ang mga transaksyong ito ay nangyayari sa isang hiwalay na network na nakapatong sa Bitcoin blockchain. Mas mabilis itong naisasagawa at mas mababa ang bayad. Karaniwan itong ginagamit kung mas mahalaga ang bilis at halaga ng transaksyon. Kumpara sa on-chain na mga transaksyon, mas mababa ang seguridad nito.


|  | Bitcoin Network | Lightning Network |
| --- | --- | --- |
| Kahulugan | Isang desentralisadong digital na network na gumagamit ng cryptography para siguraduhin ang mga transaksyong pinansyal. | Isang second layer na payment protocol na gumagana sa ibabaw ng Bitcoin blockchain, na nagpapabilis at nagpapamura ng mga transaksyon. |
| Mga Kalamangan | Desentralisado at ligtas. Walang chargeback o panlilinlang. Maaaring gamitin nang pseudonymous. Tinatanggap sa buong mundo. | Mas mabilis at mas murang mga transaksyon. Mas mataas na scalability. Ang mga off-chain na transaksyon ay hindi bumabara sa blockchain. |
| Mga Kahinaan | Mabagal ang oras ng transaksyon. Mataas ang bayad para sa ilang uri ng transaksyon. Kumplikado para sa mga baguhan. | Maaaring mangailangan ng tiwala sa mga operator ng channel. Nangangailangan ng on-chain na transaksyon para magbukas at magsara ng mga channel. |
