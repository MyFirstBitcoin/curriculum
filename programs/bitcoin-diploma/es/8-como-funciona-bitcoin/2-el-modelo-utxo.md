# 8.2 El modelo UTXO

##### ¿Qué son los UTXO?

No te dejes intimidar por este nombre extraño. Puedes pensar en los UTXO como piezas de bitcoin, similares a los billetes y monedas de tu billetera. Por ejemplo, si pagas un artículo de 6 MXN con un billete de 10 MXN, recibes 4 MXN de cambio. Bitcoin funciona de manera similar.

Todo el bitcoin que posees está compuesto por diferentes UTXO. Cuando envías bitcoin, tu billetera utiliza una o más de estas piezas para realizar el pago.

Si la pieza que gastas es mayor que la cantidad que envías, el valor restante vuelve a ti como cambio en forma de un nuevo UTXO. Al mismo tiempo, el destinatario recibe un nuevo UTXO que representa el bitcoin que enviaste.

El saldo de tu billetera es simplemente el valor total de todos los UTXO que controlas.


> **Callout – Privacidad**
>
> No deberías permitir que otras personas sepan cuáles son tus UTXO, porque cuando alguien los conoce, puede rastrear tus transacciones y finalmente sabrá cuánto dinero posees.


###### Ejemplo

1. Alicia quiere enviarle 5 BTC a Roberto.
1. Su billetera utiliza dos de sus UTXO que juntos valen 6 BTC.
1. La transacción envía **5 BTC a Roberto**, creando un nuevo UTXO en la billetera de Roberto.
1. Los **0.99 BTC restantes vuelven a Alicia como cambio**, después de pagar una **comisión de transacción de 0.01 BTC**.
1. Una vez que la transacción se confirma, se añade al libro contable de Bitcoin y los UTXO utilizados por Alicia se marcan como gastados, por lo que no pueden volver a utilizarse.

###### Recursos


[▶ Mira “Cómo funciona Bitcoin por dentro”](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
