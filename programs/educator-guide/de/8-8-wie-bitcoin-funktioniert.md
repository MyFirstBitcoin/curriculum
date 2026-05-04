# 8 - Wie Bitcoin funktioniert

Dauer: 90 Minuten

Kernidee: Die Sicherheit von Bitcoin beruht auf einfachen, aber leistungsstarken technischen Konzepten wie Schlüsseln, Signaturen, Hashing und UTXOs, die Besitz und Verifizierung ohne zentrale Autorität ermöglichen.

#### Lernziele

Am Ende dieser Lektion sollten die Schüler in der Lage sein:

* Erklären, wie öffentliche und private Schlüssel den Besitz und die Transaktionen von Bitcoin absichern.
* Beschreiben, was eine digitale Signatur ist und wie sie beweist, dass eine Transaktion vom rechtmäßigen Besitzer autorisiert wurde.
* Einfach erklären, was Kryptografie, Verschlüsselung und Entschlüsselung im Kontext von Bitcoin bedeuten.
* Hashing definieren und beschreiben, warum Hashfunktionen für die Sicherheit und Datenintegrität von Bitcoin wichtig sind.
* Grundlegende Eigenschaften einer Hashfunktion erkennen, wie z. B. feste Ausgabelänge, Einwegfunktion und Empfindlichkeit gegenüber kleinen Änderungen der Eingabe.
* Das UTXO-Modell erklären und wie Bitcoin durch Transaktionsausgänge ausgegeben, empfangen und als Wechselgeld zurückgegeben wird.
* Beschreiben, wie Nodes helfen, Doppelausgaben zu verhindern, indem sie prüfen, ob ein Ausgang bereits ausgegeben wurde.

#### Werkzeuge & Ressourcen

##### Visuelle Hilfsmittel

* Kapitel 8 – Wie Bitcoin funktioniert

##### Unterstützungsbibliothek

* Vokabelkarte — Kapitel 8 — Begriffe: Kryptografie, Hash, UTXO, digitale Signatur, privater/öffentlicher Schlüssel, Merkle-Baum, Blockchain
* Missverständnis-Bibliotheken — Kapitel 8 — Adressen: „verlorene Seed-Phrase kann wiederhergestellt werden“, „privater Schlüssel = Passwort“, „Blockchain ist anonym“
* Technische Erklärungen & Deep-Dives — Hashfunktionen, öffentliche/private Schlüssel, UTXO-Modell, Proof-of-Work-Sicherheit

#### Aktivitäten

* Transaktionen in Aktion
* Erkundung des Mempools

#### Online-Unterricht

* Verwenden Sie ein digitales Whiteboard und zeichnen Sie jedes Konzept live, anstatt sich nur auf mündliche Erklärungen zu verlassen.
* Vermitteln Sie jeweils nur ein technisches Konzept und machen Sie häufig Pausen für Verständnisfragen.
* Verwenden Sie Visualisierungen für Schlüssel, Signaturen, Hashes und UTXOs, damit die Schüler die Struktur nachvollziehen können.
* Bleiben Sie beim konzeptionellen Ziel und vermeiden Sie es, zu tief in Mathematik oder Fachjargon einzutauchen.

#### Vorbereitung

* Bereiten Sie laminierte Diagramme vor: Paare aus öffentlichem/privatem Schlüssel, digitale Signaturen, UTXO-Modell, Hashing (Einwegfunktion).
* Setzen Sie Lesezeichen für Blockchain-Explorer und SHA-256-Hash-Rechner; wählen Sie 2–3 echte Bitcoin-Transaktionen aus, um sie Schritt für Schritt durchzugehen.
* Bereiten Sie Whiteboard-Notizen vor, um Inputs, Outputs und die Bestätigung von Transaktionen auf der Blockchain zu erklären.

#### Ablauf

Diese Lektion gibt den Schülern einen ersten Einblick in die technische Seite von Bitcoin, ohne technisches Vorwissen vorauszusetzen. Der Leitfaden folgt nun derselben komprimierten Struktur wie das Diplom, wobei Kryptografie unter einer Überschrift und UTXOs unter einer anderen zusammengefasst werden.

##### 8.0 Einführung, 8 Minuten

Beginnen Sie mit der Klärung der Erwartungen:

* Was macht Bitcoin sicher, wenn keine Zentralbank es kontrolliert?
* Wie kann das Netzwerk wissen, ob eine Person wirklich die Bitcoin besitzt, die sie senden möchte?
* Was passiert eigentlich im Hintergrund, wenn jemand eine Bitcoin-Transaktion durchführt?

Stellen Sie klar, dass sich dieses Kapitel auf die grundlegenden technischen Grundlagen von Bitcoin konzentriert, insbesondere auf Schlüssel, Signaturen, Hashing und UTXOs. Beruhigen Sie die Schüler auch, dass sie keine Ingenieure werden müssen, um die wesentliche Logik zu verstehen. Das Kapitel selbst macht diesen Punkt deutlich, indem es Bitcoin mit dem Internet vergleicht – viele Menschen nutzen es täglich, ohne jede darunterliegende Schicht vollständig zu verstehen.

##### 8.1 Sicherheit durch Kryptografie, 57 Minuten

**Bitcoin als ein auf vielen Computern gespeichertes Hauptbuch**

Beginnen Sie mit der einfachen Darstellung des Bitcoin-Netzwerks aus dem Kapitel:

* Bitcoin ist eine Aufzeichnung von Transaktionen
* diese Aufzeichnung wird auf vielen Computern gespeichert, die Nodes genannt werden
* das Hauptbuch ist öffentlich und pseudonym
* es zeigt Adressen und Transaktionshistorie, aber keine persönlichen Identitätsdaten

Dieser Abschnitt hilft den Schülern, an ihr Vorwissen aus früheren Kapiteln anzuknüpfen. Bitcoin basiert nicht auf versteckten Konten innerhalb einer Bank. Es basiert auf einem gemeinsamen Hauptbuch, das viele Teilnehmer überprüfen können. ist hier besonders hilfreich, da es Benutzer, Wallets und das größere Bitcoin-Netzwerk zeigt, die mit dem öffentlichen Hauptbuch verbunden sind.

**Öffentliche und private Schlüssel**

Gehen Sie nun zur Kryptografie über.

Erklären Sie, dass jeder Bitcoin-Nutzer Folgendes hat:

* einen privaten Schlüssel, der geheim bleiben muss
* ein öffentlicher Schlüssel, der geteilt werden kann

Erklären Sie ihren Zweck in einfachen Worten:

* der private Schlüssel beweist die Kontrolle und autorisiert das Ausgeben
* der öffentliche Schlüssel hilft anderen zu überprüfen, dass die Transaktion korrekt autorisiert wurde

Ein wichtiger Lehrpunkt aus dem Kapitel ist, dass Bitcoin öffentliche/private Schlüssel-Kryptographie verwendet und nicht das ältere Modell, bei dem zwei Personen zuerst denselben geheimen Schlüssel teilen müssen. Das ist wichtig, weil es eine sichere Verifizierung ermöglicht, ohne dass Nutzer das Geheimnis preisgeben müssen, das ihre Gelder schützt.

Sie können es so erklären:

* der private Schlüssel ist wie der geheime Beweis, dass der Bitcoin Ihnen gehört
* der öffentliche Schlüssel ist Teil dessen, was dem Netzwerk erlaubt, Ihre Autorisierung zu überprüfen
* wer den privaten Schlüssel kontrolliert, kontrolliert die Möglichkeit, den Bitcoin auszugeben

Achten Sie darauf, die Sprache der Verschlüsselung hier nicht zu kompliziert zu machen. Der wichtigste Punkt für die Lernenden ist Besitz und Autorisierung.

**Digitale Signaturen und Transaktionsautorisierung**

Erklären Sie nun, was passiert, wenn jemand Bitcoin sendet.

Nutzen Sie die Reihenfolge aus dem Kapitel:

* ein Nutzer erstellt eine Transaktion
* der Absender erzeugt eine digitale Signatur mit seinem privaten Schlüssel
* die Transaktion wird an das Netzwerk gesendet
* Knoten überprüfen, ob die Signatur gültig ist
* nach der Überprüfung und Bestätigung wird der Besitz im Hauptbuch übertragen

Machen Sie deutlich, dass eine digitale Signatur nicht dasselbe ist wie das Eintippen eines Namens. Sie ist ein kryptografischer Beweis, dass der tatsächliche Besitzer die Transaktion autorisiert hat. Das ist einer der Kernmechanismen, der es Bitcoin ermöglicht, ohne eine zentrale Instanz zu funktionieren, die Transaktionen manuell genehmigt. Die Grafik ist hilfreich, weil sie das Signieren und Überprüfen sowie den Weg der Transaktion vom Absender bis zur Netzwerkkontrolle visuell darstellt.

Ein guter Satz für den Unterricht ist:

Bitcoin-Transaktionen werden nicht genehmigt, weil eine Bank es sagt. Sie werden akzeptiert, weil das Netzwerk einen gültigen kryptografischen Nachweis überprüfen kann.

**Hashing und Einwegfunktionen**

Erklären Sie als Nächstes das Hashing.

Beginnen Sie einfach:

* eine Funktion nimmt eine Eingabe und erzeugt eine Ausgabe
* eine Einwegfunktion ist leicht in eine Richtung auszuführen, aber praktisch unmöglich umzukehren
* eine Hashfunktion nimmt Daten beliebiger Größe und wandelt sie in eine Ausgabe fester Länge um, die als Hash bezeichnet wird

Verwenden Sie eine der Analogien aus dem Kapitel, je nachdem, was für Ihr Publikum am verständlichsten ist:

* die Smoothie-Analogie für Einwegfunktionen
* die Fingerabdruck-Analogie für Hashes
* die Partitur-Analogie, um zu prüfen, ob sich etwas verändert hat

Die Fingerabdruck-Analogie ist wahrscheinlich für die meisten Klassen am verständlichsten:

* ein Hash ist wie ein digitaler Fingerabdruck für Daten
* wenn sich die Eingabe auch nur minimal ändert, ändert sich der Hash komplett
* das hilft Computern, die Integrität zu prüfen und Manipulationen zu erkennen

Erklären Sie dann, warum Hashing bei Bitcoin wichtig ist:

* Transaktionen werden gehasht
* das Netzwerk verwendet Hashes, um die Integrität zu überprüfen
* wenn eine Transaktion verändert wird, ändert sich der Hash
* das hilft, das Hauptbuch vor unbemerkter Manipulation zu schützen

Die Abbildungen auf den Seiten 7 bis 10 sind hier sehr hilfreich. Das Kapitel zeigt sowohl das Prinzip der Ausgabe fester Länge als auch das Prinzip „kleine Änderung, völlig anderes Ergebnis“, das zu den wichtigsten Konzepten für die Lernenden gehört.

**Grundlegende Eigenschaften von Hashfunktionen**

Gehen Sie kurz die im Kapitel hervorgehobenen Eigenschaften durch, ohne sie zu akademisch wirken zu lassen:

* Deterministisch: Die gleiche Eingabe ergibt jedes Mal die gleiche Ausgabe
* Einweg / Vorbildresistenz: Sie können den Prozess praktisch nicht umkehren
* Empfindlich auf Änderungen: Schon eine kleine Änderung der Eingabe erzeugt eine ganz andere Ausgabe
* Kollisionsresistenz: Es ist extrem schwierig, zwei verschiedene Eingaben mit derselben Ausgabe zu finden
* Schnell zu überprüfen: Die Funktion ist effizient auszuführen und zu prüfen

Die Lernenden müssen sich nicht jeden Begriff merken, aber sie sollten das Grundprinzip verstehen: Hashing gibt Bitcoin eine zuverlässige Möglichkeit, Daten zu identifizieren und Veränderungen zu erkennen.

##### 8.2 Das UTXO-Modell, 25 Minuten

**Das UTXO-Modell**

Nun kommen wir zum zweiten Hauptteil des Kapitels: UTXOs, oder Unspent Transaction Outputs (nicht ausgegebene Transaktionsausgänge).

Erklären Sie es einfach mit der Bargeld-Analogie aus dem Kapitel:

* Bitcoin wird nicht wie ein Bankkontostand verfolgt
* stattdessen besteht es aus ausgebbaren Stücken, die UTXOs genannt werden
* wenn Sie Bitcoin ausgeben, verwenden Sie einen oder mehrere bestehende UTXOs als Eingaben
* neue UTXOs werden dann als Ausgänge erstellt

Nutzen Sie das Beispiel aus dem Kapitel:

* wenn Sie ein 10 BTC UTXO haben
* und Sie senden 6 BTC
* geht ein neues 6 BTC UTXO an den Empfänger
* ein neues Wechselgeld-UTXO kommt zu Ihnen zurück
* ein kleiner Teil wird als Miner-Gebühr bezahlt

Das hilft den Lernenden zu erkennen, dass Bitcoin eher wie das Ausgeben von Bargeld mit Rückgeld funktioniert als wie das einfache Abziehen von Zahlen von einem Kontostand. Die Diagramme sind hier besonders hilfreich, weil sie visuell zeigen, wie ein UTXO in Empfängerausgang, Wechselgeld und Gebühr aufgeteilt wird.

Machen Sie zwei zentrale Punkte deutlich:

* Ihr Wallet-Guthaben ist die Summe Ihrer UTXOs
* wenn Sie ausgeben, werden alte UTXOs verbraucht und neue erstellt

**Verhinderung von Double-Spending**

Schließen Sie den Inhalt ab, indem Sie eine der wichtigsten Folgen des UTXO-Modells erklären.

Wenn jemand versucht, denselben Ausgang zweimal auszugeben, lehnen die Nodes den zweiten Versuch ab, weil sie das Kassenbuch führen und überprüfen können, ob dieses UTXO bereits ausgegeben wurde. So verhindert Bitcoin Double-Spending, ohne dass ein zentrales Zahlungsunternehmen die Aufzeichnungen verwalten muss. Das Beispiel ist hier sehr hilfreich, weil es zeigt, wie Alice UTXOs kombiniert, Geld an Bob sendet, Wechselgeld erhält und die bestätigte Transaktion das Kassenbuch über alle Nodes hinweg aktualisiert.

Eine klare Formulierung für den Unterricht ist:

Bitcoin verhindert Double-Spending, weil das Netzwerk verfolgt, welche Ausgänge noch nicht ausgegeben und welche bereits verwendet wurden.

###### Zusammenfassung und Verständnisüberprüfung

Schließen Sie mit ein paar kurzen Fragen ab:

* Was ist der Unterschied zwischen einem öffentlichen und einem privaten Schlüssel?
* Was beweist eine digitale Signatur?
* Warum ist Hashing in Bitcoin nützlich?
* Was passiert, wenn eine Transaktion nach dem Hashen verändert wird?
* Was ist ein UTXO in einfachen Worten?
* Wie verhindert das Netzwerk, dass jemand dieselben Bitcoins zweimal ausgibt?

#### Hinweise für Lehrkräfte

Dieses Kapitel enthält mehr technische Begriffe als die vorherigen, daher sollten Klarheit, Analogien und Wiederholungen im Vordergrund stehen.

Das Ziel ist nicht, die Lernenden zu Entwicklern zu machen. Das Ziel ist, ihnen zu helfen zu verstehen, warum die Sicherheit von Bitcoin funktioniert.

Die wichtigsten Punkte, die Sie bei Zeitmangel priorisieren sollten, sind:

* privater Schlüssel vs. öffentlicher Schlüssel
* digitale Signaturen
* was Hashing bewirkt
* UTXOs als ausgebbare Stücke von Bitcoin
* wie Double-Spending verhindert wird

Die nützlichsten Visualisierungen in diesem Kapitel sind:

* das Benutzer-Wallet-Netzwerk-Diagramm
* die Visualisierung der digitalen Signatur
* die Hashing-Beispiele und Diagramme mit fester Ausgabelänge auf den Seiten 7 bis 10
* die UTXO-Diagramme auf den Seiten 10 bis 12

##### Was gutes Lernen ausmacht

* Es ist wichtig, Kryptografie als Grundlage und nicht als Mysterium zu behandeln, viele Visualisierungen zu nutzen, tiefe Mathematik zu vermeiden, immer wieder auf frühere Kapitel zu verweisen und das Verständnis mit Anwendungen wie „Wenn jemand eine Transaktion ändert, was geht kaputt?“ zu testen.
* Lehrkräfte sollten geduldig mit Lernenden sein, die Schwierigkeiten haben, visuell denken und alles zeichnen, ehrlich sagen, was nicht verstanden werden muss, bereit sein zu sagen „Ich weiß es nicht, aber so würden wir es herausfinden“, und die Lernenden stets ermutigen.
* Lernende verstehen, warum Bitcoin nicht gehackt werden kann, weil es durch Mathematik geschützt ist, respektieren das elegante Design des Systems, fühlen sich mit der Komplexität wohl, weil sie nicht jedes Detail wissen müssen, gewinnen Vertrauen darin, Fragen ohne Angst zu stellen, und erkennen, dass sie ihr Verständnis auf ein neues Level gehoben haben.
* Die Lernziele sind erreicht, wenn Lernende die Grundlagen der Kryptografie wie Einwegfunktionen und digitale Signaturen ohne tiefe Mathematik erklären können, das UTXO-Modell verstehen und erkennen, dass sie Münzen und keine Konten besitzen, Hashing als Grundlage der Bitcoin-Sicherheit erkennen, den Aufbau von Transaktionen inklusive Signaturen und Bestätigungen verstehen, erklären können, warum Bitcoin unveränderlich ist, und kritische Fragen zu möglichen Angriffen oder Schwachstellen stellen.

##### Zeitmanagement

Wenn die Zeit knapp ist, priorisieren Sie:

* Privater Schlüssel vs. öffentlicher Schlüssel
* Digitale Signaturen
* Was Hashing bewirkt
* UTXOs als ausgebbare Einheiten von Bitcoin
* Wie Doppelausgaben verhindert werden

Wenn Sie voraus sind, nehmen Sie sich Zeit für:

* Benutzer-Wallet-Netzwerk-Diagramm und visuelles Sicherheitsmodell
* Digitale Signatur visuell: detaillierter kryptografischer Prozess
* Merkle-Bäume und Kettensicherheit
* Fortgeschrittene Angriffsvektoren und warum sie scheitern

##### Wenn Studierende Schwierigkeiten haben

* Kryptografie als bedrohlich → „Sie nutzen sie täglich; Bitcoin verwendet sie auf die gleiche Weise.“
* Hashing als Konzept → Fingerabdruck-Analogie; einzigartig, kann nicht geändert werden, ohne dass sich der Hash ändert.
* Digitale Signaturen → „Beweist Autorisierung, ohne das Passwort preiszugeben.“
