# 3.4 Hashcash

Hashcash a fost creat de Adam Back, un alt inovator timpuriu în acest domeniu. Adam avea un interes puternic pentru piețele libere și pentru confidențialitatea pe internet și a descoperit lista de discuții Cypherpunks, la care s-a alăturat și a devenit un participant activ.

Era foarte interesat de banii digitali și a făcut câteva sugestii despre cum grupul ar putea colabora mai strâns cu Chaum la DigiCash, dar aceste idei nu au avut succes. Apoi și-a îndreptat atenția către o altă problemă emergentă – spamul pe email. El și ceilalți membri Cypherpunks doreau să găsească o soluție la problema spamului, unde era foarte ușor pentru spammeri să creeze și să trimită mii de emailuri care aglomerau rețelele. Soluția sa inovatoare se baza pe hashing – capacitatea criptografiei de a transforma orice bucată de date într-un șir unic și aleatoriu de o lungime specifică, pentru a crea echivalentul unei „ștampile” digitale care trebuia adăugată emailului pentru ca acesta să fie considerat valid și transmis prin rețea. Un cost nesemnificativ pentru un email autentic, dar prohibitiv pentru un spammer.

Inovația cheie pe care a adus-o Hashcash a fost legarea resurselor din lumea reală – puterea de calcul – de o rețea digitală. În timp ce resursele digitale până la acel moment puteau fi replicate fără limite, numărul de „hashcash” creat era limitat de câtă energie erau oamenii dispuși să investească.

Deși soluția îndeplinea unele dintre criteriile pe care Adam le considera necesare pentru un sistem de bani digitali; era anonimă, rezistentă și fără încredere, fiecare hashcash nu era reutilizabil și nici cu adevărat rar. El a sugerat alte modalități prin care aceste probleme ar putea fi abordate folosind terți externi.

##### BitGold

Nick Szabo a dezvoltat conceptul de Hashcash și dovada muncii pentru a propune o soluție alternativă, pe care a descris-o pe o listă de discuții la un an după publicarea Hashcash, în 1998.

Deși se apropia de o soluție, această propunere avea încă mai multe provocări.

* Cine ar administra Registrul deținerii hash-urilor și cum ar putea fi de încredere?
* Hashing-ul ar deveni în general mai ieftin în timp, o provocare și pentru HashCash.

Deoarece hash-urile legate ar fi marcate temporal, el a propus o formă de urmărire istorică a dificultății hashing-ului la momentul respectiv; un hash mai vechi ar necesita mai multe costuri de procesare decât unul mai nou, deoarece costurile au scăzut. Din păcate, asta însemna că hash-urile nu ar fi „fungibile”, adică de valoare egală, considerat un atribut cheie al banilor digitali. Pentru a ajuta la rezolvarea acestei probleme, Nick a sugerat o formă de „free banking” care să funcționeze peste BitGold și să poată agrega diferite grupuri de hash-uri care să fie evaluate la fel.

##### B-Money

La scurt timp după propunerea Bit Gold, Wei Dai a propus o soluție similară. El dezvoltase deja mai multe alte instrumente pentru Cypherpunks și avea propriile sale idei despre banii digitali.

Propunerea sa semăna cu Bit Gold prin faptul că folosea semnături digitale pentru a transfera bani, iar înregistrările tranzacțiilor ar fi stocate într-un registru, conținând chei publice și suma de unități monetare atribuite fiecăreia. Ca și la Bit-Gold, terții de încredere erau considerați puncte slabe de securitate, iar convingerea era că un sistem de bani electronici nu ar trebui să se bazeze pe o singură entitate pentru a urmări soldurile, tranzacțiile sau pentru a preveni dubla cheltuire.

Wei Dai a propus mai multe soluții pentru aceste probleme, una dintre ele fiind ca, în loc ca o entitate centrală să mențină registrul, TOATE nodurile să păstreze o copie. Dacă toți utilizatorii își verifică propriul registru și validitatea fiecărei tranzacții, atâta timp cât toate nodurile rămân actualizate, registrele ar trebui să rămână sincronizate în întreaga rețea. Acest sistem extrem de distribuit ar fi dificil de corupt.

Wei Dai a recunoscut că aceasta nu rezolva problema generalilor bizantini (1), deoarece nodurile puteau pierde ușor sincronizarea sau puteau minți pur și simplu. El a sugerat metode alternative, cum ar fi existența unui subset de servere „de încredere” care să mențină registrul și crearea unor stimulente financiare pentru a menține aceste servere oneste.

Pentru politica monetară, el a propus ancorarea puterii de cumpărare a B-Money la o formă de indice extern al prețurilor de consum. Dorea ca aceeași cantitate de B-Money să poată cumpăra o cotă egală din indice în timp, oferind astfel o anumită stabilitate a prețului. Astfel, oricine putea genera noi unități monetare furnizând un hash valid, dar dificultatea generării unui hash putea varia în timp în funcție de costurile CPU și de indicele de prețuri, astfel încât fiecare unitate să fie „imutabilă”.
