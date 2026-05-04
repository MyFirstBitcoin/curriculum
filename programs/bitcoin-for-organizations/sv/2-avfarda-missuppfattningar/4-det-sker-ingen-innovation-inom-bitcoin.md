# 2.4 Det sker ingen innovation inom Bitcoin

> Skapandet av tusen skogar finns i ett enda ekollon.   
_Ralph Waldo Emerson_

Kritiker försöker ofta hävda att Bitcoin är 'gammal' eller 'död' teknologi eftersom dess grundläggande protokoll inte förändras lika ofta som konkurrerande blockkedjor. Detta påstående bortser både från varför förändringar i Bitcoin införs långsamt och från den mängd innovation som sker för att skala nätverket på högre lager, såsom Lightning Network. Det ignorerar också att många av våra mest flexibla och hållbara teknologier inte heller utvecklas snabbt på grundnivån.

Till exempel sker det ingen innovation i Transmission Control Protocol (TCP), som ligger till grund för internet. TCP skapades först 1974. Senast TCP uppdaterades var 1982. Det gör det som behövs. Det är inte perfekt, och det finns debatter om vi behöver uppgradera IPv4 för att stödja framtida internetutveckling. Men att påstå att det inte har skett någon innovation på internet sedan 1982 vore ett anmärkningsvärt påstående. All denna innovation har skett 'på' TCP, snarare än 'i' det.

Den stora majoriteten av innovationen sker inte 'i' Bitcoin utan 'på' Bitcoin. En dag kommer det troligen inte ske någon innovation 'i' Bitcoin, och det bör vara ett mål och inte en kritik, eftersom det skulle spegla hur grundläggande det har blivit för att stödja den globala ekonomin genom att tillhandahålla grunden för globalt, neutralt och tillståndslöst sund valuta. Pengar som är sunda både i ekonomisk mening, eftersom det finns en fast tillgång och en oföränderlig huvudbok, men också sunda i teknisk mening eftersom det inte förändras och det som körs har haft år av oavbruten drifttid. Bitcoin har redan uppnått 100% drifttid under de senaste 10 åren.

Det vore dock oroande om det inte skedde någon innovation 'på' Bitcoin. Låt oss titta på det under de senaste 10 åren:



#### 'I' Bitcoin

Segregated Witness (SegWit) implementerades 2017 för att skydda mot transaktionsföränderlighet och för att öka blockkapaciteten. SegWit var också en nödvändig föregångare för att lightning och vissa sidokedjor skulle fungera effektivt.

Taproot implementerades 2021 för att möjliggöra batchning och validering av flera signaturer genom att införa Schnorr-signaturer, introducera ett skriptspråk för mer komplex funktionalitet och öka integriteten och censurmotståndet för transaktioner.



#### 'På' Bitcoin

##### Liquid Sidechain

Liquid sidechain implementerades 2018. Liquid, liksom andra sidokedjor, är en separat blockkedjehuvudbok som är kopplad till den huvudsakliga Bitcoin-blockkedjan enligt ett fördefinierat regelverk. Dessa regler är tillräckligt flexibla för att tillåta Liquid-kedjan att utvecklas och införliva design- och skalbarhetsförbättringar över tid. Men kopplingen till Bitcoin-blockkedjan säkerställer att det totala utbudstaket på 21 miljoner bitcoin är konsekvent över båda kedjorna.

Tillgången i Liquid, L-BTC, är tvåvägsbunden till bitcoin på huvudkedjan. Det finns avvägningar mellan kostnad, hastighet, integritet och säkerhet som gör L-BTC idealisk för vissa tillämpningar. Kostnad, hastighet och integritet förbättras alla med L-BTC, på bekostnad av att man måste lita på de organisationer som utgör Liquid Federation, vilka tillsammans kontrollerar en 11 av 15 multisig-process för att växla in och ut L-BTC till bitcoin och vice versa.

##### Lightning Network

Lightning-nätverket implementerades 2018. Lightning är utformat som ett peer-to-peer-betalningsnätverk i form av en graf av noder som är sammankopplade via kanaler; det är inte en blockkedja. Bitcoin låses av en nodoperatör på huvudblockkedjan för att göra den tillgänglig för användning på Lightning Network, vilket säkerställer att endast 'riktig' bitcoin används. Noder kan sedan öppna likviditetskanaler via multisig smarta kontrakt med varandra. Betalningar hittar vägar genom nätverket från källa till destination, optimerat för kostnad mot kravet att tillräcklig likviditet finns i rätt riktning mellan varje nodsteg på vägen. Lightning Network förbättrar kostnad, hastighet och integritet avsevärt i utbyte mot en förlust av säkerhet (eller ökat förtroende som krävs) och ökad komplexitet. Det är dock avsett för högvolym, lågvärdesbetalningar i vardagen, så detta anses vara en mycket rimlig kompromiss för dess miljontals dagliga transaktioner (källa: River, 2023).

##### Chaumian eCash-mynt

Fedimints kan ses som ett gemenskapsbegränsat lightning-nätverk. De är utformade för att utnyttja det inneboende förtroende som finns inom vissa gemenskaper (t.ex. familjer, byar, vänskapsgrupper) i utbyte mot att förenkla komplexiteten och öka integriteten för användarna. De är modulära, öppen källkodsprotokoll för att förvara och transaktera bitcoin i ett gemenskapssammanhang. De är interoperabla med själva Lightning Network.

**Cashu** är ett innehavar-token som kan lagras på en enhet såsom en mobiltelefon; designen syftar till att återskapa fördelarna med fysiska kontanter men i digital form. Cashu är ett exempel på Chaumian eCash byggt på Bitcoin och ökar integritet och censurmotstånd samt minskar komplexitet i utbyte mot att man litar på den eCash-mynt som används. Cashu-mynt utfärdar eCash-tokens, som representerar bitcoin, och dessa kan spenderas av användare utan att avslöja deras identitet. Cashu är interoperabelt med Lightning Network.

Det kommer sannolikt att byggas många fler lager 2-applikationer i framtiden, med många lager 3-applikationer som i sin tur byggs ovanpå var och en av dessa.

Som ett exempel på det otroliga antalet applikationer som byggs ovanpå Lightning, här är ett utdrag från en Lightning Network Research Report av River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
