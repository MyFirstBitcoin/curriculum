# 3.4 Hashcash

Hashcash an ƙirƙira ta Adam Back, wani daga cikin masu ƙirƙira na farko a wannan fanni. Adam yana da sha'awar kasuwanni masu 'yanci da sirri a intanet, kuma ya ci karo da jerin wasiƙun Cypherpunks inda ya shiga kuma ya zama mai shiga sosai.

Yana da matuƙar sha'awa game da kuɗin dijital, kuma ya ba da wasu shawarwari kan yadda ƙungiyar za ta iya aiki tare da Chaum a kan DigiCash, amma hakan bai kai ko'ina ba. Daga nan sai ya mayar da hankali kan wata matsala da ke fitowa – spam ɗin imel. Shi da sauran Cypherpunks suna son samo mafita ga matsalar spam, inda masu aika spam ke iya ƙirƙira da aika dubban imel cikin sauƙi wanda ke cunkushe hanyoyin sadarwa. Mafitarsa mai ƙirƙira ta ta'allaka ne da hashing – fasahar da ke amfani da lissafi don sauya kowanne bayanai zuwa wata dabara ta musamman da bazuwar igiyar haruffa mai tsawon da aka kayyade, don ƙirƙirar tamkar tambarin dijital da dole a saka a imel kafin a ɗauke shi da muhimmanci kuma a aika shi ta hanyar sadarwa. Ƙananan kuɗi ne ga imel na gaskiya, amma babbar matsala ga mai aika spam.

Babban ƙirƙira da Hashcash ta kawo shi ne haɗa albarkatun duniya na gaske – ƙarfin kwamfuta – da hanyar sadarwar dijital. Duk da cewa albarkatun dijital kafin wannan lokaci ana iya kwafi ba tare da iyaka ba, adadin 'hashcash' da aka ƙirƙira yana iyakance da yadda mutane za su iya sadaukar da makamashi a kai.

Ko da yake mafitar ta cika wasu daga cikin ƙa'idodin da Adam ke ganin ya kamata a samu a tsarin kuɗin dijital; tana da sirri, ƙarfi da rashin buƙatar amincewa, kowanne hashcash ba za a iya sake amfani da shi ba kuma ba shi da ƙarancin gaske. Ya ba da wasu hanyoyi da za a iya magance waɗannan matsalolin ta amfani da wasu ɓangarori na waje.

##### BitGold

Nick Szabo ya gina a kan ra'ayin Hashcash da proof of work don gabatar da wata mafita daban, wanda ya bayyana a cikin jerin wasiƙu shekara guda bayan an wallafa Hashcash, a 1998.

Duk da cewa yana ƙara kusanci da mafita, wannan shirin har yanzu yana da ƙalubale da dama.

* Wa zai gudanar da Rijistar mallakar hash kuma ta yaya za a iya amincewa da su?.
* Hashing gaba ɗaya zai ragu farashinsa da lokaci, matsala ce ga HashCash ma.

Tunda an ɗaure hash ɗin da lokaci, ya ba da shawarar a riƙa bin diddigin wahalar hashing a lokacin; hash na baya zai buƙaci ƙarin ƙoƙari fiye da na gaba tunda farashin ya ragu. Abin takaici, hakan na nufin hash ba za su zama 'fungible' ba wato ba su da daidaiton daraja, wanda ake ɗauka a matsayin muhimmin sifa na kuɗin dijital. Don taimakawa magance wannan, Nick ya ba da shawarar wani irin 'free banking' da zai yi aiki a kan BitGold wanda zai iya haɗa rukuni daban-daban na hash da za a ɗauka daidai daraja.

##### B-Money

Bayan shirin Bit Gold, Wei Dai ya gabatar da mafita makamanciya. Ya riga ya ƙirƙiri wasu kayan aiki da dama ga Cypherpunks, kuma yana da nasa ra'ayoyi game da kuɗin dijital.

Shirinsa ya yi kama da Bit Gold wajen amfani da sa hannun dijital don canja kuɗi, kuma bayanan mu'amala za a adana su a littafin ajiyar bayanai, wanda ke ɗauke da mabuɗan jama'a da adadin kuɗin da aka danganta wa kowane. Kamar Bit-Gold, amintattun ɓangarori na uku ana ɗaukar su a matsayin gurɓatattun hanyoyi, kuma akidar ita ce tsarin kuɗin lantarki bai kamata ya dogara da ɓangare guda ɗaya don bibiyar ma'auni, mu'amala ko hana kashe kuɗi sau biyu ba.

Wei-Dai ya gabatar da wasu mafita ga waɗannan matsalolin, ɗaya daga ciki shi ne maimakon wata cibiyar guda ɗaya ko fiye ke kula da littafin ajiyar bayanai, DUK nodes za su riƙe kwafi. Idan duk masu amfani sun duba nasu littafin da ingancin kowace mu'amala, muddin duk nodes suna sabunta bayanansu, to littattafan za su ci gaba da daidaita a duk hanyar sadarwa. Wannan tsarin da ya yadu sosai zai yi wahala a lalata.

Wei Dai ya gane cewa wannan bai magance matsalar janar-jagororin Byzantine ba (1), domin nodes na iya rasa daidaito ko kuma su yi ƙarya kawai. Ya ba da wasu hanyoyi kamar a samu wani rukuni na 'amintattun' sabobin da za su kula da littafin, da kuma ƙirƙirar ƙarfafawa ta kuɗi don tabbatar da gaskiyar waɗannan sabobin.

Don manufofin kuɗi, ya ba da shawarar a daure ƙarfin sayen B-Money da wani nau'in ma'aunin farashin kayayyakin masarufi. Yana so adadin B-Money ɗaya ya iya sayen daidai kaso na wannan ma'auni a tsawon lokaci, don samar da daidaiton farashi. Saboda haka, kowa zai iya ƙirƙirar sabbin kuɗi ta hanyar samar da hash mai inganci, amma wahalar ƙirƙirar hash na iya canzawa da lokaci bisa farashin CPU da ma'aunin farashi, don haka kowanne raka'a zai kasance 'ba za a iya canzawa ba'.
