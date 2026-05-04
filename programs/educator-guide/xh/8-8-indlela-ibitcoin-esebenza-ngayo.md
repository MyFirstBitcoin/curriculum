# 8 - Indlela iBitcoin esebenza ngayo

Ixesha: Imizuzu engama-90

Ingcamango Ephambili: Ukhuseleko lweBitcoin luxhomekeke kwiingcamango zobugcisa ezilula kodwa ezinamandla ezifana nezitshixo, utyikityo, i-hashing, kunye ne-UTXO, ezivumela ubunini kunye nokuqinisekiswa ngaphandle komphathi ophakathi.

#### Iinjongo Zokufunda

Ekupheleni kwesi sifundo, abafundi kufuneka bakwazi:

* Chaza indlela izitshixo zikawonke-wonke nezabucala ezikhusela ngayo ubunini beBitcoin kunye nokuthengiselana.
* Chaza ukuba yintoni utyikityo lwedijithali kwaye lubonisa njani ukuba ukuthengiselana kugunyaziswe ngumnini ofanelekileyo.
* Chaza, ngendlela elula, ukuba kuthetha ntoni i-cryptography, i-encryption, kunye ne-decryption kumxholo weBitcoin.
* Chaza ukuba yintoni i-hashing kwaye uchaze ukuba kutheni imisebenzi ye-hash ibalulekile kukhuseleko lweBitcoin kunye nokuthembeka kwedatha.
* Chonga iimpawu ezisisiseko zomsebenzi we-hash, ezifana nemveliso yobude obusisigxina, indlela yokusebenza engabuyiyo, kunye nokutshintsha okukhulu xa kungena utshintsho oluncinane.
* Chaza imodeli ye-UTXO kunye nendlela i-bitcoin echithwa, yamkelwa, kwaye ibuyiselwa njengenguqu kwiimveliso zokuthengiselana.
* Chaza indlela iinodi ezinqanda ngayo ukuphinda kusetyenziswe imali ngokujonga ukuba imveliso sele isetyenzisiwe na.

#### Izixhobo & Nezixhobo Zokufundisa

##### Izixhobo Zibonakalayo

* Isahluko 8 - Indlela IBitcoin Esebenza Ngayo

##### IThala leencwadi loNcedo

* Ikhadi leNgcaciso yeGama — Isahluko 8 — Amagama: cryptography, hash, UTXO, digital signature, private/public key, merkle tree, blockchain
* IThala leencwadi leNgcamango Engalunganga — Isahluko 8 — Idilesi: "igama lemfihlo elilahlekileyo linokubuyiselwa," "isitshixo sabucala = iphasiwedi," "i-blockchain ayaziwa"
* Iingcaciso Zobugcisa & Ukujonga Ngokunzulu — Imisebenzi ye-hash, izitshixo zikawonke-wonke/ezabucala, imodeli ye-UTXO, ukhuseleko lwe-Proof of Work

#### Imisebenzi

* Ukuthengiselana Kwenzeka
* Ukuhlola iMempool

#### Ukufundisa Kwi-Intanethi

* Sebenzisa ibhodi emhlophe yedijithali kwaye uzobe ingcamango nganye ngexesha endaweni yokuxhomekeka kwinkcazo yomlomo kuphela.
* Fundisa ingcamango yobugcisa enye ngexesha kwaye ume rhoqo ukuze ubuze imibuzo yokuqinisekisa.
* Sebenzisa imizobo yezitshixo, utyikityo, i-hash, kunye ne-UTXO ukuze abafundi bakwazi ukulandela ulwakhiwo.
* Gcina injongo ikwizingqinisiso kwaye uphephe ukungena nzulu kwizibalo okanye amagama anzima.

#### Ukulungiselela

* Lungiselela kwaye ulaminate iidayagram: izibini zezitshixo zikawonke-wonke/ezabucala, utyikityo lwedijithali, imodeli ye-UTXO, i-hashing (umsebenzi ongabuyiyo).
* Phawula i-blockchain explorer kunye ne-SHA-256 hash calculator; khetha ukuthengiselana kweBitcoin eziyi-2-3 zokuhamba nazo inyathelo ngenyathelo.
* Lungiselela amanqaku ebhodi emhlophe okuchaza izinto ezingenayo, eziphumayo, kunye nendlela ukuthengiselana okuqinisekiswa ngayo kwi-blockchain.

#### Inkqubo

Esi sifundo sinika abafundi umbono wokuqala kwicala lobugcisa leBitcoin ngaphandle kokufuna ulwazi lobugcisa lwangaphambili. Isikhokelo ngoku silandela ulwakhiwo olufutshane olufana neDiploma, apho i-cryptography idityanisiwe phantsi kwesihloko esinye kwaye i-UTXO phantsi kwesinye.

##### 8.0 Intshayelelo, imizuzu eyi-8

Qala ngokumisela okulindelweyo:

* Yintoni eyenza iBitcoin ikhuseleke xa kungekho bhanki ephakathi eyilawulayo?
* Ithungelwano lingazi njani ukuba umntu uyinyani na onobunini bebitcoin azama ukuyithumela?
* Kwenzeka ntoni ngokwenene emva kwekhowudi xa umntu enza ukuthengiselana ngeBitcoin?

Cacisa ukuba esi sahluko sigxile kwiziseko zobugcisa ezisisiseko zeBitcoin, ngakumbi izitshixo, utyikityo, i-hashing, kunye ne-UTXO. Kwakhona qinisekisa abafundi ukuba akufuneki babe ngonjiniyela ukuze baqonde ingqiqo ephambili. Isahluko ngokwaso senza le ngongoma icace ngokuthelekisa iBitcoin kwi-intanethi, abantu abaninzi bayisebenzisa yonke imihla bengaqondi onke amanqanaba angaphantsi kwayo.

##### 8.1 Ukhuseleko NgeCryptography, imizuzu eyi-57

**I-Bitcoin NjengeNcwadi Egcinwe Kwiikhompyutha Ezininzi**

Qala ngombono olula wesahluko wenethiwekhi yeBitcoin:

* I-Bitcoin yingxelo yokuthengiselana
* leyo ngxelo igcinwa kwiikhompyutha ezininzi ezibizwa ngokuba zi-nodes
* incwadi yobalo yoluntu kwaye ayinazigama
* ibonisa iidilesi kunye nembali yokuthengiselana, hayi iinkcukacha zobuqu zomntu

Le ndawo inceda abafundi badibanise koko sele bekuyazi kumacandelo angaphambili. IBitcoin ayisekelwe kwiakhawunti ezifihlakeleyo ngaphakathi kwebhanki. Isekwe kwincwadi yobalo esetyenziswa ngabantu abaninzi abanokuyiqinisekisa. iluncedo kakhulu apha kuba ibonisa abasebenzisi, iiwallets, kunye nenethiwekhi yeBitcoin edibanisa kwincwadi yobalo yoluntu.

**Izitshixo Zikawonke-wonke Nezabucala**

Ngoku ngenisa i-cryptography.

Chaza ukuba umsebenzisi ngamnye weBitcoin une:

* isitshixo sabucala, esimele sihlale sifihlakele
* isitshixo sikawonke-wonke, esinokuthi sabelwe abanye

Cacisa injongo yazo ngamagama alula:

* isitshixo sabucala sibonisa ulawulo kwaye sivumela ukuchitha imali
* isitshixo sikawonke-wonke sinceda abanye baqinisekise ukuba intengiselwano igunyaziswe ngokuchanekileyo

Eyona nto ibalulekileyo ekufundeni kweli candelo kukuba iBitcoin isebenzisa i-cryptography yesitshixo sikawonke-wonke/abucala, hayi imodeli endala apho abantu ababini kufuneka babelane ngesitshixo esiyimfihlo kuqala. Oku kubalulekile kuba kuvumela ukuqinisekiswa okukhuselekileyo ngaphandle kokunyanzela abasebenzisi ukuba babonakalise imfihlo egcina imali yabo ikhuselekile.

Ungayichaza ngolu hlobo:

* isitshixo sabucala sifana nobungqina obufihliweyo bokuba i-bitcoin yeyakho
* isitshixo sikawonke-wonke siyinxalenye yento evumela inethiwekhi ukuba iqinisekise igunya lakho
* nabani na olawula isitshixo sabucala ulawula amandla okuchitha i-bitcoin

Qaphela ungayenzi nzima kakhulu inkcazo ye-encryption. Eyona nto ibalulekileyo kubafundi kukubaqonda ubunini kunye negunya.

**Utyikityo Lwedijithali kunye Nokugunyaziswa Kwentengiselwano**

Ngoku chaza ukuba kwenzeka ntoni xa umntu ethumela i-bitcoin.

Sebenzisa ulungelelwaniso lwesahluko:

* umsebenzisi wenza intengiselwano
* umthumeli wenza utyikityo lwedijithali esebenzisa isitshixo sabucala sakhe
* intengiselwano isasazwa kwinethiwekhi
* i-node ziqinisekisa ukuba utyikityo luchanekile
* xa sele iqinisekisiwe kwaye iqinisekisiwe, ubunini budluliselwa kwirekhodi

Cacisa ukuba utyikityo lwedijithali alufani nokubhala igama lakho. Liyingqinisiso ye-cryptography yokuba umnini wokwenene ugunyazise intengiselwano. Le yenye yezona ndlela ziphambili ezivumela iBitcoin ukuba isebenze ngaphandle komphathi ophakathi ovuma intengiselwano ngesandla. Umzobo uluncedo kuba ubonisa utyikityo kunye nokuqinisekiswa ngokubonakalayo, kunye nendlela yentengiselwano ukusuka kumthumeli ukuya ekuqinisekisweni kwenethiwekhi.

Isivakalisi esihle sekilasi singaba:

Iintengiselwano zeBitcoin azivunywa kuba ibhanki itshilo. Zamkelwa kuba inethiwekhi inokuthi iqinisekise ubungqina be-cryptography obuchanekileyo.

**Ukugaya kunye neMisebenzi eyaKwicala elinye**

Okulandelayo, chaza ukugaya (hashing).

Qala lula:

* umsebenzi uthatha igalelo aze uvelise imveliso
* umsebenzi oya kwicala elinye kulula ukuwusebenzisa kwicala elinye, kodwa akunakwenzeka ngokwenene ukuwubuyisela umva
* umsebenzi wokugaya uthatha idatha yobungakanani obubhaliweyo aze ayiguqulele kwimveliso yobude obusisigxina ebizwa ngokuba yi-hash

Sebenzisa enye yeengqiyame zesahluko, leyo uziva icacile kubaphulaphuli bakho:

* umzekelo we-smoothie kumsebenzi oya kwicala elinye
* umzekelo womnwe wedijithali kwiihash
* umzekelo womculo wokujonga ukuba into itshintshile na

Umzekelo womnwe wedijithali mhlawumbi ucace gca kwiiklasi ezininzi:

* i-hash ifana nomnwe wedijithali wedijithali wedatha
* ukuba igalelo litshintsha kancinci, i-hash itshintsha ngokupheleleyo
* oku kunceda iikhompyutha ziqinisekise ukuthembeka kwaye zifumanise ukungenelela okungekho semthethweni

Emva koko chaza ukuba kutheni ukugaya kubalulekile kwiBitcoin:

* iintengiselwano zigayiwe (hashed)
* inethiwekhi isebenzisa iihash ukunceda ukuqinisekisa ukuthembeka
* ukuba intengiselwano itshintshiwe, i-hash iyatshintsha
* oku kunceda ukukhusela irekhodi ekuphazamisekeni okungabonakaliyo

Imizobo kumaphepha 7 ukuya ku-10 iluncedo kakhulu apha. Isahluko sibonisa zombini umbono wemveliso yobude obusisigxina kunye nomgaqo wokuba "utshintsho oluncinci, isiphumo esahlukileyo ngokupheleleyo", ongomnye wemigaqo ebalulekileyo abafundi ekufuneka bayiqonde.

**Iimpawu Eziqhelekileyo zeMisebenzi yeHash**

Hamba ngokufutshane ngeempawu ezigxininiswe kwisahluko, ungazenzi nzima kakhulu:

* Iyazinzisa: igalelo elifanayo linika imveliso efanayo rhoqo
* Iya kwicala elinye / ukumelana nomfanekiso wangaphambili: awukwazi ngokwenene ukubuyisela inkqubo umva
* Ivakalelwa kukutshintsha: utshintsho oluncinci kwigalelo lwenza imveliso eyahlukileyo ngokupheleleyo
* Ukumelana nokungquzulana: kunzima kakhulu ukufumana iigalelo ezimbini ezahlukeneyo ezinemveliso efanayo
* Iyakhawuleza ukuqinisekisa: umsebenzi usebenza kakuhle kwaye kulula ukuwujonga

Awudingi ukuba abafundi bafunde amagama onke, kodwa kufuneka baqonde umxholo jikelele: ukugaya kunika iBitcoin indlela ethembekileyo yokuchonga idatha kunye nokufumanisa utshintsho.

##### 8.2 Imodeli ye-UTXO, imizuzu engama-25

**Imodeli ye-UTXO**

Ngoku singena kwicandelo lesibini elikhulu lesahluko: ii-UTXO, okanye ii-Unspent Transaction Outputs.

Chaza ngamagama alula usebenzisa umzekelo wemali esahlukweni:

* i-bitcoin ayilandelwa njengobalo lweakhawunti yebhanki kuphela
* endaweni yoko, yenziwe ngamaqhekeza anokuchithwa abizwa ngokuba yi-UTXO
* xa uchitha i-bitcoin, usebenzisa enye okanye ezingaphezulu ii-UTXO ezikhoyo njengemvelaphi
* ii-UTXO ezintsha zenziwa njengeziphumo

Sebenzisa umzekelo osesahlukweni:

* ukuba une-UTXO ye-10 BTC
* kwaye uthumela i-6 BTC
* i-UTXO entsha ye-6 BTC iya kumamkeli
* i-UTXO entsha yenguqu iya kubuya kuwe
* inxalenye encinci ihlawulwa njengemali yomvuzo wembiwa-migodi

Oku kunceda abafundi babone ukuba iBitcoin isebenza ngathi uchitha imali kwaye ufumana inguqu, hayi ngokususa amanani kwilayini yeakhawunti elula. Imizobo ibalasele kakhulu apha kuba ibonisa ngokucacileyo i-UTXO enye yahlulwe yaba yimveliso yomamkeli, imveliso yenguqu, kunye nemali yomvuzo.

Yenza la manqaku mabini abalulekileyo acace:

* ibhalansi ye-wallet yakho yisixa see-UTXO zakho
* xa uchitha, ii-UTXO ezindala ziyasetyenziswa kwaye ezintsha zenziwa

**Ukuthintela Ukuphindaphinda Kweendleko (Double-Spending)**

Vala umxholo ngokuchaza enye yezona zinto zibalulekileyo kwimodeli ye-UTXO.

Ukuba umntu uzama ukuchitha imveliso enye kabini, iinodi ziyala umzamo wesibini kuba zigcina i-ledger kwaye zingaqinisekisa ukuba loo UTXO sele isetyenzisiwe. Le ndlela iBitcoin ithintela ngayo ukuphindaphinda kweendleko ngaphandle kokufuna inkampani ephakathi yokulawula iirekhodi. Umzekelo uluncedo kakhulu apha kuba ubonisa u-Alice edibanisa ii-UTXO, ethumela imali kuSipho, efumana inguqu, kwaye itransekshini eqinisekisiweyo ihlaziya i-ledger kuzo zonke iinodi.

Indlela ecacileyo yokuyithetha eklasini yile:

I-Bitcoin ithintela ukuphindaphinda kweendleko kuba inethiwekhi igcina umkhondo wokuba zeziphi iimveliso ezingekachithwa kwaye zeziphi sele zisetyenzisiwe.

###### Isishwankathelo kunye nokuJonga uQwalaselo

Vala ngemibuzo embalwa ekhawulezayo:

* Yintoni umahluko phakathi kwesitshixo sikawonke-wonke nesitshixo sabucala?
* Yintoni eboniswa sisiginitsha yedijithali?
* Kutheni i-hashing iluncedo kwiBitcoin?
* Kwenzeka ntoni ukuba itransekshini itshintshwa emva kokuba i-hash yenziwe?
* Yintoni i-UTXO ngamagama alula?
* Inethiwekhi iyimisa njani umntu ekuchitheni i-bitcoin enye kabini?

#### Amanqaku oTitshala

Esi sahluko sinegama lobugcisa elingakumbi kunamahluko angaphambili, ngoko ke phambili ekucaciseni, umzekelo, kunye nokuphindaphinda.

Injongo ayikokwenza abafundi babe ngabaqambi beenkqubo. Injongo kukubanceda baqonde ukuba kutheni ukhuseleko lweBitcoin lusebenza.

Amanqaku abalaseleyo okufanele aphambili, ukuba ixesha lifutshane, ngala:

* isitshixo sabucala vs isitshixo sikawonke-wonke
* izisiginitsha zedijithali
* yintoni i-hashing eyenzayo
* ii-UTXO njengezicucu ze-bitcoin ezinokuchithwa
* indlela yokuthintela ukuphindaphinda kweendleko

Ezona mizobo ziluncedo kweli sahluko zezi:

* umzobo womsebenzisi-i-wallet-inethiwekhi
* umzobo wesiginitsha yedijithali
* imizekelo ye-hashing kunye nemizobo yemveliso yobude obusisigxina kumaphepha 7 ukuya ku-10
* imizobo ye-UTXO kumaphepha 10 ukuya ku-12

##### Oko Kukubonakala Kuhle

* Kubalulekile ukuphatha i-cryptography njengesiseko hayi imfihlakalo, usebenzise imizobo eninzi, uphephe imathematika enzulu, uqhagamshele kwicandelo langaphambili, kwaye uvavanye ukuqonda ngokusetyenziswa njengokuthi "Ukuba umntu utshintsha itransekshini enye, yintoni ephukayo?"
* Ootitshala kufuneka babe nomonde kubafundi abaxakekileyo, bacinge ngendlela yemizobo kwaye bazobe yonke into, bathethe inyaniso malunga nezinto abafundi abangadingi kuziqonda, bavume ukusho "Andazi kodwa nantsi indlela esinokuyifumana ngayo," kwaye bahlale bekhuthaza ngalo lonke ixesha.
* Abafundi bayaqonda ukuba kutheni iBitcoin ingenakugatywa kuba ikhuselekile ngemithetho yezibalo, bayahlonipha uyilo oluhle lwenkqubo, bazive bekhululekile kwinkimbinkimbi besazi ukuba abadingi yonke into, bafumane ukuzithemba ekubuzweni imibuzo ngaphandle kokugwetywa, kwaye baqaphele ukuba baphucule ukuqonda kwabo into abantu abaninzi abangayiqondiyo.
* Iziphumo zoFundo kufuneka zifezekiswe ukuba abafundi banokuchaza izisiseko ze-cryptography ezifana nemisebenzi yendlela enye kunye nezisiginitsha zedijithali ngaphandle kwemathematika enzulu, baqonde imodeli ye-UTXO ebonisa ukuba ungumnini weemali hayi ii-akhawunti, baqaphele i-hashing njengesiseko sokhuseleko lweBitcoin, baqonde isakhiwo setransekshini kubandakanya izisiginitsha kunye nokuqinisekiswa, bachaze ukuba kutheni iBitcoin ingatshintshi, kwaye babuze imibuzo ebalulekileyo malunga nokuhlaselwa okunokwenzeka okanye ubuthathaka.

##### Ulawulo lwexesha

Ukuba ixesha lifutshane, nikezela ingqalelo kwi:

* Isitshixo sabucala vs isitshixo sikawonkewonke
* Iisayini zedijithali
* Okwenziwa kukuhashisha
* UTXO njengezicucu ze-bitcoin ezinokusetyenziswa
* Indlela ekuthintelwa ngayo ukuphinda kusetyenziswe imali enye kabini

Ukuba uhamba phambili, thatha ixesha kwi:

* Umzobo womsebenzisi-i-wallet-inethiwekhi kunye nomfanekiso wokhuseleko
* Umfanekiso wesayini yedijithali: inkqubo ye-cryptography eneenkcukacha
* Imithi yeMerkle kunye nokhuseleko lwenkqubo
* Iindlela eziphambili zokuhlasela kunye nesizathu sokuba zingaphumeleli

##### Ukuba abafundi banengxaki

* I-cryptography ibonakala isoyikisa → "Uyisebenzisa yonke imihla; i-Bitcoin iyisebenzisa ngendlela efanayo."
* Ukuhashisha njengengcamango → Umzekelo weminwe; yahlukile, ayinakutshintshwa ngaphandle kokutshintsha i-hash.
* Iisayini zedijithali → "Ibonisa imvume ngaphandle kokutyhila iphasiwedi."
