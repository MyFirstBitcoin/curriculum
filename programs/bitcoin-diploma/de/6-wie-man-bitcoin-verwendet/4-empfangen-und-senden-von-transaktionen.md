# 6.4 Empfangen und Senden von Transaktionen

Eine Bitcoin-Transaktion ist die Übertragung des Eigentums an Bitcoin auf einen neuen Besitzer. Beachte, dass nicht die eigentlichen Münzen übertragen werden, sondern das Eigentum an ihnen: Mit anderen Worten, das Recht, sie auszugeben. Jedes Mal, wenn eine Transaktion in einen Block aufgenommen wird, aktualisieren alle Knoten im Netzwerk ihre lokale Kopie des öffentlichen Hauptbuchs, um den Eigentümerwechsel widerzuspiegeln. In dieser Hinsicht ähnelt eine Bitcoin-Transaktion eher einer Immobilien- (oder anderen Eigentums-)Transaktion als einer Bargeldtransaktion.

Um Bitcoin zu „senden“, signiert der Absender eine Nachricht mit seinem privaten Schlüssel und signalisiert dem Netzwerk, dass der rechtmäßige Besitzer der Bitcoin das Eigentum an den Empfänger übertragen hat.

Die Bitcoin sind nun mit der Adresse des Empfängers verknüpft, wodurch dieser das Eigentum an den Bitcoin erhält, sodass nur der neue Besitzer sie mit seinem privaten Schlüssel ausgeben kann.

Neue Bitcoin-Transaktionen werden von Wallets auf der ganzen Welt initiiert, aber es gibt keinen zentralen Zahlungsabwickler. Stattdessen konkurrieren Miner darum, Transaktionen im Hauptbuch zu verzeichnen.

Nehmen wir an, Jens schuldet Eliana 0,5 BTC und ist bereit, sie zurückzuzahlen. Beide haben digitale Wallets.

1. Eliana teilt Jens ihre Adresse mit.
1. Jens verwendet seine Wallet-Software, um die Transaktion zu erstellen. Diese enthält Elianas Adresse, den zu übertragenden Betrag (0,5 BTC) und eine Gebühr für den Miner. Höhere Gebühren erhöhen die Wahrscheinlichkeit, dass ein Miner die Transaktion in den nächsten Block aufnimmt.
1. Nachdem die Transaktion signiert wurde, wird sie an das Netzwerk gesendet, wo sie von den Knoten überprüft wird. Sie prüfen, ob Jens genügend Guthaben hat und der rechtmäßige Besitzer der Münzen ist, die er ausgeben möchte. Falls nicht, wird die Transaktion sofort abgelehnt.
1. Sobald die Transaktion verifiziert ist, wählen Miner aus, ob sie die Transaktion in den nächsten Block aufnehmen, meist basierend auf der gewählten Gebühr. Sobald die Transaktion in einen Block aufgenommen wurde, wird sie zur Blockchain hinzugefügt und die Mittel werden an Elianas Adresse übertragen.
1. Das Eigentum wurde auf Eliana übertragen. Sie kann nun ihren privaten Schlüssel verwenden, um die Mittel auszugeben.

_Es ist wichtig zu beachten, dass eine abgeschlossene Transaktion nicht rückgängig gemacht werden kann._


> **Light – Wie eine Bitcoin-Transaktion funktioniert**
>
> 1. Jemand fordert eine Transaktion an
> 1. Transaktion wird an P2P-Computer (Knoten) gesendet
> 1. Miner überprüfen die Transaktion
> 1. Transaktionen werden zu einem Datenblock zusammengefasst
> 1. Neuer Block wird zur bestehenden Blockchain hinzugefügt
> 1. Die Transaktion ist abgeschlossen



> **Light – Bitcoin-Transaktionen empfangen**
>
> Um Bitcoin zu empfangen, musst du dem Absender eine Bitcoin-Öffentlich-Adresse bereitstellen. Dies ist eine einzigartige Zeichenfolge aus Buchstaben und Zahlen, die deine Wallet repräsentiert und zur Identifizierung im Bitcoin-Netzwerk dient.
>
> Du findest deine öffentliche Adresse, indem du deine Bitcoin-Wallet öffnest und nach einer Option wie „Empfangen“ oder „Einzahlen“ suchst.
>
> Du kannst deine Bitcoin-Adresse dann auf verschiedene Arten teilen:
>
> 1. **Adresse kopieren und einfügen**: Du kannst die Adresse markieren und auf „Kopieren“ drücken, dann in eine E-Mail oder Nachricht einfügen.
> 1. **Einen Link zu deiner Bitcoin-Wallet teilen**: Manche Bitcoin-Wallets erlauben es dir, einen Link zu deiner Wallet zu erstellen, den du mit dem Absender teilen kannst. Dieser kann dann auf den Link klicken, um auf deine Wallet zuzugreifen und Bitcoin zu senden.
> 1. **Einen QR-Code teilen**: Wenn der Absender ein Smartphone mit einer Bitcoin-Wallet-App hat, kann er den QR-Code scannen, um deine Bitcoin-Adresse zu erhalten.


Sobald der Absender deine Adresse hat, kann er dir Bitcoin senden, indem er deine Adresse und den gewünschten Betrag eingibt. Die Bitcoin werden dann von seiner Wallet an deine Wallet gesendet.

Die Transaktion wird vom Bitcoin-Netzwerk bestätigt und dauert in der Regel etwa 10 Minuten. Für mehr Sicherheit empfiehlt es sich, auf zwei Bestätigungen zu warten, was etwa 20 Minuten dauert.


> **Light – Bitcoin-Transaktionen senden**
>
> Um Bitcoin zu senden, benötigst du Folgendes: eine Bitcoin-Wallet, die öffentliche Adresse des Empfängers und den Betrag an Bitcoin, den du senden möchtest.
>
> 1. Öffne deine Bitcoin-Wallet.
> 1. Gehe zum „Senden“-Button und füge die Adresse des Empfängers in das Feld „An“ ein. Alternativ kannst du auch den QR-Code scannen, falls der Empfänger einen bereitstellt.
> 1. Gib den Betrag an Bitcoin ein, den du im Feld „Betrag“ senden möchtest.
> 1. Überprüfe die Adresse des Empfängers und den zu sendenden Betrag sorgfältig. Denke daran: Transaktionen sind unwiderruflich!
> 1. Bevor du auf „Bestätigen und Senden“ klickst, empfehlen wir, die Transaktionsdetails noch einmal zu überprüfen, um sicherzustellen, dass du den richtigen Betrag an die richtige Adresse sendest.
> 1. Sende die Transaktion und warte, bis das Netzwerk die Transaktion bestätigt.
>
> Jetzt weißt du, wie du eine selbstverwaltete Bitcoin-Wallet auswählst, einrichtest und bewertest. Das Senden und Empfangen von Bitcoin im Bitcoin-Netzwerk wird als „On-Chain“-Transaktion bezeichnet. Das liegt daran, dass die Transaktionen im Hauptnetzwerk von Bitcoin stattfinden und in der Blockchain aufgezeichnet werden.
>
> On-Chain-Transaktionen sind die sicherste Art, mit Bitcoin zu handeln, da die dezentrale Verifizierung durch das Netzwerk erfolgt.
>
> Allerdings sind On-Chain-Transaktionen langsamer und können aufgrund der Miner-Gebühr deutlich teurer sein als andere Optionen (die wir in Modul 7 besprechen werden).


#### Aktivität: Transaktionen in Aktion


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Dies ist eine kooperative Übung, die die grundlegenden Rollen der an einer Bitcoin-Transaktion beteiligten Personen vereinfacht.**

###### Wichtige Punkte

1. Es gibt vier Arten von Teilnehmern bei jeder Bitcoin-Transaktion: den Absender, den Empfänger, die Miner und die Knotenbetreiber.
1. Der Absender muss (kryptografisch) genehmigen **den Bitcoin-Betrag** zum Senden UND die **spezifische Adresse** an die gesendet werden soll.
1. Der Empfänger muss dem Absender eine **gültige Adresse** bereitstellen UND überprüfen, dass die Transaktion erfolgreich auf der Blockchain bestätigt wurde.
1. Miner stellen sicher, dass alle Kriterien erfüllt sind, bevor sie Transaktionen zu zukünftigen Blöcken hinzufügen.
1. Node-Betreiber überprüfen, ob geminte Blöcke gültig sind, bevor sie ihre Version der Blockchain (das Hauptbuch) aktualisieren.

###### Tipp für Lernende

Wechselt zwischen allen vier Rollen, um zu erleben, was jeder Teilnehmer macht.
