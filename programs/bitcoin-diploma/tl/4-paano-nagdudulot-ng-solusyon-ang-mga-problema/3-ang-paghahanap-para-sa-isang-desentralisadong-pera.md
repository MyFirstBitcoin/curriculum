# 4.3 Ang Paghahanap para sa Isang Desentralisadong Pera

Napansin natin ang unti-unting pagkontrol ng pera ng mga bangko at gobyerno sa kasaysayan, na nagresulta sa sistemang fiat na alam natin ngayon at sa mga mapaminsalang epekto nito sa lipunan. Ngunit ang pag-usbong ng mga bagong teknolohiya tulad ng encryption at internet ay nagbigay-daan sa mga bagong ideya, gaya ng malayang digital na pera — malaya mula sa pakikialam ng gobyerno, bukas at abot-kaya para sa lahat. Tuklasin natin ang paglalakbay ng mga nanguna sa rebolusyonaryong kilusang ito: ang mga Cypherpunk.

#### Ang mga Cypherpunk

> Maaaring gamitin ang computer bilang kasangkapan upang palayain at protektahan ang mga tao, sa halip na kontrolin sila.  
_Hal Finney_

Sa ikalawang kalahati ng ika-20 siglo, sumibol ang makapangyarihang mga teknolohiya tulad ng personal na computer at internet. Binago ng mga inobasyong ito ang paraan ng pakikipagkomunikasyon, pagbabahagi ng impormasyon, at pag-oorganisa ng lipunan.

Napansin ng ilang mga palaisip at programmer na maaaring gamitin ang mga teknolohiyang ito upang palakasin ang kalayaan ng bawat isa o gawing mas madali para sa gobyerno at mga korporasyon na bantayan at kontrolin ang mga tao.

Nakilala ang grupong ito bilang mga Cypherpunk. Naniniwala sila na ang cryptography, ang paggamit ng matematikal na code upang gawing ligtas ang impormasyon, ay makakapagprotekta sa kalayaan ng bawat isa sa digital na panahon.

Nagtrabaho ang mga Cypherpunk sa mga kasangkapan na makakapagprotekta ng privacy online, makakapagpanatili ng ligtas na komunikasyon, at magpapahintulot sa mga tao na makipag-ugnayan sa internet nang hindi umaasa sa mga sentralisadong awtoridad.

Isa sa kanilang pangunahing layunin ay makalikha ng uri ng digital na pera na maaaring gamitin ng mga tao nang hindi kinokontrol ng mga bangko o gobyerno. Ang Bitcoin ay nilikha kalaunan bilang solusyon sa problemang ito.


> **Definition – Kahulugan ng orwellian na hinaharap**
>
> **Orwellian na hinaharap** ay tumutukoy sa isang dystopian na lipunan kung saan isang makapangyarihang awtoridad, kadalasan ang gobyerno, ang mahigpit na kumokontrol sa buhay ng mga tao. Sa ganitong mundo, palaging binabantayan ang mga mamamayan, minamanipula ang impormasyon, at ang pagsalungat sa mga nasa kapangyarihan ay maaaring magdulot ng parusa. Limitado ang mga personal na kalayaan, at madalas binabaluktot ang katotohanan upang mapanatili ang kontrol sa populasyon.


Kabilang sa mga pangunahing personalidad ng kilusang Cypherpunk sina Eric Hughes, Timothy C. May, at John Gilmore. Noong 1992, isinulat ni Eric Hughes ang _A Cypherpunk Manifesto_, na nagsasaad na dapat may karapatan ang mga tao sa privacy at kontrol sa kanilang digital na buhay.

Naniniwala ang mga Cypherpunk na kayang protektahan ng cryptography ang bawat isa online. Noong 1991, nilikha ni Phil Zimmermann ang PGP (Pretty Good Privacy), isang kasangkapan na nagpapahintulot sa mga tao na magpadala ng encrypted na email upang ang tanging makakabasa ay ang pinadalhan.

Naniniwala sila na ang encryption, kapag pinagsama sa internet at computer, ay magpapahintulot sa mga tao na makipagkomunikasyon at makipag-ugnayan online nang hindi umaasa sa mga sentralisadong awtoridad.

Gayunpaman, may isang malaking problema na hindi pa rin nalulutas: wala pa ring desentralisadong digital na pera na malayang magagamit ng mga tao sa internet.

#### Sentralisado vs Desentralisadong Sistema

##### Sentralisadong Sistema

Sa isang sentralisadong sistema, umiikot ang lahat sa isang pangunahing awtoridad, parang isang mataas na gusali sa lungsod. Kontrolado ng awtoridad na ito kung paano gumagana ang buong sistema. Isipin ang mga tradisyonal na bangko bilang halimbawa, kung saan isang maliit na grupo ang gumagawa ng lahat ng desisyon.

###### Mga Problema sa Sentralisadong Sistema

* **Sentral na punto ng kabiguan**: Kapag nagkaproblema ang sentral na awtoridad, maaaring bumagsak ang buong sistema.
* **Kontrol**: Isang maliit na grupo sa itaas ang may hawak ng lahat ng kapangyarihan, na kadalasan ay nagreresulta sa mga desisyong pabor sa kanila kaysa sa nakararami.
* **Hindi episyente at maraming tagapamagitan**: Parang trapik sa lungsod, maaaring bumagal at maging magastos ang sentralisadong sistema dahil sa mga hindi kailangang tagapamagitan.
* **Kawalan ng kalayaan**: Maaaring hindi makagawa ng sariling desisyon sa pananalapi ang mga tao; lahat ay dinidiktahan ng nasa itaas.
* **Sensura at restriksyon**: Parang may mga bahagi ng lungsod na isinasara, maaaring harangan o limitahan ng sentralisadong sistema ang access sa ilang pinansyal na mapagkukunan.
* **Mga hamon sa paglawak**: Kapag mas maraming tao ang nangangailangan ng serbisyo, maaaring hindi kayanin ng sentralisadong sistema ang demand.
* **Mga panganib sa seguridad**: Ang mga problema sa sentral na awtoridad ay maaaring magdulot ng panganib sa buong sistema laban sa cyberattacks.
* **Kawalan ng transparency at tiwala**: Mahirap maintindihan ang takbo ng sentralisadong sistema, kaya mahirap pagkatiwalaan ng mga tao.


> **Light**
>
> Noong 2022, sa panahon ng mapayapang protesta sa Canada, nag-freeze ang mga bangko ng account ng mga nagpoprotesta, na nagpapakita kung paano kayang kontrolin ng sentral na awtoridad ang access sa pananalapi.


##### Desentralisadong Sistema

Isipin ang desentralisadong sistema na parang isang gubat. Bawat puno ay isang hiwalay na bahagi, at ang buong gubat ang sistema. Hindi tulad ng lungsod na may isang sentral na punto, mas matibay ang desentralisadong sistema at patuloy na gumagana kahit may masira na bahagi.

###### Mga Benepisyo ng Desentralisadong Sistema

* **Mas matibay at maaasahan**: Walang iisang punto ng kabiguan, kaya matatag ang sistema kahit may mga problema.
* **Mas mataas na seguridad**: Sa tamang encryption/proteksyon, mas mahirap kontrolin ng iisang awtoridad ang desentralisadong sistema.
* **Mas Malaking Kalayaan**: Mas may kontrol ang mga tao sa kanilang pera, datos, at mga desisyon.
* **Mas malinaw na transparency**: Pare-pareho ang impormasyong nakikita ng lahat, kaya mas mapagkakatiwalaan ang sistema.
* **Walang hadlang at walang limitasyon**: Kahit sino ay maaaring sumali o makibahagi.
* **Pantay-pantay na oportunidad**: Lahat ay may patas na pagkakataon na makibahagi at magpahayag ng opinyon.
* **Mas pinahusay na Pagkapribado**: Ang datos ay nakakalat sa maraming kalahok at kadalasan ay pseudonymous, kaya mas pribado ang mga desentralisadong sistema.

Bagama't maraming benepisyo ang mga desentralisadong sistema, maaaring maging mahirap ang paggawa ng desisyon nang sama-sama. Kinakailangan nito ang pagtutulungan ng lahat.

Sa mundo ng sentralisado at desentralisadong mga sistema, ang mahalaga ay kung sino ang may hawak ng kapangyarihan. Ang mga sentralisadong sistema ay nagbibigay ng kapangyarihan sa iilang tao, samantalang ang mga desentralisadong sistema ay hinahati-hati ito, kaya't lahat ay may boses. Ang pagbabagong ito ng kapangyarihan ay nangangahulugan ng mas patas na hinaharap, kung saan maraming tao ang may impluwensya sa sistemang humuhubog sa kanilang buhay.


> **Light**
>
> Ang Tor Network ay lumilikha ng isang desentralisadong sistema kung saan maaaring manatiling anonymous ang mga tao online at mahirap pigilan o i-censor ang network.


#### Maikling Kasaysayan ng Digital na Pera

Isa sa mga pangunahing ideyang tinalakay ng mga Cypherpunk ay **digital cash**. Naniniwala sila na dapat ihiwalay ang pera mula sa kontrol ng gobyerno upang ang mga tao ay malayang makapagpadala at tumanggap ng bayad online nang pribado.

Maagang cryptographer na si **David Chaum** ay lumikha ng isa sa mga unang sistema ng digital na pera gamit ang cryptography upang gawing ligtas at pribado ang mga transaksyon. Gayunpaman, ang kanyang sistema ay umaasa pa rin sa isang **sentral na awtoridad** upang gumana, kaya't maaari itong mabigo o mag-censor ng mga transaksyon.

Sa mga sumunod na dekada, maraming Cypherpunk ang nagtangkang magdisenyo ng uri ng digital na pera na hindi umaasa sa sentral na awtoridad. Bagama't nagpakilala sila ng mahahalagang inobasyon, wala sa kanilang mga sistema ang nakalutas sa lahat ng hamon para sa isang ligtas, desentralisado, at malawakang magagamit na digital na pera.

Ang mga pagtatangkang ito ay tumulong upang matukoy kung ano ang kulang. Kalaunan, may isang taong gumamit ng mga ideyang ito at sa wakas ay nakalikha ng gumaganang sistema para sa desentralisadong digital na pera.

###### Mga Sanggunian


[▶ Panoorin ang video na ito at tuklasin ang kwento ng mga Cypherpunk!](https://www.youtube.com/watch?v=9vM0oIEhMag)
