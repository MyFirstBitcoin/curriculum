# 8.2 O Modelo UTXO

##### O que são UTXOs?

Não se intimide com o nome estranho. Você pode pensar nos UTXOs como pedaços de bitcoin, semelhantes às notas e moedas na sua carteira. Por exemplo, se você paga por um item de R$ 6 com uma nota de R$ 10, você recebe R$ 4 de troco. O Bitcoin funciona de forma parecida.

Todo o bitcoin que você possui é composto por diferentes UTXOs. Quando você envia bitcoin, sua carteira utiliza um ou mais desses pedaços para realizar o pagamento.

Se o pedaço que você gasta for maior do que o valor que você envia, o valor restante volta para você como troco, na forma de um novo UTXO. Ao mesmo tempo, o destinatário recebe um novo UTXO representando o bitcoin que você enviou.

O saldo da sua carteira é simplesmente o valor total de todos os UTXOs que você controla.


> **Callout – Privacidade**
>
> Você não deve tornar seus UTXOs conhecidos por outras pessoas, pois quando alguém os conhece, pode rastrear suas transações e, no final, saberá quanto dinheiro você possui.


###### Exemplo

1. Alice quer enviar 5 BTC para Bob.
1. A carteira dela utiliza dois de seus UTXOs que juntos valem 6 BTC.
1. A transação envia **5 BTC para Bob**, criando um novo UTXO na carteira de Bob.
1. O restante **0,99 BTC retorna para Alice como troco**, após pagar uma **taxa de transação de 0,01 BTC**.
1. Assim que a transação é confirmada, ela é adicionada ao registro do Bitcoin e os UTXOs usados por Alice são marcados como gastos, então não podem ser usados novamente.

###### Recursos


[▶ Assista “How Bitcoin Works under the Hood”](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
