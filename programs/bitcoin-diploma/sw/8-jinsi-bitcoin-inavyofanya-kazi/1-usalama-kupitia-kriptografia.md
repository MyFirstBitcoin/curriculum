# 8.1 Usalama Kupitia Kriptografia

> Kile ambacho Bitcoin inatupatia ni ahadi thabiti: programu itatekelezwa kikamilifu kama ilivyoainishwa.  
_Andreas M. Antonopoulos_

#### Kriptografia ya Ufunguo wa Umma/Binafsi


> **Definition – Maana ya Kriptografia**
>
> **Kriptografia** ni utaratibu wa kubadilisha taarifa kuwa siri ambayo ni watu sahihi tu wanaoweza kuisoma.


* **Usimbaji** ni mchakato wa kubadilisha taarifa kuwa mfumo wa nambari ili ni mtu mwenye ufunguo sahihi tu aweze kuisoma.
* **Ufunguaji** ni mchakato wa kubadilisha taarifa hiyo iliyofichwa kuwa kitu kinachosomeka tena.

Katika kriptografia ya jadi, watu wawili wanaotaka kuwasiliana kwa siri lazima kwanza washirikiane ufunguo mmoja wa siri, sawa na neno la siri la pamoja. Mtu mmoja hutumia ufunguo huu kusimba ujumbe kabla ya kuutuma, na mwingine hutumia ufunguo huo huo kufungua na kuusoma.

Tatizo la mfumo huu ni kwamba watu wote wawili lazima tayari wawe na ufunguo wa siri. Iwapo mtu mwingine atapata ufunguo huo, anaweza kusoma ujumbe wowote uliodakuliwa.

Bitcoin inatatua tatizo hili kwa kutumia njia tofauti inayoitwa kriptografia ya ufunguo wa umma, ambapo watumiaji hawahitaji kushirikiana funguo za siri mapema.

Kriptografia ya ufunguo wa umma/binafsi inatatua tatizo la kushirikiana siri. Badala ya kushirikiana neno la siri, kila mtu anakuwa na funguo mbili: ufunguo wa umma na ufunguo wa binafsi.

* **ufunguo wa umma** unaweza kushirikiwa na mtu yeyote.
*  **ufunguo wa binafsi** lazima ubaki siri wakati wote.

Kama Juma anataka kumtumia Asha kitu, anaweza kutumia ufunguo wa umma wa Asha. Ni Asha pekee anayeweza kufungua kwa kutumia ufunguo wake binafsi. Hata kama mtu mwingine atadukua ujumbe huo, hawezi kuusoma wala kuutumia bila ufunguo wa binafsi.

Katika Bitcoin, mfumo huu unatumika kutengeneza saini za kidijitali. Saini ya kidijitali inathibitisha kwamba mwenye ufunguo binafsi amekubali muamala, sawa na kusaini jina lako kwenye hati. Hii ndiyo inafanya miamala ya Bitcoin kuwa salama na kuthibitishwa bila kuhitaji kuamini mtu wa tatu.

Miamala ya Bitcoin inahusisha kuhamisha umiliki wa bitcoin kutoka anwani moja kwenda nyingine.

Usimbaji hutumika kuhakikisha kwamba ni mmiliki halisi wa bitcoin pekee ndiye mwenye mamlaka ya kutuma fedha zake kwa mtu mwingine. Inahakikisha mali yao inalindwa dhidi ya watu wabaya.

Kama hatua ya ziada ya ulinzi, kila muamala wa Bitcoin hupata saini ya kipekee ya kidijitali moja kwa moja. Saini hii ya kipekee ya kidijitali inaendeshwa na teknolojia isiyoweza kuchezewa ambayo inasaidia mtandao kuthibitisha kwamba mmiliki halisi wa bitcoin, na si mtu mwingine, ndiye aliyezituma.


> **Dark**
>
> Kila mtumiaji ana funguo mbili: **ufunguo binafsi**, ambao **unabaki siri**, na **ufunguo wa umma** ambao unaweza **kushirikiwa na wengine**. **Ufunguo binafsi** hutumika kama njia ya utambulisho na uthibitisho wa umiliki, ikithibitisha: “Anwani hii ni yangu na ninaidhibiti.”


###### Jinsi Muamala wa Bitcoin Unavyofanya Kazi

1. **Kuunda Muamala**: Mtumiaji anaanzisha muamala wa Bitcoin kwa kuweka maelezo kama vile anwani ya mpokeaji na kiasi cha bitcoin kinachotumwa.
1. **Uzalishaji wa Saini ya Kidijitali**: Mtumaji anazalisha **saini ya kipekee ya kidijitali** kwa kutumia **ufunguo wake binafsi**. Saini hii ni msimbo wa kipekee unaothibitisha uhalali wa muamala.
1. **Kutangaza Muamala**: Muamala uliosainiwa unatolewa kwenye mtandao wa Bitcoin, ukionyesha nia ya kuhamisha umiliki wa bitcoin kutoka kwa mtumaji kwenda kwa mpokeaji.
1. **Uthibitishaji kwenye Mtandao**: Node kwenye mtandao wa Bitcoin zinapokea muamala na kutumia **ufunguo wa umma wa mpokeaji** kuthibitisha uhalisi wa sahihi. ya muamala. Wakati huo huo, wanatumia **ufunguo wa umma** kuthibitisha **sahihi ya kidijitali**.
1. **Uthibitisho kwenye mtandao wa Bitcoin**: Ikiwa uthibitisho umefanikiwa, muamala utaongezwa kwenye daftari, ambalo hutumika kama rekodi salama na wazi ya miamala yote. Mara tu imethibitishwa, umiliki wa bitcoin unahamishwa rasmi kutoka kwa mtumaji kwenda kwa mpokeaji.


> **Callout – Muhtasari**
>
> Sahihi ya kidijitali**sahihi ya kidijitali**, iliyoundwa kwa kutumia **ufunguo wa siri** wa mtumaji, inathibitisha kwamba muamala umeidhinishwa na mmiliki wa bitcoin. Mtandao wa Bitcoin unaweza kisha kuthibitisha ushahidi huu na kurekodi muamala.


#### Maelezo ya Hashing

Tafadhali usiogope maneno ya kiteknolojia na dhana za kihisabati zinazokuja. Tunaelewa kwamba si kila mtu anapenda hesabu, lakini unaweza kujishangaza na kuona kwamba hata mawazo magumu zaidi yanaweza kueleweka kwa jitihada kidogo.


> **Definition – Ufafanuzi wa kazi**
>
> Kazi**kazi** ni kama mashine inayopokea taarifa na kuibadilisha kuwa kitu kipya. Taarifa unayotoa kwenye kazi ni **ingizo**. Taarifa mpya inayotolewa na kazi ni **matokeo**. Kazi husaidia kompyuta kufanya kazi na kutatua matatizo.


##### Kazi ni nini?

Kazi ni seti ya maagizo inayopokea ingizo na kutoa matokeo. Unaweza kufikiria kama mapishi: unafuata hatua na viungo fulani, na kila wakati unapata matokeo yanayotarajiwa.

Katika Bitcoin, kazi hutumika kuchakata na kuthibitisha miamala. Mtu anapotuma bitcoin, kazi za kriptografia husaidia kukagua kama muamala ni halali, kuthibitisha kama mtumaji ana fedha za kutosha, na kusasisha salio kwenye daftari la Bitcoin. Mara tu imethibitishwa na kuongezwa kwenye bloku, muamala unakuwa sehemu ya rekodi ya kudumu kwenye blockchain.

##### Kazi ya njia moja ni nini?

Kazi ya njia moja ni aina maalum ya kazi ambayo ni rahisi kuhesabu upande mmoja lakini ni ngumu sana kuirudisha nyuma. Kwa mfano, kuchanganya viungo kutengeneza juisi ni rahisi, lakini huwezi kutenganisha juisi hiyo kurudisha viungo vya awali.

Usalama wa Bitcoin unategemea kazi za njia moja. Zinatumika kwenye kriptografia ya funguo za umma na za siri, kuruhusu watu kushiriki ufunguo wa umma huku wakihifadhi ufunguo wa siri. Hata kama ufunguo wa umma unaonekana, haiwezekani kupata ufunguo wa siri kutoka kwake. Hii ndiyo inafanya miamala ya Bitcoin kuwa salama.

##### Kazi ya hash ni nini?

Kazi ya hash**kazi ya hash** ni kama mashine ya siri ya kutengeneza msimbo. Inapokea ujumbe na kuubadilisha kuwa msimbo.

###### Jinsi Hashing Inavyofanya Kazi Katika Miamala ya Bitcoin

Katika Bitcoin, kila muamala hubadilishwa kuwa hash kabla ya kuongezwa kwenye blockchain. Hash ni alama ya kipekee ya kidijitali ya muamala. Mtu yeyote akijaribu kubadilisha hata sehemu ndogo ya muamala, hash itabadilika kabisa. Hii inafanya iwe rahisi kwa mtandao kugundua udanganyifu.

###### Nafasi ya Hashing Katika Usalama wa Bitcoin

Hashing husaidia kulinda mtandao wa Bitcoin kwa kufanya miamala iwe rahisi kuthibitisha na haiwezekani kubadilishwa kimya kimya. Kwa sababu kila muamala una hash yake ya kipekee, mtandao unaweza kugundua haraka kama kitu kimebadilishwa.

Kazi ya hash inapokea data na kuibadilisha kuwa mfululizo wa kudumu wa nambari na herufi unaoitwa hash. Ingizo lile lile litatengeneza hash ile ile kila wakati, lakini hata mabadiliko madogo kwenye ingizo yatatoa matokeo tofauti kabisa. Sifa hii inaruhusu kompyuta kukagua kuwa data haijabadilishwa.


> **Definition – Ufafanuzi wa Hashing**
>
> **Hashing** ni kama kutengeneza alama ya vidole kwa data ya kidijitali. Ni mchakato wa kuchukua ujumbe wa kidijitali na kuubadilisha kuwa msimbo wa urefu maalum, ambao hutumika kama kitambulisho cha kipekee. Kama vile alama ya kidole inavyoweza kumtambua mtu, hash inaweza kutambua ujumbe wa kidijitali.


Matokeo**matokeo**, au hash, huwa na urefu uleule kila wakati, haijalishi taarifa ya awali ilikuwa ndefu kiasi gani. Bitcoin hutumia aina chache maalum za kazi ya hash zinazoitwa **SHA-256** na **RIPEMD160**.

Mifano michache iko hapa chini:

* SHA256 hash ya mfuatano wa herufi **habari dunia**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256 hash ya maandishi **habari dunia.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Angalia kwamba mabadiliko madogo tu kwenye ingizo yanabadilisha kabisa matokeo ukilinganisha na la kwanza
* SHA256 hash ya faili la iso linaloweza kupakuliwa **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Ingizo hili ni faili kubwa sana lakini matokeo bado ni urefu uleule wa kudumu

Unaweza pia kufikiria hashing kama noti ya muziki inayoshika kiini cha kipande cha muziki. Kama vile noti ya muziki ni uwakilishi wa kipekee wa wimbo, thamani ya hash ni uwakilishi wa kipekee wa data.

Kwa kulinganisha noti ya kipande cha muziki na uchezaji halisi, mwanamuziki anaweza kujua kama uchezaji ni sahihi. Vivyo hivyo, kwa kulinganisha thamani ya hash ya data iliyopokelewa na thamani ya hash ya asili, mtu anaweza kujua kama data imebadilishwa wakati wa usafirishaji.

Kama vile mabadiliko madogo kwenye uchezaji wa muziki yanaweza kufanya usikike tofauti, hata mabadiliko madogo kabisa kwenye data ya asili yatasababisha thamani tofauti ya hash. Hii inafanya hashing kuwa chombo chenye nguvu kuhakikisha uadilifu na uhalisi wa muamala wa Bitcoin.

Mchakato wa kusimba **ufunguo wa umma** kupitia hashing hutumika kuboresha usalama wa taarifa kwa kuibadilisha kuwa muundo wa urefu wa kudumu usiosomeka. Bitcoin hutumia algoriti za SHA-256 na RIPEMD160 kutengeneza anwani za umma. Matokeo yanayotokana yanatumika kama kitambulisho cha kipekee kwa **ufunguo wa umma** na husaidia kuhakikisha uadilifu na usalama wa miamala iliyohifadhiwa kwenye leja. Kwa kusimba taarifa kwa njia hii, inakuwa vigumu zaidi kwa watu wasioidhinishwa kupata na kubadilisha data.

##### Sifa za kazi ya hashing

* **Ya kudumu**: Viungo vilevile daima vinatengeneza smoothie ileile. Vivyo hivyo, data ileile daima itatoa hash ileile.
* **Upinzani wa picha ya awali**: Ukiwa na smoothie pekee, huwezi kujua matunda halisi yaliyotumika. Vivyo hivyo, ukiwa na hash pekee, huwezi kujua data ya asili.
* **Athari ya maporomoko**: Kubadilisha hata sehemu ndogo ya viungo kunatengeneza smoothie tofauti kabisa. Katika hashing, mabadiliko madogo sana kwenye data yanatoa hash tofauti kabisa.
* **Upinzani wa mgongano**: Ni vigumu sana kupata seti mbili tofauti za viungo vinavyotengeneza smoothie ileile kabisa. Vivyo hivyo, ni nadra sana data mbili tofauti kutoa hash ileile.
* **Rahisi kuthibitisha**: Kutengeneza smoothie ni haraka, na ni rahisi kuangalia kama ni smoothie. Kazi za hash ni za haraka kuhesabu na rahisi kwa yeyote kuthibitisha.

#### Shughuli: Tengeneza SHA 256 Hash


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Una hamu ya kujua jinsi hashing inavyofanya kazi? Skanisha msimbo wa QR ili kutengeneza mara moja SHA256 hash kutoka kwa neno, sentensi, au ingizo lolote unalotaka. Kazi za hash ni kama alama za vidole za kidijitali: ni njia moja tu, maana yake ukishahash, haiwezi kurudishwa nyuma. Jaribu na ujionee mwenyewe!
