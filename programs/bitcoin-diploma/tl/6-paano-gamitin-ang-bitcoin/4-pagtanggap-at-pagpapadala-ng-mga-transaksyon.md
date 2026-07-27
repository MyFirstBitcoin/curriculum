# 6.4 Pagtanggap at Pagpapadala ng mga Transaksyon

Ang isang Bitcoin transaction ay paglilipat ng pagmamay-ari ng bitcoin sa isang bagong may-ari. Tandaan na hindi ang aktwal na mga coin ang naililipat, kundi ang pagmamay-ari ng mga ito: sa madaling salita, ang karapatang gastusin ang mga ito. Sa tuwing ang isang transaksyon ay tinatanggap sa isang block, lahat ng node sa network ay ina-update ang kanilang lokal na kopya ng pampublikong ledger upang ipakita ang pagbabago ng pagmamay-ari. Sa aspetong ito, ang isang Bitcoin transaction ay mas kahalintulad ng isang transaksyon sa real estate (o ibang ari-arian) kaysa sa isang transaksyon gamit ang salapi.

Upang "magpadala" ng bitcoin, ang nagpapadala ay pumipirma ng isang mensahe gamit ang kanyang private key, bilang hudyat sa network na nailipat na ng tamang may-ari ng bitcoin ang pagmamay-ari nito sa tatanggap.

Ang bitcoin ay ngayon nakatali na sa address ng tatanggap, na nagbibigay sa kanya ng pagmamay-ari ng bitcoin, kaya't tanging ang bagong may-ari lamang ang maaaring gumastos nito gamit ang kanyang private key.

Ang mga bagong Bitcoin transaction ay sinisimulan mula sa mga wallet sa iba't ibang panig ng mundo, ngunit walang sentralisadong tagaproseso ng bayad. Sa halip, ang mga miner ay nagkakaroon ng kumpetisyon upang maitala ang mga transaksyon sa ledger.

Halimbawa, may utang si Jim kay Eliana ng 0.5 BTC at handa na siyang bayaran ito. Pareho silang may digital wallet.

1. Ibinahagi ni Eliana ang kanyang address kay Jim.
1. Ginagamit ni Jim ang kanyang wallet software upang likhain ang transaksyon, na kinabibilangan ng address ni Eliana, ang halagang ililipat (0.5 BTC), at isang bayad para sa miner. Mas mataas na bayad ay nagpapataas ng posibilidad na maisama ng miner ang transaksyon sa susunod na block.
1. Pagkatapos mapirmahan ang transaksyon, ito ay ibinobroadcast sa network, kung saan ito ay tinitiyak ng mga node. Sini-check nila kung may sapat na pondo si Jim at siya ang tamang may-ari ng mga coin na nais niyang gastusin. Kung hindi, agad nilang tinatanggihan ang transaksyon.
1. Kapag na-verify na ang transaksyon, pipiliin ng mga miner kung isasama ang transaksyon sa susunod na block, kadalasan batay sa napiling bayad. Kapag ang transaksyon ay napasama na sa isang block, ito ay idinadagdag sa blockchain at ang pondo ay naililipat sa address ni Eliana.
1. Naipasa na ang pagmamay-ari kay Eliana. Maaari na niyang gamitin ang kanyang private key upang gastusin ang pondo.

_Mahalagang tandaan na kapag natapos na ang transaksyon, hindi na ito maaaring baligtarin._


> **Light – Paano Gumagana ang Isang Bitcoin Transaction**
>
> 1. May isang humihiling ng transaksyon
> 1. Ang transaksyon ay ibinobroadcast sa mga P2P computer (node)
> 1. Tinitiyak ng mga miner ang transaksyon
> 1. Pinagsasama-sama ang mga transaksyon upang bumuo ng isang data block
> 1. Ang bagong block ay idinadagdag sa umiiral na blockchain
> 1. Tapos na ang transaksyon



> **Light – Pagtanggap ng Bitcoin Transaction**
>
> Upang makatanggap ng bitcoin, kailangan mong ibigay sa nagpapadala ang iyong Bitcoin public address. Ito ay isang natatanging string ng mga letra at numero na kumakatawan sa iyong wallet at ginagamit upang kilalanin ito sa Bitcoin network.
>
> Maaari mong makita ang iyong public address sa pamamagitan ng pagbubukas ng iyong Bitcoin wallet at hanapin ang opsyon na “Receive” o “Deposit” bitcoin.
>
> Maaari mo nang ibahagi ang iyong Bitcoin address sa isa sa ilang paraan:
>
> 1. **Kopyahin at i-paste ang address**: Maaari mong kopyahin ang address sa pamamagitan ng pag-highlight nito at pagpindot sa "Copy", pagkatapos ay i-paste ito sa isang email o mensahe.
> 1. **Ibahagi ang link ng iyong Bitcoin wallet**: Ang ilang Bitcoin wallet ay nagpapahintulot sa iyo na gumawa ng link papunta sa iyong wallet na maaari mong ibahagi sa nagpapadala. Maaari nilang i-click ang link upang ma-access ang iyong wallet at magpadala ng bitcoin.
> 1. **Ibahagi ang QR code**: Kung ang nagpapadala ay may smartphone na may Bitcoin wallet app, maaari nilang i-scan ang QR code upang makuha ang iyong Bitcoin address.


Kapag nakuha na ng nagpapadala ang iyong address, maaari ka na niyang padalhan ng bitcoin sa pamamagitan ng paglalagay ng iyong address at ang halagang nais niyang ipadala. Ang bitcoin ay ipapadala mula sa kanilang wallet papunta sa iyong wallet.

Ang transaksyon ay kinukumpirma ng Bitcoin Network at karaniwang tumatagal ng mga 10 minuto. Para sa mas mataas na seguridad, inirerekomenda na maghintay ng dalawang kumpirmasyon, na tumatagal ng mga 20 minuto.


> **Light – Pagpapadala ng Bitcoin Transaction**
>
> Upang magpadala ng bitcoin, kakailanganin mo ng ilang bagay: isang Bitcoin wallet, ang public address ng tatanggap, at ang halaga ng bitcoin na nais mong ipadala.
>
> 1. Buksan ang iyong Bitcoin wallet.
> 1. Pumunta sa “Send” button at i-paste ang address ng tatanggap sa "To" field. Bilang alternatibo, maaari mo ring i-scan ang QR code kung nagbigay ang tatanggap.
> 1. Ilagay ang halaga ng bitcoin na nais mong ipadala sa “Amount” field.
> 1. I-double check ang address ng tatanggap at ang halagang ipapadala. Tandaan na hindi na mababawi ang mga transaksyon!
> 1. Bago i-click ang “Confirm and Send”, inirerekomenda naming i-double check mo pa ulit ang mga detalye ng transaksyon upang matiyak na tama ang halaga ng bitcoin at address na iyong pinapadalhan.
> 1. I-broadcast ang transaksyon at maghintay na makumpirma ito ng network.
>
> Ngayon alam mo na kung paano suriin, pumili, at mag-set up ng self-custodial Bitcoin wallet. Ang pagpapadala at pagtanggap ng bitcoin sa Bitcoin network ay tinatawag na “on-chain” transactions. Ito ay dahil ang mga transaksyon ay nangyayari sa pangunahing Bitcoin network at naitatala sa blockchain.
>
> Ang on-chain transactions ang pinakaligtas na paraan ng pag-transact gamit ang bitcoin dahil sa desentralisadong beripikasyon na ibinibigay ng network.
>
> Gayunpaman, ang on-chain transactions ay mas mabagal at maaaring mas mahal kumpara sa ibang opsyon (na tatalakayin natin sa Module 7) dahil sa bayad sa miner.


#### Gawain: Mga Transaksyon sa Aksyon


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Ito ay isang kooperatibong ehersisyo na nagpapasimple sa mga pangunahing papel ng mga taong kasangkot sa isang Bitcoin transaction.**

###### Mga Pangunahing Punto

1. May apat na uri ng kalahok sa bawat bitcoin transaction: ang nagpapadala, ang tatanggap, ang mga miner, at ang mga node operator.
1. Dapat aprubahan ng nagpapadala (cryptographically sign) ang **halaga ng bitcoin** na ipapadala AT ang **partikular na address** na padadalhan.
1. Ang tatanggap ay kailangang magbigay ng **wastong address** sa nagpadala AT tiyakin na matagumpay na nakumpirma ang transaksyon sa blockchain.
1. Tinitiyak ng mga minero na lahat ng pamantayan ay tama bago idagdag ang mga transaksyon sa mga susunod na block.
1. Tinitiyak ng mga operator ng node na tama ang mga namina na block bago i-update ang kanilang bersyon ng blockchain (ang ledger).

###### Tip ng Mag-aaral

Umikot sa lahat ng apat na papel upang maranasan kung ano ang ginagawa ng bawat kalahok.
