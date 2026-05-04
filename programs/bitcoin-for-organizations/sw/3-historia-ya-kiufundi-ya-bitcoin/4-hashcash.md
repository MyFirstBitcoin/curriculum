# 3.4 Hashcash

Hashcash iliundwa na Adam Back, mmoja wa wavumbuzi wa mwanzo katika eneo hili. Adam alikuwa na shauku kubwa kuhusu masoko huru na faragha kwenye mtandao, na alikutana na orodha ya barua pepe ya Cypherpunks ambayo alijiunga nayo na kuwa mshiriki hai.

Alivutiwa sana na pesa za kidijitali, na alipendekeza jinsi kundi hilo lingeweza kufanya kazi kwa karibu zaidi na DigiCash pamoja na Chaum, lakini mapendekezo haya hayakuendelea. Kisha akageukia tatizo lingine lililokuwa linaibuka – barua taka (spam) za barua pepe. Yeye na Cypherpunks wengine walitaka kupata suluhisho la tatizo la spam, ambapo ilikuwa rahisi kwa watumaji wa spam kuunda na kutuma maelfu ya barua pepe zinazoziba mitandao. Suluhisho lake la ubunifu lilitegemea hashing – uwezo wa kriptografia kubadilisha data yoyote kuwa mfuatano wa herufi na nambari wa kipekee na wa urefu maalum, ili kuunda kile kinachofanana na 'stempu' ya kidijitali ambayo ilihitajika kuongezwa kwenye barua pepe ili ichukuliwe kuwa halali na kusafirishwa kwenye mtandao. Gharama ndogo kwa barua pepe halisi, lakini kubwa mno kwa mtumaji wa spam.

Ubunifu mkuu ambao Hashcash ulileta ulikuwa ni kuunganisha rasilimali za ulimwengu halisi – nguvu ya kompyuta – kwenye mtandao wa kidijitali. Wakati rasilimali za kidijitali hadi wakati huo zingeweza kurudiwa bila kikomo, idadi ya 'hashcash' iliyoundwa ilitegemea ni kiasi gani cha nishati watu walikuwa tayari kuwekeza ndani yake.

Ingawa suluhisho hilo lilitimiza baadhi ya vigezo ambavyo Adam aliamini vinahitajika kwenye mfumo wa pesa za kidijitali; ilikuwa ya faragha, imara na isiyohitaji kuamini mtu, kila hashcash haikuweza kutumika tena na haikuwa adimu kweli. Alipendekeza njia nyingine ambazo matatizo haya yangeweza kutatuliwa kwa kutumia wahusika wa tatu wa nje.

##### BitGold

Nick Szabo alijenga juu ya wazo la Hashcash na uthibitisho wa kazi (proof of work) ili kupendekeza suluhisho mbadala, ambalo alilielezea kwenye orodha ya barua pepe mwaka mmoja baada ya Hashcash kuchapishwa, mwaka 1998.

Ingawa ilikuwa inakaribia suluhisho, pendekezo hili bado lilikuwa na changamoto kadhaa.

* Nani angeendesha Daftari la umiliki wa hash na wanawezaje kuaminiwa?
* Hashing kwa ujumla ingekuwa rahisi na nafuu zaidi kadri muda unavyopita, changamoto pia kwa HashCash.

Kwa kuwa hash zilizounganishwa zingekuwa na alama ya muda, alipendekeza aina fulani ya ufuatiliaji wa kihistoria wa ugumu wa hashing kwa wakati huo; hash ya awali ingehitaji gharama zaidi za usindikaji kuliko ya baadaye kwa kuwa gharama zimepungua. Kwa bahati mbaya, hii ilimaanisha kwamba hash hazingekuwa 'fungible' yaani na thamani sawa, jambo linalochukuliwa kuwa sifa kuu ya pesa za kidijitali. Ili kusaidia kutatua hili Nick alipendekeza aina fulani ya 'benki huru' inayofanya kazi juu ya BitGold ambayo ingeweza kuunganisha makundi tofauti ya hash ambazo zingekuwa na thamani sawa.

##### B-Money

Muda mfupi baada ya pendekezo la Bit Gold, Wei Dai alipendekeza suluhisho linalofanana. Tayari alikuwa ametengeneza zana nyingine kadhaa kwa ajili ya Cypherpunks, na alikuwa na mawazo yake mwenyewe kuhusu pesa za kidijitali.

Pendekezo lake lilifanana na Bit Gold kwa kuwa lilitumia saini za kidijitali kuhamisha pesa, na rekodi za miamala zingehifadhiwa kwenye daftari, likiwa na funguo za umma na kiasi cha vitengo vya sarafu vilivyotolewa kwa kila mmoja. Kama ilivyo kwa Bit-Gold, wahusika wa tatu waliaminika walionekana kama mianya ya usalama, na imani ilikuwa kwamba mfumo wa pesa za kielektroniki haupaswi kutegemea chombo kimoja kufuatilia salio, miamala au kuzuia matumizi mara mbili.

Wei Dai alipendekeza suluhisho kadhaa kwa masuala haya, mojawapo ikiwa ni badala ya chombo kimoja (au vyombo) cha kati kudumisha daftari, NODI zote zingekuwa na nakala. Ikiwa watumiaji wote watakagua daftari lao na uhalali wa kila muamala, mradi nodi zote ziwe za kisasa basi daftari zitabaki zimesawazishwa kwenye mtandao. Mfumo huu uliosambazwa sana ungekuwa mgumu kuharibu.

Wei Dai alitambua kwamba hili halikusuluhisha tatizo la majenerali wa Byzantine (1), kwani nodi zingeweza kupoteza usawazishaji au kusema uongo tu. Alipendekeza mbinu mbadala kama vile kuwa na sehemu ndogo ya seva 'zinazoaminika' zinazodumisha daftari, na kuunda motisha za kifedha kuzifanya seva hizi ziwe waaminifu.

Kwa sera ya fedha, alipendekeza kufunga nguvu ya ununuzi ya B-Money kwa aina fulani ya fahirisi ya bei ya bidhaa za walaji. Alitaka kiasi sawa cha B-Money kiweze kununua sehemu sawa ya fahirisi hiyo kwa muda, ili kutoa utulivu wa bei. Hivyo, mtu yeyote angeweza kuunda vitengo vipya vya sarafu kwa kutoa hash halali, lakini ugumu wa kuunda hash ungeweza kubadilika kadri muda unavyopita kulingana na gharama za CPU na fahirisi ya bei, ili kila kitengo kiwe 'kisichobadilika'.
