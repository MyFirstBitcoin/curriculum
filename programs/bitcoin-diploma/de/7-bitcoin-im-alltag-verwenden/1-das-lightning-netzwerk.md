# 7.1 Das Lightning-Netzwerk

Das Lightning Network ist ein Zahlungssystem, das es Nutzern ermöglicht, Bitcoin schnell und kostengünstig zu senden und zu empfangen. Es funktioniert, indem eine gemeinsame Wallet eingerichtet wird, in die beide Parteien einen Teil ihrer Bitcoin einzahlen. Anschließend können sie unbegrenzt viele Transaktionen miteinander durchführen, ohne jede einzelne auf der Haupt-Blockchain aufzeichnen zu müssen. Dadurch entfällt die Notwendigkeit, jede Transaktion einzeln zu verifizieren und in einen Block aufzunehmen, was den Prozess sowohl schnell als auch kosteneffizient macht. Die niedrigeren Gebühren bedeuten, dass das Lightning Network auch für Kleinstbeträge genutzt werden kann, die auf der Blockchain nicht immer praktikabel wären. Sobald die Parteien ihre Zusammenarbeit beenden möchten, wird nur der Endsaldo auf der Blockchain festgehalten.

Stellen Sie sich einen Tag in einem Café vor. Sie planen, länger zu bleiben, und eröffnen eine Rechnung, indem Sie im Voraus bezahlen, anstatt jede Bestellung einzeln zu begleichen. Am Ende des Tages überprüfen Sie und der Inhaber gemeinsam die Rechnung, um den Betrag auszugleichen. Wenn Ihre Anzahlung höher war als Ihre Ausgaben, erhalten Sie die Differenz zurück; haben Sie mehr ausgegeben, zahlen Sie den Restbetrag nach.

Dieses System lässt sich auf mehrere Teilnehmer ausweiten. Zum Beispiel bringen Sie bei einem Ihrer Besuche im Café einen Freund mit, den der Barkeeper nicht kennt und für den er keine Rechnung eröffnen kann. Sie bieten Ihrem Freund an, Ihre bestehende Rechnung zu nutzen, um seine Ausgaben zu decken, und vereinbaren, dass er Sie privat zurückzahlt. Stellen Sie sich nun vor, Tausende von Menschen würden das gleichzeitig tun und anderen erlauben, bestehende Rechnungen zu nutzen, um mit noch mehr Personen verbunden zu werden – so funktioniert das Lightning Network!

Mit Lightning können Sie Zahlungen an jeden im Netzwerk senden, nicht nur an die Person, mit der Sie eine direkte Rechnung teilen – vorausgesetzt, es lässt sich eine Route zwischen den beiden Parteien finden. Ihre Zahlung kann durch das Netzwerk geleitet werden, bis sie ihr Ziel erreicht, selbst wenn Sie keinen direkten Kanal zum Empfänger geöffnet haben.

Schauen wir uns den Unterschied zwischen On-Chain- und Off-Chain-Transaktionen an.

##### On-Chain-Transaktionen

Dies sind Transaktionen, die direkt auf der Bitcoin-Blockchain stattfinden. Sie benötigen etwa 10 Minuten zur Bestätigung, und die Gebühren hängen von der Größe der Transaktion in virtuellen Bytes ab. Sie sind sicherer, aber langsamer, da sie den Konsens des Netzwerks erfordern.

##### Lightning Network-Transaktionen

Diese Transaktionen finden in einem separaten Netzwerk statt, das auf der Bitcoin-Blockchain aufbaut. Sie werden schneller und mit geringeren Gebühren abgewickelt. Sie werden häufig dort eingesetzt, wo Geschwindigkeit und Kosten der Transaktionen wichtiger sind. Im Vergleich zu On-Chain-Transaktionen sind sie weniger sicher.


|  | Bitcoin-Netzwerk | Lightning Network |
| --- | --- | --- |
| Definition | Ein dezentrales digitales Netzwerk, das Kryptografie nutzt, um Finanztransaktionen zu sichern. | Ein Zahlungsprotokoll der zweiten Ebene, das auf der Bitcoin-Blockchain aufsetzt und schnellere sowie günstigere Transaktionen ermöglicht. |
| Vorteile | Dezentral und sicher. Keine Rückbuchungen oder Betrug. Kann pseudonym genutzt werden. Weltweite Akzeptanz. | Schnellere und günstigere Transaktionen. Erhöhte Skalierbarkeit. Off-Chain-Transaktionen überlasten die Blockchain nicht. |
| Nachteile | Langsame Transaktionszeiten. Hohe Gebühren bei bestimmten Transaktionsarten. Komplex für Anfänger. | Kann Vertrauen in die Betreiber der Kanäle erfordern. Erfordert On-Chain-Transaktionen zum Öffnen und Schließen von Kanälen. |
