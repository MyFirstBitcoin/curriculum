# 6.4 Ta emot och skicka transaktioner

En Bitcoin-transaktion är en överföring av äganderätten till bitcoin till en ny ägare. Observera att det inte är de faktiska mynten som överförs, utan äganderätten till dem: med andra ord, rätten att spendera dem. Varje gång en transaktion accepteras i ett block uppdaterar alla noder i nätverket sin lokala kopia av den offentliga huvudboken för att återspegla ägarbytet. På detta sätt liknar en Bitcoin-transaktion mer en fastighetsaffär (eller annan egendomsaffär) än en kontanttransaktion.

För att "skicka" bitcoin signerar avsändaren ett meddelande med sin privata nyckel, vilket signalerar till nätverket att den rättmätiga ägaren av bitcoinen har överfört äganderätten till mottagaren.

Bitcoinen kommer nu att vara kopplad till mottagarens adress, vilket ger denne äganderätt till bitcoinen, så att endast den nya ägaren kan spendera dem genom att använda sin privata nyckel.

Nya Bitcoin-transaktioner initieras från plånböcker runt om i världen, men det finns ingen central betalningsförmedlare. Istället tävlar miners om att registrera transaktioner i huvudboken.

Låt oss säga att Johan är skyldig Elin 0,5 BTC och är redo att betala tillbaka henne. Båda har digitala plånböcker.

1. Elin delar sin adress med Johan.
1. Johan använder sin plånboksprogramvara för att skapa transaktionen, som inkluderar Elins adress, beloppet som ska överföras (0,5 BTC) och en avgift till minern. Högre avgifter gör det mer sannolikt att en miner inkluderar transaktionen i nästa block.
1. Efter att ha signerat transaktionen sänds den ut till nätverket, där den verifieras av noder. De kontrollerar om Johan har tillräckligt med medel och är den rättmätiga ägaren av de mynt han vill spendera. Om han inte är det, avvisas transaktionen omedelbart.
1. När transaktionen har verifierats väljer miners om de ska lägga till transaktionen i nästa block, vanligtvis baserat på vald avgift. När transaktionen kommer med i ett block läggs den till i blockkedjan och medlen överförs till Elins adress.
1. Äganderätten har överförts till Elin. Hon kan nu använda sin privata nyckel för att spendera medlen.

_Det är viktigt att notera att när transaktionen är slutförd kan den inte återkallas._


> **Light – Hur en Bitcoin-transaktion fungerar**
>
> 1. Någon begär en transaktion
> 1. Transaktionen sänds ut till P2P-datorer (noder)
> 1. Miners verifierar transaktionen
> 1. Transaktioner kombineras för att bilda ett datablock
> 1. Nytt block läggs till i den befintliga blockkedjan
> 1. Transaktionen är slutförd



> **Light – Ta emot Bitcoin-transaktioner**
>
> För att ta emot bitcoin behöver du ge avsändaren en Bitcoin-publik adress. Detta är en unik sträng av bokstäver och siffror som representerar din plånbok och används för att identifiera den på Bitcoin-nätverket.
>
> Du hittar din publika adress genom att öppna din Bitcoin-plånbok och leta efter ett alternativ för att “Ta emot” eller “Sätta in” bitcoin.
>
> Du kan sedan dela din Bitcoin-adress på ett av flera sätt:
>
> 1. **Kopiera och klistra in adressen**: Du kan kopiera adressen genom att markera den och trycka på "Kopiera", och sedan klistra in den i ett e-postmeddelande eller ett meddelande.
> 1. **Dela en länk till din Bitcoin-plånbok**: Vissa Bitcoin-plånböcker låter dig skapa en länk till din plånbok som du kan dela med avsändaren. De kan då klicka på länken för att komma åt din plånbok och skicka bitcoin.
> 1. **Dela en QR-kod**: Om avsändaren har en smartphone med en Bitcoin-plånboksapp installerad kan de skanna QR-koden för att få din Bitcoin-adress.


När avsändaren har din adress kan de skicka dig bitcoin genom att ange din adress och det belopp de vill skicka. Bitcoinen skickas då från deras plånbok till din plånbok.

Transaktionen bekräftas av Bitcoin-nätverket och tar vanligtvis cirka 10 minuter. För ökad säkerhet rekommenderas att vänta på två bekräftelser, vilket tar cirka 20 minuter.


> **Light – Skicka Bitcoin-transaktioner**
>
> För att skicka bitcoin behöver du några saker: en Bitcoin-plånbok, mottagarens publika adress och det belopp av bitcoin du vill skicka.
>
> 1. Öppna din Bitcoin-plånbok.
> 1. Navigera till knappen “Skicka” och klistra in mottagarens adress i fältet "Till". Alternativt kan du också skanna QR-koden om mottagaren tillhandahåller en sådan.
> 1. Ange det belopp av bitcoin du vill skicka i fältet “Belopp”.
> 1. Dubbelkolla mottagarens adress och beloppet som ska skickas. Kom ihåg att transaktioner är oåterkalleliga!
> 1. Innan du klickar på “Bekräfta och skicka” rekommenderar vi att du dubbelkollar transaktionsuppgifterna en gång till för att säkerställa att du skickar rätt mängd bitcoin till rätt adress.
> 1. Sänd ut transaktionen och vänta på att nätverket bekräftar transaktionen.
>
> Nu vet du hur du utvärderar, väljer och sätter upp en självförvarad Bitcoin-plånbok. Att skicka och ta emot bitcoin på Bitcoin-nätverket kallas “on-chain”-transaktioner. Detta eftersom transaktionerna sker på det huvudsakliga Bitcoin-nätverket och registreras i blockkedjan.
>
> On-chain-transaktioner är det säkraste sättet att transagera med bitcoin tack vare den decentraliserade verifieringen som nätverket tillhandahåller.
>
> Dock är on-chain-transaktioner långsammare och kan vara betydligt dyrare än andra alternativ (som vi kommer att diskutera i Modul 7) på grund av miner-avgiften.


#### Aktivitet: Transaktioner i praktiken


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Detta är en samarbetsövning som förenklar de grundläggande rollerna för personer som är involverade i en Bitcoin-transaktion.**

###### Viktiga punkter

1. Det finns fyra typer av deltagare i varje bitcoin-transaktion: avsändaren, mottagaren, miners och nodoperatörer.
1. Avsändaren måste godkänna (kryptografiskt signera) **mängden bitcoin** som ska skickas OCH **specifik adress** att skicka till.
1. Mottagaren måste ge en **giltig adress** till avsändaren OCH verifiera att transaktionen har bekräftats på blockkedjan.
1. Miners säkerställer att alla kriterier är uppfyllda innan de lägger till transaktioner i framtida block.
1. Node-operatörer verifierar att minerade block är giltiga innan de uppdaterar sin version av blockkedjan (huvudboken).

###### Tips till studenten

Byt mellan alla fyra roller för att uppleva vad varje deltagare gör.
