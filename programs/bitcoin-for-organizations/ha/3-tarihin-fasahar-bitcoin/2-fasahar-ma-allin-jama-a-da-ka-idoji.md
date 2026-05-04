# 3.2 Fasahar Maɓallin Jama'a da Ka'idoji

Yanzu haka, Intanet da mafi yawan tsarin kwamfuta na zamani suna dogara da ilimin ɓoye-ɓoye, wata hanya ce ta ɓoye bayanai domin kawai wanda aka aika masa da bayanin ne zai iya fassara su. Asalin ilimin ɓoye-ɓoye da ake amfani da shi wajen kare Bitcoin ana iya bin sawunsa tun daga shekarun 70.

Matsalar farko da za a warware ita ce – yadda za a aika sirrin da aka raba ta hanyar da ba ta da tsaro.

Whitfield Diffie da Martin Hellman ne suka fara duba wannan batu.

Matsalar: bangarori biyu – galibi ana kiran su da Aisha da Bala – suna son su raba bayanan sirri ta hanyar hanyar sadarwa inda wasu na iya sauraro. Don cimma wannan, suka kirkiro tsarin musayar maballin Diffie-Hellman.

Wannan sirrin da aka raba za a iya amfani da shi a matsayin asali don ƙirƙirar maballan daidaitattu da yawa don ɓoye da fassara saƙonni da za su aika wa juna ba tare da bayyana maballin a fili ba.

Tunda ba a taɓa raba maballin sirri ba, kuma ana amfani da maballai daban-daban a kowanne ɓangare don ɓoye da fassara, ana kiran wannan da tsarin ɓoye-ɓoye na asymmetrik.

Misalan amfani:

* Aisha ta sanya hannu a kan saƙo da maballin jama'a na Bala – shi kaɗai ne zai iya fassara saƙon ta amfani da maballin sirrinsa
* Aisha ta sanya hannu a kan saƙo da maballin sirrinta – ta hanyar fassara da maballin jama'arta kowa zai iya tabbatar da cewa Aisha ce ta aika saƙon, ba tare da sanin maballin sirrinta ba
* Idan aka haɗa waɗannan hanyoyi biyu da matakai biyu na ɓoye-ɓoye, za a iya aika saƙo da aka ɓoye wanda Bala kaɗai zai iya fassara, sannan zai iya tabbatar da cewa Aisha ce ta aiko masa

Ko da yake ba a rubuta sunansa a takarda ba, Ralph Merkle ya taka muhimmiyar rawa wajen taimakawa warware abin da ake ganin ba zai warware ba a wancan lokacin – yadda za a kafa ko dawo da sadarwar sirri a kan hanyar sadarwa da ke bude kuma mai yiwuwa da hatsari.

Wannan hanyar ita kaɗai tana da rauni ga harin ƙoƙari da ƙarfi (brute force), inda mai hari zai iya ɗaukar lambobin da aka raba ya ƙirƙiri maballin da aka raba daga baya idan ya samu lokaci da albarkatu, don haka ba cikakkiyar mafita ba ce ita kaɗai.

##### Ka'idoji don Tsarin Maballin Jama'a na Ilimin ɓoye-ɓoye

Baya ga taimakawa wajen tsarin maballin jama'a na Diffie-Hellman da aka bayyana a sama, **Ralph Merkle** ya ci gaba da bada gudummawa a wannan fanni na tsawon shekaru, kuma ya taka muhimmiyar rawa wajen haɓaka wasu muhimman abubuwa da ake amfani da su a Bitcoin.

Aikin hash na ilimin ɓoye-ɓoye wata dabara ce ta lissafi da ke karɓar bayanai masu girma ko ƙanƙanta kuma ta aiwatar da lissafi mai rikitarwa don samar da ƙimar hash a cikin bits, wanda galibi ake wakilta da sakamako mai tsawon dindindin na haruffa da lambobi ta amfani da tsarin hexadecimal.

* Ana iya shigar da bayanai masu girma ko ƙanƙanta
* Sakamakon koyaushe yana da tsawon dindindin kuma yana da tabbaci (idan an shigar da abu ɗaya, za a samu hash ɗaya koyaushe)
* Yana da sauƙin tabbatarwa amma yana da matuƙar wahala a juya baya don gano abin da aka shigar
* Ko ƙaramin canji a bayanan zai sauya sakamakon gaba ɗaya

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/1d5c5131cb38ab07330b740866109d8486b25d10-515x331.svg)

Hashing muhimmin ɓangare ne na tsarin My First Bitcoin. SHA-256, wanda ake amfani da shi a Bitcoin, hukumar NSA ce ta ƙirƙira shi kuma misali ne na dabara ta hash na ilimin ɓoye-ɓoye.

* Kowane bulok a cikin sarkar ana yin hash dinsa don kada a iya canza bayanai – hakan yana tabbatar da sahihancin littafin bayanai da aka raba.
* Hash da aka samar dole ne ya cika ka'idar 'Shaidar aiki' (Proof of work) kafin a ɗauke shi a matsayin bulok mai inganci
* Itatuwan Merkle – ta hanyar amfani da rassa da hash na hash, itatuwan hash na iya ba da damar tabbatar da manyan bayanai da ƙaramin ajiya
* Hash da sa hannu da maballai za a iya amfani da su don walat, adireshi da izinin mu'amaloli

Tantancewar da aka raba ta yanayin blockchain da tsarin littafin bayanai da ba za a iya gyarawa ba yana yiwuwa ne ta hanyar hashing mai hanya ɗaya. Ayyukan hash suna ba da hanya mai dogaro da tabbaci don tabbatar da abubuwan da suka faru a kan littafin bayanai na jama'a kamar My First Bitcoin ba tare da tsarin dogaro da cibiyar tsakiya ba.

Wadannan sabbin damar a fannin ilimin ɓoye-ɓoye, masu ƙirƙira su sun yi tsammanin za su kawo sabon juyin halitta a wannan fanni.

##### Ilimin ɓoye-ɓoye na lanƙwasa elliptic

Ɗaya daga cikin waɗannan sababbin abubuwa daga baya ya zo ne ta hanyar ilimin ɓoye-ɓoye na lanƙwasa elliptic.

An gabatar da ilimin ɓoye-ɓoye na lanƙwasa elliptic a shekarar 1985 daga masana biyu, N. Koblitz da V. Miller. Sun gabatar da ra'ayin amfani da maki da lanƙwasa elliptic suka ƙayyade maimakon filayen firam ɗin da aka saba amfani da su a tsarin musayar maballin Diffie-Hellman. Cikakkun bayanai yadda wannan ke aiki ya wuce wannan sashe, amma a taƙaice, lanƙwasa elliptic tarin maki ne da ke cika wata ƙa'ida ta lissafi.

Ƙa'idar lanƙwasa elliptic tana kama da haka:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Wannan yana da wasu fa'idodi masu amfani:

* Daidaikun maki a kan lanƙwasa za a iya juyar da su a kan layin x kuma su ci gaba da kasancewa a kan lanƙwasa ɗaya.
* Kowane layi da ba na tsaye ba zai iya haɗuwa da lanƙwasa a wurare uku kawai ko ƙasa da haka.
* Ƙananan girman maballai yana da matuƙar muhimmanci don adanawa da aika maballin jama'a cikin sauƙi a blockchain.

Wadannan siffofi za a iya amfani da su don ƙirƙirar ma'auratan maballai kamar yadda ake yi a tsarin Diffie-Hellman. My First Bitcoin na amfani da ECDSA, wanda ke nufin Elliptic Curve Digital Signature Algorithm. Tsari ne da ke amfani da lanƙwasa elliptic da fili mai iyaka don 'sa hannu' a bayanai ta yadda wasu za su iya tabbatar da sahihancin sa hannun ba tare da samun damar ƙirƙirar sa hannun ba. A cikin bitcoin, bayanan da ake sa hannu a kai su ne mu'amaloli da ke canja mallaka.

Sashen 'mai iyaka' yana kama da tsarin 'mod' a Diffie-Hellman, inda sakamakon ƙa'idar za a raba shi kuma a ɗauki saura don tabbatar da cewa yana cikin wani iyaka na lambobi.
