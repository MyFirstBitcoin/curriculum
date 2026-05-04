# 7.2 Bygga det förnybara energinätet

#### 7.2.0: Introduktion

Bitcoin är beroende av energi för sin konsensusmekanism ‘proof of work’, vilket hjälper till att säkerställa att det förblir en decentraliserad och tillståndsfri form av pengar. Elnätet står inför utmaningar med att integrera nya energiformer från förnybara källor, vilket sätter press på den nuvarande infrastrukturen. Detta kapitel ger en kort introduktion till dessa utmaningar och en översikt över relevanta aspekter av Bitcoin innan det visas hur det bidrar till utvecklingen av det förnybara energinätet.


> **Info – Bitcoin som energivaluta**
>
> Den 4 december 1921 publicerade New York Tribune en artikel som beskrev Fords vision om att ersätta guld med en energivaluta som han trodde kunde bryta bankeliternas grepp om världens rikedom och sätta stopp för krig. Han avsåg att göra detta genom att bygga “världens största kraftverk” och skapa ett nytt valutasystem baserat på “kraftenheter”.


Som Henry Ford föreställde sig använder Bitcoin energi för att skapa och skydda valutan oberoende av statliga eller företagsintressen. Detta gör det till den första verkligt decentraliserade globala formen av pengar världen har sett. Sättet som Bitcoin-mining – termen för processen att skapa och lägga till nya block i nätverket – fungerar på är mycket konkurrensutsatt och driver Bitcoin-miners att söka efter billiga energikällor. Det är också mycket anpassningsbart och kan snabbt öka eller minska energianvändningen i specifika miljöer. Denna egenskap kan vara mycket fördelaktig för ett elnät som använder förnybara energikällor.

##### Vikten av utveckling av förnybara energinät

Övergången till förnybara energikällor skapar nya utmaningar för nätoperatörer, såsom intermittens och den distribuerade naturen hos energikällorna, flaskhalsar i överföringen och nuvarande begränsningar i energilagring. Detta tillför en komplexitet till nätets drift som inte fanns när man enbart använde centraliserade och pålitliga baskraftkällor. För att hantera detta måste nätoperatörer undersöka smarta nät-teknologier och AI-baserad prognosteknik för att förbättra effektiviteten. Ett alternativ som används idag är efterfrågeflexibilitetsprogram, som kräver en energikälla som dynamiskt kan anpassa sig i nästan realtid för att hjälpa till att matcha energiefterfrågan med utbudet. Det är här Bitcoin-mining kan hjälpa till.



#### 7.2.1 Utmaningarna med integration av förnybar energi

Nätoperatörer måste ständigt matcha tillgång och efterfrågan på elektricitet. Om efterfrågan på el blir för hög kan nätet fallera, vilket leder till rullande brownouts eller till och med rullande blackouts.

Om för mycket energi tillförs nätet kan det också orsaka problem såsom ökad värme och skador på infrastrukturen. I allvarliga fall kan detta utlösa en automatisk säkerhetsavstängning, vilket triggar en kedjereaktion över nätet och skapar brownouts eller blackouts. Blackouts är katastrofala händelser som kostar företag miljarder kronor. De kostar även liv.

##### Status för nuvarande infrastruktur

Dagens nätinfrastruktur är optimerad för traditionella energikällor som fossila bränslen, såsom kol, gas eller kärnkraft, vilka kan leverera ett stabilt, centraliserat och kontrollerat energiflöde för att möta efterfrågan. Detta gör balansen mellan tillgång och efterfrågan relativt enkel. Med införandet av förnybar energi måste nätet nu hantera olika distribuerade energityper, som alla beter sig mycket annorlunda än de energikällor det ursprungligen var designat för. Förnybara källor som vind och sol genererar el intermittent. Till exempel, under en vindstilla period kan ett vindkraftverk producera lite eller ingen el, medan under kraftiga vindar kan turbinerna översvämma nätet med överskottsel. Nuvarande nätsystem är inte utrustade för att hantera dessa fluktuationer effektivt.

##### Efterfrågeflexibilitet

Det finns ett par möjliga tillvägagångssätt som nätoperatören kan använda för att hantera fluktuationerna i tillgång och efterfrågan:

* Bygg ut konventionella (fossilbränslebaserade) kraftverk som kan hållas i beredskap till en kostnad. Vid oväntad ökning i efterfrågan kan dessa tas i drift för att leverera den extra energi som behövs.
* Bygg ut förnybara energikällor och inför sedan begränsningsplaner för att förhindra att dessa källor översvämmar nätet vid tider av hög elproduktion utan motsvarande efterfrågan.

Det andra alternativet är att försöka minska efterfrågan vid tider av hög belastning**.** Dock hade nätoperatörer aldrig hittat ett tillförlitligt, snabbt och skalbart sätt att minska efterfrågan innan Bitcoin-mining, vilket lämnade dem med få alternativ annat än att investera i reservkraftverk eller betala de förnybara källorna för att stänga av – båda dyra lösningar.

##### Isolerad energi

Utmaningarna med att ansluta vindkraftsparker till nätet innefattar vanligtvis flera steg; tillgångsstudie, detaljerad konsekvensanalys, implementeringsplan och anslutningsavtal. Denna process kan ta många år. Som exempel visar diagrammet nedan den totala vindkraftskapaciteten som väntar på nätbedömning i mitten av 2024.

![Total wind energy on the waiting list for grid connection assessment](https://cdn.sanity.io/images/vje9ehw2/staging/47c8e509b367a51a036409fe4fd0b7c845ae550a-1694x1410.png)

_Total vindkraft på väntelistan för nätanslutningsbedömning (Källa: windeurope.org)_

##### Nätanslutning

Efter att de förnybara energikällorna har byggts finns det ofta en försening innan de kan anslutas på grund av brist på kapacitet i nätet. Detta leder till att kapacitet står oanvänd och går till spillo tills anslutningen kan ske, under vilken tid den potentiella energin som genereras skulle kunna användas för att driva bitcoin-miners och generera en inkomst.

##### Överproduktion och begränsning

När denna kapacitet har lagts till nätet flyttas problemet till ett av begränsning. När vinden producerar mer kapacitet än vad som behövs vid ett givet tillfälle finns det idag ingen teknik för att lagra detta, så kapaciteten går helt enkelt till spillo. För att ta risken att bygga vindkraftverken får operatörerna ett garanterat pris för all producerad energi, och för att undvika överbelastning av nätet får de betalt för att stänga av vindkraftverken. Som exempel betalade brittiska konsumenter 1 miljard pund 2024 för att ‘begränsa’ 6,6 GWh kapacitet.

Ett annat tillvägagångssätt för begränsning är användningen av gaskraftverk för topplast. Detta är ett kraftverk som använder naturgas för att generera el under perioder av hög efterfrågan. De används också för att balansera elnätet genom att generera el när efterfrågan är hög eller utbudet är lågt. Som namnet antyder används de vanligtvis bara vid topplast, men måste installeras och underhållas kontinuerligt, så de är i praktiken ‘begränsade’ större delen av tiden och står i beredskap. Vid hög efterfrågan kan nätoperatören använda dem för att öka utbudet. Som exempel uppskattas att implementeringen av Bitcoin-mining istället för att köpa och driva gaskraftverk har sparat Texas 18 miljarder dollar.

##### Modernisering av nätet

Smarta nät byggs för att hantera denna alltmer diversifierade mix av energikällor, och integrerar sömlöst både traditionella fossila bränslen och moderna förnybara metoder i ett enda fungerande nätverk. Genom att använda avancerad teknik som batterilagring kan smarta nät potentiellt lagra överskottsenergi och släppa ut den vid behov, vilket gör det möjligt att hantera fluktuationer och intermittens hos förnybar energi, såsom toppar vid hög produktion och brist vid låg produktion. Vid tiden för denna text är detta fortfarande i ett tidigt utvecklingsskede.

##### Teknologiska framsteg

Övervakning och analys är nyckeln till att implementera smarta nät i stor skala. Det börjar med att installera sensorer och övervakningsteknik på plats i anläggningen där energin genereras. Analysmjukvara analyserar sedan och förutspår trender baserat på data som samlats in genom denna övervakning, och ger råd om anläggningens hälsa såsom potentiella avstängningar och fel för att förbereda det smarta nätet för dessa situationer. Smarta mätare är slutdestinationen för datainsamling, och övervakar konsumenternas energianvändning vid källan. Användningen av AI förväntas hjälpa till att hantera denna komplexitet, och därför måste nätoperatörer öka sina färdigheter inom detta område.

##### Sammanfattning

Regeringars snabba satsning på att implementera förnybar energi i stor skala i nätet sätter press på den befintliga nätstrukturen och kräver enorma investeringar för att hantera den distribuerade och dynamiska naturen hos förnybara energikällor. Den nuvarande designen är mycket slösaktig med energi, vilket driver upp kostnaderna för industrin och konsumenten. Många av de teknologier som kommer att behövas för att detta ska lyckas är fortfarande under utveckling vid tiden för denna text. En bättre lösning behövs.



#### 7.2.2 Introduktion till Bitcoin-mining

##### Vad är Bitcoin-mining?

Bitcoin-mining är processen som används för att generera nya enheter av bitcoin och verifiera nya transaktioner. Det involverar ett nätverk av datorer runt om i världen som verifierar och säkrar blockkedjan – en virtuell huvudbok som dokumenterar alla transaktioner och löser ‘dubbelspenderingsproblemet’ där samma pengar potentiellt skulle kunna spenderas två gånger.

Bitcoin-miners är datorer som använder specialiserade ASICs (application specific integrated circuit) för att skapa nya potentiella block och få möjligheten att lägga till ett nytt block i huvudboken genom att generera en kryptografisk lösning som matchar specifika kriterier. Ju fler miners som är aktiva i nätverket, desto svårare är denna lösning att hitta, vilket justeras dynamiskt av en del av protokollet som kallas svårighetsjustering. Belöningen för att lägga till ett nytt block är tilldelningen av nya mynt samt blockavgifterna till den framgångsrika minern.

Denna kapplöpning om att skapa nästa block och få belöningarna har skapat ett enormt, decentraliserat nätverk av miners som jagar billig energi för att kunna konkurrera, och introducerar en intressant dynamik i kapplöpningen om att lägga till förnybar energi i elnätet.

##### Kontrovers kring energiförbrukning

Som nämnts i introduktionen är Bitcoin-mining kopplat till verklig energianvändning. Denna energianvändning har varit på nyheterna i flera år. Det kritiseras ofta för att använda för mycket energi, inte använda sin energi effektivt, eller i extrema fall, vara en ren klimat-/energi-katastrof. Men Bitcoin-nätverket är och kommer alltid att vara en avrundningsfel när det gäller global energiförbrukning, oavsett om det är framgångsrikt eller inte, och dess energianvändning kommer inte att överstiga dess långsiktiga nytta (hur hög eller låg den än blir). Som vi kommer att se kan de specifika egenskaperna hos dess energianvändning hjälpa till med införandet av förnybar energi.

##### Geografisk flexibilitet för mining-verksamheter

> En intressant bieffekt av PoW-mynt – de är alltid villiga energiköpare vid 3–5 öre/kWh. Och några av de bästa energitillgångarna finns utanför nätet. Detta globala energinät frigör isolerade tillgångar och gör nya möjliga. Föreställ dig en 3D-topografisk karta över världen där billiga energipunkter är lägre och dyra energipunkter är högre. Jag föreställer mig att Bitcoin-mining är som ett glas vatten som hälls över ytan, som letar sig in i skrymslen och vrår och jämnar ut den._Nic Carter_

Vid varje given tidpunkt försöker Bitcoin-gruvmaskiner runt om i världen skapa nästa block, och eftersom den största kostnaden för gruvarbetare är el, skapar detta en konkurrens om att hitta och använda energi från de billigaste källorna, var de än finns. Folk föreställer sig ofta att Bitcoin-gruvarbetare konkurrerar med andra industrier om el, som om Bitcoin-gruvdrift måste tränga undan någon annan användning av el för att fungera. Men eftersom Bitcoin-gruvarbetare i grunden kräver extremt billig el, så _kan de inte_ normalt konkurrera med vanliga elkonsumenter. Som ett resultat söker Bitcoin-gruvarbetare upp ineffektiviteter runt om i världen där el underutnyttjas och slösas bort. Detta beskrevs väl 2018 av Nic Carter.

##### Efterfrågeflexibilitet hos gruvdrift

> Bitcoin-gruvarbetare är unika elköpare eftersom de erbjuder mycket flexibel och lätt avbrytbar belastning, betalar ut i en globalt likvid kryptovaluta och är helt platsoberoende, de behöver bara en internetuppkoppling. Dessa kombinerade egenskaper utgör en extraordinär tillgång: en elköpare i sista hand som kan slås på eller av med kort varsel var som helst i världen.  
_Jack Dorsey_

Utöver geografisk flexibilitet kan Bitcoin-gruvarbetare även erbjuda efterfrågeflexibilitet. Bitcoin-gruvdrift gör det lönsamt att överdimensionera förnybara energikällor, eftersom det gör det möjligt att tjäna pengar på överskottsproduktionen. Varje samhälle som vill ha tillförlitlig el behöver ändå överdimensionerad kapacitet, och för vind, sol och vattenkraft är det ännu viktigare eftersom de är variabla. Men att överdimensionera är vanligtvis inte särskilt kostnadseffektivt, om man inte kan använda det till något lönsamt och användbart när det annars inte behövs. Bitcoin-gruvarbetare är en unik lösning på det problemet, kan göra överdimensionering lönsam och fungerar därmed indirekt som en energilagringslösning.

Under den stora majoriteten av tiden när det finns mer tillgång än efterfrågan fungerar Bitcoin-gruvarbetare som en av elkonsumenterna i samhället som kan driva sina maskiner, tjäna pengar och betala sina elkostnader. Om det sker en ökning i efterfrågan på el eller en minskning i tillgången som annars skulle orsaka strömavbrott i regionen, kan dessa gruvarbetare tillfälligt stänga av.

Ett välstrukturerat kommersiellt elavtal kan få detta att fungera smidigt. Elbolaget kan erbjuda gruvarbetaren det lägsta möjliga priset i området, i utbyte mot att de har högre tolerans för variation och andra flexibla avtalsvillkor.

Sammanfattningsvis är Bitcoin-gruvarbetare unika eftersom:

* Nästan hela deras driftskostnad är el
* De kan tolerera intermittent förbrukning
* De är flexibla med sin placering, så de kan undvika dyra överföringsnät genom att placera sig nära kraftkällan.

Som ett resultat kan de avstå från variabler som de flesta andra företag inte kan, i utbyte mot extremt låga elpriser när el är i överflöd. Det betyder att vi med Bitcoin-gruvdrift nu har en köpare för varje producerad watt energi, var som helst i världen, dygnet runt.



#### 7.2.3 Fallstudier

Teoretiskt kan vi se att Bitcoin-gruvdrift kan spela en stor roll i att påskynda användningen av förnybar energi. Låt oss titta på några exempel på tillämpningar idag.

##### Isolerad vattenkraft

Vattenkraftverk genererar el kontinuerligt, vilket också kan variera under året beroende på plats och säsong. Detta innebär vanligtvis att el slösas bort antingen under natten när alla sover, eller genom ökad produktion under regnperioden, som i Kina. Eftersom Bitcoin-gruvarbetare kan ta sig till energikällan brukade de samlas i Sichuan under regnperioden för att använda den annars bortslösade energin. De gjorde detta inte för att de är altruistiska miljövänner, utan helt enkelt för att det är billigt och ingen annan använder den. När Kina förbjöd bitcoin-gruvdrift packade de helt enkelt ihop och åkte därifrån.

Avlägsna samhällen eller byar nära potentiella vattenkraftskällor har ofta inte råd med investeringen som krävs för att bygga ut överföringsinfrastrukturen för att leverera elen. I denna situation kan Bitcoin-gruvarbetare samla in det kapital som krävs för att bygga anläggningen, förse de lokala invånarna med billig el och använda överskottsenergin till gruvdriften. Återigen, detta sker inte av altruism, utan för vinst; en win/win för gruvarbetarna och det lokala samhället.

##### Bitcoin-gruvdrift för att stabilisera elnätet

El-nät måste kompensera för två saker: förändrade tillgångsnivåer och förändrade efterfrågenivåer. Vissa elkällor är mycket stabila, som baskraft från kärnkraftverk, som kan köras dygnet runt. Andra källor, som vind, sol och till viss del vattenkraft, är mer variabla beroende på vad naturen erbjuder i form av vind, sol och regn under en viss period. På grund av denna variation måste elproduktionen överdimensioneras så att det även under en särskilt 'låg' dag i produktionen ändå räcker till för samhället. I Texas var standardplanen att bygga ut fossildrivna reservkraftverk som kunde stå i beredskap för att möta ökad efterfrågan. Det alternativa tillvägagångssättet var att öka flexibiliteten i efterfrågan genom att integrera Bitcoin-gruvarbetare i nätet. Detta sparade Texasborna många miljoner i investeringar och gav ett mer miljövänligt alternativ.

##### Andra närliggande fördelar

Även om det inte är direkt kopplat till förnybar elinfrastruktur, finns det andra energirelaterade lösningar som Bitcoin-gruvdrift kan bidra med:

* Facklad gas: undvika att ventilerad eller facklad gas släpps ut i atmosfären genom att använda den för lokal gruvdrift.
* Deponigas: fånga upp metan på soptippar och använda det för elproduktion för att minska skadliga växthusutsläpp
* Främja ny teknik: Ocean Thermal Energy Conversion (OTEC) är en välkänd metod för att utnyttja temperaturskillnaden mellan ytan och djupare havslager för att generera el. Detta har inte varit kommersiellt gångbart före Bitcoin.
* Kickstarta elutveckling i utvecklingsländer: Som nämnts tidigare kan Bitcoin-gruvarbetare vara 'ankartenanten' som alltid använder den producerade elen, vilket motiverar den initiala investeringen och sedan flyttar vidare när det lokala samhället utvecklas och hittar bättre användning för elen.

##### Sammanfattning

Bitcoin-gruvdrift kan bidra till investeringar i och hållbarheten för förnybar energiinfrastruktur:

* Absorbera överskottsenergi under perioder med låg efterfrågan
* Stabilisera elnätet genom att matcha tillgång och efterfrågan
* Ge en intäktsström för utvecklare av förnybar energi
* Finansiera avlägsna eller underförsörjda energiprojekt
* Driva på gränserna för energieffektivitet
* Agera som köpare i sista hand för annars bortslösad energi var som helst i världen, när som helst



#### 7.2.4 Att bemöta farhågor

Vi har sett hur Bitcoin-gruvdrift kan bidra till tillväxten av förnybar energi, men vilka är hindren för detta?

##### Miljöpåverkan och missuppfattningar

För att Bitcoin ska kunna integreras i något så kritiskt som elnätet måste alla farhågor kring miljöpåverkan och missuppfattningar, såsom energianvändningen, bemötas. Organisationer som Bitcoinpolicy.uk arbetar hårt för att bemöta dessa farhågor med relevanta branscher och myndigheter, men det är ofta en uppförsbacke. Att hjälpa till att utbilda marknaden om de potentiella fördelarna med att tjäna pengar på isolerad energi eller använda överskottsenergi är avgörande för framgångsrik adoption.

##### Regleringar och incitament för miljövänlig gruvdrift

Länder kan ha mycket olika tillvägagångssätt för att tillåta gruvdrift, från länder som Bhutan som själva utvinner Bitcoin, till amerikanska delstater som Texas där gruvdrift tillåts utan att aktivt motarbetas, till Kina som införde ett totalt förbud mot gruvdrift.

Andra länder som Storbritannien kan betala stora summor till vindkraftsoperatörer för att stänga av elproduktionen vid kraftiga vindar. Incitamentet för att integrera Bitcoin-gruvdrift är därför begränsat i sådana fall, även om det skulle kunna förändra affärsmodellen från en kostnad för konsumenten till en vinst som kan sänka räkningarna.

##### Indirekta regulatoriska hinder

Andra indirekta regulatoriska hinder kan finnas som inte direkt hänvisar till Bitcoin men ändå kan ha en påverkan. Till exempel kan infrastrukturen som behöver byggas för havsbaserade vindkraftsparker för att ansluta till elnätet vara förbjuden att delas med datacenterinfrastruktur som skulle krävas för Bitcoin-gruvdrift.



#### 7.2.5 Slutsats och uppmaning till handling

* Bitcoin tillhandahåller en tjänst som människor kan använda för att lagra och överföra värde. Hittills har marknaden med miljontals deltagare beslutat att detta nätverk har ett värde, och likt allt av värde förbrukar det energi.
* Bitcoin-gruvdrift använder mindre än 0,1 % av världens energi, och farhågorna om att energianvändningen skulle vara slösaktig har nu blivit fullt bemötta på marknaden.
* En betydande del av energin som används av Bitcoin-gruvdrift är annars isolerad och bortslösad energi. Detta beror på att Bitcoin-gruvarbetare har den unika förmågan att ta sig till avlägsna platser och hantera inkonsekvent el som andra konsumenter inte kan använda.
* Bitcoin kan hjälpa till att stabilisera elnätet, vara ankartenant genom att vara den första att använda och betala för el tills den kan anslutas till nätet och användas någon annanstans, samt bidra till efterfrågeflexibilitet genom att snabbt stänga av under perioder med hög efterfrågan.

Bitcoin- och energimarknaderna konvergerar, och ägandet av tillgångar kommer sannolikt också att konvergera. Potentiell överlappning finns även med AI, som kräver liknande kompetens och infrastruktur som Bitcoin och kommer att användas för att hantera det smarta elnätet. Företag som anpassar sin utvecklingsplan för att inkludera dessa trender kommer att vara bäst positionerade för att dra nytta av dessa utvecklingar.



###### Bilaga - Referenser

1. [https://www.btcpolicy.org](https://www.btcpolicy.org/)
1. [https://www.da-ri.org/articles/how-bitcoin-mining-saved-texans-18-billion](https://www.da-ri.org/articles/how-bitcoin-mining-saved-texans-18-billion)
1. [https://gript.ie/uks-hidden-1billion-cost-of-wind-energy/](https://gript.ie/uks-hidden-1billion-cost-of-wind-energy/)
1. [https://www.lynalden.com/bitcoin-energy/#electricity](https://www.lynalden.com/bitcoin-energy/#electricity)
1. [https://squareup.com/gb/en/press/bcei-white-paper](https://squareup.com/gb/en/press/bcei-white-paper)
1. [https://www.mara.com/posts/bitcoin-mining-the-environment-the-positive-externalities](https://www.mara.com/posts/bitcoin-mining-the-environment-the-positive-externalities)
