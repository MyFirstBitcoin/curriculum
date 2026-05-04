# 3.7 Bitcoin

Bayan shekaru da dama da kuma yunkurin da suka ci tura, mafi yawan Cypherpunks sun fara rasa sha'awa ga ra'ayin kudin dijital mara izini, lokacin da Adam Back ya karɓi wani imel da ke ɗauke da haɗin zuwa wani takaitaccen farar takarda mai taken ‘electronic cash without a third party’ daga wani mutum marar suna da ya kira kansa Satoshi Nakamoto.

Don taƙaita a wannan lokaci, muna da aƙalla waɗannan ra'ayoyin:

* Sa hannun lambar sirri da za su iya samar da wani matakin sirri da ɓoyewa
* Ra'ayin kudin da ba shi da tushe (B-Money)
* Shawarwari (amma babu hanyar) don takaita fitar da sabbin kuɗi
* Kudaden dijital da mallakarsu ke da alaƙa da mabuɗan jama'a (B-Money) kuma za a iya motsa su ta hanyar sa hannu da sake warewa bisa adireshin mai karɓa (RPOW da Hashcash)
* Dukkan nodes suna riƙe da kwafin ajiyar bayanai da aka rarraba gaba ɗaya (B-Money) (an yi watsi da wannan a lokacin saboda rashin yiwuwa)
* Tsarin ɗora lokaci– amfani da Merkle tree hashing don samar da tarihin abubuwa da za a iya tabbatar da shi ta hanyar lissafi wanda yana da wahalar ƙirƙira idan duk masu amfani suna da irin wannan bayanan
* Shaidar aiki don haɗa ƙoƙari na gaske da tsarin (amma ana amfani da hash ɗin kansa a matsayin kuɗi)
* Cikakkun hanyoyin sadarwa da ba su da shugabanci inda duk masu amfani suke daidai kuma za su iya shiga ko fita daga hanyar sadarwa (BitTorrent)
* Ra'ayin haɗa sabbin hashes da tsoffin hashes (Bit Gold da ɗora lokaci)

Abubuwan da ba su wanzu a wannan lokaci sun haɗa da:

* Ingantaccen mafita don warware matsalar ‘Byzantine generals’
* Hanyar takaita yawan kuɗin da ke yawo duk da ci gaban kayan aiki na kwamfuta
* Tsarin lada don sa mutane su shiga (matsalar kaza da ƙwai)

Babban bambanci tsakanin ƙoƙarin baya-bayan nan da Bitcoin shi ne cewa Satoshi ya dade yana aiki kan lambar kafin ya bayyana ta a jerin imel, bisa ga ainihin ruhin ‘Cypherpunks write code’, sabanin Bit Gold da B-Money waɗanda suka fi zama ra'ayi kawai.

Menene ƙirƙira da ya bambanta Bitcoin da ƙoƙarin da aka yi a baya na kuɗin dijital?

Shaidar aiki za a yi amfani da ita a matsayin hanyar cimma matsaya da kuma samar da tsaro da rashin sauyawa: Maimakon amfani da hash a matsayin kuɗi, za a yi amfani da shi ta hanyar sabon tsarin da ake kira mining, inda node ɗaya za ta tara wasu mu'amaloli, ta ƙara lamba bazuwar sannan ta yi hashing ga ‘block’ na bayanai. Block mai inganci da ya cika buƙatar hash za a sanar da shi ga hanyar sadarwa. Za a ɗaure waɗannan blocks tare ta amfani da hash na block na baya a kowanne, kuma mafi tsawon blockchain za a yi amfani da shi idan an samu sabani inda nodes daban-daban za su tabbatar da blocks daban a lokaci guda don haifar da rarrabuwar sarkar. Shaidar aiki ta zama hanyar warware sabani a rarrabuwar sarkar don magance matsalar Byzantine generals.

Waɗannan ma'adinai kuma an ba su lada don samar da CPU da ake buƙata wajen aiwatar da shaidar aiki ta hanyar samun sabbin bitcoin a kowane block. Adadin Bitcoin da ake ba su an tsara shi ya ragu kusan kowace shekara 4 har sai an ƙirƙiri duk Bitcoin, wanda ke samar da iyaka mai ƙarfi ga jimillar Bitcoin da za ta taɓa kasancewa a yawo zuwa 21M.

Mafi asali daga cikin ra'ayoyin shine yadda ya warware matsalar yawan kuɗin da ake ƙirƙira yayin da kayan aiki ke ƙaruwa kuma ana iya amfani da ƙarin ƙarfin kwamfuta a hanyar sadarwa. Ana ƙididdige matsakaicin lokacin blocks guda 2016, idan ana ƙirƙira su da sauri fiye da kima, za a ƙara wahalar hash da ake buƙata don ƙirƙirar sabon block, idan kuma suna tafiya a hankali za a sauƙaƙa. Wannan an gina shi cikin tsarin da aka rarraba da duk nodes ke amfani da shi, don haka duk wani ma'adini da ya ƙi bin wannan zai ɓata makamashi wajen hakar block ba tare da riba ba domin sauran hanyar sadarwa za ta ƙi karɓa. Wannan gyara yana tabbatar da cewa ƙirƙirar sabbin blocks yana tafiya daidai da jadawalin da aka tsara, kuma yana ba ma'adinai kwarin gwiwa su ‘bi doka’.

####   
Taƙaitawa

Yawancin sassan da ake buƙata don gina tsarin kuɗin dijital na peer to peer da aka gina bisa ƙa'idar kuɗi mai ƙarfi sun riga sun kasance kafin Satoshi ya fitar da farar takardarsa da kuma bayan sakin lambar farko.

> Irin tsarin Bitcoin ne da zarar an saki sigar 0.1 an kafa ƙirar asali har abada  
_Satoshi Nakamoto_

Duk da cewa an gabatar da ra'ayoyi da dama na ingantawa (BIPs) kuma an karɓa, Bitcoin tana aiki tun daga 2009 bisa tsarin da aka tsara a cikin sakin farko ba tare da wata matsala mai tsanani ba. Duk gyare-gyare an yi su ne tare da tabbatar da cewa ana iya amfani da tsoffin sigogi.



##### Bayanan kula

1. Don karin bayani game da matsalar Byzantine Generals - duba [https://en.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
