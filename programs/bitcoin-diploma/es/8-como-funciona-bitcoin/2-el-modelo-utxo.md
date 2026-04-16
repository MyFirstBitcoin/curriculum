# 8.2 El modelo UTXO

##### ¿Qué son los UTXOs?

No te dejes intimidar por el nombre extraño. Puedes pensar en los UTXOs como piezas de bitcoin, similares a los billetes y monedas en tu billetera. Por ejemplo, si pagas un artículo de $6 con un billete de $10, recibes $4 de cambio. Bitcoin funciona de manera similar.

Todos los bitcoin que posees están formados por diferentes UTXOs. Cuando envías bitcoin, tu billetera utiliza una o más de estas piezas para realizar el pago.

Si la pieza que gastas es mayor que la cantidad que envías, el valor restante se te devuelve como cambio en forma de un nuevo UTXO. Al mismo tiempo, el destinatario recibe un nuevo UTXO que representa los bitcoin que le enviaste.

El saldo de tu billetera es simplemente el valor total de todos los UTXOs que controlas.


> **Callout – Privacidad**
>
> Es importante tener en cuenta que no debes hacer que otros conozcan tus UTXOs, porque cuando alguien los conoce, puede rastrear tus transacciones y, en última instancia, sabrá cuánto dinero posees.


###### Ejemplo

1. Alice quiere enviar a Bob 5 BTC.
1. Su billetera utiliza dos de sus UTXOs que juntos valen 6 BTC.
1. La transacción envía **5 BTC a Bob**, creando un nuevo UTXO en la billetera de Bob.
1. El resto, **0.99 BTC, regresa a Alice como cambio**, después de pagar una **comisión de transacción de 0.01 BTC**.
1. Una vez que la transacción se confirma, se añade al libro contable de Bitcoin y los UTXOs utilizados por Alice se marcan como gastados, por lo que no pueden volver a usarse.

###### Recursos


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
