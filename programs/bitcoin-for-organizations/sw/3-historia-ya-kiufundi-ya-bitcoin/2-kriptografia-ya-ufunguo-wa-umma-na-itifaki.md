# 3.2 Kriptografia ya Ufunguo wa Umma na Itifaki

Mtandao wa leo, na mifumo mingi ya kisasa ya kompyuta, hutegemea kriptografia, mbinu ya kuficha taarifa ili ni mpokeaji tu wa taarifa ndiye anayeweza kuifasiri. Misingi ya kriptografia inayotumika kulinda Bitcoin inaweza kufuatiliwa hadi miaka ya 70.

Tatizo la kwanza la kutatua ni – jinsi ya kutuma siri ya pamoja kupitia njia isiyo salama.

Hili lilichunguzwa kwanza na Whitfield Diffie na Martin Hellman.

Tatizo: pande mbili – kwa kawaida huitwa Alice na Bob – wanataka kushirikiana taarifa za siri kupitia mtandao ambapo wengine wanaweza kuwa wanasikiliza. Ili kufanikisha hili, walibuni mchakato wa kubadilishana funguo wa Diffie-Hellman.

Siri hii ya pamoja inaweza kutumika kama mbegu ya kuunda funguo nyingi za usimbaji wa symmetria ili kusimba na kufasiri ujumbe wanaotumiana bila kushiriki funguo yenyewe waziwazi.

Kwa kuwa funguo binafsi haihitaji kushirikiwa, na funguo tofauti zinatumika kila upande kusimba na kufasiri, hii inaitwa algorithimu ya usimbaji wa asymmetria.

Matumizi:

* Alice anasaini ujumbe kwa kutumia funguo ya umma ya Bob – ambaye ndiye pekee anayeweza kuufasiri kwa kutumia funguo yake binafsi
* Alice anasaini ujumbe kwa kutumia funguo yake binafsi – kwa kufasiri kwa kutumia funguo yake ya umma, mtu yeyote anaweza kuthibitisha kuwa ujumbe umetumwa na Alice, bila kujua funguo yake binafsi
* Kwa kuchanganya mbinu hizi mbili na tabaka mbili za usimbaji, ujumbe unaweza kutumwa ukiwa umesimbwa ili ni Bob tu aweze kuufasiri, na anaweza pia kuthibitisha kuwa mtumaji alikuwa kweli ni Alice

Ingawa hakutajwa kwenye karatasi hiyo, Ralph Merkle alikuwa muhimu sana katika kusaidia kutatua kile kilichochukuliwa hadi wakati huo kama fumbo lisiloweza kutatuliwa – jinsi ya kuanzisha au kuanzisha upya mawasiliano ya siri kupitia mtandao ulio wazi na unaoweza kuwa na uhasama.

Mbinu hii peke yake inakabiliwa na shambulio la nguvu kubwa (brute force), ambapo mshambuliaji anaweza kuchukua nambari zilizoshirikiwa na hatimaye kuunda funguo ya pamoja baada ya muda na rasilimali za kutosha, hivyo si jibu kamili peke yake.

##### Itifaki za Mifumo ya Funguo za Umma za Kriptografia

Mbali na kuchangia kwenye mfumo wa funguo ya umma wa Diffie-Hellman ulioelezwa hapo juu, **Ralph Merkle** aliendelea kuchangia katika eneo hili kwa miaka mingi, na alikuwa muhimu katika maendeleo ya baadhi ya vipengele muhimu vinavyotumiwa na Bitcoin.

Kazi ya hash ya kriptografia ni algorithimu ya kihisabati inayopokea viingilio vya ukubwa wowote na kufanya mahesabu magumu ili kutoa thamani ya hash kwa bits, ambayo kawaida huwakilishwa na matokeo ya urefu maalum ya herufi na nambari kwa kutumia mfumo wa hexadecimal.

* Viingilio vinaweza kuwa vya ukubwa wowote
* Matokeo huwa na urefu maalum na ni ya uhakika (kiingilio kilekile kinatoa hash ileile kila wakati)
* Ni rahisi kuthibitisha lakini ni vigumu sana kurudisha nyuma mchakato ili kujua kiingilio
* Mabadiliko madogo tu kwenye data hubadilisha kabisa matokeo

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/84656891fe213376dd33805583d394afaec74e4a-515x331.svg)

Hashing ni sehemu muhimu ya itifaki ya Bitcoin. SHA-256, inayotumika kwenye Bitcoin, iliundwa na NSA na ni mfano wa algorithimu ya hashing ya kriptografia.

* Kila block kwenye mnyororo inafanyiwa hash ili data isibadilishwe – kuhakikisha uadilifu wa leja iliyosambazwa
* Hash inayozalishwa inahitaji kukidhi vigezo vya ‘Uthibitisho wa kazi’ ili kuchukuliwa kama block halali
* Miti ya Merkle – kwa kutumia matawi na hash za hash, miti ya hash inaweza kuwezesha uthibitishaji wa seti kubwa za data kwa uhifadhi mdogo
* Saini na Funguo zinazotegemea Hash zinaweza kutumika kwa pochi, anwani na uidhinishaji wa miamala

Uthibitishaji uliosambazwa wa hali za blockchain na mifumo ya leja isiyoweza kurekebishwa unafanywa kuwa inawezekana na hashing ya njia moja. Kazi za hash hutoa njia ya uhakika, ya uhakika ya kuthibitisha matukio kwenye leja za umma kama Bitcoin bila mfano wa uaminifu wa kati.

Uwezo huu mpya katika eneo la kriptografia ulitarajiwa na wabunifu wake kuleta wimbi jipya la ubunifu katika eneo hili.

##### Kriptografia ya curve ya elliptic

Moja ya ubunifu huu wa baadaye ulitokea katika mfumo wa kriptografia ya curve ya elliptic.

Kriptografia ya curve ya elliptic ilianzishwa mwaka 1985 na wanasayansi wawili, N. Koblitz na V. Miller. Walipendekeza wazo la kutumia pointi zilizofafanuliwa na curve za elliptic badala ya mashamba ya nambari za msingi kama inavyotumika kawaida kwenye itifaki ya kubadilishana funguo ya Diffie-Hellman. Maelezo ya jinsi hii inavyofanya kazi yako nje ya wigo wa sehemu hii, lakini kwa muhtasari, curve ya elliptic ni seti ya pointi zinazokidhi mlinganyo maalum wa kihisabati.

Mlinganyo wa curve ya elliptic unaonekana kama:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Hii ina sifa kadhaa muhimu:

* Ulinganifu wa mlalo. Pointi yoyote kwenye curve inaweza kuakisiwa juu ya mhimili wa x na kubaki kwenye curve ileile.
* mstari wowote usio wima utakutana na curve kwenye sehemu zisizozidi tatu.
* Ukubwa mdogo wa funguo ni muhimu kwa uhifadhi na usafirishaji bora wa funguo za umma kwenye blockchain.

Sifa hizi zinaweza kutumika kuunda jozi za funguo kwa njia inayofanana na algorithimu ya Diffie-Hellman. Bitcoin hutumia ECDSA, ambayo ni kifupi cha Elliptic Curve Digital Signature Algorithm. Ni mchakato unaotumia curve ya elliptic na uwanja wa nambari ulio na kikomo ili “kusaini” data kwa namna ambayo watu wengine wanaweza kuthibitisha uhalali wa saini huku msaini akibaki na uwezo wa kipekee wa kuunda saini hiyo. Kwa bitcoin, data inayosainiwa ni muamala unaohamisha umiliki.

Sehemu ya ‘kikomo’ ni sawa na mbinu ya ‘mod’ kwenye Diffie-Hellman, ambapo matokeo ya mlinganyo hugawanywa na mabaki hutumika kuhakikisha yanaingia kwenye wigo wa nambari fulani.
