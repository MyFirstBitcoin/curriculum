# 3.4 Hashcash

UHashcash wadalwa nguAdam Back, omnye wabantu bokuqala abenza izinto ezintsha kweli candelo. UAdam wayenomdla omkhulu kwiimarike ezikhululekileyo kunye nobumfihlo kwi-intanethi, kwaye wadibana noluhlu lwe-imeyile lweCypherpunks apho wajoyina waba ngumthathi-nxaxheba osebenzayo.

Wayenomdla kakhulu kwimali yedijithali, kwaye wenza iingcebiso ezithile zokuba iqela linokusebenza ngokusondeleyo kwiDigiCash kunye noChaum, kodwa ezi azizange ziphumelele. Emva koko wajolisa ingqalelo yakhe kwenye ingxaki eyayisanda kuvela – i-imeyile engafunekiyo (spam). Yena kunye nabanye beCypherpunks babefuna ukufumana isisombululo kule ngxaki ye-spam, apho kwakulula kakhulu kubathumeli be-spam ukwenza nokuthumela amawaka e-imeyile ezalisayo iinethiwekhi. Isisombululo sakhe esiyingqayizivele sasisebenzisa i-hashing – amandla e-cryptography okuguqula naluphi na ulwazi lube ngumtya owodwa nowahlukileyo wobude obuthile, ukwenza into efana 'nesitampu' sedijithali ekufuneka yongezwe kwi-imeyile ukuze ithathwe njengeyiyo kwaye ithunyelwe kwinethiwekhi. Iindleko ezincinci kwi-imeyile yokwenene, kodwa ezinzima kumthumeli we-spam.

Uphuhliso oluphambili olwenziwa yiHashcash yayikukudibanisa izixhobo zangempela – amandla okusebenza kwekhompyutha – kwinethiwekhi yedijithali. Ngelixa izixhobo zedijithali kude kube ngelo xesha zazisenokuphindaphindwa ngaphandle komda, inani le 'hashcash' elenziwayo lalilinganiselwe ngokuba abantu bazimisele ukusebenzisa amandla amangakanani kuyo.

Nangona isisombululo sasihlangabezana nezinye zeemfuno uAdam wayekholelwa ukuba ziyimfuneko kwinkqubo yemali yedijithali; yayiyimfihlo, yomelele kwaye ingaxhomekekanga kuthembeko, kodwa i-hashcash nganye yayingasetyenziswa kwakhona kwaye yayinganyaniyo ngokwenene. Wacebisa ezinye iindlela zokuba ezi ngxaki zingasombululwa kusetyenziswa amaqela angaphandle.

##### BitGold

UNick Szabo wakha phezu kwengcamango yeHashcash kunye nobungqina bomsebenzi (proof of work) ukuze acebise esinye isisombululo, awayesichaza kuluhlu lwe-imeyile kunyaka emva kokupapashwa kweHashcash, ngo-1998.

Nangona esondela kwisombululo, esi siphakamiso sasisenemingeni emininzi.

* Ngubani oza kulawula iRegistry yobunini be-hash kwaye bangathembeka njani?.
* Ukusebenzisa i-hashing kuya kuthi kungabizi mali kakhulu ngokuhamba kwexesha, leyo yayingumceli-mngeni nakwiHashCash.

Njengoko ii-hash ezinxulumeneyo ziya kufakwa i-time-stamp, wacebisa uhlobo oluthile lokulandelela imbali yobunzima bokwenza i-hashing ngelo xesha; i-hash yangaphambili yayiza kufuna iindleko zokusebenza eziphezulu kunele yakamva njengoko iindleko ziye zehla. Ngelishwa, oku kwakuthetha ukuba ii-hash bezingayi kuba 'fungible' oko kukuthi, zexabiso elifanayo, nto leyo ithathwa njengento ephambili kwimali yedijithali. Ukuze ancede ukusombulula oku, uNick wacebisa uhlobo oluthile 'lwebhanki ezikhululekileyo' ezisebenza phezu kweBitGold ezaziza kuhlanganisa amaqela ahlukeneyo ee-hash ezaziza kuxatyiswa ngokufanayo.

##### B-Money

Kungekudala emva kwesiphakamiso seBit Gold, uWei Dai wacebisa isisombululo esifana neso. Wayesele ephuhlise ezinye izixhobo ezininzi zeCypherpunks, kwaye wayenezimvo zakhe ngemali yedijithali.

Isiphakamiso sakhe sasifana neBit Gold kuba sasisebenzisa utyikityo lwedijithali ukugqithisela imali, kwaye iirekhodi zotshintshiselwano zaziza kugcinwa kwiledger, equlathe izitshixo zoluntu kunye nenani leyunithi zemali ezinxulunyaniswa nomntu ngamnye. NjengeBit-Gold, amaqela athembekileyo athathwa njengezithuba zokhuseleko, kwaye inkolelo yayikukuba inkqubo yemali yombane akufuneki ixhomekeke kwiqela elinye ukulandelela ibhalansi, iintengiselwano okanye ukuthintela ukusetyenziswa kabini kwemali.

UWei-Dai wacebisa izisombululo ezininzi kwezi ngxaki, enye yazo yayikukuba endaweni yokuba kube nombutho ophakathi ogcina i-ledger, ZONKE i-node zaziza kugcina ikopi yayo. Ukuba bonke abasebenzisi bajonga i-ledger yabo kunye nokusebenziseka kwentengiselwano nganye, logama zonke ii-node zihlaziywa ngexesha, ii-ledger ziza kuhlala zidityanisiwe kwinethiwekhi. Le nkqubo isasazeke kakhulu yayingayi kuba lula ukonakaliswa.

UWei Dai waqonda ukuba oku akusombululi ingxaki ye-Byzantine generals (1), njengoko ii-node zinokuphulukana lula nokudityaniswa okanye zixoke nje. Wacebisa ezinye iindlela ezifana nokuba kube neseti yeeseva 'ezithembekileyo' ezigcina i-ledger, kunye nokudala imivuzo yezemali ukugcina ezi seva zithembekile.

Kwipolisi yemali, wacebisa ukuxhasa amandla okuthenga kweB-Money kwindlela ethile ye-consumer price index yangaphandle. Wayefuna ukuba inani elifanayo leB-Money likwazi ukuthenga isabelo esilinganayo kwi-index ngokuhamba kwexesha, ukubonelela uzinzo lwamaxabiso. Ke, nabani na wayenokwenza iiyunithi zemali ezintsha ngokubonelela nge-hash esebenzayo, kodwa ubunzima bokwenza i-hash bunokutshintsha ngokuhamba kwexesha ngokusekelwe kwiindleko ze-CPU kunye ne-price index, ukuze iyunithi nganye ibe 'ngatshintshiyo'.
