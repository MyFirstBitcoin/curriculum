# 3.7 Bitcoin

Efter många år och misslyckade försök hade Cypherpunks till stor del börjat tappa intresset för idén om en digital valuta utan tillstånd, när Adam Back fick ett mejl med en länk till ett utkast av en vitbok kallad 'electronic cash without a third party' från en anonym person som kallade sig Satoshi Nakamoto.

För att sammanfatta vid denna punkt har vi åtminstone idéerna om:

* Kryptografiska signaturer som kan ge en viss nivå av integritet och anonymitet
* Konceptet av en icke-täckt valuta (B-Money)
* Förslag (men inga medel) för att begränsa utgivningen av ny valuta
* Digitala mynt vars ägande tilldelades genom publika nycklar (B-Money) och kunde flyttas genom signering och omfördelas baserat på mottagarens adress (RPOW och Hashcash)
* Alla noder underhåller en kopia av en helt distribuerad huvudbok (B-Money) (avfärdades då som opraktiskt)
* Tidsstämplingsprotokoll – att använda Merkle-trädhashning för att ge en matematiskt bevisbar kronologi av händelser som är svår att förfalska om alla användare behåller samma register
* Proof of work för att knyta verklig ansträngning till systemet (men där själva hashen användes som valuta)
* Helt decentraliserade nätverk där alla deltagare är jämlika och kan komma och gå från nätverket (BitTorrent)
* Konceptet att knyta nya hashar till tidigare hashar (Bit Gold och tidsstämpling)

Det som saknades vid denna tidpunkt inkluderade:

* En fungerande lösning på 'Byzantine generals'-problemet
* En metod för att begränsa mängden pengar i omlopp trots kontinuerliga förbättringar av hårdvara
* Incitamentsystem för att få folk att delta (hönan och ägget-problemet)

Den andra stora skillnaden mellan de senaste försöken och Bitcoin var att Satoshi hade arbetat på koden under en längre tid i sann 'Cypherpunks write code'-anda innan han tillkännagav den på e-postlistorna, till skillnad från Bit Gold och B-Money som var mer konceptuella.

Vad var innovationen som gjorde att Bitcoin skiljde sig från tidigare försök med elektroniska pengar?

Proof of work skulle användas som ett konsensusmekanism och ett sätt att ge säkerhet och oföränderlighet: Istället för att använda hashen som en form av pengar, skulle den användas av en ny konceptuell process kallad mining, där en nod samlar ihop en uppsättning transaktioner, lägger till ett slumpmässigt tal och sedan applicerar hashningen på 'blocket' av data. Ett giltigt block som uppfyllde hashkravet skulle sedan annonseras till nätverket. Dessa block skulle kopplas ihop genom att använda hashen från föregående block i varje, och den längsta blockkedjan skulle användas vid oavgjort där olika noder validerar och annonserar olika block samtidigt och skapar kedjedelningar. Proof of work blev den distribuerade skiljedomaren för att lösa Byzantine generals-problemet.

Dessa miners fick också ett incitament att tillhandahålla den CPU-kraft som krävdes för att utföra proof-of-work genom att tilldelas nya bitcoin för varje block. Mängden Bitcoin de belönas med är också programmerad att minska ungefär vart fjärde år tills alla Bitcoin har skapats, vilket skapar en hård gräns för det totala antalet Bitcoin som någonsin kommer att finnas i omlopp till 21 miljoner.

Den mest originella idén var hur han löste frågan om hur mycket pengar som skapas när hårdvaran förbättras och mer kraft kan användas på nätverket. Tidsstämplarna för ett visst antal block (2016) skulle medelvärdesberäknas, och om de skapas för snabbt skulle hashen som krävs för att skapa ett nytt block göras svårare, om det går för långsamt skulle det göras lättare. Detta byggdes in i det decentraliserade protokollet som alla noder kör, så att varje miner som ignorerar det skulle slösa energi på att mina ett block utan nytta eftersom det skulle avvisas av resten av nätverket. Denna justering säkerställer att skapandet av nya block förblir enligt den planerade utgivningstakten och ger incitament för miners att 'följa reglerna'.

####   
Sammanfattning

Många av pusselbitarna för vad som krävs för att bygga ett decentraliserat peer-to-peer-system för elektroniska pengar baserat på sunda penningprinciper fanns på plats innan Satoshi släppte sin vitbok och kort därefter den första versionen av koden.

> Bitcoin är av sådan natur att när version 0.1 släpptes var kärndesignen fastslagen för resten av dess livstid  
_Satoshi Nakamoto_

Även om många idéer för förbättringar (BIP:er) har föreslagits och antagits, har Bitcoin arbetat på i bakgrunden sedan 2009 enligt protokollet som designades i den första versionen och med knappt någon störning. Alla förbättringar har gjorts samtidigt som bakåtkompatibilitet med alla tidigare versioner har bibehållits.



##### Anteckningar

1. För en förklaring av Byzantine Generals-problemet – se [https://sv.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
