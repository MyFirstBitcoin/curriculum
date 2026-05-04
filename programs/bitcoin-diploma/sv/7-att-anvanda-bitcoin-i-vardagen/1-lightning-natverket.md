# 7.1 Lightning-nätverket

Lightning-nätverket är ett betalningssystem som gör det möjligt för användare att skicka och ta emot bitcoin snabbt och billigt. Det fungerar genom att upprätta en delad plånbok där båda parter sätter in en del av sina bitcoin. De kan sedan göra obegränsat antal transaktioner med varandra utan att behöva registrera varje enskild transaktion på huvudblockkedjan. På så sätt slipper de verifiera och inkludera varje transaktion i ett block, vilket gör processen både snabb och kostnadseffektiv. De lägre avgifterna innebär att Lightning-nätverket kan användas för små betalningar som inte alltid är möjliga på blockkedjan. När parterna bestämmer sig för att avsluta sitt samarbete registreras endast det slutliga saldot på blockkedjan.

Föreställ dig en dag när du arbetar på ett café. Du planerar att stanna ett tag och öppnar en nota och förbetalar istället för att betala för varje beställning. I slutet av dagen går du och ägaren igenom notan för att göra upp räkningen. Om din insättning är större än vad du har spenderat får du tillbaka mellanskillnaden; om du har spenderat mer betalar du det du fortfarande är skyldig.

Detta upplägg kan skalas upp för att inkludera fler deltagare. Till exempel, vid ett av dina besök på caféet tar du med en vän som bartendern inte känner och därför inte kan öppna en nota åt. Du erbjuder din vän att använda din befintliga nota för att täcka deras utgifter, och ni kommer överens om att de betalar tillbaka till dig privat. Föreställ dig nu tusentals personer som gör samma sak samtidigt, vilket gör det möjligt för andra att använda befintliga notor för att koppla ihop sig med ännu fler personer — det är så Lightning-nätverket fungerar!

Med Lightning kan du göra betalningar till vem som helst på nätverket, inte bara till den du har en direkt nota med — så länge det finns en väg mellan parterna. Din betalning kan ta sig genom nätverket tills den når mottagaren, även om du inte har en öppen kanal direkt med den personen.

Låt oss titta på skillnaden mellan transaktioner på kedjan och utanför kedjan.

##### Transaktioner på kedjan

Detta är transaktioner som sker direkt på Bitcoin-blockkedjan. De tar cirka 10 minuter att bekräfta, och avgifterna beror på transaktionens storlek i virtuella byte. De är säkrare men långsammare, eftersom de kräver nätverkets konsensus.

##### Transaktioner via Lightning-nätverket

Dessa transaktioner sker på ett separat nätverk byggt ovanpå Bitcoin-blockkedjan. De slutförs snabbare och med lägre avgifter. De används ofta där faktorer som hastighet och kostnad är viktigare. Jämfört med transaktioner på kedjan är de mindre säkra.


|  | Bitcoin-nätverket | Lightning-nätverket |
| --- | --- | --- |
| Definition | Ett decentraliserat digitalt nätverk som använder kryptografi för att säkra finansiella transaktioner. | Ett betalningsprotokoll i ett andra lager som körs ovanpå Bitcoin-blockkedjan och möjliggör snabbare och billigare transaktioner. |
| Fördelar | Decentraliserat och säkert. Inga återbetalningar eller bedrägerier. Kan användas pseudonymt. Global acceptans. | Snabbare och billigare transaktioner. Ökad skalbarhet. Transaktioner utanför kedjan belastar inte blockkedjan. |
| Nackdelar | Långsamma transaktionstider. Höga avgifter för vissa typer av transaktioner. Komplicerat för nybörjare. | Kan kräva förtroende för kanaloperatörer. Kräver transaktion på kedjan för att öppna och stänga kanaler. |
