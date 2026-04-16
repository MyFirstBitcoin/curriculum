# 8.2 Das UTXO-Modell

##### Was sind UTXOs?

Lassen Sie sich nicht von dem seltsamen Namen einschüchtern. Sie können sich UTXOs als Stücke von Bitcoin vorstellen, ähnlich wie die Scheine und Münzen in Ihrem Portemonnaie. Wenn Sie zum Beispiel einen Artikel für 6 $ mit einem 10-$-Schein bezahlen, erhalten Sie 4 $ Wechselgeld zurück. Bitcoin funktioniert auf ähnliche Weise.

Alle Bitcoin, die Sie besitzen, bestehen aus verschiedenen UTXOs. Wenn Sie Bitcoin versenden, verwendet Ihre Wallet eines oder mehrere dieser Stücke, um die Zahlung zu tätigen.

Wenn das Stück, das Sie ausgeben, größer ist als der Betrag, den Sie senden, erhalten Sie den verbleibenden Wert als Wechselgeld in Form eines neuen UTXO zurück. Gleichzeitig erhält der Empfänger ein neues UTXO, das die von Ihnen gesendeten Bitcoin repräsentiert.

Ihr Wallet-Guthaben ist einfach der Gesamtwert aller UTXOs, die Sie kontrollieren.


> **Callout – Privatsphäre**
>
> Es ist wichtig zu beachten, dass Sie anderen Ihre UTXOs nicht bekannt machen sollten, denn wenn jemand diese kennt, kann er Ihre Transaktionen nachverfolgen und letztlich wissen, wie viel Geld Sie besitzen.


###### Beispiel

1. Alice möchte Bob 5 BTC senden.
1. Ihre Wallet verwendet zwei ihrer UTXOs, die zusammen 6 BTC wert sind.
1. Die Transaktion sendet **5 BTC an Bob**, wodurch ein neues UTXO in Bobs Wallet entsteht.
1. Die verbleibenden **0,99 BTC gehen als Wechselgeld an Alice zurück**, nachdem eine **Transaktionsgebühr von 0,01 BTC** bezahlt wurde.
1. Sobald die Transaktion bestätigt ist, wird sie in das Bitcoin-Hauptbuch aufgenommen und die von Alice verwendeten UTXOs werden als ausgegeben markiert, sodass sie nicht erneut verwendet werden können.

###### Ressourcen


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
