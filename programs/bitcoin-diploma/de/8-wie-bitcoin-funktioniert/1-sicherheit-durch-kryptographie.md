# 8.1 Sicherheit durch Kryptographie

> Was Bitcoin uns gibt, ist ein festes Versprechen: Das Programm wird genau wie angegeben ausgeführt.  
_Andreas M. Antonopoulos_

#### Öffentliche/Private Schlüssel-Kryptographie


> **Definition – Definition von Kryptographie**
>
> **Kryptographie** ist die Praxis, Informationen in ein Geheimnis zu verwandeln, das nur die richtigen Personen lesen können.


* **Verschlüsselung** ist der Prozess, Informationen in eine codierte Form zu bringen, sodass nur jemand mit dem richtigen Schlüssel sie lesen kann.
* **Entschlüsselung** ist der Prozess, diese codierten Informationen wieder in etwas Lesbares zu verwandeln.

In der traditionellen Kryptographie müssen zwei Personen, die privat kommunizieren möchten, zunächst denselben geheimen Schlüssel teilen, ähnlich wie ein gemeinsames Passwort. Eine Person verwendet diesen Schlüssel, um die Nachricht vor dem Senden zu verschlüsseln, und die andere Person verwendet denselben Schlüssel, um sie zu entschlüsseln und zu lesen.

Das Problem bei diesem System ist, dass beide Personen den geheimen Schlüssel bereits teilen müssen. Wenn jemand anderes Zugriff auf diesen Schlüssel erhält, kann er alle abgefangenen Nachrichten lesen.

Bitcoin löst dieses Problem mit einem anderen Ansatz, der als Public-Key-Kryptographie bezeichnet wird, bei dem Benutzer geheime Schlüssel nicht im Voraus teilen müssen.

Die öffentliche/private Schlüssel-Kryptographie löst das Problem des Teilens von Geheimnissen. Anstatt ein Passwort zu teilen, hat jede Person zwei Schlüssel: einen öffentlichen Schlüssel und einen privaten Schlüssel.

* Der **öffentliche Schlüssel** kann mit jedem geteilt werden.
* Der **private Schlüssel** muss immer geheim gehalten werden.

Wenn Gerhard etwas an Arel senden möchte, kann er Arels öffentlichen Schlüssel verwenden. Nur Arel kann es mit seinem privaten Schlüssel entschlüsseln. Selbst wenn jemand die Nachricht abfängt, kann er sie ohne den privaten Schlüssel nicht lesen oder verwenden.

In Bitcoin wird dieses System verwendet, um digitale Signaturen zu erstellen. Eine digitale Signatur beweist, dass der Besitzer eines privaten Schlüssels eine Transaktion genehmigt hat, ähnlich wie das Unterschreiben eines Dokuments. Das ermöglicht es, Bitcoin-Transaktionen sicher und überprüfbar zu machen, ohne einer dritten Partei vertrauen zu müssen.

Bitcoin-Transaktionen beinhalten die Übertragung des Eigentums an Bitcoin von einer Adresse zu einer anderen.

Verschlüsselung wird verwendet, um sicherzustellen, dass nur der tatsächliche Besitzer der Bitcoin die Befugnis hat, sein Geld an jemand anderen zu senden. Sie stellt sicher, dass sein Eigentum vor böswilligen Akteuren geschützt ist.

Als zusätzliche Schutzmaßnahme erhält jede Bitcoin-Transaktion automatisch eine EINZIGARTIGE digitale Signatur. Diese einzigartige digitale Signatur wird durch manipulationssichere Technologie ermöglicht, die dem Netzwerk hilft zu überprüfen, dass der tatsächliche Besitzer der Bitcoin – und nicht jemand anderes – sie gesendet hat.


> **Dark**
>
> Jeder Nutzer hat zwei Schlüssel: einen **privaten Schlüssel**, der **geheim gehalten** wird, und einen **öffentlichen Schlüssel**, der **mit anderen geteilt** werden kann. Der **private Schlüssel** dient als eine Art Identifikation und Eigentumsnachweis und bestätigt: „Diese Adresse gehört mir und ich habe die Kontrolle darüber.“


###### Wie eine Bitcoin-Transaktion funktioniert

1. **Erstellung der Transaktion**: Ein Nutzer startet eine Bitcoin-Transaktion, indem er Details wie die Empfängeradresse und den zu sendenden Bitcoin-Betrag angibt.
1. **Erzeugung der digitalen Signatur**: Der Absender erzeugt eine einzigartige **digitale Signatur** mit seinem **privaten Schlüssel**. Diese Signatur ist ein einzigartiger Code, der die Echtheit der Transaktion bestätigt.
1. **Übertragung der Transaktion**: Die signierte Transaktion wird an das Bitcoin-Netzwerk gesendet und zeigt die Absicht an, das Eigentum an Bitcoin vom Absender auf den Empfänger zu übertragen.
1. **Verifizierung im Netzwerk**: Knoten im Bitcoin-Netzwerk empfangen die Transaktion und verwenden den **öffentlichen Schlüssel** um die Echtheit der Signatur der Transaktion zu überprüfen. Gleichzeitig verwenden sie den öffentlichen Schlüssel des Absenders,**öffentlichen Schlüssel** um die **digitale Signatur** zu überprüfen.
1. **Bestätigung im Bitcoin-Netzwerk**: Wenn die Überprüfung erfolgreich ist, wird die Transaktion dem Hauptbuch hinzugefügt, das als sichere und transparente Aufzeichnung aller Transaktionen dient. Nach der Bestätigung wird das Eigentum an dem Bitcoin offiziell vom Absender auf den Empfänger übertragen.


> **Callout – Zusammenfassung**
>
> Die **digitale Signatur**, die mit dem **privaten Schlüssel** des Absenders erstellt wurde, beweist, dass die Transaktion vom Eigentümer des Bitcoin autorisiert wurde. Das Bitcoin-Netzwerk kann diesen Nachweis dann überprüfen und die Transaktion aufzeichnen.


#### Erklärung zum Hashing

Bitte lassen Sie sich nicht von den technischen Begriffen und mathematischen Konzepten abschrecken. Wir verstehen, dass nicht jeder ein Fan von Mathematik ist, aber vielleicht überraschen Sie sich selbst und sehen, dass selbst die komplexesten Ideen mit ein wenig Mühe verständlich werden können.


> **Definition – Definition einer Funktion**
>
> Eine **Funktion** ist wie eine Maschine, die Informationen entgegennimmt und daraus etwas Neues macht. Die Informationen, die Sie der Funktion geben, sind die **Eingabe**. Die neuen Informationen, die die Funktion erstellt, sind die **Ausgabe**. Funktionen helfen Computern, Aufgaben zu erledigen und Probleme zu lösen.


##### Was ist eine Funktion?

Eine Funktion ist eine Reihe von Anweisungen, die eine Eingabe nimmt und eine Ausgabe erzeugt. Sie können sie sich wie ein Rezept vorstellen: Sie befolgen die Schritte mit bestimmten Zutaten und erhalten immer ein vorhersehbares Ergebnis.

Im Bitcoin-System werden Funktionen verwendet, um Transaktionen zu verarbeiten und zu überprüfen. Wenn jemand Bitcoin sendet, helfen kryptografische Funktionen dabei, zu prüfen, ob die Transaktion gültig ist, zu bestätigen, dass der Absender genügend Guthaben hat, und die Salden im Bitcoin-Hauptbuch zu aktualisieren. Nach der Überprüfung und Aufnahme in einen Block wird die Transaktion Teil des dauerhaften Eintrags in der Blockchain.

##### Was ist eine Einwegfunktion?

Eine Einwegfunktion ist eine spezielle Art von Funktion, die in eine Richtung leicht zu berechnen, aber extrem schwer umzukehren ist. Zum Beispiel ist es einfach, Zutaten zu einem Smoothie zu mixen, aber Sie können den Smoothie nicht wieder in die ursprünglichen Zutaten zurückverwandeln.

Die Sicherheit von Bitcoin beruht auf Einwegfunktionen. Sie werden in der öffentlichen und privaten Schlüsselkryptografie verwendet und ermöglichen es Menschen, einen öffentlichen Schlüssel zu teilen, während ihr privater Schlüssel geheim bleibt. Auch wenn der öffentliche Schlüssel sichtbar ist, ist es unmöglich, daraus den privaten Schlüssel abzuleiten. Das macht Bitcoin-Transaktionen sicher.

##### Was ist eine Hashfunktion?

Eine **Hashfunktion** ist wie eine Geheimbotschaft-Maschine. Sie nimmt eine Nachricht und verwandelt sie in einen Code.

###### Wie Hashing bei Bitcoin-Transaktionen funktioniert

Bei Bitcoin wird jede Transaktion in einen Hash umgewandelt, bevor sie zur Blockchain hinzugefügt wird. Ein Hash ist ein einzigartiger digitaler Fingerabdruck der Transaktion. Wenn jemand versucht, auch nur einen kleinen Teil der Transaktion zu ändern, ändert sich der Hash vollständig. Das macht es dem Netzwerk leicht, Manipulationen zu erkennen.

###### Die Rolle des Hashings in der Bitcoin-Sicherheit

Hashing hilft, das Bitcoin-Netzwerk zu schützen, indem es Transaktionen leicht überprüfbar und unmöglich stillschweigend veränderbar macht. Da jede Transaktion ihren eigenen einzigartigen Hash hat, kann das Netzwerk schnell erkennen, ob etwas verändert wurde.

Eine Hashfunktion nimmt Daten und wandelt sie in eine feste Zeichenkette aus Zahlen und Buchstaben um, die als Hash bezeichnet wird. Die gleiche Eingabe erzeugt immer den gleichen Hash, aber schon eine winzige Änderung der Eingabe führt zu einem völlig anderen Ergebnis. Diese Eigenschaft ermöglicht es Computern zu überprüfen, dass Daten nicht verändert wurden.


> **Definition – Definition von Hashing**
>
> **Hashing** ist wie das Erstellen eines Fingerabdrucks für digitale Daten. Es ist der Prozess, eine digitale Nachricht zu nehmen und sie in einen Code fester Länge zu verwandeln, der als eindeutiger Identifikator dient. So wie ein Fingerabdruck eine Person identifizieren kann, kann ein Hash eine digitale Nachricht identifizieren.


Die **Ausgabe**, oder der Hash, hat immer die gleiche Länge, egal wie lang die ursprünglichen Informationen waren. Bitcoin verwendet einige spezielle Arten von Hashfunktionen, die **SHA-256** und **RIPEMD160** heißen.

Einige Beispiele finden Sie unten:

* SHA256-Hash der Zeichenkette **hallo Welt**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256-Hash der Zeichenkette **hallo Welt.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Beachte, dass schon eine kleine Änderung der Eingabe das Ergebnis im Vergleich zum ersten komplett verändert
* SHA256-Hash der herunterladbaren ISO-Datei **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Diese Eingabe ist eine riesige Datei, aber das Ergebnis hat trotzdem die gleiche feste Länge

Man kann sich Hashing auch wie eine Partitur vorstellen, die das Wesen eines Musikstücks einfängt. So wie eine Partitur eine einzigartige Darstellung einer Melodie ist, ist ein Hashwert eine einzigartige Darstellung von Daten.

Indem ein Musiker die Partitur eines Musikstücks mit der tatsächlichen Aufführung vergleicht, kann er feststellen, ob die Aufführung korrekt ist. Ebenso kann man durch den Vergleich des Hashwerts empfangener Daten mit dem ursprünglichen Hashwert feststellen, ob die Daten während der Übertragung verändert wurden.

Genauso wie schon eine kleine Abweichung in einer musikalischen Aufführung dazu führen kann, dass sie anders klingt, führt selbst die kleinste Änderung an den Originaldaten zu einem anderen Hashwert. Das macht Hashing zu einem mächtigen Werkzeug, um die Integrität und Authentizität einer Bitcoin-Transaktion zu gewährleisten.

Der Prozess der Kodierung des **öffentlichen Schlüssels** durch Hashing wird verwendet, um die Sicherheit von Informationen zu erhöhen, indem sie in ein festlängiges, unlesbares Format umgewandelt werden. Bitcoin verwendet die Algorithmen SHA-256 und RIPEMD160, um öffentliche Adressen zu erzeugen. Das resultierende Ergebnis dient als eindeutiger Identifikator für den **öffentlichen Schlüssel** und hilft, die Integrität und Sicherheit der im Hauptbuch gespeicherten Transaktionen zu gewährleisten. Durch die Verschlüsselung der Informationen auf diese Weise wird es Unbefugten erschwert, auf die Daten zuzugreifen und sie zu manipulieren.

##### Eigenschaften einer Hashfunktion

* **Deterministisch**: Die gleichen Zutaten ergeben immer den gleichen Smoothie. Genauso erzeugen die gleichen Daten immer denselben Hash.
* **Pre-Image-Resistenz**: Wenn du nur den Smoothie hast, kannst du nicht herausfinden, welche Früchte verwendet wurden. Ebenso kann man aus einem Hash nicht die ursprünglichen Daten bestimmen.
* **Lawineneffekt**: Schon eine winzige Änderung der Zutaten ergibt einen völlig anderen Smoothie. Beim Hashing führt eine sehr kleine Änderung der Daten zu einem völlig anderen Hash.
* **Kollisionsresistenz**: Es ist extrem schwierig, zwei verschiedene Zutatenmischungen zu finden, die genau denselben Smoothie ergeben. Genauso ist es extrem unwahrscheinlich, dass zwei verschiedene Datensätze denselben Hash erzeugen.
* **Schnell zu überprüfen**: Einen Smoothie zu machen geht schnell, und es ist einfach zu prüfen, dass das Ergebnis ein Smoothie ist. Hashfunktionen sind schnell berechnet und für jeden leicht zu überprüfen.

#### Aktivität: Erzeuge einen SHA-256-Hash


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Neugierig, wie Hashing funktioniert? Scanne den QR-Code, um sofort einen SHA256-Hash aus einem beliebigen Wort, Satz oder einer Eingabe deiner Wahl zu erzeugen. Hashfunktionen sind wie digitale Fingerabdrücke: Sie sind nur in eine Richtung anwendbar, das heißt, einmal gehasht, kann es nicht mehr rückgängig gemacht werden. Probiere es aus und überzeuge dich selbst!
