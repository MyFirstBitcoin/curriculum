# 2.7 Bitcoin är inte riktigt decentraliserat

> Kryptons komplexitet uppstår från försöken till decentralisering—genom att sprida makt och styrning i systemet finns det teoretiskt sett inget behov av betrodda mellanhänder som finansiella institutioner. Det var utgångspunkten i det ursprungliga Bitcoin-whitepaper, som erbjöd en kryptografisk lösning avsedd att möjliggöra betalningar utan att involvera någon finansiell institution eller annan betrodd mellanhand. Dock blev Bitcoin snabbt centraliserat och är nu beroende av en liten grupp mjukvaruutvecklare och miningpooler för att fungera  
_Internationella valutafonden_

Som citatet ovan från ett ganska nyligt inlägg av Internationella valutafonden visar, fortsätter den traditionella finansindustrin att hävda att Bitcoin inte är decentraliserat, samt förväxlar Bitcoin med andra krypto-tillgångar.

##### Introduktion

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/bcd27cfd513dc9f99096e0a08882278fb6e080b5-161x167.svg)

Decentralisering är en avgörande aspekt av Bitcoin. Förmågan att upprätthålla protokollets regler såsom knapphet och distribution utan en central myndighet säkerställer att det kan fungera som tillståndslösa pengar för ett globalt samhälle.

Som Satoshi noterade i sin korrespondens online, stod decentraliserade tjänster som BitTorrent ‘på egna ben’ mot statliga nedslag, i jämförelse med tjänster med identifierade ägare och centraliserade servrar. Han var tydligt oroad över den potentiella risken att regeringar eller andra intressen skulle stänga ner eller på annat sätt negativt påverka Bitcoin.

I detta sammanhang är vi intresserade av decentralisering av:

* Utvecklingen och hanteringen av koden som kör protokollet; vem får ändra reglerna?
* Miningfunktionen som skapar nya block enligt reglerna och validerar mot dubbelspendering
* Noderna som validerar transaktioner för giltighet och håller en kopia av blockkedjan

##### Utvecklare

Bitcoin är ett öppen källkodsprotokoll som vem som helst fritt kan granska, ladda ner, kopiera eller föreslå ändringar till. Det finns tillgängligt i ett GitHub-bibliotek, där källkoden ursprungligen lanserades 2009 av Satoshi Nakamoto. Vem som helst kan ladda ner koden och köra en nod, varav de flesta kör den ursprungliga Bitcoin Core-mjukvaran, som har uppdaterats över tid.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Källa: https://river.com/learn/what-is-bitcoin-core/_

Utvecklingen av Bitcoin Core följer bästa praxis för öppen källkodsutveckling. När som helst kan ett valfritt antal utvecklare skriva eller granska kodändringar. De behöver lyssna på synpunkter från nodoperatörer och miners, samt användarbasen innan någon kritisk ändring görs i koden, som kommer att granskas och godkännas enligt flödesschemat ovan innan de införs i koden.

Reglerna för Bitcoin är sedan kodade i denna Bitcoin Core-mjukvara, som körs på varje nod. Vem som helst kan föreslå en ändring av reglerna – reglerna är kod, men de är inte_bara_kod, de är_överenskommen_kod. Om de ändras ensidigt är den nya koden inte längre en del av konsensus och är inte längre en del av Bitcoin. Att ändra något med Bitcoin och ändå förbli i konsensus är svårt. Föreslagna ändringar av koden faller i en av tre kategorier:

* Inom befintliga regler: Mindre uppgraderingar som stavfel, snyggare användargränssnitt eller databehandling kan falla inom denna kategori och är relativt enkla att få godkännande för.
* Att lägga till en ny regel som lägger till restriktioner till reglerna – till exempel att minska blockstorleken. Detta kallas en ‘mjuk gaffel’ (soft fork). Noder som väljer att inte implementera kodändringen och stannar på den gamla versionen kan fortfarande delta i nätverket.
* Att lägga till en ny regel som bryter mot de nuvarande reglerna, t.ex. en ökning av blockstorleken. Noder som inte uppgraderar till den nya koden kommer att avvisa ett block som skapats i den större storleken som ogiltigt. Detta kallas en ‘hård gaffel’ (hard fork) och skapar en kedjedelning mellan noder som kör den ursprungliga och nya koden och skapar en ny coin. Detta har hänt tidigare men har inte lett till någon långsiktig framgång för den nya coinen eftersom majoriteten av noderna valde att hålla sig till den ursprungliga koden.

Därför kan en enskild part eller grupp av personer inte ensidigt ändra Bitcoin-koden utan att uppnå konsensus, annars riskerar de en kedjedelning och skapandet av en ny coin med ett annat regelverk.

##### Mining

Miningfunktionen validerar transaktionerna precis som vilken annan nod som helst i nätverket, men den kommer sedan att använda den energi som krävs för att skapa ett nytt block som uppfyller konsensusreglerna i koden. Lyckas man får minern belöningar i form av transaktionsavgifter och Bitcoin-belöningar (vid skrivande stund 3,125 coins per block).

Mining utförs normalt av miningpooler där personer slår ihop sin miningkraft eller hash rate för att öka chansen att lyckas mina ett block och dela på belöningarna. Det finns en risk att en eller flera av dessa miningpooler skulle kunna gå ihop för att uppnå 51 % dominans i mining och i princip överrösta nätverkets valideringsprotokoll till sin fördel för att dubbelspendera coins. Detta skulle kräva enorma resurser till stor kostnad, och enskilda miners kan mycket enkelt byta till en annan miningpool när som helst. En sådan attack skulle troligen också få värdet på bitcoin att kollapsa, eftersom det skulle vara uppenbart att nätverkets integritet hade komprometterats. En angripare skulle därför behöva konvertera alla bitcoin som erhållits snabbt till fiat innan värdet urholkas. Detta skulle göra det ännu svårare att upprätthålla en attack under lång tid, och därför är det mer lönsamt för en miner eller pooloperatör att följa reglerna och försöka mina giltiga block.

Den geografiska spridningen av miningfunktionen är också viktig för att undvika att exempelvis regeringar tar över miningkapacitet eller stänger ner den. Till exempel visade ett nyligt förbud mot mining i Kina Bitcoins förmåga att anpassa sig och överleva sådan statlig inblandning, och nätverket återhämtade sig snabbt från den resulterande förlusten av hashkraft.

##### Noder

Till skillnad från mining, som kräver en betydande ekonomisk investering för att effektivt kunna tävla om att mina nya block, eller kodutveckling som kräver kodningskompetens, är det att köra en nod något som vem som helst som är intresserad av att hjälpa till att upprätthålla Bitcoins decentralisering kan göra.

Noder kör Bitcoin Core-mjukvaran och upprätthåller de regler som koden innehåller för att säkerställa att miners inte fuskar, till exempel genom att ge sig själva en större blockbelöning än vad som är tillåtet. De upprätthåller också 21 miljoner-taket för utbudet, vilket är avgörande för att bevara Bitcoins knapphet. För att någon regering eller illasinnad aktör ska kunna stoppa Bitcoin, skulle de behöva förstöra varje enskild kopia av blockkedjan, som för närvarande körs på tusentals noder globalt, en nästintill omöjlig uppgift.

##### Människor

En annan aspekt av potentiell centralisering är människor. Varje annan ‘alt-coin’ har en frontfigur—någon som potentiellt kan tvingas att förespråka förändringar som inte är till Bitcoins bästa. Satoshi Nakamoto stannade kvar tillräckligt länge för att säkerställa att Bitcoin var på väg mot framgång innan han försvann för gott, och lämnade det i andras händer att förbättra och anpassa mjukvaran.

Hur är det med innehavare av stora mängder Bitcoin? Tidiga investerare, som har behållit sina coins och inte förlorat dem, är nu extremt förmögna. Det är viktigt att notera att detta mycket väl kan vara fallet, men det ger dem inte mer inflytande över systemet än någon annan, till skillnad från ‘proof of stake’-coins där de tidiga användarna som redan är rika på den coinen får fördelar i beslutsfattande och distribution av framtida coins. Detta har eller kommer oundvikligen att leda till centralisering över tid.

##### Slutsats

Vilka är de potentiella hot som decentralisering kan försöka motverka?

* Regeringar som stänger ner eller förbjuder Bitcoin
* Oönskade ändringar i koden som gynnar ett intresse i Bitcoin, t.ex. att öka blockbelöningen
* Påverkan av protokollet av regeringar eller illasinnade aktörer för att styra protokollets riktning
* Möjlighet för en miningpool att ta över nätverket och ‘dubbelspendera’ Bitcoin – en 51 %-attack

Som vi kan se decentraliserar kombinationen av noder, kodutvecklare och miners, samt användningen av ‘proof of work’-mekanismen, Bitcoin till en tillräcklig nivå där dessa potentiella hot inte anses vara av stor oro. Gemenskapen måste fortsätta att övervaka situationen för att säkerställa att det förblir så.
