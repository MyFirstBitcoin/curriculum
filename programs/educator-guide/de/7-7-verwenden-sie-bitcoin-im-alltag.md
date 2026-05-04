# 7 - Verwenden Sie Bitcoin im Alltag

Dauer: 90 Minuten

Kernidee: Das Lightning-Netzwerk macht Bitcoin für alltägliche Zahlungen praktischer, indem es schnellere und günstigere Transaktionen ermöglicht, während Bitcoin weiterhin die Grundlage bleibt.

#### Lernziele

Am Ende dieser Lektion sollten die Schüler in der Lage sein:

* Erklären, was das Lightning-Netzwerk ist und warum es auf Bitcoin aufgebaut wurde.
* On-Chain- und Lightning-Transaktionen hinsichtlich Geschwindigkeit, Kosten und Sicherheitskompromissen vergleichen.
* Zwischen verwahrten und selbstverwahrten Lightning-Wallets unterscheiden und erklären, warum Selbstverwahrung wichtig ist.
* Ein Lightning-Wallet einrichten und die Rolle der Seed-Phrase bei der Wiederherstellung des Wallets beschreiben.
* Demonstrieren, wie Lightning-Zahlungen durch das Netzwerk geleitet werden, auch wenn zwei Nutzer keinen direkten Kanal teilen.
* Reale Möglichkeiten aufzeigen, wie Bitcoin im Alltag durch Lightning genutzt werden kann, z. B. für Kaffee, Lebensmittel, Händlerzahlungen und lokale Ausgaben.
* Erklären, wie Werkzeuge wie BTCPay Server, BTCMap und Geschenkkarten die Bitcoin-Nutzung in der Praxis erweitern.
* Beschreiben, was eine Bitcoin-Kreislaufwirtschaft ist und warum Lightning sie praktikabler macht.

#### Werkzeuge & Ressourcen

##### Visuelle Hilfsmittel

* Kapitel 7 – Bitcoin im Alltag nutzen

##### Unterstützungsbibliothek

* Vokabelkarte — Begriffe: Lightning-Netzwerk, Zahlungskanal, Routing, Layer 2, Kreislaufwirtschaft, Überweisung
* Bibliothek mit Praxisbeispielen & Fallstudien — El Salvador, Kreislaufwirtschaft in Austin, Geschichten zur Lightning-Akzeptanz bei Händlern
* Vergleichstabellen & Übersichtsblätter — On-Chain vs. Lightning Vergleich; Gebühren- & Geschwindigkeitsvergleich verschiedener Zahlungsmethoden
* Lightning-Netzwerk einfach erklärt — Wie Zahlungskanäle funktionieren ohne Fachjargon; Routing; Sicherheit; Anwendungsfälle
* Zahlungsszenarien Schritt für Schritt — Schritt-für-Schritt: an Freund senden, Zahlung empfangen, Überweisungen, als Freelancer akzeptieren
* Gebühren- & Geschwindigkeitsvergleichstool — Wann Lightning, On-Chain oder Banküberweisung nutzen (mit Kostenbeispielen)

#### Aktivitäten

* Lightning-Staffellauf

#### Online-Unterricht

* Verwenden Sie eine Vergleichsfolie mit On-Chain- und Lightning-Zahlungen nebeneinander.
* Beginnen Sie mit einem realen Anwendungsfall wie Kaffee oder Überweisungen, damit die Schüler verstehen, warum es Lightning gibt.
* Verwenden Sie ein einfaches Routing-Diagramm mit drei Personen, damit die Erklärung des Netzwerks klar bleibt.
* Halten Sie die Kanalmechanik einfach, es sei denn, die Klasse hat bereits ein solides Grundwissen.

#### Vorbereitung

* Laden Sie ein Lightning-Wallet herunter und bereiten Sie Screenshots vor, die On-Chain- (langsam) und Lightning- (schnell) Transaktionsgeschwindigkeiten nebeneinander zeigen.
* Recherchieren Sie 2–3 echte Händler oder Communities, die Lightning nutzen; speichern Sie BTCMap.org als Referenz.
* Bereiten Sie eine Vergleichstabelle On-Chain vs. Lightning (Geschwindigkeit, Gebühren, Sicherheit, Anwendungsfall) zur Verteilung vor.

#### Ablauf

Diese Lektion zeigt den Schülern, wie Bitcoin durch das Lightning-Netzwerk für alltägliche Zahlungen praktisch wird. Der Leitfaden folgt nun direkt der Diplomstruktur, sodass die wichtigsten Lightning-Abschnitte dem Schülerleitfaden entsprechen, während Vergleiche, Händler-Tools und Kreislaufwirtschaftsmaterial dort bleiben, wo sie hingehören.

##### 7.0 Einführung, 8 Minuten

Beginnen Sie damit, dieses Kapitel mit dem vorherigen zu verbinden:

* Wenn Bitcoin On-Chain funktioniert, warum wurde eine weitere Ebene benötigt?
* Was passiert, wenn Menschen viele kleine Zahlungen schnell tätigen möchten?
* Welche Art von Zahlungssystem wäre besser geeignet für Kaffee, Lebensmittel oder eine Zahlung an einen Freund?

Stellen Sie klar, dass sich dieses Kapitel auf Bitcoin für den Alltag konzentriert, besonders wenn Geschwindigkeit und niedrige Gebühren wichtig sind. Machen Sie deutlich, dass Lightning auf Bitcoin aufbaut und nicht davon getrennt ist.

##### 7.1 Das Lightning-Netzwerk, 25 Minuten

**Was ist das Lightning-Netzwerk**

Erklären Sie, dass das Lightning-Netzwerk ein Zahlungssystem ist, das auf Bitcoin aufbaut und es Nutzern ermöglicht, Bitcoin schnell und kostengünstig zu senden und zu empfangen. Es funktioniert, indem viele kleine Zahlungen außerhalb der Haupt-Blockchain abgewickelt und nur das Endergebnis später On-Chain beglichen wird.

Eine hilfreiche Erklärung ist der Café-Tab-Vergleich aus dem Kapitel:

* anstatt jeden Artikel einzeln On-Chain zu bezahlen
* öffnen zwei Parteien einen Kanal
* sie aktualisieren die Guthaben, während sie Transaktionen durchführen
* nur das Endguthaben wird auf der Blockchain vermerkt, wenn sie den Kanal schließen

Das macht Lightning schneller und günstiger für häufige, kleine Zahlungen. Erklären Sie außerdem, dass Lightning-Zahlungen durch das Netzwerk geroutet werden können, sodass Nutzer keinen direkten Kanal zu jeder Person benötigen, an die sie zahlen.

**On-Chain vs. Lightning**

Stellen Sie den Unterschied jetzt sehr deutlich heraus.

On-Chain-Transaktionen

* finden direkt auf der Bitcoin-Blockchain statt
* sind in der Regel langsamer
* hängen von der Aufnahme in einen Block und der Bestätigung ab
* gelten als tendenziell sicherer
* können je nach Gebühren teurer sein

Lightning-Transaktionen

* finden auf einer zweiten Schicht statt, die auf Bitcoin aufbaut
* werden viel schneller abgewickelt
* kosten in der Regel deutlich weniger
* sind nützlich für kleine und häufige Zahlungen
* beinhalten Kompromisse im Vergleich zur On-Chain-Abwicklung

Halten Sie die Hauptaussage einfach: On-Chain ist stärker für endgültige Abwicklung, Lightning ist stärker für Geschwindigkeit und günstige Alltagsnutzung. Der Vergleich ist hier besonders hilfreich.

##### 7.2 Verschiedene Arten von Lightning-Wallets, 10 Minuten

Erklären Sie, dass eine Lightning-Wallet die gleiche Grundfunktion wie eine Bitcoin-Wallet erfüllt – Bitcoin empfangen und senden –, aber für die Nutzung im Lightning-Netzwerk konzipiert ist. Gehen Sie dann die wichtigsten Wallet-Unterscheidungen des Kapitels durch:

* selbstverwahrend: Der Nutzer kontrolliert die Schlüssel
* verwahrend: Jemand anderes kontrolliert die Schlüssel

Stellen Sie den zentralen Kompromiss klar:

* verwahrende Wallets wirken oft einfacher und bequemer
* aber der Nutzer ist auf die Erlaubnis und Kontrolle anderer angewiesen
* selbstverwahrende Wallets bieten mehr Eigentum und Souveränität

Betonen Sie außerdem die Empfehlung des Kapitels, Open-Source-Wallets zu bevorzugen, da Open-Source-Tools von der Community überprüft, verbessert und verifiziert werden können.

##### 7.3 Einrichten einer Bitcoin-Lightning-Wallet, 10 Minuten

Führen Sie die Lernenden durch den grundlegenden Einrichtungsablauf:

* eine Lightning-Wallet herunterladen
* eine neue Wallet erstellen
* die Wiederherstellungsphrase aufschreiben
* die Wörter in der richtigen Reihenfolge bestätigen
* zusätzliche Sicherheit hinzufügen, falls die Wallet dies erlaubt
* mit der Nutzung der Wallet beginnen

Seien Sie besonders klar bezüglich der Seed-Phrase:

* sie ermöglicht dem Nutzer den Zugang zur Wiederherstellung
* geht sie verloren, kann der Zugang zu den Geldern verloren gehen
* gelangt sie in fremde Hände, können andere über die Gelder verfügen

Dieser Abschnitt sollte Verantwortung und sicheren Umgang besonders betonen, genauso wie im On-Chain-Kapitel.

##### 7.4 Lightning-Transaktionen senden und empfangen, 17 Minuten

**Wie Lightning-Transaktionen in der Praxis funktionieren**

Nutzen Sie das Beispiel mit Marcia, Jeff und Eve, um das Routing zu erklären. Marcia benötigt keinen direkten Kanal zu Eve. Ihre Zahlung kann über Jeff laufen, der mit dem Netzwerk verbunden ist, und erreicht Eve trotzdem sicher.

Machen Sie diese Punkte deutlich:

* Lightning-Zahlungen können über Zwischenstationen laufen
* diese Zwischenstationen helfen beim Routing der Zahlungen
* der Routing-Prozess bedeutet nicht, dass Nutzer einer Bank oder einem zentralen Zahlungsdienstleister vertrauen
* das Netzwerk nutzt Kryptografie, damit die Zahlung beim vorgesehenen Empfänger ankommt

Das hilft den Lernenden zu verstehen, dass Lightning auch dann Peer-to-Peer bleibt, wenn Zahlungen durch ein größeres Netzwerk laufen. Falls hilfreich, weisen Sie darauf hin, dass das Kapitel auch erwähnt, dass Node-Betreiber durch das Routing von Zahlungen Gebühren verdienen und das Netzwerk stärken können.

**Kanäle finanzieren und Lightning wiederholt nutzen**

Erklären Sie das Mina-Beispiel weiter:

* Mina verschiebt Bitcoin aus ihrer On-Chain-Wallet in ihre Lightning-Wallet
* damit finanziert sie einen Zahlungskanal
* Sie kann dann wiederholt Zahlungen leisten, ohne den Prozess jedes Mal neu zu starten.
* Wenn der Kanal geschlossen wird, wird das endgültige Guthaben wieder on-chain abgerechnet.

Machen Sie eine wichtige Einschränkung deutlich: Gelder, die in einem aktiven Kanal gebunden sind, werden für Lightning verwendet und stehen nicht gleichzeitig für separate On-Chain-Nutzung frei zur Verfügung. Das hilft den Lernenden zu verstehen, dass Lightning zwar leistungsfähig ist, aber eine andere Zahlungsstruktur mit sich bringt.

##### 7.5 Kaffee und Lebensmittel mit Bitcoin kaufen, 20 Minuten

**Alltägliche Anwendungsfälle**

Wechseln Sie von der Technik zur Praxis.

Erklären Sie, dass Lightning besonders nützlich ist für:

* Kaffee kaufen
* Lebensmittel
* Einkaufen
* Freunde bezahlen
* alltägliche Kleinbetragszahlungen

Das Mina-Beispiel in diesem Kapitel zeigt, warum Lightning für viele Situationen besser geeignet ist als traditionelle Zahlungswege: Es ist schnell, gebührenarm, grenzenlos und auch für Menschen zugänglich, die vielleicht kein Bankkonto haben. Die Vergleichstabelle und das Zahlungsabwicklungsdiagramm sind hier besonders hilfreiche Lehrmittel, vor allem um zu zeigen, wie viele Zwischenhändler es bei traditionellen Kartenzahlungen gibt.

**Händler-Tools und Bitcoin im Alltag ausgeben**

Erklären Sie nun, wie Unternehmen und Nutzer Lightning im Alltag praktisch nutzen können.

Gehen Sie auf die drei wichtigsten Werkzeuge oder Wege im Kapitel ein:

BTCPay Server

* Open-Source-Zahlungsabwickler
* ermöglicht Händlern, Bitcoin direkt zu akzeptieren
* kein Mittelsmann kontrolliert die Gelder
* nützlich für Online- und Vor-Ort-Geschäftszahlungen

BTCMap

* hilft Nutzern, Händler und Gemeinschaften zu finden, die Bitcoin akzeptieren
* ermöglicht lokale Suche
* kann von der Community aktualisiert werden

Geschenkkarten und Gutscheine

* Übergangswerkzeuge, um Bitcoin auszugeben, wo direkte Akzeptanz noch nicht existiert
* helfen, die Lücke zu überbrücken, während die Akzeptanz wächst

Dieser Abschnitt ist wichtig, weil er zeigt, dass die Nutzung von Bitcoin nicht nur theoretisch ist. Es gibt bereits heute echte Werkzeuge, die Menschen nutzen können.

**Kreiswirtschaften und Bitcoin als Tauschmittel**

Schließen Sie den Hauptinhalt ab, indem Sie erklären, dass eine Kreislaufwirtschaft eine Gemeinschaft ist, in der die Teilnehmer versuchen, so viel wie möglich untereinander zu kaufen und zu verkaufen. Auf Bitcoin angewandt bedeutet das, dass Händler, Arbeitnehmer und Nutzer sich entscheiden, in Bitcoin zu handeln und sich gegenseitig wirtschaftlich zu unterstützen.

Machen Sie deutlich, warum Lightning hier wichtig ist:

* Zahlungen sind nahezu sofort
* Gebühren sind niedrig
* Kleinbetragszahlungen werden praktikabel
* Lokaler Handel lässt sich leichter aufrechterhalten

Sie können erwähnen, dass das Kapitel auf Beispiele wie Arnhem und Bitcoin Beach verweist und zeigt, dass Kreislaufwirtschaften nicht hypothetisch sind. Sie existieren bereits und wachsen weiter. Die visuelle Zeitleiste ist hier besonders hilfreich.

###### Abschluss und Verständnisüberprüfung

Schließen Sie mit ein paar kurzen Fragen ab:

* Warum wurde das Lightning-Netzwerk gebaut?
* Was ist ein wesentlicher Unterschied zwischen On-Chain- und Lightning-Zahlungen?
* Warum ist Selbstverwahrung in einer Lightning-Wallet wichtig?
* Wie kann jemand eine Lightning-Zahlung empfangen, ohne einen direkten Kanal zu jeder Person zu haben?
* Was ist eine Bitcoin-Kreislaufwirtschaft?

#### Hinweise für Lehrkräfte

Halten Sie den roten Faden klar: Bitcoin ist die Basisschicht, Lightning hilft, alltägliche Zahlungen schneller und günstiger zu machen.

Dieses Kapitel sollte praktisch und anschaulich wirken, nicht übermäßig technisch.

Priorisieren Sie das Verständnis vor tiefgehender Kanaltechnik.

Die wichtigsten Punkte, die Sie bei Zeitmangel priorisieren sollten, sind:

* was Lightning ist
* Abwägungen zwischen On-Chain und Lightning
* Wallet-Verwahrung und Einrichtung
* Zahlungen in der realen Welt
* zirkuläre Wirtschaften

Die nützlichsten Schaubilder in diesem Kapitel sind:

* der Vergleich zwischen On-Chain und Lightning
* die Unterschiede zwischen Wallets
* das Routing-Beispiel mit Marcia, Jeff und Eve
* die Vergleichstabelle und das Kapazitätsdiagramm
* das traditionelle Diagramm zur Zahlungsabwicklung
* die Zeitleiste der zirkulären Wirtschaft

##### Wie es gut aussieht

* Es ist wichtig, mit dem Schmerzpunkt „Bitcoin dauert 10 Minuten und kostet 2 $“ zu beginnen, Lightning als Überholspur auf Bitcoin zu erklären, echte Beispiele von Händlern und Überweisungskorridoren zu verwenden und Entscheidungsbäume zu erstellen, wann On-Chain oder Lightning genutzt werden sollte.
* Lehrende sollten pragmatisch sein, was Lightning tatsächlich löst, Erfahrungsberichte aus der Praxis teilen, in denen Bitcoin genutzt wird, die spezifischen Abwägungen klar benennen und realistisch in Bezug auf die Akzeptanz bleiben, während sie sich über die Möglichkeiten freuen.
* Die Lernenden erleben, wie Bitcoin tatsächlich für echte Zahlungen an realen Orten funktioniert, verstehen, dass Geschwindigkeit und Kosten bei Zahlungen wichtig sind, stellen sich eine zirkuläre Wirtschaft vor, in der Bitcoin lokal bleibt, erkennen, dass Lightning ≠ Bitcoin ist (verschiedene Werkzeuge für verschiedene Zwecke), und werden neugierig auf Wirtschaftssysteme, die auf Bitcoin-Zahlungen basieren.
* Die Lernziele sind erreicht, wenn die Lernenden das Lightning-Netzwerk als Schicht auf Bitcoin erklären können, die Grundlagen von Zahlungskanälen und Routing verstehen, reale Anwendungsfälle für Lightning-Zahlungen sehen, On-Chain und Lightning für verschiedene Szenarien vergleichen, das Konzept der zirkulären Wirtschaft verstehen und die spezifischen Abwägungen jeder Herangehensweise erkennen.

##### Zeitmanagement

Wenn die Zeit knapp ist, priorisieren:

* Was Lightning ist
* Abwägungen zwischen On-Chain und Lightning
* Zahlungen in der realen Welt
* Zirkuläre Wirtschaften

Wenn Zeit übrig ist, vertiefen Sie:

* Mechanik von Zahlungskanälen und Routing
* Vergleichswerkzeug für Gebühren und Geschwindigkeit
* Fallstudien zu zirkulären Wirtschaften in El Salvador und Austin
* Praktische Durchläufe von Lightning-Zahlungsszenarien

##### Wenn Lernende Schwierigkeiten haben

* Warum es Lightning gibt → Vergleich: 10 Min/2 $ vs. Sekunden/Bruchteile eines Cents.
* Zahlungskanäle → Café-Tab-Analogie; intern abrechnen und dann auf Bitcoin ausgleichen.
* Warum es global wichtig ist → „Was, wenn keine Bank, aber Bitcoin?“
