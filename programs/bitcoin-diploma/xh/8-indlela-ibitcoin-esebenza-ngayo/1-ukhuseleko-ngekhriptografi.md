# 8.1 Ukhuseleko ngeKhriptografi

> Oko uBitcoin asipha kona sisithembiso esinzima: inkqubo iya kwenziwa kanye njengoko kuchaziwe.  
_Andreas M. Antonopoulos_

#### Ubuchwephesha beSitshixo soLuntu/soBucala


> **Definition – Inkcazo yoBugqwetha**
>
> **Ubugqwetha** yindlela yokuguqula ulwazi lube yimfihlo enokufundwa kuphela ngabantu abafanelekileyo.


* **Ukubethela** yinkqubo yokuguqula ulwazi lube yikhowudi ukuze kuphela umntu onositshixo oluchanekileyo akwazi ukufunda.
* **Ukukhupha ikhowudi** yinkqubo yokuguqula olo lwazi lufihliweyo lube yinto enokufundwa.

Kwiindlela zobugqwetha zemveli, abantu ababini abafuna ukunxibelelana ngasese kufuneka kuqala babelane ngesitshixo esiyimfihlo, njengokungathi babelana ngephasiwedi. Omnye umntu usebenzisa esi sitshixo ukubethela umyalezo phambi kokuwuthumela, kwaye omnye umntu usebenzisa esi sitshixo sinye ukukhupha ikhowudi aze awufunde.

Ingxaki ngale nkqubo kukuba bobabini kufuneka sele benesitshixo esiyimfihlo. Ukuba omnye umntu ufumana esi sitshixo, angakwazi ukufunda nawuphi na umyalezo abawubambileyo.

My First Bitcoin isombulula le ngxaki ngokusebenzisa indlela eyahlukileyo ebizwa ngokuba bubuchwephesha be-sitshixo soluntu, apho abasebenzisi bengadingi ukwabelana ngezitshixo ezimfihlo kwangaphambili.

Ubuchwephesha be-sitshixo soluntu/soBucala busombulula ingxaki yokwabelana ngeemfihlo. Endaweni yokwabelana ngephasiwedi, umntu ngamnye unazo izitshixo ezimbini: isitshixo soluntu nesitshixo sobucala.

* Isitshixo **soluntu** sinokwabelwana ngaso nabani na.
* Isitshixo **sobucala** kufuneka sihlale sifihlakele.

Ukuba uSipho ufuna ukuthumela into ku-Ayanda, angasebenzisa isitshixo soluntu sika-Ayanda. Kuphela u-Ayanda onokuyivula esebenzisa isitshixo sakhe sobucala. Nokuba umntu othile ubamba umyalezo, akakwazi kuwufunda okanye awusebenzise ngaphandle kwesitshixo sobucala.

KwiBitcoin, le nkqubo isetyenziswa ukwenza utyikityo lwedijithali. Utyikityo lwedijithali lubonisa ukuba umnini wesitshixo sobucala uvumile urhwebo, njengokutyikitya igama lakho kwixwebhu. Le nto yenza ukuba urhwebo lweBitcoin lukhuseleke kwaye lube nokuqinisekiswa ngaphandle kokuthembela kumntu wesithathu.

Urhwebo lweBitcoin lubandakanya ukudluliselwa kobunini bebitcoin ukusuka kwidilesi enye ukuya kwenye.

Ukubethela kusetyenziswa ukuqinisekisa ukuba kuphela umnini wokwenyani webitcoin onelungelo lokuthumela imali yakhe komnye umntu. Oku kuqinisekisa ukuba impahla yabo ikhuselekile kubantu abaneenjongo ezimbi.

Njengenye indlela yokhuseleko, urhwebo ngalunye lweBitcoin lufumana ngokuzenzekelayo utyikityo lwedijithali OLUKHETHEKILEYO. Olu tyikityo lwedijithali lukhethekileyo luxhaswa yitekhnoloji engatshintshiyo enceda inethiwekhi iqinisekise ukuba umnini wokwenyani webitcoin, hayi omnye umntu, nguye othumele yona.


> **Dark**
>
> Umsebenzisi ngamnye unazo izitshixo ezimbini: **isitshixo sobucala**, esimele **sifihlwe**, kunye ne **sitshixo soluntu** esinokuthi **sabelwane nabanye**. Isitshixo **sobucala** sisebenza njengobungqina bokuba le dilesi yeyam kwaye ndinolawulo kuyo.


###### Indlela esebenza ngayo urhwebo lweBitcoin

1. **Ukwenza urhwebo**: Umsebenzisi uqala urhwebo lweBitcoin ngokucacisa iinkcukacha ezifana nedilesi yomamkeli kunye nesixa sebitcoin esiza kuthunyelwa.
1. **Ukwenziwa koTyikityo lweDijithali**: Umthumeli wenza utyikityo lwedijithali olukhethekileyo **utyikityo lwedijithali** esebenzisa **isitshixo sakhe sobucala**. Olu tyikityo luyikhowudi ekhethekileyo eqinisekisa ubuqiniso borhwebo.
1. **Ukusasazwa koRhwebo**: Urhwebo olutyikitywe luthunyelwa kwinethiwekhi yeBitcoin, lubonisa injongo yokudlulisa ubunini bebitcoin ukusuka kumthumeli ukuya kumamkeli.
1. **Ukuqinisekiswa kwiNethiwekhi**: Iinodi kwinethiwekhi yeBitcoin zamkela urhwebo kwaye zisebenzisa isitshixo **soluntu somamkeli**ukuqinisekisa ubuqiniso lotsayino. lwentengiselwano. Ngaxeshanye, basebenzisa i-**isitshixo sikawonke-wonke**ukuqinisekisa **utsayino yedijithali**.
1. **Uqinisekiso kwinethiwekhi yeBitcoin**: Ukuba uqinisekiso luphumelele, intengiselwano iya kongezwa kwincwadi-mali, esebenza njengerekhodi ekhuselekileyo, ecacileyo yazo zonke iintengiselwano. Xa sele iqinisekisiwe, ubunini bebitcoin budluliselwa ngokusemthethweni kumamkeli.


> **Callout – Isishwankathelo**
>
> I-**utsayino yedijithali**, eyenziwe ngesitshixo sangasese somthumeli **isitshixo sangasese**, ibonisa ukuba intengiselwano igunyaziswe ngumnini webitcoin. Inethiwekhi yeBitcoin inokuqinisekisa obu bungqina kwaye irekhode intengiselwano.


#### Inkcazelo yeHashing

Nceda ungoyiki amagama ezobuchwephesha kunye neengcamango zezibalo ezizayo. Siyaqonda ukuba ayingabo bonke abantu abathanda izibalo, kodwa unokuzothusa ngokwakho kwaye ubone ukuba neengcinga ezinzima kakhulu zinokuqondwa xa uzama kancinci.


> **Definition – Inkcazelo yomsebenzi**
>
> Umsebenzi **umsebenzi** ufana nomatshini othatha ulwazi athi aluguqulele kwinto entsha. Ulwazi olufakwa kumsebenzi luthiwa **igalelo**. Ulwazi olutsha olwenziwa ngumsebenzi luthiwa **imveliso**. Imisebenzi inceda iikhompyutha ukwenza imisebenzi kunye nokusombulula iingxaki.


##### Yintoni umsebenzi?

Umsebenzi siseti yemiyalelo ethatha igalelo ize ivelise imveliso. Ungacinga ngawo njengeresiphi: ulandela amanyathelo usebenzisa izithako ezithile, kwaye usoloko ufumana isiphumo esilindelekileyo.

KwiBitcoin, imisebenzi isetyenziswa ukuqhuba nokujonga iintengiselwano. Xa umntu ethumela iBitcoin, imisebenzi ye-cryptography inceda ukujonga ukuba intengiselwano ivumelekile, iqinisekisa ukuba umthumeli unemali eyaneleyo, kwaye ihlaziya ibhalansi kwincwadi-mali yeBitcoin. Xa sele iqinisekisiwe kwaye yongezwa kwibhloko, intengiselwano iba yinxalenye yerekhodi esisigxina kwi-blockchain.

##### Yintoni umsebenzi oneendlela enye?

Umsebenzi oneendlela enye ngumsebenzi okhethekileyo olula ukuwenza kwicala elinye kodwa kunzima kakhulu ukuwubuyisela umva. Umzekelo, ukuxuba izithako ukwenza ismoothie kulula, kodwa awukwazi ukuhlukanisa ismoothie ubuyele kwizithako zokuqala.

Ukhuseleko lweBitcoin luxhomekeke kwimisebenzi eneendlela enye. Zisetyenziswa kwi-cryptography yesitshixo sikawonke-wonke nesitshixo sangasese, okuvumela abantu ukuba babelane ngesitshixo sikawonke-wonke ngelixa begcina isitshixo sangasese sifihlakele. Nangona isitshixo sikawonke-wonke sibonakala, akunakwenzeka ukufumana isitshixo sangasese kuso. Le nto yenza iintengiselwano zeBitcoin zikhuseleke.

##### Yintoni umsebenzi wehash?

Umsebenzi we-**hash** ufana nomatshini wokwenza ikhowudi efihlakeleyo. Uthatha umyalezo uwuguqulele kwikhowudi.

###### Indlela iHashing esebenza ngayo kwiNtengiselwano zeBitcoin

KwiBitcoin, yonke intengiselwano iguqulelwa kwi-hash phambi kokuba yongezwe kwi-blockchain. I-hash yifingaphrinti yedijithali eyahlukileyo yentengiselwano. Ukuba nabani na uzama ukutshintsha naliphi na icandelo lencinci lentengiselwano, i-hash iya kutshintsha ngokupheleleyo. Oku kwenza kube lula kwinethiwekhi ukufumanisa ukuba kukho utshintsho olungagunyaziswanga.

###### Indima yeHashing kuKhuseleko lweBitcoin

IHashing inceda ukukhusela inethiwekhi yeBitcoin ngokwenza iintengiselwano zibe lula ukujonga kwaye kube nzima kakhulu ukuzitshintsha ngasese. Kuba intengiselwano nganye inehash yayo eyahlukileyo, inethiwekhi inokufumanisa ngokukhawuleza ukuba kukho into etshintshiweyo.

Umsebenzi wehash uthatha idatha uyiguqulele kumtya omfutshane olinganayo weenombolo kunye noonobumba obizwa ngokuba yi-hash. Igalelo elifanayo lihlala livelisa i-hash efanayo, kodwa utshintsho oluncinane kwigalelo lwenza isiphumo esahlukileyo ngokupheleleyo. Le mpawu ivumela iikhompyutha ukuba zijonge ukuba idatha ayitshintshwanga.


> **Definition – Inkcazelo yeHashing**
>
> **IHashing** ifana nokwenza ifingaphrinti yedatha yedijithali. Yinkqubo yokuthatha umyalezo wedijithali uwuguqulele kwikhowudi yobude obusisigxina, esebenza njengomazisi okhethekileyo. Njengokuba ifingaphrinti inokuchaza umntu, i-hash inokuchaza umyalezo wedijithali.


Imveliso **imveliso**, okanye i-hash, ihlala inobude obufanayo, nokuba ulwazi lwantlandlolo lude kangakanani. IBitcoin isebenzisa iintlobo ezithile zomsebenzi wehash ezibizwa ngokuba yi-**SHA-256** kunye ne-**RIPEMD160**.

Imizekelo embalwa ingezantsi:

* I-SHA256 hash yomtya othi **molo hlabathi**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256 hash yombhalo othi **molo hlabathi.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Qaphela ukuba utshintsho oluncinane kwigalelo liyatshintsha ngokupheleleyo isiphumo xa kuthelekiswa nesokuqala
* SHA256 hash yefayile ye-iso ekhutshelwayo **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Le galelo yifayile enkulu kakhulu kodwa isiphumo sisahleli sikhulu esifanayo

Unokucinga ngokuhashisha njengomculo obhalwe phantsi, ogcina umongo womculo. Njengoko umculo obhalwe phantsi umele ngokukodwa ingoma, ixabiso le-hash limele ngokukodwa idatha.

Xa kuthelekiswa umculo obhalwe phantsi nomculo odlalwayo, umculi angabona ukuba umculo udlalwe ngokuchanekileyo na. Ngokufanayo, xa kuthelekiswa ixabiso le-hash ledatha efunyenweyo nelokuqala, umntu angabona ukuba idatha itshintshile na ngexesha lokuthunyelwa.

Njengoko utshintsho oluncinane kumculo odlalwayo lungabangela ukuba umculo uvele uhluke, kwakhona utshintsho oluncinane kwidatha yokuqala luvelisa ixabiso le-hash elahlukileyo. Oku kwenza ukuhashisha kube sisixhobo esinamandla sokuqinisekisa ukuthembeka kunye nobunyani botshintshiselwano lweBitcoin.

Inkqubo yokuguqulela i-**public key** ngokusebenzisa ukuhashisha isetyenziswa ukuphucula ukhuseleko lolwazi ngokuluguqula lube yifomathi ende engafundekiyo. IBitcoin isebenzisa i-SHA-256 kunye ne-RIPEMD160 ukwenza iidilesi zoluntu. Isiphumo esivelayo siba sisazisi esikhethekileyo se-**public key** kwaye sinceda ukuqinisekisa ukuthembeka nokhuseleko lwentengiselwano ezigcinwe kwincwadi yeerekhodi. Ngokufihla ulwazi ngale ndlela, kuba nzima ngakumbi kubantu abangagunyaziswanga ukufikelela nokuguqula idatha.

##### Iimpawu zomsebenzi wokuhashisha

* **Iyazinzisa**: Izithako ezifanayo zihlala zivelisa ismoothie efanayo. Ngokufanayo, idatha efanayo iya kuvelisa i-hash efanayo.
* **Ukuxhathisa kwangaphambili**: Ukuba unayo kuphela i-smoothie, awunakukwazi ukufumanisa iziqhamo ezasetyenziswa. Ngokufanayo, ukuba unayo kuphela i-hash, awunakukwazi ukufumanisa idatha yokuqala.
* **Umphumo we-avalanche**: Ukutshintsha nencinci kweyona ndawo yezithako kudala i-smoothie eyahlukileyo ngokupheleleyo. Kwi-hash, utshintsho oluncinane kwidatha lwenza i-hash eyahlukileyo ngokupheleleyo.
* **Ukuxhathisa ukungquzulana**: Kunzima kakhulu ukufumana izithako ezimbini ezahlukeneyo ezivelisa i-smoothie efanayo. Ngokufanayo, akunakwenzeka phantse ukuba iidatha ezimbini ezahlukeneyo zivelise i-hash efanayo.
* **Kukhawuleza ukujonga**: Ukwenza i-smoothie kuyakhawuleza, kwaye kulula ukuqinisekisa ukuba sismoothie. Imisebenzi ye-hash iyakhawuleza ukuyenza kwaye kulula ukuba nabani na ayijonge.

#### Umsebenzi: Yenza i-SHA 256 Hash


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Uyazibuza ukuba ukuhashisha kusebenza njani? Skena i-QR code ukuze wenze i-SHA256 hash kwangoko ukusuka nasiphi na isihloko, isivakalisi, okanye igalelo olukhethayo. Imisebenzi ye-hash ifana neminwe yedijithali: zisebenza ngendlela enye kuphela, oko kuthetha ukuba xa into sele ihashishiweyo, ayinakubuyiselwa umva. Zama ngoku uzibonele!
