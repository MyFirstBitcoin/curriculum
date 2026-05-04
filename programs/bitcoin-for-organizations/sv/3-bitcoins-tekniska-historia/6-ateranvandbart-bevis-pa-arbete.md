# 3.6 Återanvändbart bevis på arbete

Hal Finney är en annan känd medlem av Cypherpunk-rörelsen, som var mycket intresserad av utvecklingen av elektroniska pengar och aktiv på e-postlistan.

Han bestämde sig för att göra ett nytt försök att utveckla ett elektroniskt kontantsystem baserat på proof-of-work. Fram till denna punkt hade hash-utdata varit unik för varje transaktion, men hans idé var att skapa 'återanvändbara proof-of-work'.

Nackdelen med detta tillvägagångssätt är den centraliserade servern, som man måste lita på inte dubbelspenderar eller stängs ner. För att lösa detta föreslog Hal att använda fri och öppen källkod som kunde köras på en säker hårdvarukomponent och valideras oberoende.

Lösningen stod fortfarande inför några av samma problem som de andra förslagen:

* Det så kallade 'hönan och ägget'-problemet med att få användning, där det saknas incitament för användare att vilja begära tokens, och säljare vill inte ansluta sig till systemet om inte användarna vill betala med dessa tokens.
* POW kommer troligen också att bli billigare över tid i takt med att datorkraften förbättras, vilket antyder att marknaden så småningom skulle översvämmas av RPOW-valutaenheter.

> Om Moores lag fortsätter att gälla kommer kostnaden för att skapa en (POW)-token att sjunka i en stadig, exponentiell takt. Kom ihåg att detta inte är pengar och inte är avsett att vara en värdebevarare, utan snarare en lättutbytbar representation av datorarbete.  
 _Hal Finney_

Dessa egenskaper begränsade projektets attraktionskraft och därmed användning, och trots hans bästa ansträngningar slutade projektet som ännu ett misslyckat försök att skapa elektroniska pengar.
