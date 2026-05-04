# 3.4 Hashcash

Hashcash wurde von Adam Back entwickelt, einem weiteren der frühen Innovatoren in diesem Bereich. Adam hatte ein starkes Interesse an freien Märkten und Privatsphäre im Internet und stieß auf die Cypherpunks-Mailingliste, der er beitrat und zu einem aktiven Teilnehmer wurde.

Er war sehr an digitalem Geld interessiert und machte einige Vorschläge, wie die Gruppe möglicherweise enger mit Chaum an DigiCash zusammenarbeiten könnte, aber daraus wurde nichts. Dann richtete er seine Aufmerksamkeit auf ein anderes aufkommendes Problem – E-Mail-Spam. Er und die anderen Cypherpunks wollten eine Lösung für das Spam-Problem finden, bei dem es für Spammer trivial war, Tausende von E-Mails zu erstellen und zu versenden, die Netzwerke verstopfen. Seine innovative Lösung basierte auf Hashing – der Fähigkeit der Kryptografie, beliebige Daten in eine einzigartige und zufällige Zeichenkette einer bestimmten Länge zu verwandeln, um das Äquivalent einer digitalen „Briefmarke“ zu schaffen, die der E-Mail hinzugefügt werden musste, damit sie als gültig gilt und über das Netzwerk übertragen werden konnte. Ein triviales Kosten für eine echte E-Mail, aber für einen Spammer unerschwinglich.

Die entscheidende Innovation, die Hashcash brachte, war die Verknüpfung von realen Ressourcen – Rechenleistung – mit einem digitalen Netzwerk. Während digitale Ressourcen bis zu diesem Zeitpunkt unbegrenzt repliziert werden konnten, war die Anzahl der erzeugten „Hashcash“ dadurch begrenzt, wie viel Energie die Menschen bereit waren, dafür aufzuwenden.

Obwohl die Lösung einige der Kriterien erfüllte, die Adam für ein digitales Geldsystem als notwendig erachtete – sie war anonym, widerstandsfähig und vertrauenslos –, war jedes Hashcash nicht wiederverwendbar und nicht wirklich knapp. Er schlug andere Wege vor, wie diese Probleme durch externe Dritte gelöst werden könnten.

##### BitGold

Nick Szabo baute auf dem Konzept von Hashcash und Proof of Work auf, um eine alternative Lösung vorzuschlagen, die er ein Jahr nach der Veröffentlichung von Hashcash, 1998, in einer Mailingliste beschrieb.

Obwohl diese Lösung dem Ziel näher kam, gab es immer noch mehrere Herausforderungen.

* Wer würde das Register des Hash-Besitzes führen und wie könnte man ihnen vertrauen?
* Hashing würde im Laufe der Zeit im Allgemeinen günstiger werden, was auch für HashCash eine Herausforderung darstellte.

Da die verknüpften Hashes mit einem Zeitstempel versehen würden, schlug er eine Art historische Nachverfolgung der Hashing-Schwierigkeit zu diesem Zeitpunkt vor; ein früherer Hash würde mehr Verarbeitungskosten erfordern als ein späterer, da die Kosten gesunken sind. Leider bedeutete dies, dass Hashes nicht „fungibel“ wären, d. h. von gleichem Wert – ein zentrales Merkmal von digitalem Geld. Um dieses Problem zu lösen, schlug Nick eine Art „Free Banking“ vor, das auf BitGold aufbaut und verschiedene Gruppen von Hashes zusammenfassen könnte, die dann gleich bewertet würden.

##### B-Money

Kurz nach dem Bit-Gold-Vorschlag schlug Wei Dai eine ähnliche Lösung vor. Er hatte bereits mehrere andere Werkzeuge für die Cypherpunks entwickelt und eigene Ideen zum digitalen Geld.

Sein Vorschlag ähnelte Bit Gold insofern, als er digitale Signaturen zur Übertragung von Geld verwendete und die Aufzeichnungen der Transaktionen in einem Ledger gespeichert würden, das öffentliche Schlüssel und die jedem zugeordneten Währungseinheiten enthielt. Wie bei Bit-Gold galten vertrauenswürdige Dritte als Sicherheitslücken, und die Überzeugung war, dass ein elektronisches Geldsystem nicht auf eine einzelne Instanz angewiesen sein sollte, um Salden, Transaktionen oder die Verhinderung von Double-Spending zu überwachen.

Wei Dai schlug mehrere Lösungen für diese Probleme vor, darunter, dass anstelle einer zentralen Instanz ALLE Knoten eine Kopie des Ledgers führen sollten. Wenn alle Nutzer ihr eigenes Ledger und die Gültigkeit jeder Transaktion überprüften, sollten die Ledgers im Netzwerk synchron bleiben, solange alle Knoten auf dem neuesten Stand sind. Dieses stark verteilte System wäre schwer zu korrumpieren.

Wei Dai erkannte, dass dies das Problem der byzantinischen Generäle (1) nicht löste, da Knoten leicht die Synchronisation verlieren oder einfach lügen könnten. Er schlug alternative Methoden vor, wie z. B. eine Teilmenge von „vertrauenswürdigen“ Servern, die das Ledger führen, und finanzielle Anreize, um diese Server ehrlich zu halten.

Für die Geldpolitik schlug er vor, die Kaufkraft von B-Money an eine Art externen Verbraucherpreisindex zu koppeln. Er wollte, dass die gleiche Menge B-Money im Laufe der Zeit einen gleichen Anteil am Index kaufen kann, um eine gewisse Preisstabilität zu gewährleisten. So konnte jeder neue Währungseinheiten erzeugen, indem er einen gültigen Hash bereitstellte, aber die Schwierigkeit, einen Hash zu erzeugen, könnte sich im Laufe der Zeit je nach CPU-Kosten und Preisindex ändern, sodass jede Einheit „unveränderlich“ wäre.
