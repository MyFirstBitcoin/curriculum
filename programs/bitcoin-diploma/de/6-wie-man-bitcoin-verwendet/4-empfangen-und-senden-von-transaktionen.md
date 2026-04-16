# 6.4 Empfangen und Senden von Transaktionen

Eine Bitcoin-Transaktion ist die Übertragung des Eigentums an Bitcoin auf einen neuen Besitzer. Beachten Sie, dass nicht die eigentlichen Münzen übertragen werden, sondern das Eigentum an ihnen: mit anderen Worten, das Recht, sie auszugeben. Jedes Mal, wenn eine Transaktion in einen Block aufgenommen wird, aktualisieren alle Knoten im Netzwerk ihre lokale Kopie des öffentlichen Hauptbuchs, um den Eigentümerwechsel widerzuspiegeln. In dieser Hinsicht ähnelt eine Bitcoin-Transaktion eher einer Immobilien- (oder anderen Eigentums-)Transaktion als einer Bargeldtransaktion.

Um Bitcoin zu „senden“, signiert der Absender eine Nachricht mit seinem privaten Schlüssel und signalisiert dem Netzwerk damit, dass der rechtmäßige Besitzer der Bitcoin das Eigentum an den Empfänger übertragen hat.

Die Bitcoin sind nun mit der Adresse des Empfängers verknüpft, wodurch dieser das Eigentum an den Bitcoin erhält, sodass nur der neue Besitzer sie mit seinem privaten Schlüssel ausgeben kann.

Neue Bitcoin-Transaktionen werden weltweit von Wallets aus initiiert, aber es gibt keinen zentralen Zahlungsabwickler. Stattdessen konkurrieren Miner darum, Transaktionen im Hauptbuch zu verzeichnen.

Nehmen wir an, Jim schuldet Eliana 0,5 BTC und ist bereit, sie zurückzuzahlen. Beide haben digitale Wallets.

1. Eliana teilt Jim ihre Adresse mit.
1. Jim verwendet seine Wallet-Software, um die Transaktion zu erstellen, die Elianas Adresse, den zu übertragenden Betrag (0,5 BTC) und eine Gebühr für den Miner enthält. Höhere Gebühren erhöhen die Wahrscheinlichkeit, dass ein Miner die Transaktion in den nächsten Block aufnimmt.
1. Nachdem die Transaktion signiert wurde, wird sie an das Netzwerk gesendet, wo sie von den Knoten überprüft wird. Sie prüfen, ob Jim über genügend Guthaben verfügt und der rechtmäßige Besitzer der Münzen ist, die er ausgeben möchte. Falls nicht, lehnen sie die Transaktion sofort ab.
1. Sobald die Transaktion verifiziert ist, entscheiden die Miner, ob sie die Transaktion in den nächsten Block aufnehmen, meist basierend auf der gewählten Gebühr. Sobald die Transaktion in einen Block aufgenommen wurde, wird sie zur Blockchain hinzugefügt und die Gelder werden an Elianas Adresse übertragen.
1. Das Eigentum wurde auf Eliana übertragen. Sie kann nun ihren privaten Schlüssel verwenden, um die erhaltenen Gelder auszugeben.

_Es ist wichtig zu beachten, dass eine abgeschlossene Transaktion nicht rückgängig gemacht werden kann._


> **Note – Wie eine Bitcoin-Transaktion funktioniert**
>
> 1. Jemand fordert eine Transaktion an
> 1. Transaktion wird an P2P-Computer (Knoten) gesendet
> 1. Miner verifizieren die Transaktion
> 1. Transaktionen werden zu einem Datenblock zusammengefasst
> 1. Neuer Block wird zur bestehenden Blockchain hinzugefügt
> 1. Die Transaktion ist abgeschlossen



> **Note – Bitcoin-Transaktionen empfangen**
>
> Um Bitcoin zu empfangen, müssen Sie dem Absender eine Bitcoin-Öffentlich-Adresse mitteilen. Dies ist eine eindeutige Zeichenfolge aus Buchstaben und Zahlen, die Ihre Wallet repräsentiert und zur Identifizierung im Bitcoin-Netzwerk dient.
>
> Sie finden Ihre öffentliche Adresse, indem Sie Ihre Bitcoin-Wallet öffnen und nach einer Option wie „Empfangen“ oder „Einzahlen“ suchen.
>
> Sie können Ihre Bitcoin-Adresse dann auf verschiedene Arten weitergeben:
>
> 1. **Adresse kopieren und einfügen**: Sie können die Adresse markieren und auf „Kopieren“ drücken, dann in eine E-Mail oder Nachricht einfügen.
> 1. **Einen Link zu Ihrer Bitcoin-Wallet teilen**: Einige Bitcoin-Wallets ermöglichen es Ihnen, einen Link zu Ihrer Wallet zu erstellen, den Sie dem Absender schicken können. Dieser kann dann auf den Link klicken, um Ihre Wallet aufzurufen und Bitcoin zu senden.
> 1. **Einen QR-Code teilen**: Wenn der Absender ein Smartphone mit einer Bitcoin-Wallet-App hat, kann er den QR-Code scannen, um Ihre Bitcoin-Adresse zu erhalten.


Sobald der Absender Ihre Adresse hat, kann er Ihnen Bitcoin senden, indem er Ihre Adresse und den gewünschten Betrag eingibt. Die Bitcoin werden dann von seiner Wallet an Ihre Wallet gesendet.

Die Transaktion wird vom Bitcoin-Netzwerk bestätigt und dauert in der Regel etwa 10 Minuten. Für mehr Sicherheit empfiehlt es sich, auf zwei Bestätigungen zu warten, was etwa 20 Minuten dauert.


> **Note – Bitcoin-Transaktionen senden**
>
> Um Bitcoin zu senden, benötigen Sie Folgendes: eine Bitcoin-Wallet, die öffentliche Adresse des Empfängers und den Betrag an Bitcoin, den Sie senden möchten.
>
> 1. Öffnen Sie Ihre Bitcoin-Wallet.
> 1. Navigieren Sie zur Schaltfläche „Senden“ und fügen Sie die Adresse des Empfängers in das Feld „An“ ein. Alternativ können Sie auch den QR-Code scannen, falls der Empfänger einen bereitstellt.
> 1. Geben Sie den Betrag an Bitcoin, den Sie senden möchten, in das Feld „Betrag“ ein.
> 1. Überprüfen Sie die Adresse des Empfängers und den zu sendenden Betrag sorgfältig. Denken Sie daran: Transaktionen sind unwiderruflich!
> 1. Bevor Sie auf „Bestätigen und Senden“ klicken, empfehlen wir, die Transaktionsdetails noch einmal zu überprüfen, um sicherzustellen, dass Sie den richtigen Betrag an die richtige Adresse senden.
> 1. Senden Sie die Transaktion und warten Sie, bis das Netzwerk die Transaktion bestätigt.
>
> Jetzt wissen Sie, wie Sie eine selbstverwaltete Bitcoin-Wallet bewerten, auswählen und einrichten. Das Senden und Empfangen von Bitcoin im Bitcoin-Netzwerk wird als „On-Chain“-Transaktion bezeichnet. Das liegt daran, dass die Transaktionen im Hauptnetzwerk von Bitcoin stattfinden und in der Blockchain aufgezeichnet werden.
>
> On-Chain-Transaktionen sind die sicherste Möglichkeit, mit Bitcoin zu handeln, da die dezentrale Verifizierung durch das Netzwerk erfolgt.
>
> Allerdings sind On-Chain-Transaktionen langsamer und können aufgrund der Miner-Gebühr deutlich teurer sein als andere Optionen (die wir in Modul 7 besprechen werden).



---


#### Aktivität: Transaktionen in Aktion

https://qr.myfirstbitcoin.org/transactions.pdf

**Dies ist eine kooperative Übung, die die grundlegenden Rollen der an einer Bitcoin-Transaktion beteiligten Personen vereinfacht.**

###### Wichtige Punkte

1. Es gibt vier Arten von Teilnehmern bei jeder Bitcoin-Transaktion: den Absender, den Empfänger, die Miner und die Knotenbetreiber.
1. Der Absender muss (kryptografisch) genehmigen: **den Betrag an Bitcoin** zum Senden UND die **spezifische Adresse** an die gesendet werden soll.
1. Der Empfänger muss dem Absender **eine gültige Adresse** bereitstellen UND bestätigen, dass die Transaktion erfolgreich auf der Blockchain bestätigt wurde.
1. Miner stellen sicher, dass alle Kriterien erfüllt sind, bevor sie Transaktionen zu zukünftigen Blöcken hinzufügen.
1. Node-Betreiber überprüfen, ob geminte Blöcke gültig sind, bevor sie ihre Version der Blockchain (das Hauptbuch) aktualisieren.

###### Tipp für Studierende

Wechselt durch alle vier Rollen, um zu erleben, was jeder Teilnehmer macht.
