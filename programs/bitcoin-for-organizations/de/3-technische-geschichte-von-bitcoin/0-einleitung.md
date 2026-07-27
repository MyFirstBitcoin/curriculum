# 3.0 Einleitung

> **Dark – Die Zusammenfassung des Bitcoin-Whitepapers**
>
> **Eine rein Peer-to-Peer-Version von elektronischem Geld** würde es ermöglichen, Online-Zahlungen direkt von einer Partei zur anderen zu senden, ohne eine Finanzinstitution zu durchlaufen. **Digitale Signaturen liefern einen Teil der Lösung**, aber die Hauptvorteile gehen verloren, wenn eine **vertrauenswürdige dritte Partei** weiterhin erforderlich ist, um Doppel-Ausgaben zu verhindern. Wir schlagen eine Lösung für das Problem der Doppel-Ausgaben vor, die ein **Peer-to-Peer-Netzwerk** verwendet. Das **Netzwerk versieht Transaktionen mit Zeitstempeln**, indem es sie in eine fortlaufende Kette von **Hash-basiertem Proof-of-Work** einfügt und so einen Datensatz bildet, der nicht verändert werden kann, ohne den **Proof-of-Work** erneut durchzuführen. Die längste Kette dient nicht nur als Nachweis der beobachteten Ereignisabfolge, sondern auch als Beweis dafür, dass sie aus dem größten Pool an Rechenleistung stammt. Solange die Mehrheit der Rechenleistung von Knoten kontrolliert wird, die nicht zusammenarbeiten, um das Netzwerk anzugreifen, werden sie die längste Kette erzeugen und Angreifer überholen.**Das Netzwerk selbst erfordert nur minimale Struktur. Nachrichten werden nach bestem Bemühen übertragen, und Knoten können das Netzwerk nach Belieben verlassen und wieder beitreten**, wobei sie die längste Proof-of-Work-Kette als Nachweis dessen akzeptieren, was während ihrer Abwesenheit geschehen ist.


Bitcoin ist nicht aus dem Nichts entstanden, sondern baut auf der Arbeit vieler Menschen in den vergangenen Jahrzehnten auf. Dieses Modul wird die Grundlagen des Internets untersuchen, auf denen Bitcoin aufbaut, sowie die im Whitepaper anerkannten Forschungen und Entwicklungen.

In den 70er Jahren betrachtete eine Gruppe von Personen, wie insbesondere die US-Regierung versuchte, den Zugang zu Kryptographie einzuschränken, und setzte sich dafür ein, dass diese Technologie allen Menschen zur Verfügung steht, um ihre Privatsphäre online zu schützen. Einige dieser frühen Pioniere konzentrierten sich auch auf die potenziellen Vorteile eines digitalen ‚harten Geldes‘, das zur Wertaufbewahrung und zum Austausch über das entstehende Internet genutzt werden könnte. Friedrich Hayek – ein führender Vertreter der Österreichischen Schule der Ökonomie – stellte sich schon lange vor dem Internet vor, wie eine ideale Währung auf Basis von freiem Wettbewerb aussehen könnte, hielt dies jedoch für technisch und politisch nicht umsetzbar. Neben digitaler Privatsphäre versuchte diese Gruppe, die später als Cypherpunks bekannt wurde, Hayeks Vision von digitalem Geld zu verwirklichen, doch diese Versuche scheiterten, bis Satoshi seine Ideen auf der Mailingliste veröffentlichte.

* TCP/IP-Protokoll (1976)
* Protokolle für Public-Key-Kryptosysteme – Ralph Merkle (1980)
* Digicash – David Chaum (1989)
* Digitale Zeitstempelung (90er Jahre)
* Hashcash – Adam Back (1997)
* BitTorrent – Bram Cohen (2001)
* Wiederverwendbarer POW – Hal Finney (2004)
* Bitcoin-Whitepaper – Satoshi Nakamoto (2008)

Ein entscheidender Einfluss auf die Entwicklung von Bitcoin war das Aufkommen der Cypherpunk-Bewegung in den 1990er Jahren. Sie entwickelten mehrere kryptographische Technologien, darunter die Public-Key-Kryptographie, um Nutzern eine sichere und private Kommunikation und Informationsaustausch zu ermöglichen. Viele der hier beschriebenen Entwicklungen und beteiligten Personen gehörten zu dieser Gruppe.

Auch der Bedarf an digitalem Geld wurde erkannt und es gab mehrere Versuche, dieses zu schaffen, doch diese hatten Einschränkungen, die ihren Erfolg verhinderten. Das Genie von Satoshi Nakamoto bestand darin, diese Fähigkeiten zusammenzuführen und mit einigen eigenen Innovationen darauf aufzubauen, um das heute verwendete Bitcoin-Protokoll zu schaffen. In den nächsten Abschnitten werden wir einige dieser Entwicklungen untersuchen und erklären, wie sie das Design von Bitcoin beeinflusst haben. Wir werden auch darauf eingehen, welche fehlenden Puzzleteile Satoshi lösen konnte.
