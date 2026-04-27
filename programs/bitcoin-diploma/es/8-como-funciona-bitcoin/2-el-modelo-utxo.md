# 8.2 El modelo UTXO

##### ¿Qué son los UTXOs?

No te intimides por el nombre extraño. Puedes pensar en los UTXOs como pedazos de bitcoin, similares a los billetes y monedas en tu cartera. Por ejemplo, si pagas un artículo de $120 MXN con un billete de $200 MXN, recibes $80 MXN de cambio. Bitcoin funciona de manera similar.

Todo el bitcoin que posees está compuesto por diferentes UTXOs. Cuando envías bitcoin, tu cartera utiliza una o más de estas piezas para realizar el pago.

Si la pieza que gastas es mayor que la cantidad que envías, el valor restante regresa a ti como cambio en forma de un nuevo UTXO. Al mismo tiempo, el destinatario recibe un nuevo UTXO que representa el bitcoin que le enviaste.

El saldo de tu cartera es simplemente el valor total de todos los UTXOs que controlas.


> **Callout – Privacidad**
>
> No deberías hacer que otros conozcan tus UTXOs porque, si alguien los sabe, puede rastrear tus transacciones y, en última instancia, sabrá cuánto dinero tienes.


###### Ejemplo

1. Alicia quiere enviarle 5 BTC a Beto.
1. Su cartera utiliza dos de sus UTXOs que juntos valen 6 BTC.
1. La transacción envía **5 BTC a Beto**, creando un nuevo UTXO en la cartera de Beto.
1. El restante **0.99 BTC regresa a Alicia como cambio**, después de pagar una **comisión de transacción de 0.01 BTC**.
1. Una vez que la transacción es confirmada, se añade al libro mayor de Bitcoin y los UTXOs usados por Alicia se marcan como gastados, por lo que no pueden volver a usarse.

###### Recursos


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
