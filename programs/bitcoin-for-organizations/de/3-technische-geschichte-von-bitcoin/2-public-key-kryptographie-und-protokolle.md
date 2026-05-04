# 3.2 Public-Key-Kryptographie und Protokolle

Das heutige Internet und die meisten modernen Computersysteme basieren auf Kryptographie, einer Methode, Informationen so zu verschleiern, dass nur der Empfänger sie entschlüsseln kann. Die Grundlagen der Kryptographie, die zur Absicherung von Bitcoin verwendet wird, lassen sich bis in die 1970er Jahre zurückverfolgen.

Das erste Problem, das gelöst werden muss, ist: Wie kann ein gemeinsames Geheimnis über ein unsicheres Medium übertragen werden?

Dies wurde erstmals von Whitfield Diffie und Martin Hellman untersucht.

Das Problem: Die beiden Parteien – üblicherweise als Alice und Bob bezeichnet – möchten geheime Informationen über ein Netzwerk austauschen, in dem andere möglicherweise mithören. Um dies zu erreichen, entwickelten sie den Diffie-Hellman-Schlüsselaustausch.

Dieses gemeinsame Geheimnis kann dann als Ausgangswert verwendet werden, um zahlreiche symmetrische Schlüssel zu erzeugen, mit denen Nachrichten verschlüsselt und entschlüsselt werden können, ohne den Schlüssel selbst offen zu teilen.

Da der private Schlüssel niemals geteilt werden muss und an jedem Ende unterschiedliche Schlüssel zum Ver- und Entschlüsseln verwendet werden, spricht man hierbei von einem asymmetrischen Verschlüsselungsalgorithmus.

Anwendungsfälle:

* Alice signiert eine Nachricht mit Bobs öffentlichem Schlüssel – nur er kann sie mit seinem privaten Schlüssel entschlüsseln.
* Alice signiert eine Nachricht mit ihrem privaten Schlüssel – durch Entschlüsselung mit ihrem öffentlichen Schlüssel kann jeder verifizieren, dass die Nachricht von Alice gesendet wurde, ohne ihren privaten Schlüssel zu kennen.
* Kombiniert man diese beiden Ansätze mit zwei Verschlüsselungsebenen, kann eine Nachricht so verschlüsselt gesendet werden, dass nur Bob sie entschlüsseln kann, und er kann anschließend den Absender als Alice verifizieren.

Obwohl er nicht als Autor des Papiers genannt wurde, war Ralph Merkle maßgeblich daran beteiligt, das bis dahin als unlösbar geltende Rätsel zu lösen – wie man private Kommunikation über ein offenes und potenziell feindliches Netzwerk aufbauen oder wiederherstellen kann.

Dieser Ansatz allein ist anfällig für einen Brute-Force-Angriff, bei dem ein Angreifer die geteilten Zahlen nehmen und mit genügend Zeit und Ressourcen schließlich einen gemeinsamen Schlüssel rekonstruieren kann. Daher ist dies allein noch keine vollständige Lösung.

##### Protokolle für Public-Key-Kryptosysteme

Neben seinem Beitrag zum oben beschriebenen Diffie-Hellman-Public-Key-System**Ralph Merkle** trug über viele Jahre weiterhin zu diesem Bereich bei und war maßgeblich an der Entwicklung einiger Schlüsselkomponenten beteiligt, die von Bitcoin verwendet werden.

Eine kryptographische Hashfunktion ist ein mathematischer Algorithmus, der Eingaben beliebiger Größe entgegennimmt und komplexe Berechnungen durchführt, um einen Hashwert in Bits zurückzugeben, der üblicherweise als alphanumerischer Ausgabewert fester Länge im Hexadezimalformat dargestellt wird.

* Eingaben können beliebige Größe haben
* Die Ausgabe hat immer eine feste Länge und ist deterministisch (gleiche Eingabe erzeugt jedes Mal denselben Hash)
* Es ist einfach zu überprüfen, aber äußerst schwierig, den Prozess umzukehren, um die Eingabe zu bestimmen.
* Eine kleine Änderung der Daten verändert die Ausgaben vollständig.

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/ab607f492f0e92ccfbe9c65abf07a30a48b9e528-515x331.svg)

Hashing ist ein integraler Bestandteil des Bitcoin-Protokolls. SHA-256, das in Bitcoin verwendet wird, wurde von der NSA entwickelt und ist ein Beispiel für einen kryptographischen Hashalgorithmus.

* Jeder Block in der Kette wird gehasht, sodass Daten nicht verändert werden können – dies gewährleistet die Integrität des verteilten Ledgers.
* Der erzeugte Hash muss die Kriterien des 'Proof of Work' erfüllen, um als gültiger Block zu gelten.
* Merkle-Bäume – durch Verzweigungen und Hashes von Hashes ermöglichen Hash-Bäume die Verifizierung großer Datensätze mit minimalem Speicherbedarf.
* Hashbasierte Signaturen und Schlüssel können für Wallets, Adressen und die Autorisierung von Transaktionen verwendet werden.

Die verteilte Verifizierung von Blockchain-Zuständen und unveränderlichen Ledger-Modellen, die gegen nachträgliche Änderungen resistent sind, wird durch Einweg-Hashing ermöglicht. Hashfunktionen bieten den zuverlässigen, deterministischen Ansatz, um Ereignisse auf öffentlichen Ledgers wie Bitcoin ohne ein zentrales Vertrauensmodell zu verifizieren.

Diese neuen Möglichkeiten im Bereich der Kryptographie sollten nach Ansicht ihrer Erfinder eine neue Welle der Innovation in diesem Bereich einleiten.

##### Elliptische-Kurven-Kryptographie

Eine dieser späteren Innovationen war die elliptische-Kurven-Kryptographie.

Die elliptische-Kurven-Kryptographie wurde 1985 von zwei Wissenschaftlern, N. Koblitz und V. Miller, eingeführt. Sie schlugen vor, Punkte, die durch elliptische Kurven definiert sind, anstelle der endlichen Primkörper zu verwenden, sodass das Diskrete-Logarithmus-Problem wie beim Standard-Diffie-Hellman-Schlüsselaustauschprotokoll gilt. Die Details, wie dies funktioniert, gehen über den Rahmen dieses Abschnitts hinaus, aber auf hoher Ebene ist eine elliptische Kurve die Menge aller Punkte, die eine bestimmte mathematische Gleichung erfüllen.

Die Gleichung für eine elliptische Kurve sieht ungefähr so aus:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Dies hat einige nützliche Eigenschaften:

* Horizontale Symmetrie. Jeder Punkt auf der Kurve kann an der x-Achse gespiegelt werden und bleibt auf derselben Kurve.
* Jede nicht-vertikale Gerade schneidet die Kurve höchstens an drei Stellen.
* Kompakte Schlüssellängen sind entscheidend für die effiziente Speicherung und Übertragung von öffentlichen Schlüsseln in der Blockchain.

Diese Eigenschaften können genutzt werden, um Schlüsselpaaren ähnlich wie beim Diffie-Hellman-Algorithmus zu erzeugen. Bitcoin verwendet ECDSA, was für Elliptic Curve Digital Signature Algorithm steht. Es handelt sich um einen Prozess, bei dem eine elliptische Kurve und ein endliches Feld verwendet werden, um Daten so zu „signieren“, dass Dritte die Echtheit der Signatur überprüfen können, während der Unterzeichner die exklusive Fähigkeit behält, die Signatur zu erstellen. Bei Bitcoin sind die zu signierenden Daten die Transaktion, die den Besitz überträgt.

Der 'endliche' Teil ist ähnlich wie beim 'mod'-Ansatz bei Diffie-Hellman, bei dem das Ergebnis der Gleichung geteilt und der Rest verwendet wird, um sicherzustellen, dass es in einen bestimmten Zahlenbereich passt.
