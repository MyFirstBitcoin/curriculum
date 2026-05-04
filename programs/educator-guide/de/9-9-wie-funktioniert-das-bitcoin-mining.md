# 9 - Wie funktioniert das Bitcoin-Mining?

Dauer: 90 Minuten

Kernidee: Bitcoin-Mining und die Validierung durch Nodes arbeiten zusammen, um das Netzwerk zu sichern, Transaktionen zu bestätigen und die Regeln des Systems durch Proof of Work durchzusetzen.

#### Lernziele

Am Ende dieser Lektion sollten die Lernenden in der Lage sein:

* Den Unterschied zwischen der Rolle von Bitcoin-Nodes und der Rolle von Bitcoin-Minern erklären.
* Beschreiben, wie Nodes Transaktionen validieren, Informationen austauschen und helfen, die Bitcoin-Regeln durchzusetzen.
* Erklären, was Miner tun, einschließlich der Auswahl von Transaktionen, dem Erstellen von Kandidatenblöcken und dem Wettbewerb um das Finden eines gültigen Block-Hashes.
* Den Mempool definieren und erklären, warum er wie ein Warteraum für unbestätigte Transaktionen funktioniert.
* Beschreiben, wie Transaktionsgebühren die Auswahl durch Miner und die Bestätigungsgeschwindigkeit beeinflussen.
* Proof of Work als Mechanismus erklären, der Bitcoin sichert, indem er Angriffe teuer macht.
* Beschreiben, wie die Schwierigkeitsanpassung hilft, eine durchschnittliche Blockzeit von etwa 10 Minuten aufrechtzuerhalten.
* Den vollständigen Lebenszyklus einer Bitcoin-Transaktion durchgehen, von der Erstellung und Signierung bis zur Bestätigung in einem Block.

#### Werkzeuge & Ressourcen

##### Visuelle Hilfsmittel

* Kapitel 9 – Wie funktioniert Bitcoin-Mining?

##### Unterstützungsbibliothek

* Vokabelkarte — Kapitel 9 — Begriffe: Mining, Proof of Work, Hash-Puzzle, Schwierigkeitsanpassung, Block-Belohnung, Mempool, 51%-Angriff
* Bibliothek der Missverständnisse — Kapitel 9 — Adressiert: „Miner erschaffen Bitcoin aus dem Nichts“, „Miner kontrollieren Bitcoin“, „mehr Mining = weniger sicher“
* Vergleichstabellen & Übersichtsblätter — Mining-Ökonomie: Einnahmen, Kosten, Anreizangleichung; Schwierigkeitsanpassung
* Technische Erklärungen & Deep-Dives — Proof of Work Sicherheit; warum Angriffe teuer sind; 51%-Schwelle

#### Aktivitäten

* Den Mempool erkunden
* Transaktionen in Aktion

#### Online-Unterricht

* Verwenden Sie ein klares Transaktionsflussdiagramm vom Wallet-Signieren bis zur Bestätigung.
* Halten Sie Nodes und Miner während der gesamten Lektion auf dem Bildschirm visuell getrennt.
* Verwenden Sie mempool.space oder einen Screenshot davon, um unbestätigte Transaktionen und den Gebühren-Druck zu zeigen.
* Machen Sie nach jeder Phase des Mining-Prozesses eine Pause und stellen Sie eine kurze Verständnisfrage.

#### Vorbereitung

* Bereiten Sie ein Diagramm des Mining-Prozesses vor (Mempool → Transaktionsauswahl → Blockerstellung → Schwierigkeitsanpassung) zur Anzeige.
* Setzen Sie ein Lesezeichen auf mempool.space oder die Mining-Seite von blockchain.com; bereiten Sie Screenshots der aktuellen Mining-Statistiken und Schwierigkeitsanpassungen vor.
* Erstellen Sie eine visuelle Erklärung von Proof of Work als Sicherheitsmechanismus; zeigen Sie die Schwierigkeitsanpassung der letzten 3–6 Monate.

#### Ablauf

Diese Lektion betrachtet genauer, wie Bitcoin-Transaktionen durch das Netzwerk wandern und Teil der Blockchain werden. Sie folgt nun direkt der Diplomstruktur, sodass die Hauptabschnitte mit dem Schülerleitfaden übereinstimmen, während die ausführlichere Erklärung für Lehrkräfte in jedem Abschnitt erhalten bleibt.

##### 9.0 Einführung, 8 Minuten

Beginnen Sie damit, dieses Kapitel mit dem vorherigen zu verbinden:

* Wenn ein Nutzer eine Transaktion mit einem privaten Schlüssel signiert, was passiert als Nächstes?
* Wer prüft, ob diese Transaktion gültig ist?
* Wie wird sie zur Blockchain hinzugefügt?
* Warum braucht Bitcoin sowohl Nodes als auch Miner?

Stellen Sie klar, dass dieses Kapitel erklärt, wie das Netzwerk Transaktionen in der Praxis verarbeitet und wie Mining das System ohne zentrale Instanz absichert.

##### 9.1 Bitcoin-Nodes und Miner, 47 Minuten

**Nodes und Miner, unterschiedliche Rollen**

Beginnen Sie damit, die beiden Rollen klar zu trennen.

Bitcoin-Nodes:

* behalten eine Kopie der Blockchain
* überprüfen, ob Transaktionen den Regeln folgen
* tauschen Informationen mit anderen Nodes aus
* helfen Wallets und anderer Software beim Zugriff auf Blockchain-Daten
* können ungültige Transaktionen oder ungültige Blöcke ablehnen

Das Kapitel beschreibt Nodes als Torwächter der Validierung und erweitert dies mit der Analogie des „digitalen Verkehrspolizisten“. Das ist hilfreich, weil es Nodes als Prüfer und Koordinatoren zeigt, nicht als Herrscher. Das Diagramm verdeutlicht außerdem, dass viele Nodes Kopien des Ledgers auf der ganzen Welt aufbewahren.

Bitcoin-Miner:

* sammeln gültige Transaktionen
* stellen Kandidatenblöcke zusammen
* konkurrieren darum, einen gültigen Block-Hash zu finden
* übertragen gültige Blöcke, wenn sie gewinnen
* erhalten Blockbelohnungen und Transaktionsgebühren

Ein zentraler Lehrpunkt des Kapitels ist, dass das Ziel des Minings nicht einfach die Erzeugung neuer Bitcoin ist, sondern die Dezentralisierung der Sicherheit von Bitcoin. Die neuen Bitcoin sind der Anreiz, während der Mining-Prozess selbst der Sicherheitsmechanismus ist.

**Was Nodes tatsächlich tun**

Erweitern Sie den Node-Abschnitt mit der im Kapitel aufgeführten Liste der Node-Funktionen:

* Torwächter der Validierung: Sie prüfen, ob Transaktionen und Blöcke den Regeln entsprechen
* Kommunikationsknotenpunkt: Sie verbinden sich miteinander und teilen Transaktionsdaten
* Qualitätsprüfer: Sie lehnen ungültige Informationen ab
* Blockchain-Informant: Sie stellen anderen Programmen wie Wallets Daten zur Verfügung
* Begrüßer neuer Nodes: Sie helfen neuen Nodes, die Blockchain zu erhalten, wobei jeder neue Node die Daten dennoch unabhängig überprüft

Dies ist ein guter Moment, um zu betonen, dass das Betreiben eines Nodes dem Nutzer mehr Unabhängigkeit verschafft. Anstatt sich vollständig auf externe Dienste zu verlassen, um den Zustand des Netzwerks zu erfahren, können sie ihn selbst überprüfen. macht diesen Punkt deutlich, einschließlich des Hinweises auf Bitcoin Core als eine Implementierung, die Nutzer betreiben können.

**Was Miner tatsächlich tun**

Erklären Sie nun das Mining genauer.

Miner:

* sammeln verifizierte, aber unbestätigte Transaktionen
* fassen sie zu einem Kandidatenblock zusammen
* hashen wiederholt Blockdaten, während sie nach einem gültigen Block-Hash suchen
* übertragen den siegreichen Block an das Netzwerk
* verdienen Belohnungen, wenn der Block akzeptiert wird

Nutzen Sie die Analogie des Kapitels vom „riesigen Heuhaufen voller Schlüssel“, wenn sie hilft. Sie gibt den Lernenden ein konkretes Bild vom Mining-Wettlauf. Die Hauptidee ist nicht, dass Miner ein nützliches mathematisches Problem im üblichen Sinne lösen, sondern dass sie beweisen, dass sie reale Energie und Rechenleistung aufgewendet haben, um das System zu sichern.

Hier ist auch der richtige Ort, um die Belohnungen der Miner zu erklären:

* Blockbelohnung: neu ausgegebene Bitcoin
* Transaktionsgebühren: Gebühren, die an Transaktionen angehängt werden, die Nutzer bestätigt haben möchten

Stellen Sie klar, dass Miner in der Regel Transaktionen mit höheren Gebühren bevorzugen, da diese ihre Belohnung erhöhen. Das Kapitel erklärt hier auch die Halbierungen, daher können Sie kurz erwähnen, dass die Blockbelohnung alle 210.000 Blöcke, also etwa alle vier Jahre, gemäß dem öffentlichen Angebotsplan von Bitcoin sinkt. Die Seiten 5 und 6 enthalten den Angebotsplan und die Tabelle zur nächsten Halbierung, was hilft, die vorhersehbare Ausgabe von Bitcoin zu verdeutlichen.

**Gültiger Block-Hash, Proof of Work und Schwierigkeitsanpassung**

Dieser Abschnitt ist der Kern des Kapitels.

Erklären Sie, dass Miner nach einem gültigen Block-Hash suchen, also einem Block-Hash, der das vom Netzwerk gesetzte Ziel erfüllt. Das Kapitel erklärt dies als das Finden einer Zahl, die niedriger ist als das vom Netzwerk gesetzte Ziel.

Erklären Sie dann Proof of Work klar:

* Miner müssen wiederholt Rechenarbeit leisten
* der erste, der einen gültigen Hash findet, beweist, dass er diese Arbeit geleistet hat
* dadurch wird es teuer, das Ledger umzuschreiben oder anzugreifen
* Nodes überprüfen dann den Block, bevor sie ihn akzeptieren

Ein starker Lehrsatz ist:

Proof of Work sichert Bitcoin, indem es Unehrlichkeit teuer und Überprüfung einfach macht.

Erklären Sie auch die Schwierigkeitsanpassung:

* das Netzwerk passt die Mining-Schwierigkeit alle 2.016 Blöcke an
* das geschieht ungefähr alle zwei Wochen
* das Ziel ist, die durchschnittliche Blockzeit bei etwa 10 Minuten zu halten
* wenn mehr Rechenleistung dem Netzwerk beitritt, steigt die Schwierigkeit
* wenn weniger Rechenleistung vorhanden ist, sinkt die Schwierigkeit

Die Seiten 7 und 8 erklären diesen Prozess und zeigen, wie schwierigere Ziele mehr Arbeit erfordern. Das hilft den Lernenden zu verstehen, dass das Timing von Bitcoin nicht von einer zentralen Instanz kontrolliert wird, sondern von Protokollregeln, die automatisch auf Netzwerkbedingungen reagieren.

##### 9.2 Was ist der Mempool?, 15 Minuten

Gehen Sie nun zum Mempool über.

Erklären Sie, dass der Mempool der Warteraum für gültige, unbestätigte Transaktionen ist. Wenn ein Nutzer eine Transaktion überträgt, überprüfen die Nodes sie zuerst. Ist sie gültig, fügen sie sie ihrem Mempool hinzu und teilen sie mit anderen Nodes. Dann können Miner aus diesen wartenden Transaktionen beim Erstellen eines Blocks auswählen. Die Seiten 10 und 11 erklären diesen Prozess direkt.

Wichtige Punkte, die betont werden sollten:

* Der Mempool ist nicht die Blockchain
* Transaktionen dort sind noch unbestätigt
* Jeder Node verwaltet seinen eigenen Mempool
* Es gibt keinen einzigen universellen Mempool
* Transaktionen mit höheren Gebühren werden mit größerer Wahrscheinlichkeit früher ausgewählt

Das Kapitel erklärt auch die häufigsten Gründe, warum eine Transaktion lange unbestätigt bleiben kann:

* niedrige Gebühr
* Netzwerküberlastung
* Versuch eines Double-Spends
* falsche oder unvollständige Daten
* fehlerhafte Transaktion

Falls sinnvoll, erwähne die Aktivität mit mempool.space als praktische Möglichkeit, unbestätigte Transaktionen und Gebührensätze zu visualisieren. Mache auch deutlich, dass mempool.space nur ein Explorer ist, nicht der Mempool selbst.

##### 9.3 Wie Bitcoin-Transaktionen funktionieren, 20 Minuten

Fasse nun alles mit der Schritt-für-Schritt-Abfolge des Kapitels zusammen.

Eine klare Version für den Unterricht ist:



1. Der Sender wählt einen UTXO aus und erstellt eine Transaktion
1. Der Sender fügt die Empfängeradresse und die Gebühr hinzu
1. Der Sender signiert die Transaktion mit seinem privaten Schlüssel
1. Die Transaktion wird an das Netzwerk gesendet
1. Nodes überprüfen sie und fügen sie ihren Mempools hinzu
1. Miner wählen sie für einen Kandidatenblock aus
1. Miner konkurrieren durch Proof of Work
1. Ein Miner findet einen gültigen Block-Hash und sendet den Block aus
1. Nodes überprüfen den Block und fügen ihn der Blockchain hinzu
1. Die Transaktion erhält Bestätigungen, während weitere Blöcke hinzugefügt werden
1. Mache den letzten Punkt explizit:
1. Sobald die Transaktion in einem gültigen Block enthalten ist, ist sie bestätigt
1. Die ausgegebenen Inputs sind nicht mehr verwendbar
1. Der Empfänger kontrolliert nun die neuen durch diese Transaktion erzeugten UTXOs

Das Übersichtsdiagramm ist hier besonders hilfreich, da es den gesamten Prozess von der Wallet-Signatur über die Aufnahme durch Miner bis zur Validierung durch Nodes und Blockverteilung visuell verbindet.

###### Abschluss und Verständnisüberprüfung

Beende die Stunde mit ein paar schnellen Fragen:

* Was ist der Unterschied zwischen einem Node und einem Miner?
* Was ist der Mempool?
* Warum werden manche Transaktionen schneller bestätigt als andere?
* Was beweist Proof of Work?
* Warum passt Bitcoin die Mining-Schwierigkeit an?
* Was sind die wichtigsten Schritte zwischen dem Senden einer Transaktion und dem Erhalt der Bestätigung?

#### Hinweise für Lehrkräfte

Halte den roten Faden klar: Nodes überprüfen, Miner konkurrieren, Proof of Work sichert, und der Mempool hält gültige Transaktionen, bis sie bestätigt sind.

Dieses Kapitel kann technisch wirken, daher sollten oft Analogien und Diagramme verwendet werden.

Vermeide es, Mining so darzustellen, als würde Bitcoin aus dem Nichts erschaffen. Sei präzise: Die Belohnung ist der Anreiz, während der Mining-Prozess das Netzwerk absichert.

Die wichtigsten Punkte, die bei Zeitmangel Priorität haben sollten, sind:



1. Unterschiede zwischen Node- und Miner-Rollen
1. Mempool als Warteraum
1. Proof of Work
1. Schwierigkeitsanpassung
1. Ablauf einer Transaktion von der Signatur bis zur Bestätigung

##### Was gutes Lehren ausmacht

* Es ist wichtig, sofort klarzustellen, dass Miner ≠ Nodes sind, Mining als wirtschaftliche Aktivität mit realen Hardware- und Stromkosten zu zeigen, die Schwierigkeitsanpassung und Proof of Work als Sicherheitsmechanismus zu erklären und das Verständnis mit Szenarien zu Netzveränderungen zu testen.
* Lehrkräfte sollten mit echten Zahlen arbeiten, um Diskussionen zu untermauern, den Unterschied zwischen Minern und Nodes glasklar und wiederholt herausstellen, realistisch auf Zentralisierungsprobleme bei Mining-Pools eingehen und die tatsächliche Komplexität des Themas respektieren.
* Die Lernenden verstehen, dass Mining von klugen Menschen betrieben wird, die komplexe Arbeit leisten, weil sie Bitcoin verdienen; sie erkennen, dass Anreize ehrliches Verhalten fördern, da der Gewinn der Miner vom Erfolg von Bitcoin abhängt; sie sehen, dass sich das System durch automatische Schwierigkeitsanpassung selbst reguliert; sie begreifen, dass Mining ein echtes Geschäft und keine Wohltätigkeit ist, und sie schätzen, dass die Sicherheit von Bitcoin echte Strom- und Geldkosten verursacht.
* Die Lernziele sind erreicht, wenn die Lernenden Miner, die Blöcke erzeugen, von Nodes, die diese validieren, unterscheiden können, Proof of Work als Sicherheitsmechanismus verstehen, der Angriffe exponentiell teuer macht, erkennen, dass die Schwierigkeitsanpassung die Blockzeit bei etwa 10 Minuten hält, die Anreize der Miner bezüglich Blockbelohnungen und Gebühren verstehen, erklären können, warum ein 51%-Angriff nicht funktioniert, und Mining als wirtschaftliche Aktivität mit echten Kosten und Nutzen sehen.

##### Zeitmanagement

Wenn die Zeit knapp ist, priorisieren Sie:

* Rollen von Node vs. Miner (die entscheidende Unterscheidung)
* Mempool als Warteraum
* Proof-of-Work-Mechanismus
* Schwierigkeitsanpassung (selbstregulierendes System)
* Ablauf einer Transaktion von der Signatur bis zur Bestätigung

Wenn Sie voraus sind, nehmen Sie sich Zeit für:

* Mining-Ökonomie und Hardware-Details
* Dynamik von Mining-Pools und Zentralisierungsprobleme
* 51%-Angriffszenarien und warum sie mathematisch scheitern
* Langfristige Sicherheit durch Anreizangleichung

##### Wenn Lernende Schwierigkeiten haben

* Miner vs. Nodes (Verwirrung) → "Nodes validieren, Miner schlagen vor; Schiedsrichter vs. Spieler."
* Proof of Work verschwenderisch → "Teure Sicherheit verhindert Angriffe; macht sie sinnlos."
* Schwierigkeitsanpassung → "Mehr Miner = schnellere Blöcke = Schwierigkeit steigt; das System atmet."
