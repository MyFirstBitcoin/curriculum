# 6 - Wie man Bitcoin verwendet

Dauer: 90 Minuten

Kernidee: Die Nutzung von Bitcoin On-Chain vermittelt den Schülern praktisch, wie Besitz, Selbstverwahrung und Verifizierung funktionieren, und verwandelt Theorie in direkte finanzielle Handlung.

#### Lernziele

Am Ende dieser Lektion sollten die Schüler in der Lage sein:

* Gängige Möglichkeiten zum Erwerb und Tausch von Bitcoin identifizieren, einschließlich Peer-to-Peer- und zentralisierter Börsenmethoden.
* Den Unterschied zwischen selbstverwahrten und verwahrten Wallets erklären und erläutern, warum Selbstverwahrung bei Bitcoin wichtig ist.
* Den Zweck von privaten Schlüsseln, öffentlichen Adressen, Seed-Phrasen und Wallet-Oberflächen beschreiben.
* Verschiedene Wallet-Typen vergleichen und deren Vor- und Nachteile in Bezug auf Sicherheit, Komfort, Privatsphäre und Kontrolle bewerten.
* Eine mobile Bitcoin-Wallet einrichten und den grundlegenden Wiederherstellungsprozess erklären.
* Demonstrieren, wie man eine On-Chain-Bitcoin-Transaktion empfängt und sendet.

Das Prinzip „Vertraue nicht, überprüfe“ auf die Wallet-Auswahl, Transaktionen und die allgemeine Bitcoin-Nutzung anwenden.

#### Werkzeuge & Ressourcen

##### Visuelle Hilfsmittel

* Kapitel 6 – Wie man Bitcoin benutzt

##### Unterstützungsbibliothek

* Vokabelkarte — Kapitel 6 — Begriffe: Wallet, privater Schlüssel, öffentliche Adresse, Seed-Phrase, Verwahrung, Selbstverwahrung, UTXO, Transaktionsgebühr
* Vergleichstabellen & Übersichtsblätter — Vergleich der Wallet-Typen (verwahrt, mobil, Hardware, Papier)
* Technische Erklärungen & Deep-Dives — Öffentliche/private Schlüssel, UTXO-Modell, Transaktionsbestätigung
* Deep-Dive zur Sicherheit privater Schlüssel — Seed-Phrasen, Schlüsselableitung, Backup-Methoden, Angriffsvektoren
* Anatomie einer Transaktion — Schritt-für-Schritt-Beispiel, wie eine Bitcoin-Transaktion funktioniert
* Checkliste für bewährte Sicherheitspraktiken — Vor dem Start, Wallet-Erstellung, Empfangen, Senden, Phishing-Prävention

#### Aktivitäten

* Transaktionen in Aktion
* Lightning-Staffellauf
* Die Mempool erkunden

#### Online-Unterricht

* Stellen Sie von Anfang an klar, ob die Schüler eine Demo ansehen oder selbst eine Wallet einrichten.
* Verwenden Sie große, gut lesbare Screenshots für jeden Schritt der Wallet-Einrichtung.
* Machen Sie nach jedem Schritt eine Pause und bitten Sie die Schüler, das Verständnis im Chat zu bestätigen, bevor Sie fortfahren.
* Geben Sie eine direkte Warnung vor dem Abschnitt zur Seed-Phrase und erinnern Sie die Schüler daran, niemals sensible Informationen online zu teilen.

#### Vorbereitung

* Laden Sie eine mobile Wallet-App herunter und testen Sie sie (Blue Wallet oder Muun); bereiten Sie Screenshots der wichtigsten Einrichtungsschritte vor.
* Bereiten Sie eine Anleitung zur Wallet-Einrichtung vor (Download → Erstellen → Seed-Backup → Empfangen) als Referenz.
* Stellen Sie sicher, dass das Netzwerk/WLAN funktioniert; halten Sie eine Demo-Adresse und einen QR-Code bereit.

#### Ablauf

Diese Lektion geht von der Theorie in die direkte Praxis über. Sie entspricht nun direkt der Struktur des Diploms, sodass Erwerb, Wallets, Einrichtung, Transaktionen und Verifizierung unter denselben Hauptüberschriften wie im Schülerleitfaden erscheinen. Zusätzliche Unterrichtshilfen bleiben innerhalb dieser Abschnitte eingebettet.

##### 6.0 Einführung, 8 Minuten

Beginnen Sie damit, dieses Kapitel mit dem vorherigen zu verbinden:

* Wenn Bitcoin Geld ist, wie bekommen und benutzen Menschen es eigentlich?
* Was bedeutet es, seine Bitcoin wirklich zu kontrollieren?
* Warum ist die Nutzung von Bitcoin anders als die Nutzung einer Banking-App?

Stellen Sie klar, dass es in diesem Kapitel um die praktische Anwendung geht. Die Schüler lernen nicht mehr nur, was Bitcoin ist, sondern wie sie direkt damit interagieren.

##### 6.1 Bitcoin erwerben und tauschen, 12 Minuten

Erklären Sie, dass Menschen Bitcoin auf verschiedene Arten erwerben können, darunter:

* in Bitcoin bezahlt werden
* Bitcoin minen
* Fiat gegen Bitcoin persönlich tauschen
* Fiat gegen Bitcoin online tauschen

Konzentrieren Sie sich dann auf die beiden wichtigsten Erwerbswege, die im Kapitel behandelt werden:

* Peer-to-Peer, persönlich
* Peer-to-Peer, online
* Zentralisierte Börsen

Machen Sie die Kompromisse deutlich.

Bei P2P vor Ort betonen Sie den direkten Austausch ohne Bank oder Vermittler, erwähnen Sie aber auch die praktischen Risiken, die mit dem Treffen von Personen für Bargeldgeschäfte verbunden sind.

Für P2P online erklären Sie Treuhand (Escrow) in einfachen Worten, als eine Möglichkeit, das Gegenparteirisiko zu verringern, während dennoch ein direkter Austausch zwischen den Teilnehmern möglich ist.

Für zentralisierte Börsen machen Sie klar, dass sie bequem sind, aber die Nutzer einer Firma vertrauen müssen, oft persönliche Informationen teilen und die Gelder bis zur Abhebung unter Kontrolle Dritter stehen. Hier ist ein guter Moment, um zu betonen, dass Bequemlichkeit oft mit Einbußen bei Privatsphäre und Souveränität einhergeht.

##### 6.2 Eine Einführung in Bitcoin-Wallets, 35 Minuten

**Was ein Bitcoin-Wallet wirklich ist**

Klären Sie gleich zu Beginn ein häufiges Missverständnis: Bitcoin wird nicht wie Bargeld in einer Tasche in der Wallet-App gespeichert.  
Die Bitcoin existieren auf dem von dem Netzwerk geführten Hauptbuch. Was der Nutzer kontrolliert, ist die Möglichkeit, sie über private Schlüssel auszugeben.

Erklären Sie dann die zwei Dinge, die Menschen oft mit „Wallet“ meinen:

* das System der privaten Schlüssel, aus denen Adressen generiert werden
* die App oder Oberfläche, die zur Interaktion mit dem Netzwerk verwendet wird

Nutzen Sie bei Bedarf die E-Mail-Analogie aus dem Kapitel:

* öffentliche Adresse = wie eine E-Mail-Adresse, die Sie weitergeben können
* privater Schlüssel = wie ein Passwort, das Sie schützen müssen

Seien Sie hier sehr deutlich: Wer die privaten Schlüssel kontrolliert, kontrolliert die Bitcoin. Das ist das zentrale Konzept, das die Lernenden verstehen müssen.

**Selbstverwahrte vs. Verwahrte Wallets**

Dies ist einer der wichtigsten Abschnitte des Kapitels.

Erklären Sie den Unterschied klar:

* Selbstverwahrte Wallet: Der Nutzer kontrolliert die privaten Schlüssel
* Verwahrte Wallet: Ein Dritter kontrolliert die privaten Schlüssel im Auftrag des Nutzers

Gehen Sie dann die jeweiligen Vor- und Nachteile durch:

Selbstverwahrung

* volle Kontrolle über die Gelder
* kein Genehmigungsprozess
* Schutz vor willkürlicher Beschlagnahmung
* größere Eigenverantwortung
* keine einfache Wiederherstellung, wenn die Seed-Phrase verloren geht

Verwahrung

* einfachere Wiederherstellung und Unterstützung
* einfacher für Anfänger
* stärker gefährdet durch Kontosperrungen, Hacks und Kontrolle Dritter
* Der Nutzer hält die Bitcoin nicht wirklich selbst

Dies ist der richtige Moment, um den Satz zu betonen:

„Nicht deine Schlüssel, nicht deine Coins.“

Die Lernenden sollten diesen Abschnitt nicht nur mit dem Slogan verlassen, sondern auch verstehen, was er in der Praxis bedeutet.

**Verschiedene Arten von Wallets und wie man eines auswählt**

Stellen Sie die im Kapitel behandelten Wallet-Typen vor:

* Online-Wallet
* Mobile Wallet
* Desktop-Wallet
* Hardware-Wallet
* Paper-Wallet

Behandeln Sie keines als perfekt. Erklären Sie stattdessen, dass jede Variante Kompromisse zwischen folgenden Aspekten erfordert:

* Sicherheit
* Privatsphäre
* Bequemlichkeit
* Kompatibilität
* Gebühren
* Kontrolle
* Ruf

Machen Sie außerdem deutlich, dass wir empfehlen, darauf zu achten, ob Wallet-Software Open Source ist, da Open-Source-Tools von der Community überprüft, geprüft und weiterentwickelt werden können. Dies steht in direktem Zusammenhang mit dem Prinzip der Verifizierung bei Bitcoin.

##### 6.3 Einrichten einer mobilen Bitcoin-Wallet, 10 Minuten

Führen Sie die Lernenden durch den im Kapitel gezeigten grundlegenden Ablauf:

* Wallet herunterladen
* eine neue Wallet erstellen
* die Wiederherstellungsphrase generieren und aufschreiben
* die Wiederherstellungsphrase bestätigen
* zusätzliche Sicherheit hinzufügen, falls verfügbar
* die Wallet öffnen und die Empfangsfunktion finden

Machen Sie die Warnung zur Seed-Phrase sehr deutlich:

* wenn die Seed-Phrase verloren geht, kann der Zugriff auf die Gelder verloren gehen
* wenn jemand anderes die Seed-Phrase erhält, kann er die Gelder stehlen

Wenn die Lernenden dies praktisch durchführen, sollte die Lehrkraft bei jedem Schritt pausieren und überprüfen, ob alle verstehen, was sie tun. Ist der Unterricht eher konzeptionell, kann dieser Abschnitt als Durchgang erklärt werden, anstatt ihn live durchzuführen. Die im Kapitel gezeigte Wiederherstellungsoption ist auch nützlich, um zu erklären, dass Wallets wiederhergestellt werden können, wenn die Seed-Phrase korrekt gesichert wurde.

##### 6.4 Empfangen und Senden von Transaktionen, 17 Minuten

**Empfangen und Senden von On-Chain-Transaktionen**

Erklären Sie nun, wie On-Chain-Transaktionen funktionieren.

Zum Empfangen von Bitcoin:

* Wallet öffnen
* auf Empfangen oder Einzahlen tippen
* die Adresse kopieren, den Link teilen oder den QR-Code anzeigen

Zum Senden von Bitcoin:

* Wallet öffnen
* die Adresse des Empfängers einfügen oder scannen
* den Betrag eingeben
* alle Angaben sorgfältig überprüfen
* die Transaktion senden
* auf die Bestätigung warten

Machen Sie diese Schlüsselpunkte deutlich:

* die Transaktion überträgt das Eigentum, nicht physische Münzen
* Transaktionen sind unumkehrbar
* Nodes überprüfen die Gültigkeit
* Miner nehmen Transaktionen in Blöcke auf
* Gebühren beeinflussen die Bestätigungspriorität
* On-Chain-Transaktionen sind im Allgemeinen sicher, aber langsamer und oft teurer als Lightning-Transaktionen

Das Transaktionsflussdiagramm im Kapitel ist hier besonders hilfreich, da es den Lernenden hilft, den Weg von der Wallet-Anfrage bis zur Bestätigung im Netzwerk zu visualisieren.

**Transaktionen in Aktion und rollenbasierte Übung**

Nutzen Sie die kooperative Übungsstruktur aus dem Kapitel, um das Verständnis zu festigen. Erklären Sie die vier beteiligten Rollen:

* Absender
* Empfänger
* Miner
* Node-Betreiber

Ein einfacher Ansatz im Unterricht ist es, Rollen zu vergeben und eine Transaktion Schritt für Schritt durchzugehen. So sehen die Lernenden, dass eine Bitcoin-Transaktion kein Zauber ist, sondern ein koordinierter Prozess, der Genehmigung, Überprüfung, Aufnahme in einen Block und Aktualisierung des Ledgers umfasst.

Das Ziel hier ist nicht technische Tiefe. Es geht darum, den Lernenden zu helfen zu verstehen, wer was bei einer Transaktion macht und warum Verifizierung wichtig ist.

##### 6.5 Nicht vertrauen, sondern verifizieren, 8 Minuten

Erklären Sie, dass dies gilt für:

* Wallets
* Börsen
* Apps
* Transaktionsdetails
* Behauptungen über "leichte Gewinne"
* Projekte, die vorgeben, wie Bitcoin zu sein

Machen Sie deutlich, dass Bitcoin von den Nutzern verlangt, kritisch zu denken, zu überprüfen, was sie verwenden, und blindes Vertrauen zu vermeiden. Erklären Sie außerdem, warum Open-Source-Tools in diesem Zusammenhang wichtig sind: Sie ermöglichen unabhängige Überprüfung.

###### Abschluss und Verständnisüberprüfung

Schließen Sie mit ein paar kurzen Fragen ab:

* Was ist der Unterschied zwischen einer Verwahrungs- und einer Selbstverwahrungs-Wallet?
* Warum ist die Seed-Phrase so wichtig?
* Was passiert, wenn Sie eine On-Chain-Transaktion senden?
* Warum sind On-Chain-Transaktionen langsamer als einige andere Bitcoin-Zahlungen?
* Was bedeutet "Nicht vertrauen, sondern überprüfen" in der Praxis?

#### Hinweise für Lehrkräfte

Dieses Kapitel ist sehr praxisorientiert, daher sollten Klarheit, Sicherheit und Wiederholung im Vordergrund stehen.

Die Schüler müssen nicht jede Wallet-Art in einer Stunde beherrschen. Die Hauptziele sind:

* Verständnis der Wallet-Grundlagen
* Verständnis von Selbstverwahrung
* Erlernen des grundlegenden Transaktionsablaufs
* Entwicklung einer verantwortungsvollen Überprüfungsmentalität

Seien Sie besonders vorsichtig, wenn Sie Seed-Phrasen und die Einrichtung von Wallets besprechen. Die Schüler sollten verstehen, dass dies keine Nebensächlichkeiten sind, sondern die Grundlage des Bitcoin-Besitzes.

Die nützlichsten Visualisierungen und Aktivitäten in diesem Kapitel sind:

* der Vergleich Selbstverwahrung vs. Verwahrung
* die Tabelle zu Wallet-Typen und deren Kompromissen
* die Schritt-für-Schritt-Übung zur Wallet-Einrichtung
* das Diagramm zum Transaktionsablauf
* die rollenbasierte Transaktionsaktivität

##### Was gutes Lernen ausmacht

* Es ist wichtig, dass die Schüler tatsächlich eine Wallet einrichten oder eine sorgfältige Demo ansehen, die Seed-Phrase als Mittelpunkt mit "Diese 12 Wörter SIND dein Bitcoin" hervorheben, Szenarien wie "Was passiert, wenn du dein Handy verlierst?" durchspielen und das Erkennen von Phishing üben.
* Lehrkräfte sollten praktische Begleiter sein, die dies schon einmal gemacht haben, sicherheitsbewusst ohne Paranoia agieren und ehrlich über die Lernkurve und den nötigen Lernaufwand sprechen.
* Die Schüler haben das Gefühl, eine echte Fähigkeit gelernt zu haben, verstehen, dass die Seed-Phrase real und wichtig ist und nicht abstrakt, fühlen sich in der Lage, ihr eigenes Bitcoin zu halten, und begreifen, dass Dezentralisierung persönliche Verantwortung erfordert.
* Die Lernziele sind erreicht, wenn die Schüler eine Wallet einrichten und öffentliche sowie private Schlüssel verstehen können, die Vor- und Nachteile von Verwahrungs- und Selbstverwahrungs-Wallets erklären, den Ablauf einer Transaktion inklusive Inputs, Outputs und Gebühren erklären, Sicherheitsbewusstsein inklusive Schutz der Seed-Phrase zeigen und kritische Fragen zu Besitz und Kontrolle stellen.

##### Zeitmanagement

Wenn die Zeit knapp ist, priorisieren Sie:

* Verständnis der Wallet-Grundlagen
* Verständnis von Selbstverwahrung
* Erlernen des grundlegenden Transaktionsablaufs
* Entwicklung einer verantwortungsvollen Überprüfungsmentalität

Wenn Sie voraus sind, nehmen Sie sich Zeit für:

* Vergleichstabelle Selbstverwahrung vs. Verwahrung
* Tabelle zu Wallet-Typen und deren Kompromissen
* Schritt-für-Schritt-Übung zur Wallet-Einrichtung mit Live-Demo
* Transaktionsablaufdiagramm mit Gebührenberechnung
* Fortgeschrittene Sicherheitspraktiken und Überlegungen zu Hardware-Wallets

##### Wenn Schüler Schwierigkeiten haben

* Seed-Phrasen als "real" → "Diese Phrase IST dein Bitcoin; kein Kundenservice."
* Öffentliche vs. private Schlüssel → E-Mail-Analogie (Adresse vs. Passwort).
* Warum es schwierig ist → "Du kontrollierst es; du bist verantwortlich." Weisen Sie auf den Kompromiss hin.
