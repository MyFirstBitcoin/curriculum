# 2.3 Bitcoin är för långsamt för att vara global valuta

> Visionärer ser en framtid med distansarbetande, interaktiva bibliotek och multimediala klassrum. De talar om elektroniska stadsmöten och virtuella gemenskaper... Sanningen är att ingen online-databas kommer att ersätta din dagliga tidning, ingen CD-ROM kan ersätta en kompetent lärare och inget datornätverk kommer att förändra hur regeringen fungerar.  
_Clifford Stroll_

17 år senare upphörde Newsweek med tryckt utgivning och blev endast tillgänglig online. Föreställ dig att leva 1974 när Transmission Control Protocol (TCP) först skapades.

Ingen förutsåg smarttelefonen, med alla dess appar, i din hand. Ingen såg SatNav-systemet i din bil.

Internet uppstod inte som en färdig produkt, utan snarare gradvis som en utveckling av protokoll och lager. Dessa utvecklingar har byggt vidare på, men huvudsakligen inte förändrat, TCP.

> Så när jag ser på övergången till framtidens kommunikationsplattformar ser jag att det vackra med internetprotokoll är att du får separationen mellan tjänst och teknik i olika lager.  
_Michael K Powell_



##### Jämför Bitcoins utveckling med internets utveckling

TCP var nödvändigt men inte tillräckligt för att allt annat på internet skulle kunna uppstå. Bitcoins utveckling verkar följa en liknande väg. Öppna system verkar vara mer motståndskraftiga och framgångsrika när de utvecklas i lager, även om det kan gå lång tid mellan att de första byggstenarna läggs och att de får bred användning. Allt-i-ett-lösningar verkar inte vara lika effektiva i öppna system som de som byggs i lager ovanpå protokoll. Precis som ingen har behövt bygga om internet för att filmer inte kunde streamas med TCP, så kommer det troligen vara med Bitcoin.

Det finns redan ett antal lager 2-protokoll ovanpå Bitcoin, och det finns många applikationer ovanpå dessa lager 2-protokoll (se avsnitt 201.4 för mer information om dessa).

Istället för att fokusera på vad bitcoin och Bitcoin-nätverket inte kan göra idag, tänk på vad som redan kan göras idag, och jämför det med vad som var möjligt för 10 år sedan. Gör samma övning med internet från 1985 till 1995, och se sedan hur mycket snabbare internet blev under de följande 30 åren och vilka applikationer som blev möjliga. Använd den insikten för att föra Bitcoin framåt och föreställ dig hur det kan se ut om bara ytterligare 10 år, eller 30 om din fantasi räcker så långt.



##### Jämför Bitcoin med det befintliga globala penningsystemet

Det centrala påståendet att Bitcoin är för långsamt för att vara globalt pengar är möjligen sant om vi är begränsade till Bitcoins baslager. Det är också sant att baslagret i våra befintliga penningsystem är för långsamt för att vara globalt pengar, om en liknande begränsning innebar att det inte fanns någon betalningsinfrastruktur byggd ovanpå av privata banker och betaltjänster som Visa och Mastercard. Vårt nuvarande system är byggt i lager, så vi kan förvänta oss att framtiden ser likadan ut. Vissa designavvägningar, som mellan tillit, hastighet och kostnad, kan överföras mellan system som levererar samma lösningar även om de är byggda för att flytta olika värdetoken.

Några av de befintliga lager 2-lösningarna på Bitcoin adresserar direkt hastighetsfrågan, till exempel Liquid och Lightning Network (se avsnitt 201.4 för mer information). Liquid är snabbare och billigare än Bitcoin-blockkedjan, och Lightning Network är ännu snabbare och billigare än Liquid. En mångfald av lager 2-lösningar, alla med olika avvägningar, är att vänta och är hälsosamt.

Det kommer troligen att finnas fler lager 2 och 3 och en explosion av applikationer som använder dessa, precis som det hände med internets utveckling.



##### Motivation

När denna kritik framförs är det värt att fundera på om kritikern har andra motiv. Har de till exempel ett nytt eller annorlunda blockkedjeprojekt? Detta kan liknas vid att försöka sälja ett bättre Transmission Control Protocol.

Skalbarhets- eller blockkedjetrilemmat togs först upp av Vitalik Buterin 2017. Det säger att det alltid finns en avvägning i blockkedjedesign mellan egenskaperna decentralisering, säkerhet och skalbarhet. Den som framför kritiken att Bitcoin är för långsamt och att de har en snabbare lösning i en lager 1-blockkedja kommer att offra viss säkerhet eller decentralisering för att uppnå det. Även om en sådan avvägning för en blockkedja designad för andra användningsområden kan vara rimlig, måste prioritetsordningen för globala pengar vara:


> **Note**
>
> * **Decentralisering**
>   * Gör det möjligt att ta bort betrodda parter
> * **Säkerhet**
>   * Hindrar illvilliga aktörer från att manipulera transaktioner eller huvudboken
> * **Skalbarhet**
>   * Gör det möjligt för systemet att växa ekonomiskt i antal användare och hastighet


De två första egenskaperna skapar förutsättningar för utgivning utan skapare, betalningar utan mellanhänder och förvaring utan förvaltare.

Bitcoin gör rätt avvägning mellan de tre blockkedjedesignelementen med tanke på att dess mål är att vara globala pengar, och den mildrar avvägningarna kring skalbarhet och hastighet genom att använda lager.

> Satoshi upptäckte hur man skyddar integriteten för digitala pengar utan betrodda parter – inga skapare, mellanhänder eller förvaltare behövs.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
