# 3.4 Hashcash

Hashcash skapades av Adam Back, en annan av de tidiga innovatörerna inom detta område. Adam hade ett starkt intresse för fria marknader och integritet på internet, och stötte på Cypherpunks e-postlista som han gick med i och blev en aktiv deltagare i.

Han var mycket intresserad av digitala pengar och kom med några förslag på hur gruppen potentiellt skulle kunna arbeta närmare med DigiCash och Chaum, men dessa ledde ingenstans. Han riktade sedan sin uppmärksamhet mot ett annat framväxande problem – skräppost via e-post. Han och resten av Cypherpunks ville hitta en lösning på problemet med skräppost, där det var enkelt för spammare att skapa och skicka tusentals mejl som överbelastar nätverken. Hans innovativa lösning baserades på hashning – möjligheten med kryptografi att omvandla vilken data som helst till en unik och slumpmässig sträng av en viss längd, för att skapa motsvarigheten till ett digitalt 'frimärke' som behövde läggas till mejlet för att det skulle anses giltigt och skickas över nätverket. En obetydlig kostnad för ett äkta mejl, men avskräckande för en spammare.

Den viktigaste innovationen som Hashcash skapade var att knyta verkliga resurser – datorkraft – till ett digitalt nätverk. Medan digitala resurser fram till denna punkt kunde kopieras utan begränsningar, begränsades antalet 'hashcash' som skapades av hur mycket energi människor var villiga att investera i det.

Även om lösningen uppfyllde några av de kriterier som Adam ansåg behövdes i ett digitalt pengasystem; den var anonym, motståndskraftig och krävde inget förtroende, var varje hashcash inte återanvändbar och inte riktigt knapp. Han föreslog andra sätt att hantera dessa problem med hjälp av externa tredje parter.

##### BitGold

Nick Szabo byggde vidare på konceptet Hashcash och proof of work för att föreslå en alternativ lösning, som han beskrev i en e-postlista ett år efter att Hashcash publicerades, 1998.

Även om detta förslag närmade sig en lösning, fanns det fortfarande flera utmaningar.

* Vem skulle driva registret över hash-ägande och hur kan de litas på?
* Hashning skulle generellt sett bli billigare över tid, vilket också var en utmaning för HashCash.

Eftersom de länkade hasharna skulle tidsstämplas, föreslog han någon form av historisk spårning av svårighetsgraden för hashning vid den tiden; en tidigare hash skulle kräva mer processorkraft än en senare eftersom kostnaderna har sjunkit. Tyvärr innebar detta att hasharna inte skulle vara 'fungibla', det vill säga av lika värde, vilket anses vara en nyckelattribut för digitala pengar. För att hjälpa till att lösa detta föreslog Nick någon form av 'fri bankverksamhet' ovanpå BitGold som kunde samla olika grupper av hashar som skulle värderas lika.

##### B-Money

Kort efter BitGold-förslaget lade Wei Dai fram en liknande lösning. Han hade redan utvecklat flera andra verktyg för Cypherpunks och hade sina egna idéer om digitala pengar.

Hans förslag liknade BitGold genom att det använde digitala signaturer för att överföra pengar, och transaktionshistoriken skulle lagras i en huvudbok som innehöll publika nycklar och mängden valutaenheter som tilldelats varje. Precis som med BitGold ansågs betrodda tredje parter vara säkerhetsrisker, och uppfattningen var att ett elektroniskt pengasystem inte skulle förlita sig på en enda aktör för att spåra saldon, transaktioner eller förhindra dubbelspendering.

Wei Dai föreslog flera lösningar på dessa problem, varav en var att istället för att en central aktör(er) underhöll huvudboken, skulle ALLA noder ha en kopia. Om alla användare kontrollerade sin egen huvudbok och giltigheten av varje transaktion, så länge alla noder är uppdaterade borde huvudböckerna förbli synkroniserade över nätverket. Detta mycket distribuerade system skulle vara svårt att korrumpera.

Wei Dai insåg att detta inte löste bysantinska generalers problem (1), eftersom noder lätt kunde tappa synkronisering eller helt enkelt ljuga. Han föreslog alternativa metoder såsom att ha en delmängd av 'betrodda' servrar som underhåller huvudboken, och skapa ekonomiska incitament för att hålla dessa servrar ärliga.

För penningpolitiken föreslog han att knyta B-Moneys köpkraft till någon form av extern konsumentprisindex. Han ville att samma mängd B-Money skulle kunna köpa en lika stor andel av indexet över tid, för att ge viss prisstabilitet. Så, vem som helst kunde skapa nya valutaenheter genom att tillhandahålla en giltig hash, men svårighetsgraden för att generera en hash kunde förändras över tid baserat på CPU-kostnader och prisindex, så att varje enhet skulle vara 'oföränderlig'.
