# 6.4 Recibir y enviar transacciones

Una transacción de Bitcoin es una transferencia de la propiedad de bitcoin a un nuevo dueño. Ten en cuenta que no son las monedas reales las que se transfieren, sino su propiedad: en otras palabras, el derecho a gastarlas. Cada vez que una transacción es aceptada en un bloque, todos los nodos de la red actualizan su copia local del libro contable público para reflejar el cambio de propiedad. En este sentido, una transacción de Bitcoin se parece más a una transacción de bienes raíces (u otra propiedad) que a una transacción en efectivo.

Para "enviar" bitcoin, el remitente firma un mensaje con su clave privada, indicando a la red que el dueño legítimo del bitcoin ha transferido su propiedad al destinatario.

El bitcoin ahora quedará vinculado a la dirección del destinatario, dándole la propiedad del bitcoin, de modo que solo el nuevo dueño pueda gastarlo usando su clave privada.

Nuevas transacciones de Bitcoin se inician desde billeteras de todo el mundo, pero no existe un procesador de pagos central. En su lugar, los mineros compiten por registrar las transacciones en el libro contable.

Digamos que Juan le debe a Eliana 0.5 BTC y está listo para pagarle. Ambos tienen billeteras digitales.

1. Eliana comparte su dirección con Juan.
1. Juan usa el software de su billetera para crear la transacción, que incluye la dirección de Eliana, el monto que se transferirá (0.5 BTC) y una comisión para el minero. Las comisiones más altas hacen que sea más probable que un minero incluya la transacción en el siguiente bloque.
1. Después de firmar la transacción, esta se transmite a la red, donde es verificada por los nodos. Ellos comprueban si Juan tiene fondos suficientes y si es el dueño legítimo de las monedas que pretende gastar. Si no lo es, rechazan la transacción de inmediato.
1. Una vez verificada la transacción, los mineros eligen si agregarla al siguiente bloque, normalmente en función de la comisión seleccionada. Una vez que la transacción entra en un bloque, se agrega a la blockchain y los fondos se transfieren a la dirección de Eliana.
1. La propiedad ha sido transferida a Eliana. Ahora ella puede usar su clave privada para gastar los fondos.

_Es importante tener en cuenta que, una vez completada la transacción, no se puede revertir._

###### Cómo funciona una transacción de Bitcoin

1. La transacción se transmite a la red
1. Los mineros agrupan transacciones en un bloque
1. El bloque se agrega a la blockchain
1. La transacción se confirma


> **Light – Recepción de transacciones de Bitcoin**
>
> Para recibir bitcoin, deberás proporcionar al remitente una dirección pública de Bitcoin. Esta es una cadena única de letras y números que representa tu billetera y se utiliza para identificarla en la red Bitcoin.
>
> Puedes encontrar tu dirección pública abriendo tu billetera de Bitcoin y buscando una opción para “Recibir” o “Depositar” bitcoin.
>
> Luego puedes compartir tu dirección de Bitcoin de una de varias maneras:
>
> 1. **Copiar y pegar la dirección**: Puedes copiar la dirección resaltándola y presionando "Copiar", luego pegarla en un correo electrónico o mensaje.
> 1. **Compartir un enlace a tu billetera de Bitcoin**: Algunas billeteras de Bitcoin te permiten crear un enlace a tu billetera que puedes compartir con el remitente. Luego puede hacer clic en el enlace para acceder a tu billetera y enviar bitcoin.
> 1. **Compartir un código QR**: Si el remitente tiene un smartphone con una app de billetera de Bitcoin instalada, puede escanear el código QR para obtener tu dirección de Bitcoin.


Una vez que el remitente tenga tu dirección, puede enviarte bitcoin ingresando tu dirección y el monto que quiere enviar. Luego el bitcoin se envía desde su billetera a la tuya.

La transacción es confirmada por la red Bitcoin y suele tardar unos 10 minutos. Para mayor seguridad, se recomienda esperar dos confirmaciones, lo que toma unos 20 minutos.


> **Light – Envío de transacciones de Bitcoin**
>
> Para enviar bitcoin, necesitarás algunas cosas: una billetera de Bitcoin, la dirección pública del destinatario y la cantidad de bitcoin que quieres enviar.
>
> 1. Abre tu billetera de Bitcoin.
> 1. Navega hasta el botón “Enviar” y pega la dirección del destinatario en el campo "Para". Como alternativa, también puedes escanear el código QR si el destinatario proporciona uno.
> 1. Ingresa la cantidad de bitcoin que quieres enviar en el campo “Cantidad”.
> 1. Verifica dos veces la dirección del destinatario y la cantidad que se enviará. ¡Recuerda que las transacciones son irreversibles!
> 1. Antes de hacer clic en “Confirmar y enviar”, te recomendamos revisar los detalles de la transacción una vez más para asegurarte de que estás enviando la cantidad correcta de bitcoin a la dirección correcta.
> 1. Transmite la transacción y espera a que la red confirme la transacción.
>
> Ahora sabes cómo evaluar, seleccionar y configurar una billetera de Bitcoin de autocustodia. Enviar y recibir bitcoin en la red Bitcoin se conoce como transacciones “on-chain”. Esto se debe a que las transacciones ocurren en la red principal de Bitcoin y se registran en la blockchain.
>
> Las transacciones on-chain son la forma más segura de transaccionar con bitcoin gracias a la verificación descentralizada proporcionada por la red.
>
> Sin embargo, las transacciones on-chain son más lentas y pueden ser significativamente más costosas que otras opciones (que discutiremos en el Módulo 7) debido a la comisión del minero.


#### Actividad: Transacciones en acción


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Este es un ejercicio cooperativo que simplifica los roles básicos de las personas involucradas en una transacción de Bitcoin.**

###### Puntos clave

1. Hay cuatro tipos de participantes en cada transacción de bitcoin: el remitente, el destinatario, los mineros y los operadores de nodos.
1. El remitente debe aprobar (firmar criptográficamente) la **cantidad de bitcoin** que enviará Y la **dirección específica** a la que enviará.
1. El destinatario debe proporcionar una **dirección válida** al remitente Y verificar que la transacción se confirmó correctamente en la cadena de bloques.
1. Los mineros se aseguran de que todos los criterios sean válidos antes de añadir transacciones a futuros bloques.
1. Los operadores de nodos verifican que los bloques minados sean válidos antes de actualizar su versión de la cadena de bloques (el libro contable).

###### Consejo para estudiantes

Pasa por los cuatro roles para experimentar lo que hace cada participante.
