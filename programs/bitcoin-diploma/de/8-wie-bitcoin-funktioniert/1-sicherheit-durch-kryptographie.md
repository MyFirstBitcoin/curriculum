# 8.1 Sicherheit durch Kryptographie

> Was Bitcoin uns gibt, ist ein festes Versprechen: Das Programm wird genau wie angegeben ausgeführt.  
_Andreas M. Antonopoulos_



#### Öffentliche/Private Schlüssel-Kryptographie


> **Definition – Definition von Kryptographie**
>
> **Kryptographie** ist die Praxis, Informationen in ein Geheimnis zu verwandeln, das nur die richtigen Personen lesen können.


* **Verschlüsselung** ist der Prozess, Informationen in eine codierte Form zu bringen, sodass nur jemand mit dem richtigen Schlüssel sie lesen kann.
* **Entschlüsselung** ist der Prozess, diese codierten Informationen wieder in eine lesbare Form zu bringen.

In der traditionellen Kryptographie müssen zwei Personen, die privat kommunizieren möchten, zunächst denselben geheimen Schlüssel teilen, ähnlich wie ein gemeinsames Passwort. Eine Person verwendet diesen Schlüssel, um die Nachricht vor dem Senden zu verschlüsseln, und die andere Person verwendet denselben Schlüssel, um sie zu entschlüsseln und zu lesen.

Das Problem bei diesem System ist, dass beide Personen den geheimen Schlüssel bereits teilen müssen. Wenn jemand anderes Zugriff auf diesen Schlüssel erhält, kann er alle abgefangenen Nachrichten lesen.

Bitcoin löst dieses Problem mit einem anderen Ansatz, der als Public-Key-Kryptographie bezeichnet wird, bei dem Benutzer geheime Schlüssel nicht im Voraus teilen müssen.

Die öffentliche/private Schlüssel-Kryptographie löst das Problem des Teilens von Geheimnissen. Anstatt ein Passwort zu teilen, hat jede Person zwei Schlüssel: einen öffentlichen Schlüssel und einen privaten Schlüssel.

* Der **öffentliche Schlüssel** kann mit jedem geteilt werden.
* Der **private Schlüssel** muss immer geheim gehalten werden.

Wenn John etwas an Arel senden möchte, kann er Arels öffentlichen Schlüssel verwenden. Nur Arel kann es mit seinem privaten Schlüssel entschlüsseln. Selbst wenn jemand die Nachricht abfängt, kann er sie ohne den privaten Schlüssel nicht lesen oder verwenden.

In Bitcoin wird dieses System verwendet, um digitale Signaturen zu erstellen. Eine digitale Signatur beweist, dass der Besitzer eines privaten Schlüssels eine Transaktion genehmigt hat, ähnlich wie das Unterschreiben eines Dokuments. Das ermöglicht es, Bitcoin-Transaktionen sicher und überprüfbar zu machen, ohne einer dritten Partei vertrauen zu müssen.


> **Info**
>
> Jeder Nutzer hat zwei Schlüssel: einen **privaten Schlüssel**, der **geheim gehalten** wird, und einen **öffentlichen Schlüssel**, der **mit anderen geteilt werden kann**.
>
> Der **private Schlüssel** dient als eine Art Identifikation und Eigentumsnachweis und bestätigt: „Diese Adresse gehört mir und ich habe die Kontrolle darüber.“
>
> **Digitale Signaturen** werden erstellt, um eindeutige Transaktionen zu identifizieren.


Bitcoin-Transaktionen beinhalten die Übertragung des Eigentums an einer bestimmten Menge Bitcoin von einer Adresse zu einer anderen.

Verschlüsselung wird verwendet, um sicherzustellen, dass nur der tatsächliche Inhaber der Bitcoins die Befugnis hat, sein Geld an jemand anderen zu senden. Sie stellt sicher, dass sein Eigentum vor böswilligen Akteuren geschützt ist.

Als zusätzliche Schutzmaßnahme erhält jede Bitcoin-Transaktion automatisch eine EINZIGARTIGE digitale Signatur. Diese einzigartige digitale Signatur wird durch manipulationssichere Technologie ermöglicht, die dem Netzwerk hilft zu überprüfen, dass der tatsächliche Besitzer der Bitcoins – und nicht jemand anderes – sie gesendet hat.

###### Wie eine Bitcoin-Transaktion funktioniert

1. **Erstellung der Transaktion**: Ein Nutzer initiiert eine Bitcoin-Transaktion, indem er Details wie die Empfängeradresse und den zu sendenden Bitcoin-Betrag angibt.
1. **Erzeugung der digitalen Signatur**: Der Absender erzeugt eine eindeutige **digitale Signatur** mit seinem **privaten Schlüssel**. Diese Signatur ist ein einzigartiger kryptografischer Code, der die Echtheit der Transaktion bestätigt.
1. **Übertragung der Transaktion**: Die signierte Transaktion wird an das Bitcoin-Netzwerk gesendet und zeigt die Absicht an, das Eigentum an Bitcoin vom Absender auf den Empfänger zu übertragen.
1. **Verifizierung im Netzwerk**: Knoten im Bitcoin-Netzwerk empfangen die Transaktion und verwenden den **öffentlichen Schlüssel** des Empfängers, um die Echtheit der Signatur der Transaktion zu überprüfen. Gleichzeitig verwenden sie den **öffentlichen Schlüssel** des Absenders, um die **digitale Signatur** zu überprüfen.
1. **Bestätigung im Bitcoin-Netzwerk**: Wenn die Verifizierung erfolgreich ist, wird die Transaktion dem Hauptbuch hinzugefügt, das als sichere und transparente Aufzeichnung aller Transaktionen dient. Nach der Bestätigung wird das Eigentum an den Bitcoin offiziell vom Absender auf den Empfänger übertragen.


> **Callout – Zusammenfassung**
>
> Die **digitale Signatur**, die mit dem **privaten Schlüssel** des Absenders erstellt wurde, beweist, dass die Transaktion vom Eigentümer der Bitcoin autorisiert wurde.
>
> Das Bitcoin-Netzwerk kann diesen Nachweis dann überprüfen und die Transaktion aufzeichnen.


#### Erklärung zum Hashing

Bitte lassen Sie sich nicht von den technischen Begriffen und mathematischen Konzepten abschrecken. Wir verstehen, dass nicht jeder ein Fan von Mathematik ist, aber Sie könnten sich selbst überraschen und feststellen, dass selbst die komplexesten Ideen mit ein wenig Mühe verständlich werden.


> **Definition – Definition einer Funktion**
>
> Eine **Funktion** ist wie eine Maschine, die Informationen nimmt und sie in etwas Neues verwandelt. Die Informationen, die Sie der Funktion geben, nennt man **Eingabe**. Die neuen Informationen, die die Funktion erzeugt, nennt man **Ausgabe**. Funktionen helfen Computern, Aufgaben zu erledigen und Probleme zu lösen.


##### Was ist eine Funktion?

Eine Funktion ist eine Reihe von Anweisungen, die eine Eingabe nimmt und eine Ausgabe erzeugt. Sie können sie sich wie ein Rezept vorstellen: Sie befolgen die Schritte mit bestimmten Zutaten und erhalten immer ein vorhersehbares Ergebnis.

Im Bitcoin-System werden Funktionen verwendet, um Transaktionen zu verarbeiten und zu überprüfen. Wenn jemand Bitcoin sendet, helfen kryptografische Funktionen dabei, zu prüfen, ob die Transaktion gültig ist, zu bestätigen, dass der Absender genügend Guthaben hat, und die Salden im Bitcoin-Hauptbuch zu aktualisieren. Sobald die Transaktion überprüft und zu einem Block hinzugefügt wurde, wird sie Teil des dauerhaften Eintrags in der Blockchain.

##### Was ist eine Einwegfunktion?

Eine Einwegfunktion ist eine besondere Art von Funktion, die in eine Richtung leicht zu berechnen, aber extrem schwer umzukehren ist.

Zum Beispiel ist es einfach, Zutaten zu einem Smoothie zu mixen, aber Sie können den Smoothie nicht wieder in die ursprünglichen Zutaten zerlegen.

Die Sicherheit von Bitcoin beruht auf Einwegfunktionen. Sie werden in der öffentlichen und privaten Schlüssel-Kryptografie verwendet und ermöglichen es, einen öffentlichen Schlüssel zu teilen, während der private Schlüssel geheim bleibt. Obwohl der öffentliche Schlüssel sichtbar ist, ist es nahezu unmöglich, daraus den privaten Schlüssel abzuleiten. Das macht Bitcoin-Transaktionen sicher.

##### Was ist eine Hashfunktion?


> **Definition – Definition einer Hashfunktion**
>
> Eine **Hashfunktion** ist wie eine Geheimcode-Maschine.
>
> Sie nimmt eine **Nachricht** und verwandelt sie in einen Code.


###### Wie Hashing bei Bitcoin-Transaktionen funktioniert

Bei Bitcoin wird jede Transaktion in einen Hash umgewandelt, bevor sie zur Blockchain hinzugefügt wird. Ein Hash ist ein einzigartiger digitaler Fingerabdruck der Transaktion. Wenn jemand versucht, auch nur einen kleinen Teil der Transaktion zu ändern, ändert sich der Hash vollständig. Dadurch kann das Netzwerk Manipulationen leicht erkennen.

###### Die Rolle des Hashings in der Bitcoin-Sicherheit

Hashing hilft, das Bitcoin-Netzwerk zu schützen, indem es Transaktionen leicht überprüfbar und unmöglich stillschweigend veränderbar macht. Da jede Transaktion ihren eigenen einzigartigen Hash hat, kann das Netzwerk schnell erkennen, ob etwas verändert wurde.

Eine Hashfunktion nimmt Daten und wandelt sie in eine feste Zeichenkette aus Zahlen und Buchstaben um, die als Hash bezeichnet wird. Die gleiche Eingabe erzeugt immer den gleichen Hash, aber schon eine winzige Änderung der Eingabe führt zu einem völlig anderen Ergebnis. Diese Eigenschaft ermöglicht es Computern zu überprüfen, dass Daten nicht verändert wurden.


> **Definition – Definition von Hashing**
>
> **Hashing** ist wie das Erstellen eines Fingerabdrucks für digitale Daten. Es ist der Prozess, eine digitale Nachricht zu nehmen und sie in einen Code fester Länge zu verwandeln, der als eindeutiger Identifikator dient. Genau wie ein Fingerabdruck eine Person identifizieren kann, kann ein Hash eine digitale Nachricht identifizieren. Hashes werden in vielen Anwendungen verwendet, einschließlich Bitcoin-Transaktionen.


Die **Ausgabe**, oder Hash, hat immer die gleiche Länge, egal wie lang die ursprüngliche Information war. Bitcoin verwendet einige spezielle Arten von Hashfunktionen, die **SHA-256** und **RIPEMD160** heißen.

Einige Beispiele sind unten aufgeführt:

* SHA256-Hash der Zeichenkette **hello world**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256-Hash der Zeichenkette **hello world.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Beachte, dass eine kleine Änderung der Eingabe die Ausgabe im Vergleich zur ersten komplett verändert.
* SHA256-Hash der herunterladbaren ISO-Datei **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Diese Eingabe ist eine riesige Datei, aber die Ausgabe hat trotzdem die gleiche feste Länge.

Man kann Hashing auch mit einer Partitur vergleichen, die das Wesen eines Musikstücks einfängt. So wie eine Partitur eine einzigartige Darstellung einer Melodie ist, ist ein Hashwert eine einzigartige Darstellung eines Datensatzes.

Indem ein Musiker die Partitur mit der tatsächlichen Aufführung vergleicht, kann er feststellen, ob die Aufführung korrekt ist. Ebenso kann man durch den Vergleich des Hashwerts der empfangenen Daten mit dem ursprünglichen Hashwert feststellen, ob die Daten während der Übertragung verändert wurden.

Genauso wie schon eine kleine Abweichung in einer musikalischen Darbietung dazu führen kann, dass sie anders klingt, führt selbst die kleinste Änderung an den Originaldaten zu einem anderen Hashwert. Das macht Hashing zu einem mächtigen Werkzeug, um die Integrität und Authentizität einer Bitcoin-Transaktion zu gewährleisten.

Der Prozess der Kodierung des **öffentlichen Schlüssels** durch Hashing wird verwendet, um die Sicherheit von Informationen zu erhöhen, indem sie in ein festlängiges, unlesbares Format umgewandelt werden. Bitcoin verwendet die Algorithmen SHA-256 und RIPEMD160, um öffentliche Adressen zu erzeugen. Die resultierende Ausgabe dient als eindeutiger Identifikator für den **öffentlichen Schlüssel** und hilft, die Integrität und Sicherheit der im Hauptbuch gespeicherten Transaktionen zu gewährleisten. Durch die Verschlüsselung der Informationen auf diese Weise wird es Unbefugten erschwert, auf die Daten zuzugreifen und sie zu manipulieren.

##### Eigenschaften einer Hashfunktion

* **Deterministisch**: Die gleichen Zutaten ergeben immer den gleichen Smoothie. Genauso erzeugen die gleichen Daten immer den gleichen Hash.
* **Pre-Image-Resistenz**: Wenn du nur den Smoothie hast, kannst du nicht herausfinden, welche Früchte verwendet wurden. Ebenso kann man aus einem Hash nicht auf die ursprünglichen Daten schließen.
* **Lawineneffekt**: Schon eine winzige Änderung der Zutaten ergibt einen völlig anderen Smoothie. Beim Hashing führt eine sehr kleine Änderung der Daten zu einem komplett anderen Hash.
* **Kollisionsresistenz**: Es ist extrem schwierig, zwei verschiedene Zutatenmischungen zu finden, die genau den gleichen Smoothie ergeben. Genauso ist es äußerst unwahrscheinlich, dass zwei verschiedene Datensätze den gleichen Hash erzeugen.
* **Schnell zu überprüfen**: Einen Smoothie zu machen geht schnell, und es ist einfach zu prüfen, dass das Ergebnis ein Smoothie ist. Hashfunktionen sind schnell berechnet und für jeden leicht zu überprüfen.

#### Aktivität: Erzeuge einen SHA-256-Hash

https://tools.keycdn.com/sha256-online-generator

Neugierig, wie Hashing funktioniert?

Scanne den QR-Code, um sofort einen SHA256-Hash aus jedem beliebigen Wort, Satz oder einer Eingabe deiner Wahl zu erzeugen.

Hashfunktionen sind wie digitale Fingerabdrücke: Sie sind nur in eine Richtung anwendbar, das heißt, einmal gehasht, kann es nicht mehr rückgängig gemacht werden.

Probiere es aus und überzeuge dich selbst!
