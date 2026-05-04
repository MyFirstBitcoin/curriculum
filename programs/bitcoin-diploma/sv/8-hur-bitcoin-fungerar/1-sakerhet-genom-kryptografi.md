# 8.1 Säkerhet genom kryptografi

> Vad Bitcoin ger oss är ett hårt löfte: programmet kommer att köras exakt som specificerat.  
_Andreas M. Antonopoulos_

#### Kryptering med offentlig/privat nyckel


> **Definition – Definition av kryptografi**
>
> **Kryptografi** är konsten att göra information till en hemlighet som bara rätt personer kan läsa.


* **Kryptering** är processen att omvandla information till en kodad form så att bara någon med rätt nyckel kan läsa den.
* **Dekryptering** är processen att omvandla den kodade informationen tillbaka till något läsbart.

I traditionell kryptografi måste två personer som vill kommunicera privat först dela samma hemliga nyckel, ungefär som ett gemensamt lösenord. En person använder denna nyckel för att kryptera meddelandet innan det skickas, och den andra personen använder samma nyckel för att dekryptera och läsa det.

Problemet med detta system är att båda personerna redan måste dela den hemliga nyckeln. Om någon annan får tillgång till nyckeln kan de läsa alla avlyssnade meddelanden.

Bitcoin löser detta problem med en annan metod som kallas offentlig-nyckel-kryptografi, där användare inte behöver dela hemliga nycklar i förväg.

Kryptering med offentlig/privat nyckel löser problemet med att dela hemligheter. Istället för att dela ett lösenord har varje person två nycklar: en offentlig nyckel och en privat nyckel.

* **offentliga nyckeln** kan delas med vem som helst.
* **privata nyckeln** måste alltid hållas hemlig.

Om Johan vill skicka något till Arvid kan han använda Arvids offentliga nyckel. Bara Arvid kan låsa upp det med sin privata nyckel. Även om någon avlyssnar meddelandet kan de inte läsa eller använda det utan den privata nyckeln.

I Bitcoin används detta system för att skapa digitala signaturer. En digital signatur bevisar att ägaren av en privat nyckel har godkänt en transaktion, ungefär som att skriva sin namnteckning på ett dokument. Det är detta som gör att Bitcoin-transaktioner kan vara säkra och verifierbara utan att man behöver lita på en tredje part.

Bitcoin-transaktioner innebär att ägandet av bitcoin överförs från en adress till en annan.

Kryptering används för att säkerställa att endast den verkliga innehavaren av bitcoinen har rätt att skicka sina pengar till någon annan. Det skyddar deras egendom mot illvilliga aktörer.

Som ett extra skydd får varje Bitcoin-transaktion automatiskt en UNIK digital signatur. Denna unika digitala signatur drivs av manipuleringssäker teknik som hjälper nätverket att verifiera att det är den verkliga ägaren av bitcoinen, och inte någon annan, som har skickat dem.


> **Info**
>
> Varje användare har två nycklar: en **privat nyckel**, som **hålls hemlig**, och en **offentlig nyckel** som kan **delas med andra**. **Den privata nyckeln** fungerar som en form av identifikation och ägarbevis, och bekräftar: ”Den här adressen tillhör mig och jag har kontroll över den.”


###### Hur en Bitcoin-transaktion fungerar

1. **Skapa transaktionen**: En användare initierar en Bitcoin-transaktion genom att ange detaljer som mottagarens adress och mängden bitcoin som ska skickas.
1. **Generering av digital signatur**: Avsändaren skapar en unik **digital signatur** med sin **privata nyckel**. Denna signatur är en unik kod som verifierar transaktionens äkthet.
1. **Sända transaktionen**: Den signerade transaktionen sänds ut till Bitcoin-nätverket och visar avsikten att överföra ägandet av bitcoin från avsändaren till mottagaren.
1. **Verifiering i nätverket**: Noder i Bitcoin-nätverket tar emot transaktionen och använder mottagarens **offentliga nyckel** för att verifiera signaturens äkthet. av transaktionen. Samtidigt använder de avsändarens **offentliga nyckel** för att verifiera **digitala signatur**.
1. **Bekräftelse på Bitcoin-nätverket**: Om verifieringen lyckas kommer transaktionen att läggas till i huvudboken, som fungerar som en säker och transparent redovisning av alla transaktioner. När den är bekräftad överförs ägandet av bitcoin officiellt från avsändaren till mottagaren.


> **Callout – Sammanfattning**
>
> Den **digitala signaturen**, skapad med avsändarens **privata nyckel**, bevisar att transaktionen har godkänts av ägaren till bitcoin. Bitcoin-nätverket kan sedan verifiera detta bevis och registrera transaktionen.


#### Förklaring av hashning

Bli inte avskräckt av de tekniska termerna och matematiska begreppen som kommer. Vi förstår att inte alla älskar matte, men du kanske överraskar dig själv och ser att även de mest komplexa idéerna kan förstås med lite ansträngning.


> **Definition – Definition av en funktion**
>
> En **funktion** är som en maskin som tar emot viss information och omvandlar den till något nytt. Informationen du ger funktionen är **inmatningen**. Den nya informationen som funktionen skapar är **utmatningen**. Funktioner hjälper datorer att utföra uppgifter och lösa problem.


##### Vad är en funktion?

En funktion är en uppsättning instruktioner som tar en inmatning och producerar en utmatning. Du kan tänka på det som ett recept: du följer stegen med vissa ingredienser och får alltid ett förutsägbart resultat.

I Bitcoin används funktioner för att behandla och verifiera transaktioner. När någon skickar bitcoin hjälper kryptografiska funktioner till att kontrollera att transaktionen är giltig, bekräfta att avsändaren har tillräckligt med medel och uppdatera saldon i Bitcoin-huvudboken. När den har verifierats och lagts till i ett block blir transaktionen en del av det permanenta registret på blockkedjan.

##### Vad är en envägsfunktion?

En envägsfunktion är en speciell typ av funktion som är lätt att beräkna i ena riktningen men extremt svår att vända. Till exempel är det enkelt att mixa ingredienser till en smoothie, men du kan inte separera smoothien tillbaka till de ursprungliga ingredienserna.

Bitcoins säkerhet bygger på envägsfunktioner. De används i kryptografi med offentliga och privata nycklar, vilket gör det möjligt för människor att dela en offentlig nyckel samtidigt som de håller sin privata nyckel hemlig. Även om den offentliga nyckeln är synlig är det omöjligt att härleda den privata nyckeln från den. Det är detta som gör Bitcoin-transaktioner säkra.

##### Vad är en hashfunktion?

En **hashfunktion** är som en hemlig kodmaskin. Den tar emot ett meddelande och omvandlar det till en kod.

###### Hur hashning fungerar i Bitcoin-transaktioner

I Bitcoin omvandlas varje transaktion till en hash innan den läggs till i blockkedjan. En hash är ett unikt digitalt fingeravtryck av transaktionen. Om någon försöker ändra ens en liten del av transaktionen kommer hashen att förändras helt. Detta gör det enkelt för nätverket att upptäcka manipulation.

###### Hashningens roll i Bitcoins säkerhet

Hashning hjälper till att skydda Bitcoin-nätverket genom att göra transaktioner enkla att verifiera och omöjliga att tyst ändra. Eftersom varje transaktion har sin egen unika hash kan nätverket snabbt upptäcka om något har ändrats.

En hashfunktion tar data och omvandlar den till en fast sträng av siffror och bokstäver som kallas en hash. Samma inmatning ger alltid samma hash, men även en liten förändring i inmatningen skapar ett helt annat resultat. Denna egenskap gör det möjligt för datorer att kontrollera att data inte har ändrats.


> **Definition – Definition av hashning**
>
> **Hashning** är som att skapa ett fingeravtryck för digital data. Det är processen att ta ett digitalt meddelande och omvandla det till en kod med fast längd, som fungerar som en unik identifierare. Precis som ett fingeravtryck kan identifiera en person kan en hash identifiera ett digitalt meddelande.


Utmatningen, **utmatningen**, eller hash, är alltid lika lång, oavsett hur lång den ursprungliga informationen var. Bitcoin använder några specifika typer av hashfunktioner som kallas **SHA-256** och **RIPEMD160**.

Några exempel visas nedan:

* SHA256-hash av strängen **hej världen**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256-hash av strängen **hej världen.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Observera att en liten förändring i indata förändrar utdata helt jämfört med den första
* SHA256-hash av den nedladdningsbara iso-filen **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Den här inmatningen är en enorm fil men utdata är ändå av samma fasta längd

Du kan också tänka på hashing som ett partitur som fångar essensen av ett musikstycke. Precis som ett partitur är en unik representation av en melodi, är ett hashvärde en unik representation av data.

Genom att jämföra partituret för ett musikstycke med själva framförandet kan en musiker avgöra om framförandet är korrekt. På samma sätt kan man, genom att jämföra hashvärdet för mottagen data med det ursprungliga hashvärdet, avgöra om datan har ändrats under överföringen.

Precis som en liten avvikelse i ett musikframförande kan få det att låta annorlunda, kommer även den minsta förändringen av ursprungsdatan att resultera i ett annat hashvärde. Detta gör hashing till ett kraftfullt verktyg för att säkerställa integriteten och äktheten i en Bitcoin-transaktion.

Processen att koda **publik nyckel** genom hashing används för att förbättra säkerheten för information genom att omvandla den till ett oläsligt format med fast längd. Bitcoin använder algoritmerna SHA-256 och RIPEMD160 för att skapa publika adresser. Den resulterande utdata fungerar som en unik identifierare för **publik nyckel** och hjälper till att säkerställa integriteten och säkerheten för transaktioner som lagras i huvudboken. Genom att kryptera informationen på detta sätt blir det svårare för obehöriga att komma åt och manipulera datan.

##### Egenskaper hos en hashfunktion

* **Deterministisk**: Samma ingredienser ger alltid samma smoothie. På samma sätt kommer samma data alltid att ge samma hash.
* **Pre-image-resistens**: Om du bara har smoothien kan du inte lista ut exakt vilka frukter som användes. På samma sätt kan du inte avgöra ursprungsdatan om du bara har en hash.
* **Avalanche-effekt**: Att ändra även en liten del av ingredienserna skapar en helt annan smoothie. Vid hashing ger en mycket liten förändring i datan ett helt annat hashvärde.
* **Kollisionsresistens**: Det är extremt svårt att hitta två olika uppsättningar ingredienser som ger exakt samma smoothie. På samma sätt är det extremt osannolikt att två olika datamängder ger samma hash.
* **Snabb att verifiera**: Att göra smoothien går snabbt, och det är lätt att kontrollera att resultatet är en smoothie. Hashfunktioner är snabba att beräkna och enkla för vem som helst att verifiera.

#### Aktivitet: Generera SHA 256-hash

https://tools.keycdn.com/sha256-online-generator

Nyfiken på hur hashing fungerar? Skanna QR-koden för att direkt generera en SHA256-hash från vilket ord, mening eller indata du vill. Hashfunktioner är som digitala fingeravtryck: de är envägs, vilket betyder att när något har hashats kan det inte återskapas. Prova själv och se!
