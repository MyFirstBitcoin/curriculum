# 9.2 Vad är Mempool?

Den **mempoolen**, en förkortning av “memory pool”, är som ett väntrum för Bitcoin-transaktioner. När du skickar bitcoin sänds din transaktion först ut till nätverket och placeras i mempoolen.

Du kan tänka på det som att vänta i kö på en restaurang. Ditt namn hamnar på en lista, och du väntar tills ett bord blir ledigt. På samma sätt väntar din transaktion i mempoolen tills en miner inkluderar den i ett block.

Bitcoin-noder kontrollerar varje ny transaktion för att säkerställa att den är giltig och att de bitcoin som spenderas inte redan har använts. Om transaktionen är giltig stannar den i mempoolen tills den bekräftas.

Miners väljer transaktioner från mempoolen och inkluderar dem i nya block. Vanligtvis väljs transaktioner med högre avgifter först.

När en transaktion har inkluderats i ett block blir den bekräftad och registreras permanent på Bitcoin-blockkedjan.

#### Aktivitet: Utforska mempoolen


https://qr.myfirstbitcoin.org/mempool.pdf

_Activity: Mempool_


**Denna aktivitet introducerar elever till ett gratis och öppen källkods-verktyg som inte kräver tekniska kunskaper. Det är användbart för Bitcoin-användare på alla nivåer, från nybörjare till erfarna.**

###### Viktiga punkter

1. **Mempoolen** syftar på listan över obekräftade transaktioner som varje Bitcoin-nod underhåller, inte en specifik tjänst eller plattform.
1. Det finns ingen enskild, universell mempool. Mempool.space är en av många.
1. [Mempool.space](https://mempool.space) är öppen källkod och välkänd för att vara en lättanvänd visuell blockutforskare. Den ger realtidsdata om obekräftade transaktioner, avgiftsnivåer och annan nätverksaktivitet.

###### Tips till elever

Mempool.space gör mycket mer än att visualisera block. Utforska andra delar av Bitcoin-ekosystemet: t.ex. Lightning, mining, hash rate, pooler och blockutrymmets "glasögon".
