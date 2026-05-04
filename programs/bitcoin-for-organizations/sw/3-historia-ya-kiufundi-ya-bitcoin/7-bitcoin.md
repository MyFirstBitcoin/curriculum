# 3.7 Bitcoin

Baada ya miaka mingi na majaribio yaliyoshindikana, Cypherpunks kwa kiasi kikubwa walianza kupoteza hamasa juu ya wazo la sarafu ya kidijitali isiyo na ruhusa, wakati Adam Back alipokea barua pepe iliyokuwa na kiungo cha rasimu ya karatasi nyeupe iliyoitwa ‘electronic cash without a third party’ kutoka kwa mtu asiyejulikana aliyejiita Satoshi Nakamoto.

Kufikia hapa, hebu tukumbuke tuna angalau mawazo yafuatayo:

* Saini za kriptografia ambazo zinaweza kutoa kiwango fulani cha faragha na kutokujulikana
* Wazo la sarafu isiyo na dhamana (B-Money)
* Mapendekezo (lakini bila njia) ya kupunguza utoaji wa sarafu mpya
* Sarafu za kidijitali ambazo umiliki wake ulitolewa kwa funguo za umma (B-Money) na zingeweza kuhamishwa kwa kusaini na kugawiwa upya kulingana na anwani ya mpokeaji (RPOW na Hashcash)
* Nodi zote zinatunza nakala ya leja iliyosambazwa kabisa (B-Money) (iliyokataliwa wakati huo kama isiyowezekana)
* Itifaki ya kuweka mihuri ya muda – kutumia Merkle tree hashing kutoa mpangilio wa matukio unaothibitishwa kihesabu na ambao ni vigumu kughushi ikiwa watumiaji wote wanatunza rekodi sawa
* Uthibitisho wa kazi (proof of work) ili kuunganisha juhudi halisi za ulimwengu kwenye mfumo (lakini kutumia hash yenyewe kama sarafu)
* Mitandao iliyogatuliwa kabisa ambapo kila mshiriki ni sawa na anaweza kuingia na kutoka kwenye mtandao (BitTorrent)
* Wazo la kuunganisha hashes mpya na hashes za awali (Bit Gold na kuweka mihuri ya muda)

Kilichokuwa kinakosekana wakati huo ni pamoja na:

* Suluhisho linalowezekana la kutatua tatizo la ‘Byzantine generals’
* Njia ya kupunguza kiasi cha pesa katika mzunguko licha ya maboresho endelevu ya vifaa
* Mpango wa motisha kwa watu kushiriki (tatizo la kuku na yai)

Tofauti nyingine kubwa kati ya majaribio ya hivi karibuni na Bitcoin ni kwamba Satoshi alikuwa akifanya kazi kwenye msimbo kwa muda mrefu katika roho ya asili ya ‘Cypherpunks write code’ kabla ya kuitangaza kwenye orodha za barua pepe, tofauti na Bit Gold na B-Money ambazo zilikuwa zaidi za kinadharia.

Ni ubunifu gani uliotofautisha Bitcoin na majaribio ya awali ya pesa za kielektroniki?

Uthibitisho wa kazi (proof of work) ungetumika kama utaratibu wa makubaliano na njia ya kutoa usalama na kutobadilika: Badala ya kutumia hash kama aina ya pesa, ingetumika na mchakato mpya wa kinadharia uitwao uchimbaji madini (mining), ambapo nodi ingekusanya pamoja kundi la miamala, kuongeza nambari ya bahati nasibu na kisha kutumia hashing kwenye ‘block’ ya data. Block halali inayokidhi mahitaji ya hash ingetangazwa kwenye mtandao. Blocks hizi zingeunganishwa kwa kutumia hash ya block iliyotangulia katika kila moja, na blockchain ndefu zaidi ingetumika iwapo kutatokea mgawanyiko ambapo nodi tofauti zingethibitisha na kutangaza blocks tofauti kwa wakati mmoja na kusababisha mgawanyiko wa mnyororo. Uthibitisho wa kazi ukawa njia ya kugatua uamuzi wa mwisho kutatua tatizo la Byzantine generals.

Wachimbaji hawa pia walipata motisha ya kutoa CPU inayohitajika kufanya uthibitisho wa kazi kwa kupewa bitcoin mpya kwa kila block. Kiasi cha Bitcoin wanachopewa pia kimepangwa kupungua takribani kila baada ya miaka 4 hadi Bitcoin zote zitakapoumbwa, na hivyo kuweka kikomo kigumu cha jumla ya Bitcoin zitakazowahi kuwepo kwenye mzunguko kuwa milioni 21.

Wazo la kipekee zaidi lilikuwa jinsi alivyotatua suala la kiasi cha pesa kinachoumbwa kadri vifaa vinavyoboreshwa na nguvu zaidi kutumika kwenye mtandao. Mihuri ya muda ya idadi fulani ya blocks (2016) ingetolewa wastani, na ikiwa zinaundwa haraka sana, hash inayohitajika kuunda block mpya ingefanywa kuwa ngumu zaidi, ikiwa ni polepole sana ingefanywa kuwa rahisi zaidi. Hii iliwekwa kwenye itifaki ya ugatuaji ambayo nodi zote zinaendesha na hivyo mchimbaji yeyote anayepuuza hili angepoteza nishati kuchimba block bila faida kwani ingekataliwa na mtandao mzima. Marekebisho haya yanahakikisha uundaji wa blocks mpya unabaki kwenye ratiba iliyopangwa ya utoaji, na kutoa motisha kwa wachimbaji ‘kufuata sheria’.

####   
Muhtasari

Sehemu nyingi za fumbo la kile kinachohitajika kujenga mfumo wa pesa za kielektroniki wa rika kwa rika uliogatuliwa na unaozingatia misingi ya pesa thabiti zilikuwepo kabla Satoshi hajatoa karatasi yake nyeupe na muda mfupi baada ya kutolewa kwa msimbo wa awali.

> Asili ya Bitcoin ni kwamba mara toleo la 0.1 lilipotolewa, muundo wa msingi uliwekwa na haukubadilika tena kwa maisha yake yote  
_Satoshi Nakamoto_

Wakati mawazo mengi ya maboresho (BIPs) yamependekezwa na kukubaliwa, Bitcoin imekuwa ikiendelea kufanya kazi kimya kimya tangu 2009 ikifuata itifaki iliyoundwa kwenye toleo la awali na bila usumbufu wowote mkubwa. Maboresho yote yamefanywa huku yakiruhusu utangamano wa nyuma na matoleo yote yaliyopita.



##### Tanbihi

1. Kwa maelezo kuhusu tatizo la Byzantine Generals - angalia [https://en.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
