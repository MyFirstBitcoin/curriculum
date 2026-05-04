# 3.2 Ubuchwephesha beKhowudi yoLuntu kunye neMigaqo-nkqubo

Namhlanje i-Intanethi, kunye neenkqubo ezininzi zekhompyutha zale mihla, zixhomekeke kwi-cryptography, indlela yokufihla ulwazi ukuze kuphela umamkeli wolwazi akwazi ukuluvula. Iziseko ze-cryptography ezisetyenziswa ukukhusela iBitcoin zingalandelwa emva kwiminyaka yee-70.

Ingxaki yokuqala ekufuneka isonjululwe yile – indlela yokuthumela imfihlo esabelwana ngayo phezu kwendlela engakhuselekanga.

Oku kwaqala kwaphandwa nguWhitfield Diffie noMartin Hellman.

Ingxaki: amaqela amabini – ahlala ebizwa ngokuba ngu-Alice no-Bob – afuna ukwabelana ngolwazi oluyimfihlo kwinethiwekhi apho abanye banokumamela. Ukuze bakwazi oku, badala inkqubo yokutshintshiselana ngesitshixo kaDiffie-Hellman.

Le mfihlo esabelwana ngayo ingasetyenziswa njengembewu yokudala izitshixo ezininzi ezifanayo zokufihla nokuvula imiyalezo abayithumelanayo ngaphandle kokwabelana ngesitshixo ngokwalo esidlangalaleni.

Njengoko isitshixo sabucala singaze sabelwane ngaso, kwaye izitshixo ezahlukeneyo zisetyenziswa kwicala ngalinye ukufihla nokuvula, oku kubizwa ngokuba yindlela yokufihla engalinganiyo (asymmetric encryption algorithm).

Iimeko zokusetyenziswa:

* UAlice usayina umyalezo ngesitshixo sikaBob soluntu – ongulowo kuphela onokuwuvula esebenzisa isitshixo sakhe sabucala
* UAlice usayina umyalezo ngesitshixo sakhe sabucala – ngokuwuvula ngesitshixo sakhe soluntu nabani na angaqinisekisa ukuba umyalezo uthunyelwe nguAlice, ngaphandle kokwazi isitshixo sakhe sabucala
* Xa ezi ndlela zimbini zidibanisiwe kunye nemigangatho emibini yokufihla, umyalezo unokuthunyelwa ufihlakele ukuze kuphela uBob akwazi ukuwuvula, aze akwazi nokuqinisekisa ukuba umthumeli ebenguAlice ngenene

Nangona engakhange anikwe imbeko ephepheni, uRalph Merkle waba negalelo elikhulu ekusombululeni le ngxaki eyayijongwa njengengenakwenzeka – indlela yokuseka okanye ukuphinda kusekwe unxibelelwano lwabucala kwinethiwekhi evulekileyo nenokuthi ibe nobungozi.

Le ndlela yodwa isengaphantsi komngcipheko wokuhlaselwa ngamandla (brute force attack), apho umhlaseli angathatha amanani abelwana ngawo aze ekugqibeleni enze isitshixo esabelwana ngaso xa enexesha nezixhobo ezaneleyo, ngoko ke ayisosisombululo sipheleleyo yodwa.

##### Iinkqubo zeNkqubo zeSitshixo soLuntu (Public Key Cryptosystems)

Ukongeza ekunikezeleni kwinkqubo yesitshixo soluntu kaDiffie-Hellman echazwe ngasentla, **Ralph Merkle** waqhubeka nokunika igalelo kule ndawo iminyaka emininzi, kwaye waba negalelo elikhulu kuphuhliso lwezinto eziphambili ezisetyenziswa yiBitcoin.

Umsebenzi wokuhashisha kwi-cryptography yindlela ye-mathematics ethatha imiyalelo yobungakanani obuphina kwaye iqhube iibalansi ezinzima ukuze ibuyise ixabiso le-hash kwi-bits, elihlala limelwe sisiphumo esingaguqukiyo sobude obuthile esisebenzisa ifomathi ye-hexadecimal.

* Imiyalelo ingaba nobungakanani obuphina
* Isiphumo sihlala sinesilinganiso esingaguqukiyo kwaye siyaphindaphindeka (umyalelo ofanayo uvelisa i-hash efanayo rhoqo)
* Kulula ukuqinisekisa kodwa kunzima kakhulu ukubuyisela umva inkqubo ukuze kufumaneke umyalelo wangaphakathi
* Utshintsho oluncinane kwidatha lutshintsha ngokupheleleyo iziphumo

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/71e66cde933040df99319f9673ea245fa73ea87c-515x331.svg)

Ukusebenza kwe-hash yinxalenye ebalulekileyo kwinkqubo yeBitcoin. I-SHA-256, esetyenziswa kwiBitcoin, yadalwa yi-NSA kwaye ngumzekelo womsebenzi wokuhashisha kwi-cryptography.

* Ibhloko nganye kwikhonkco iyahashishwa ukuze idatha ingatshintshwa – oku kuqinisekisa ukuthembeka kwe-ledger esasazekileyo
* I-hash evelisiweyo kufuneka ihlangabezane nemigangatho ye-‘Proof of work’ ukuze ithathwe njengebhloko evumelekileyo
* Imithi kaMerkle – ngokusebenzisa amasebe kunye ne-hash ye-hash, imithi ye-hash ingavumela ukuqinisekiswa kweedatha ezinkulu ngokugcina indawo encinci
* Iisayini kunye nezitshixo ezisekwe kwi-hash zingasetyenziswa kwi-wallets, iidilesi kunye nemvume yokwenza iintengiselwano

Ukuqinisekiswa okusasazekileyo kweemeko zeblockchain kunye nemodeli ye-ledger enokongezwa kuphela engalungiswayo kwenziwa yindlela yokuhashisha engabuyiswayo. Imisebenzi ye-hash ibonelela ngendlela ethembekileyo, ephindaphindekayo yokuqinisekisa iziganeko kwiiledger zoluntu ezifana neBitcoin xa kungekho mzekelo wokuthembana ophakathi.

Ezi zakhono zintsha kwindawo ye-cryptography zazilindeleke ngabadali bazo ukuba zize nezinto ezintsha kule ndawo.

##### I-cryptography ye-elliptic curve

Enye yezi zinto zintsha kamva yafika ngendlela ye-elliptic curve cryptography.

I-elliptic curve cryptography yaziswa ngo-1985 ngososayensi ababini, uN. Koblitz noV. Miller. Bacebisa umbono wokusebenzisa amanqaku achazwe yi-elliptic curves endaweni yamacandelo aphambili anemida ukuze ingxaki ye-Discrete Logarithm isebenze, njengoko kusetyenziswa rhoqo kwinkqubo yesitshixo kaDiffie-Hellman. Iinkcukacha zokusebenza kwayo ziphaya kolu candelo, kodwa ngokubanzi, i-elliptic curve yiseti yamanqaku ahlangabezana nelinge lemathematics elithile.

Ilinge le-elliptic curve libonakala ngolu hlobo:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Oku kuneempawu eziluncedo:

* Ukulingana ngokuthe nkqo. Naliphi na inqaku kwicurve linokuboniswa kwakhona ngaphezulu kwe-x axis kwaye lihlale likwicurve efanayo.
* naluphi na ulayini ongathe nkqo uya kudibana ne-curve kwiindawo ezingaphezulu kwezintathu kuphela.
* Ubungakanani bezitshixo ezincinci bubalulekile ekugcineni nasekuthumeleni izitshixo zoluntu kwi-blockchain ngendlela efanelekileyo.

Ezi mpawu zingasetyenziswa ukudala izibini zezitshixo ngendlela efanayo ne-algorithm kaDiffie-Hellman. IBitcoin isebenzisa i-ECDSA, ethetha i-Elliptic Curve Digital Signature Algorithm. Yinkqubo esebenzisa i-elliptic curve kunye nentsimi enomda 'finite field' ukuze 'isayine' idatha ngendlela yokuba abantu besithathu bakwazi ukuqinisekisa ubuqiniso besayini ngelixa umsayini egcina amandla okukwazi ukwenza isayini kuphela. KwiBitcoin, idatha esayinwayo yintengiselwano edlulisa ubunini.

Icandelo 'elinemida' lifana nendlela ye-'mod' kwiDiffie-Hellman, apho isiphumo selinge sahlulwe kwaye intsalela isetyenziswa ukuqinisekisa ukuba ihlala kuluhlu lweenani.
