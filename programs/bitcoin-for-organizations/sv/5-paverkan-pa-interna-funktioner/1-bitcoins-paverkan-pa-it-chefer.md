# 5.1 Bitcoins påverkan på IT-chefer

> Varje informerad person behöver känna till Bitcoin eftersom det kan vara en av världens viktigaste utvecklingar.  
_Leon Luow_



#### 5.1.0 Introduktion

IT-chefer har ansvar gentemot verksamheten, där de använder teknik både för att driva innovation och konkurrenskraft för sina företag, samt för att hitta sätt att förbättra interna effektivitet för att sänka kostnaderna.

Det finns flera vanliga risker och missuppfattningar kring Bitcoin som är bra att förstå och kunna ge vägledning om:

* Det ses ofta som en del av en större 'krypto'-industri, och lösningar som bygger på en av de viktigaste innovationerna, blockkedjan.
* Det uppfattas som att det 'slösar energi' för att driva nätverket.
* Det finns en risk för användare av publika molntjänster att miljön kan bli hackad och användas för att 'minera' Bitcoin eller andra kryptovalutor av en illvillig aktör, vilket kan leda till en mycket stor och oväntad faktura, samt påverka prestandan för affärsapplikationer.
* Det finns en brist på kunskap om teknologin bakom Bitcoin.

På den positiva sidan kan Bitcoin gynna vilket företag som helst genom att:

* Läggas till i företagets kassa som en tillgång, antingen genom att mineras direkt eller köpas på den öppna marknaden.
* Använda annars overksamma resurser för att mina Bitcoin åt företaget.
* Ge motivering för investeringar i AI-lösningar som kräver liknande högpresterande datorkraft.
* Lägga till en alternativ betalningsmetod för köp av företagets tjänster eller produkter.
* Minska globala valutaväxlingsavgifter.
* Erbjuda en extra personalförmån genom incitament baserade på Lightning-betalningar.
* Bygga nya intäktsströmmar för företaget baserat på Bitcoin.

Varje IT-chef behöver ta sig tid att förstå Bitcoin, den potentiella påverkan och riskerna som är förknippade med det, samt möjliga fördelar, för att kunna ge vägledning och ledarskap till verksamheten.

> Bitcoin är en anmärkningsvärd kryptografisk prestation. Förmågan att skapa något som inte kan dupliceras i den digitala världen har enormt värde. Många människor kommer att bygga företag ovanpå detta.  
_Eric Schmidt_



#### 5.1.1 Risker och missuppfattningar kring Bitcoin

##### Bitcoin som en del av en större 'krypto'-industri.

Bitcoin var det första lyckade försöket att skapa en ändlig digital tillgång och har gett upphov till en hel industri av 'alt-coins' som försöker använda en del av den underliggande teknologin för att antingen 'förbättra' Bitcoin eller bygga en lösning för att adressera andra potentiella marknadsmöjligheter.

De publika molnleverantörerna har skapat blockkedjeplattformar för att möjliggöra för företag att bygga dessa lösningar, men intresset för dessa tenderar att gå upp och ner i takt med branschens hype, och Microsoft lade faktiskt ner sin blockkedjetjänst 2021.

* Fram till 2017 stod Bitcoin för så mycket som 95 % av det totala marknadsvärdet för krypto.
* Den första vågen av 'alternativa' krypto-ICO:er såg dominansen falla till en rekordlåg nivå på 37,6 %.
* När dessa misslyckades med att leverera verkliga affärsnyttor och började försvinna, började Bitcoins dominans öka igen.
* År 2021, när Bitcoinpriset steg, dök en ny våg av NFT-baserade alternativa lösningar upp på marknaden, vilket återigen pressade ner Bitcoins dominans.
* Efter att även denna hype misslyckades med att leverera verkliga fördelar har Bitcoins dominans börjat stiga igen.
* När och om Bitcoin går in i en ny tjurmarknad är det möjligt att en ny våg av 'alt-coins' dyker upp för att kapitalisera på en ny trend, men de kommer troligen att möta ett liknande öde.

Om verksamheten kommer till IT-chefen med det senaste 'blanka föremålet' som marknadsförs för en viss blockkedjeapplikation, eller som ett alternativ till Bitcoin, är det viktigt att ha denna trend i åtanke och fråga:

* Vad är syftet med blockkedjan?
* Behövs en blockkedja överhuvudtaget, med tanke på dess prestandanackdelar jämfört med en centraliserad relationsdatabas?
* Vem kan ändra protokollet och vad får det för konsekvenser för lösningen?
* Vilka uppoffringar har gjorts för säkerhet eller decentralisering för att uppnå den påstådda prestandan?
* Vilken nytta kan det ge som inte kan levereras med Bitcoin och tillhörande protokoll, såsom Lightning?

##### Konsekvenserna av att driva Bitcoin

Beroende på vilken sektor företaget verkar inom kan det finnas potentiella fördelar med Bitcoin-mining, särskilt där den genererade värmen kan användas till något nyttigt. Det finns dock ofta motstånd på grund av uppfattningen att Bitcoin är dåligt för miljön, slösar energi eller har liten nytta.

Som IT-chef är det nödvändigt att förstå denna dynamik och om det finns potentiella fördelar för företaget för att kunna ge effektiv vägledning. Den allmänna uppfattningen har varit att Bitcoin inte är 'bra för miljön' och 'slösar energi'. Men detta förändras snabbt, fler positiva rapporter publiceras, och det förväntas att narrativet kommer att ändras till att Bitcoin-mining kan ses som positivt för miljön och övergången till förnybara energikällor. Detta är något som många företag fokuserar på i sina ESG-initiativ.

##### Förstå de potentiella riskerna med kryptomining

Det har funnits exempel tidigare där det publika moln som hanteras av ett företag har tagits över av hackare, som snabbt kan aktivera extra datorkraft för att mina krypto. Ju fler resurser som aktiveras med den högsta prestandaprofilen (dyrast), desto bättre chans har hackaren att mina Bitcoin eller annan krypto. Detta kallas 'Crypto-Jacking' – enligt AWS:

'Detta är en typ av cyberbrottslighet som innebär obehörig användning av enheter (edge-datorer, smartphones, surfplattor eller till och med servrar) för att mina kryptovaluta. I takt med att kryptovalutapriserna stiger och kraftfullare edge-enheter med GPU-kapacitet används för att köra maskininlärning vid edge, ökar hotet från cryptojackers som utnyttjar säkerhetsbrister på edge-enheter. När detta händer används edge-datorresurser för att mina kryptovaluta, vilket leder till högre CPU/GPU-användning och försämrad prestanda för edge-applikationer samt ökade inferenstider för ML vid edge.'

Det är därför avgörande att all användning av publika molnresurser är korrekt utformad enligt bästa praxis. Dessa beskrivs vanligtvis i någon form av Cloud Adoption Framework, med rekommendationer kring säkerhet, prestanda, övervakning, motståndskraft och drift. IT-chefen bör säkerställa att dessa följs och att någon form av realtidsövervakning är aktiverad för att identifiera och mildra sådana attacker innan stora kostnader uppstår.

##### Brist på kunskap om teknologin som används av Bitcoin

Det finns många missuppfattningar kring teknologin bakom Bitcoin, vilket leder till frågor om det kan hackas, energin som används, eller om det kommer att ersättas av en ny version som ofta har hänt med teknik. Som teknisk ledare är det användbart att förstå den underliggande teknologin för att kunna positionera Bitcoin korrekt internt och bemöta dessa farhågor.



#### 5.1.2 På den positiva sidan.

##### Bitcoin som en kassatillgång

Det finns potentiella ekonomiska fördelar för ett företag att lägga till Bitcoin i bokföringen som en kassatillgång.

* Värdebevarande och skydd mot inflation
* Minskande förtroende för fiatvalutor som värdebevarare
* Motpartsrisk inom banksektorn
* Försteg för företag som lägger till Bitcoin i sin kassa

Även om de ekonomiska konsekvenserna av detta ur ett redovisningsperspektiv inte är IT-ledarens ansvar, är det däremot viktigt att förstå hur detta kan fungera och hur Bitcoin kan köpas, lagras och säkras.

Det finns tjänster på marknaden som hjälper till att köpa, förvara och erbjuda utlåningstjänster mot de lagrade tillgångarna. Om detta blir en diskussion inom företaget, vilket det bör bli, kan IT-ledaren hjälpa till att kvalificera potentiella tredjepartsföretag som erbjuder dessa tjänster. Noggrann due diligence för att säkerställa att de erbjudna tjänsterna uppfyller nödvändiga säkerhetskrav, transparens och tjänstefunktioner hjälper till att välja en pålitlig partner.

##### Fördelar med Bitcoin-mining

Användningen av datacenter förväntas bara öka i framtiden, och en stor del av kostnaderna för att driva ett datacenter är att avleda den värme som genereras. Detta gäller särskilt för applikationer som använder högpresterande datorkraft, såsom AI/ML och Bitcoin-mining.

Företag i olika sektorer globalt har identifierat hur denna ökade värmeproduktion kan bli en nettofördel för verksamheten istället för en kostnad genom att använda den genererade värmen till:

* Simhallar/spa
* Simanläggningar
* Odling av blommor/grönsaker i växthus
* Uppvärmning av företagets egna lokaler och varmvattenberedning

Detta kan uppnås antingen genom att samarbeta med ett Bitcoin-miningföretag som använder företagets lokaler för att mina Bitcoin mot vinst och tillhandahåller värmen för allmänt bruk, eller

att företaget själv utför denna funktion för att bygga upp en egen Bitcoin-kassa direkt. Detta tillvägagångssätt kan också hjälpa ett företag med eventuella ESG-initiativ.

En mer indirekt metod för att få några av dessa fördelar kan uppnås genom att flytta datorkrav till datacenter som använder detta tillvägagångssätt och erbjuder rackutrymme eller infrastruktur som en del av en hanterad tjänst och som vidarebefordrar en del av dessa kostnadsbesparingar till företaget.

Som IT-ledare kommer du genom att hålla dig uppdaterad inom detta område kunna ge vägledning till företaget vid införandet av lösningar som kan gynna verksamheten.

##### Bitcoin och AI

Användningen av AI och ML förväntas öka kraftigt de kommande åren. Skärningspunkten mellan Bitcoin och artificiell intelligens leder till en ny era av digital innovation, särskilt genom integrationen av AI med Bitcoins Lightning-nätverk. Denna förening är på väg att revolutionera delar av internet, från mikrobatalningar till AI-drivna ekonomiska agenter online.

* Finjustering av AI-modeller är ett viktigt steg i AI-utveckling – mikrobatalningar via Lightning kan möjliggöra att individer världen över får betalt per uppgift i Bitcoin, vilket uppmuntrar till deltagande.
* I scenarier där AI-enheter transagerar för tjänster är Lightning-nätverket ett oumbärligt verktyg för AI-drivna ekonomiska aktiviteter där hastighet är avgörande.
* När AI-systemet väl är utvecklat kan mikrobatalningar möjliggöra en mer rättvis betalning-per-användning-modell där användare bara betalar för de AI-resurser de faktiskt använder.

För alla företag som överväger att använda AI, antingen som en tjänst de behöver betala för eller i utvecklingen av en egen AI-lösning, är det viktigt att förstå hur Bitcoin och Lightning integreras i och tillför värde till varje lösning.

Källa: [https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/](https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/)

##### Nya betalningsalternativ för detaljhandeln

Alla företag som tar emot betalningar för tjänster, antingen direkt i butik eller online, kan dra nytta av att acceptera Bitcoin-betalningar på följande sätt:

* Ökad kundtillströmning och affärstillväxt genom att rikta sig till Bitcoin-kunder
* Låga till inga betalningsavgifter
* Omedelbar avräkning
* Inga återbetalningar (chargebacks)

Ur ett redovisningsperspektiv finns det olika sätt att hantera de Bitcoin som tas emot, att behålla dem som en del av kassan eller att direkt konvertera till fiat, eller någon kombination enligt överenskommelse. Beroende på verksamheten kan det finnas vissa tekniska implikationer för att uppnå detta, såsom nya POS-terminaler eller integration med en mjukvarulösning för onlinebetalningar, vilket IT-ledaren behöver förstå de tekniska konsekvenserna av om det beslutas som ett mål för företaget.

##### Minska globala valutaväxlingsavgifter

För företag som överför stora summor pengar globalt kan kostnaderna och komplexiteten ofta vara utmanande. Nya lösningar baserade på Bitcoin erbjuds på marknaden som minskar dessa kostnader och ger snabbare och omedelbar avräkning. Att anta dessa tjänster kan potentiellt vara till nytta för företaget, och att ha förståelse för denna marknad, de erbjudna tjänsterna och att arbeta med ekonomiavdelningen för att implementera den bästa lösningen kräver en viss teknisk kunskap och förståelse som IT-ledaren kan bidra med.

##### Personal­förmåner

De flesta företag undersöker hur de kan erbjuda förmåner och incitament till sina anställda för att förbättra rekrytering och behålla personal. Nyligen har flera välkända professionella idrottare och politiker meddelat att de tar ut hela eller delar av sin lön i Bitcoin. Möjligheten att betala delar av lönen i Bitcoin kommer att vara viktig för arbetsgivare när det börjar bli avgörande vid nyckelrekryteringar, eller när kärnmedarbetare börjar efterfråga detta eller söker sig till arbetsgivare som erbjuder det på annat håll.

* Att integrera möjligheten till hel- eller dellön i Bitcoin ger en organisation ett konkurrensförsprång och hjälper dem att ligga steget före. Bitcoin-löne­lösningar gör det enkelt att integrera denna process.
* Företag som MicroStrategy undersöker sätt att belöna prestation eller till och med närvaro vid möten med mikrobatalningar via Lightning.

Även om beslutet att införa sådana förmåner för anställda inte ligger direkt hos IT-ledaren, kan det vara deras ansvar att förklara varför detta kan vara fördelaktigt, vilka lösningar som finns och de tekniska konsekvenserna av implementeringen. IT-direktörer som proaktivt lyfter idéer till kollegor kan visa sitt bredare strategiska värde för verksamheten.

##### Nya marknadsmöjligheter

Som citatet från Google visade kommer många företag att vilja bygga nya intäktsströmmar baserat på det växande Bitcoin-ekosystemet. Detta kan öppna nya marknader för företaget att överväga, där IT-ledaren kan vara avgörande för att utvärdera lämplighet, tekniska utmaningar och potentiella möjligheter dessa kan erbjuda.



#### 5.1.3 Sammanfattning

Bitcoin förväntas fortsätta sin resa mot ökad adoption och bli allt viktigare för företag över tid, vilket påverkar både affärs- och tekniska strategier samt initiativ inom flera områden. Som teknisk ledare för företaget kommer IT-ledaren att gynnas av att ligga steget före i dessa utvecklingar, ge vägledning till företaget och säkerställa att det får största möjliga nytta av att implementera Bitcoin-lösningar i hela organisationen.
