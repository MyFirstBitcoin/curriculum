# 8.2 Mått för att analysera huvudboken

Eftersom Bitcoins transparens skiljer sig från traditionella finansiella system – där mycket av penningflödet sker bakom stängda institutionella dörrar – uppstår ett rikt område av on-chain-analys, där data på nätverksnivå blir ett verktyg för att förstå användarbeteende, penningflöden och långsiktiga trender. Dessa mätvärden kan hjälpa till att besvara specifika frågor, såsom hur aktivt nätverket används, om mynt ackumuleras eller säljs av, och om nätverket blir säkrare.

Att förstå dessa mätvärden är användbart inte bara för Bitcoin-användare, utan även för forskare eller beslutsfattare som söker insikt i detta unikt transparenta finansiella system.

Detta avsnitt innehåller några vanliga mätvärden för att analysera Bitcoin-aktivitet, grupperade i underkategorier. Det är inte en fullständig lista. Besök [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) för en mer komplett lista och beskrivningar.



#### 8.2.1 Adressmätvärden

Adressmätvärden är användbara att följa över tid eftersom de indikerar aktivitetsnivån på Bitcoin-nätverket. Till exempel, när Bitcoin blir mer använt ökar antalet aktiva adresser. Vi kan undersöka detta vidare genom att särskilja antalet adresser som innehar en viss minsta mängd Bitcoin, säg 0,1 BTC, under en viss tidsperiod, till exempel ett år. Även om detta ger en bild av Bitcoins adoption över tid är det inte perfekt, eftersom en individ kan ha flera Bitcoin-adresser. Omvänt kan börser eller ETF:er framstå som enskilda enheter när de håller medel för många individer.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adresser som hodlar Bitcoin > X BTC per år. Källa: Bitcoin Magazine Pro._

Genom att jämföra adresser med det aktuella marknadspriset på BTC är det möjligt att se andelen av alla Bitcoin-adresser som ligger på vinst. Detta gör att vi kan följa marknadssentimentet, eftersom vi kan se vilken andel av marknaden som håller BTC med vinst eller förlust.

Till exempel visar **Procent orealiserad vinst** diagrammet nedan andelen av alla adressers saldo med orealiserad vinst mätt i amerikanska dollar. Observera att eftersom diagrammet nedan togs nära Bitcoins högsta notering någonsin, är andelen adresser med orealiserad vinst nära hundra procent. Vi kan också se att långvariga perioder med Procent orealiserad vinst under en standardavvikelse från medelvärdet är ovanliga. Därför kan ett fall under denna linje antyda en bra ingångspunkt för köpare.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Procent orealiserad vinst. Källa: checkonchain.com_



#### 8.2.2 On-chain-indikatorer

On-chain-indikatorer är användbara eftersom de ger insikt i nätverksbeteende, utöver vad pris- och adressmätvärden ensamma kan visa. De hjälper analytiker att förstå handlingar och sentiment hos olika typer av deltagare, såsom långsiktiga innehavare jämfört med kortsiktiga handlare, genom att följa hur mynt hålls, flyttas eller värderas över tid. Dessa indikatorer drar nytta av den transparenta huvudboken för att avslöja dolda marknadsdynamiker som ackumulering, distribution eller till och med investerarövertygelse. Detta gör dem särskilt användbara för att identifiera strukturella trender, bedöma om marknaden är överhettad eller undervärderad, och förutse vändpunkter i en marknadscykel.

Till exempel, genom att undersöka värdet av BTC-innehav sedan de senast transakterades, kan vi dra slutsatser om marknaden är under stress (som den kan vara under en större cykelbotten). Denna mätning kallas **Realiserat pris** och ger oss ett 'genomsnittligt anskaffningsvärde' för all BTC i omlopp. Om marknadspriset faller under Realiserat pris visar det att majoriteten av adresserna sammantaget håller en pappersförlust.

Genom att ytterligare gruppera huvudboksdata i åldersband kan vi visa hur mängden BTC rör sig mellan adresser över tid, vilket skapar vågliknande mönster i ett diagram som kallas **HODL-vågor**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL-vågor. Källa: Bitcoin Magazine Pro._

HODL-vågorna visar vad långsiktiga, medellånga och kortsiktiga innehavare gör med sin BTC. Till exempel, i diagrammet ovan visas kortsiktiga innehavare i rött och orange och vi kan se toppar i aktivitet när denna grupp rusar för att köpa nära marknadstoppar. I andra änden ser vi att mycket långsiktiga innehavare (i lila och blått) stadigt ökar sin andel av nätverket, vilket indikerar hög övertygelse bland dessa grupper. Diagrammet är inte perfekt eftersom vissa mynt kan flyttas från gamla till nya adresser under samma användares kontroll. Det ger dock en intressant inblick i långsiktiga innehavares övertygelse.

Ett annat sätt att undersöka 'smart money' hos långsiktiga innehavare är att titta på **Coin Days Destroyed** (CDD). Begreppet 'Coin Days' är antalet BTC multiplicerat med antalet dagar sedan mynten senast flyttades. Till exempel, 5 BTC som inte har rört sig på 100 dagar har ackumulerat 500 coin days och 10 BTC som inte har rört sig på 10 dagar har ackumulerat 100 coin days. På så sätt ger vi extra vikt åt mynt som hålls längre. När dessa mynt flyttas 'förstörs' dessa coin days. Denna indikator visar ökningar i CDD vid betydande prisrörelser, vilket ger analytiker ett sätt att särskilja rutinmässig marknadsaktivitet från meningsfulla förändringar i långsiktiga innehavares sentiment.

Ett annat mått som kan hjälpa till att identifiera om marknaden undervärderar eller övervärderar BTC är Market-Value to Realised Value eller **MVRV**. Det beräknas helt enkelt som förhållandet mellan marknadsvärde (antalet BTC i omlopp multiplicerat med marknadspriset) dividerat med realiserat värde (summan av all BTC sedan de senast flyttades). Ett högt MVRV tyder på att fler mynt är på vinst (ofta sett nära marknadstoppar) och ett lågt MVRV indikerar att många mynt hålls med förlust (sett nära marknadsbottnar).



#### 8.2.3 Gruvdriftsmätvärden

Gruvdriftsmätvärden är användbara för att förstå säkerheten, de ekonomiska incitamenten och den övergripande hälsan i Bitcoin-nätverket. Mätvärden som hashrate, gruvarbetarnas intäkter, svårighetsgrad och avgiftsförhållanden visar hur mycket datorkraft som säkrar blockkedjan och hur väl gruvarbetarna kompenseras för sina aktiviteter.

Den **Hashrate** för Bitcoin-nätverket är kanske den mest refererade indikatorn på nätverkets hälsa och säkerhetsstyrka. Eftersom gruvdriftprocessen säkrar nätverket och bekräftar att transaktioner på huvudboken är giltiga, gäller att ju högre datorkraft (eller hashkraft) som finns, desto svårare blir det för en illasinnad aktör att övermanna och attackera nätverket.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Källa: Bitcoin Magazine Pro._

Diagrammet ovan visar att nätverkets totala datorkraft i maj 2025 ligger på cirka 900 TeraHash/s (900 biljoner kryptografiska 'hash'-beräkningar per sekund). Om hashraten stiger visar det att nätverket blir säkrare, vilket är lugnande för användare.

Puell-multipeln (utvecklad av David Puell) ser på marknadscykeln ur gruvarbetarnas och deras intäkters perspektiv. Måttet beräknas genom att dela den dagliga utgivningen av BTC (i USD) med det 365-dagars glidande medelvärdet av dagligt utgivningsvärde. Måttet hjälper till att identifiera perioder av stress eller lättnad för gruvarbetare. Historiskt har en multipel över 3 föregått en nedgång i BTC:s marknadsvärde, eftersom det indikerar att gruvarbetarna är mycket lönsamma. Ett värde under 0,5 indikerar stress och har historiskt markerat marknadsbottnar för BTC:s värde.
