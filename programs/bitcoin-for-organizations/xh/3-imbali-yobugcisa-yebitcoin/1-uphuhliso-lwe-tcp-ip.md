# 3.1 Uphuhliso lwe-TCP/IP

Uninzi lwethu luqhelene neendlela ze-TCP/IP ezisetyenziswa namhlanje njengesiseko se-intanethi. Imvelaphi yazo ibuyela emva kwiminyaka yoo-1970 xa izazinzulu zaziphanda ezinye iindlela zokuyila i-Arpanet – inethiwekhi eyayisungulwe ngaphambili nguMphathiswa Wezokhuselo waseMelika ukuze kwabelwane ngezixhobo phakathi kweekhompyutha ezikude. I-TCP/IP yaba ngumgangatho wenkqubo ye-Arpanet ngo-1983, nto leyo eyabangela ukuba ibe yindlela ephambili yokunxibelelana ngothungelwano ekupheleni kweminyaka yoo-1990 kwaye yaba siseko se-intanethi apho iBitcoin isebenza khona namhlanje.


| Umzekelo we-OSI | TCP/IP |
| --- | --- |
| Isicelo | Isicelo |
| Ukwazisa | Isicelo |
| Iseshoni | Isicelo |
| Ezothutho | Ezothutho |
| Inethiwekhi | Inethiwekhi |
| Ikhonkco Ledatha | Ikhonkco Ledatha |
| Umzimba | Umzimba |


Ngexesha elifanayo xa kwakuphuhliswa imodeli ye-TCP/IP, kwakuphuhliswa nesakhelo esifanayo kodwa esibanzi ngakumbi yi-International Standards Organisation (ISO) kunye neshishini le-Telecoms (CCITT). Inkqubo yokuphuhlisa iindlela ezintsha okanye ukucetyiswa kweetshintsho yayihamba kancinci kwaye inzima xa ithelekiswa nendlela engaphezulu yokuzimela eyasetyenziswa kuphuhliso lwe-TCP/IP, nto leyo eyabangela ukuba le ndlela ibe ngumphambili namhlanje.

##### Isicelo Senguqu

Nawuphi na uphuhliso olucetywayo kwiindlela ezikhoyo okanye izimvo ezintsha zingacetyiswa kwimodeli ye-TCP/IP ngokusebenzisa **Isicelo Senguqu** inkqubo. Ezi zidlula kwinkqubo yokuvunywa, ephethwe yi-Internet Engineering Task Force (IETF), kwaye ziba yisoftware evulekileyo xa zivunyiwe ukuze nabani na akwazi ukuzisebenzisa nokuzamkela. Eminye imizekelo ebalulekileyo:

* 1969 RFC 1 Ixhase indlela iipakethi eziza kuthunyelwa ngayo kwi-Arpanet
* 1981 RFC791 ichaze indlela ye-Internet protocol V4 – esisetyenziswa kakhulu nanamhlanje
* 1982 RFC 821 Inkqubo elula yokuthumela i-imeyile
* 1987 Inkqubo yeDomain Name System – indlela amagama e-domain aguqulelwa ngayo kwiidilesi ze-IP
* 1999 RDC 2616 Inkqubo yeHypertext Transfer – ebalulekileyo ekukhangeleni kwiwebhu


> **Callout**
>
> I-**Bitcoin Improvement Proposal** (BIP) ilandela indlela efanayo ne-RFC, kodwa igxile kuphela ekuphuculeni iBitcoin ngokwayo endaweni yokuphuhlisa iindlela ezintsha okanye ezizezinye. IBitcoin ikwathatha kule modeli enamanqanaba, kwaye uza kubona ezinye iindlela zichazwa njengomphakamo wesibini okanye wesithathu.


Njengokuba amanqanaba asezantsi emodeli ye-TCP/IP engatshintshanga kakhulu kule minyaka idlulileyo, ngelixa izinto ezintsha zenzeka kumphakamo ophezulu, umphakamo osezantsi weBitcoin kulindeleke ukuba utshintshe kancinci ngeli xesha, nezisombululo zokwandisa ezifana ne-Lightning ne-Liquid zenzeka ngaphezulu.

Umzekelo olungileyo wokuba indlela esisiseko yokunxibelelana iba nzima ukuyitshintsha ngokuhamba kwexesha yi-IPv6. Ukuphela okulindelekileyo kwendawo yeedilesi kwi-IPv4 kwadala imfuno yendlela entsha. Umgaqo-siseko wokuqala wadalwa ngo-1998, kodwa awuvunywanga njengomgangatho we-intanethi de kwango-2017. Nangona isombulule iingxaki ezininzi ze-IPv4 kwaye iyakwazi ukumelana nekamva, isasetyenziswa kancinci kakhulu kwishishini namhlanje. Ngeli xesha, iindlela ezininzi ezintsha zichaziwe kumphakamo ophezulu ukuvumela imultimedia, i-imeyile njl.

##### Izinto ezisisiseko ezisetyenziswa yiBitcoin

Olu lwahlulo lweengxaki zonxibelelwano luvumela iindlela zokunxibelelana ukuba ziphuhliswe ngokuzimeleyo kumphakamo ongaphezulu okanye ongezantsi kwayo. Endaweni yokuphinda kusonjululwe iingxaki kumphakamo ngamnye, inethiwekhi yeBitcoin inokuxhomekeka kumandla esisiseko anikezelwa kumphakamo womzimba kunye nekhonkco ledatha.


| Umphakamo | TCP/IP Yoqobo |
| --- | --- |
| Isicelo | Isebenzisa iDomain Name System (DNS) ukuchonga iinodi ezikufutshane. IPort 8333 ibonisa inkqubo yeBitcoin. |
| Ezothutho | I-UDP isetyenziswa kwi-FIBRE phakathi kwabavukuzi ukuze kube nokulibaziseka okuphantsi. I-TCP isetyenziswa kunxibelelwano lwe-P2P phakathi kweenodi. |
| Ezothutho | TOR Routing: Ivumela ubumfihlo kunye nobumfihlo. Inkqubo yokusasaza: Iqhuba itrafikhi kulo lonke uthungelwano. |
| Ikhonkco | Isebenza kuyo nayiphi na indlela (umzekelo, i-Ethernet, i-Wi-Fi, njl.) |
| Umzimba | Ukudluliselwa komzimba nge-wireless, i-Ethernet, okanye ezinye izixhobo zomzimba. |


##### I-Bitcoin yindlela engathathi hlangothi yokudlulisa ixabiso njengoko i-HTTPS iyindlela yokudlulisa ulwazi

* **HTTPS**: IiWebhusayithi Ezikhuselekileyo
* **SMTP**: Thumela ii-imeyile
* **FTP**: Guqulela iifayile
* **DNS**: Lawula amagama edomain
* **BTC**: Gcina kwaye guqulela ixabiso

I-Bitcoin ivumela ukuba ixabiso lithuthwe ngokuthembekileyo kwaye ngaphandle kokufuna umntu wesithathu phakathi kwabantu okanye izixhobo kwi-Intanethi. Oku kulindeleke ukuba kuvule ixabiso elikhulu.
