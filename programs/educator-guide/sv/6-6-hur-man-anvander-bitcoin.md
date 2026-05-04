# 6 - Hur man använder Bitcoin

Tidsåtgång: 90 minuter

Kärnidé: Att använda Bitcoin on-chain lär eleverna hur ägande, egen förvaring och verifiering fungerar i praktiken, och förvandlar teori till direkt finansiell handling.

#### Lärandemål

Efter denna lektion ska eleverna kunna:

* Identifiera vanliga sätt att skaffa och byta bitcoin, inklusive person-till-person och centraliserade börsmetoder.
* Förklara skillnaden mellan egenförvaltade och förvaltade plånböcker, och varför egen förvaring är viktigt i Bitcoin.
* Beskriva syftet med privata nycklar, publika adresser, seed phrases och plånboksgränssnitt.
* Jämföra olika plånbokstyper och utvärdera deras kompromisser utifrån säkerhet, bekvämlighet, integritet och kontroll.
* Installera en mobil Bitcoin-plånbok och förklara den grundläggande återställningsprocessen.
* Visa hur man tar emot och skickar en on-chain bitcoin-transaktion.

Tillämpa principen "Don't Trust, Verify" vid val av plånbok, transaktioner och bredare användning av Bitcoin.

#### Verktyg & Resurser

##### Visuella hjälpmedel

* Kapitel 6 - Hur man använder Bitcoin

##### Stödbibliotek

* Ordkortsreferens — Kapitel 6 — Termer: plånbok, privat nyckel, publik adress, seed phrase, förvaltad, egenförvaltad, UTXO, transaktionsavgift
* Jämförelsediagram & referensblad — Jämförelse av plånbokstyper (förvaltad, mobil, hårdvara, papper)
* Tekniska förklaringar & fördjupningar — Publika/privata nycklar, UTXO-modell, transaktionsbekräftelse
* Fördjupning i privat nyckelsäkerhet — Seed phrases, nyckelderivering, backupmetoder, attackvektorer
* Transaktionsanatomiguide — Steg-för-steg-exempel på hur en Bitcoin-transaktion fungerar
* Checklista för bästa säkerhetspraxis — Innan du börjar, skapa plånbok, ta emot, skicka, förebygga phishing

#### Aktiviteter

* Transaktioner i praktiken
* Lightning-stafetten
* Utforska mempoolen

#### Undervisning online

* Var tydlig från början om eleverna tittar på en demonstration eller själva ska installera en plånbok.
* Använd stora, tydliga skärmdumpar för varje steg i plånboksinstallationen.
* Pausa efter varje steg och be eleverna bekräfta förståelsen i chatten innan ni går vidare.
* Ge en tydlig varning innan seed phrase-avsnittet och påminn eleverna om att aldrig dela känslig information online.

#### Förberedelser

* Ladda ner och testa en mobil plånboksapp (Blue Wallet eller Muun); förbered skärmdumpar av viktiga installationssteg.
* Förbered en guide för plånboksinstallation (ladda ner → skapa → säkerhetskopiera seed → ta emot) som referens.
* Säkerställ att nätverket/WiFi fungerar; ha en demo-adress och QR-kod redo att visa.

#### Genomförande

Denna lektion går från teori till direkt praktik. Den matchar nu Diplomastrukturen direkt så att förvärv, plånböcker, installation, transaktioner och verifiering ligger under samma huvudrubriker som elevguiden. Extra lärarstöd finns kvar inbäddat i dessa avsnitt.

##### 6.0 Introduktion, 8 minuter

Börja med att koppla detta kapitel till det föregående:

* Om Bitcoin är pengar, hur får och använder folk det egentligen?
* Vad innebär det att verkligen kontrollera sina bitcoin?
* Varför är det annorlunda att använda Bitcoin jämfört med en bankapp?

Förtydliga att detta kapitel handlar om praktisk användning. Eleverna lär sig inte längre bara vad Bitcoin är, utan hur de interagerar med det direkt.

##### 6.1 Att skaffa och byta Bitcoin, 12 minuter

Förklara att man kan skaffa bitcoin på olika sätt, bland annat:

* få betalt i bitcoin
* mining av bitcoin
* växla fiat mot bitcoin personligen
* växla fiat mot bitcoin online

Fokusera sedan på de två huvudsakliga sätten att skaffa bitcoin som tas upp i kapitlet:

* person-till-person, i verkliga livet
* peer-to-peer, online
* centraliserade börser

Gör kompromisserna tydliga.

För P2P i person, betona direkt utbyte utan bank eller mellanhand, men nämn också de praktiska riskerna med att träffa personer för kontantaffärer.

För P2P online, förklara escrow på ett enkelt sätt, som ett sätt att minska motpartsrisk samtidigt som det möjliggör direkt utbyte mellan parter.

För centraliserade börser, var tydlig med att de är bekväma, men att de kräver att användaren litar på ett företag, ofta delar personlig information och lämnar medel under tredjeparts kontroll tills de tas ut. Här är det bra att förstärka att bekvämlighet ofta innebär kompromisser med integritet och självbestämmande.

##### 6.2 En introduktion till Bitcoin-plånböcker, 35 minuter

**Vad en Bitcoin-plånbok egentligen är**

Klargör ett vanligt missförstånd direkt: bitcoin lagras inte i plånboksappen som fysiska kontanter i en väska.  
Bitcoinen existerar på huvudboken som nätverket underhåller. Det användaren kontrollerar är möjligheten att spendera dem genom privata nycklar.

Förklara sedan de två saker som folk ofta menar med "plånbok":

* det privata nyckelsystemet, från vilket adresser genereras
* appen eller gränssnittet som används för att interagera med nätverket

Använd kapitlets e-postanalogi om det är hjälpsamt:

* offentlig adress = som en e-postadress du kan dela
* privat nyckel = som ett lösenord du måste skydda

Var mycket tydlig här: den som kontrollerar de privata nycklarna kontrollerar bitcoinen. Det är det centrala konceptet som eleverna måste förstå.

**Självförvaring vs förvaringsplånböcker**

Detta är en av de viktigaste delarna av kapitlet.

Förklara skillnaden tydligt:

* Självförvaringsplånbok: användaren kontrollerar de privata nycklarna
* Förvaringsplånbok: en tredje part kontrollerar de privata nycklarna åt användaren

Gå sedan igenom kompromisserna:

Självförvaring

* full kontroll över medlen
* ingen godkännandeprocess
* skydd mot godtyckligt beslagtagande
* större ansvar
* ingen enkel återställning om fröfrasen tappas bort

Förvaring

* enklare återställning och support
* enklare för nybörjare
* mer utsatt för kontofrysningar, hack och tredjepartskontroll
* användaren håller inte egentligen bitcoinen

Detta är rätt tillfälle att betona frasen:

"Not your keys, not your coins."

Eleverna ska lämna detta avsnitt med förståelse inte bara för slagordet, utan vad det faktiskt innebär i praktiken.

**Olika typer av plånböcker och hur man väljer en**

Introducera de plånbokstyper som tas upp i kapitlet:

* onlineplånbok
* mobilplånbok
* datorplånbok
* hårdvaruplånbok
* pappersplånbok

Behandla inte någon som perfekt. Förklara istället att varje typ innebär kompromisser mellan:

* säkerhet
* integritet
* bekvämlighet
* kompatibilitet
* avgifter
* kontroll
* anseende

Gör också tydligt att vi rekommenderar att vara uppmärksam på om plånboksprogramvaran är öppen källkod, eftersom verktyg med öppen källkod kan granskas, revideras och vidareutvecklas av gemenskapen. Detta hänger direkt ihop med principen om verifiering i Bitcoin.

##### 6.3 Installera en mobil Bitcoin-plånbok, 10 minuter

Gå igenom den grundläggande processen som visas i kapitlet tillsammans med eleverna:

* ladda ner plånboken
* skapa en ny plånbok
* generera och skriv ner återställningsfrasen
* bekräfta återställningsfrasen
* lägg till extra säkerhet om det finns tillgängligt
* öppna plånboken och hitta funktionen för att ta emot

Gör varningen om seed phrase (återställningsfras) mycket tydlig:

* om återställningsfrasen tappas bort kan tillgången till pengarna gå förlorad
* om någon annan får tag på återställningsfrasen kan de ta pengarna

Om eleverna gör detta praktiskt bör läraren pausa vid varje steg och kontrollera att alla förstår vad de gör. Om lektionen är mer teoretisk kan detta avsnitt förklaras som en genomgång istället för att utföras live. Återställningsalternativet som visas i kapitlet är också användbart för att förklara att plånböcker kan återställas om återställningsfrasen har säkerhetskopierats korrekt.

##### 6.4 Ta emot och skicka transaktioner, 17 minuter

**Ta emot och skicka transaktioner på blockkedjan**

Förklara nu hur transaktioner på blockkedjan fungerar.

För att ta emot bitcoin:

* öppna plånboken
* tryck på ta emot eller sätt in
* kopiera adressen, dela länken eller visa QR-koden

För att skicka bitcoin:

* öppna plånboken
* klistra in eller skanna mottagarens adress
* ange beloppet
* dubbelkolla alla uppgifter
* skicka transaktionen
* vänta på bekräftelse

Gör dessa nyckelpunkter tydliga:

* transaktionen överför äganderätt, inte fysiska mynt
* transaktioner är oåterkalleliga
* noder verifierar giltighet
* minare inkluderar transaktioner i block
* avgifter påverkar bekräftelseprioritet
* transaktioner på blockkedjan är generellt säkra, men långsammare och ofta dyrare än Lightning-transaktioner

Flödesschemat för transaktioner i kapitlet är särskilt användbart här, eftersom det hjälper eleverna att visualisera vägen från plånboksbegäran till nätverksbekräftelse.

**Transaktioner i praktiken och rollbaserad övning**

Använd den samarbetsövning som beskrivs i kapitlet för att förstärka förståelsen. Förklara de fyra rollerna som är inblandade:

* avsändare
* mottagare
* minare
* nodoperatör

Ett enkelt sätt i klassrummet är att tilldela roller och gå igenom en transaktion steg för steg. Detta hjälper eleverna att se att en Bitcoin-transaktion inte är magi, utan en samordnad process som involverar godkännande, verifiering, inkludering i ett block och uppdatering av huvudboken.

Målet här är inte teknisk fördjupning. Det är att hjälpa eleverna att förstå vem som gör vad i en transaktion och varför verifiering är viktigt.

##### 6.5 Lita inte, verifiera, 8 minuter

Förklara att detta gäller för:

* plånböcker
* växlingsplattformar
* appar
* transaktionsdetaljer
* påståenden om "enkla vinster"
* projekt som låtsas vara som Bitcoin

Var tydlig med att Bitcoin kräver att användare tänker kritiskt, verifierar vad de använder och undviker blind tillit. Förklara också varför öppen källkod är viktigt i detta sammanhang: det möjliggör oberoende verifiering.

###### Sammanfattning och kontroll av förståelse

Avsluta med några snabba frågor:

* Vad är skillnaden mellan en förvaringsplånbok och en självförvaringsplånbok?
* Varför är seed phrase så viktig?
* Vad händer när du skickar en on-chain-transaktion?
* Varför är on-chain-transaktioner långsammare än vissa andra Bitcoin-betalningar?
* Vad betyder "Don't Trust, Verify" i praktiken?

#### Läraranteckningar

Detta kapitel är mycket praktiskt, så prioritera tydlighet, säkerhet och upprepning.

Eleverna behöver inte bemästra varje plånbokstyp på en lektion. Huvudmålen är:

* förståelse för plånbokens grunder
* förståelse för självförvaring
* lära sig det grundläggande transaktionsflödet
* anta ett ansvarsfullt verifieringstänk

Var särskilt noggrann när du diskuterar seed phrases och plånboksinställning. Eleverna ska förstå att detta inte är smådetaljer, utan grunden för Bitcoin-ägande.

De mest användbara bilderna och aktiviteterna i detta kapitel är:

* jämförelsen mellan självförvaring och förvaring
* tabellen över plånbokstyper och kompromisser
* övningen steg-för-steg för plånboksinställning
* diagrammet över transaktionsflödet
* rollbaserad transaktionsaktivitet

##### Vad som är bra

* Det är viktigt att eleverna faktiskt sätter upp en plånbok eller ser en noggrann demonstration, gör seed phrase till huvudfokus med "Dessa 12 ord ÄR din Bitcoin", testar scenarier som "Vad händer om du tappar din telefon?" och övar på att känna igen phishing.
* Lärare bör vara praktiska guider som har gjort detta tidigare, vara säkerhetsmedvetna utan paranoia och vara ärliga om svårighetsgraden och det lärande som krävs.
* Eleverna känner att de har lärt sig en faktisk färdighet de kan använda, förstår att seed phrase är verklig och viktig snarare än abstrakt, känner sig kapabla att hålla sin egen Bitcoin och förstår att decentralisering kräver personligt ansvar.
* Lärandemålen bör vara uppfyllda om eleverna kan sätta upp en plånbok och förstå skillnaden mellan publika och privata nycklar, förstå kompromisser mellan förvarings- och självförvaringsplånböcker, förklara hur en transaktion fungerar inklusive inputs, outputs och avgifter, visa säkerhetsmedvetenhet inklusive skydd av seed phrase, och ställa kritiska frågor om ägande och kontroll.

##### Tidsplanering

Om tiden är knapp, prioritera:

* Förståelse för plånbokens grunder
* Förståelse för självförvaring
* Lära sig det grundläggande transaktionsflödet
* Anta ett ansvarsfullt verifieringstänk

Om du ligger före, ta tid på:

* Jämförelsetabell mellan självförvaring och förvaring
* Tabell över plånbokstyper och kompromisser
* Steg-för-steg-övning för plånboksinställning med live-demo
* Transaktionsflödesdiagram med avgiftsberäkningar
* Avancerade säkerhetsrutiner och överväganden kring hårdvaruplånböcker

##### Om eleverna har svårt

* Seed phrases som "verkliga" → "Denna fras ÄR din bitcoin; ingen kundtjänst."
* Publika vs. privata nycklar → E-post-analogi (adress vs. lösenord).
* Varför det är svårt → "Du kontrollerar det; du är ansvarig." Erkänn kompromissen.
