# 6.4 Recibir y enviar transacciones

Una transacción de bitcoin es una transferencia de propiedad de bitcoin a un nuevo propietario. Ten en cuenta que no se transfieren las monedas en sí, sino la propiedad de las mismas: es decir, el derecho a gastarlas. Cada vez que una transacción es aceptada en un bloque, todos los nodos de la red actualizan su copia local del libro público para reflejar el cambio de propiedad. En este sentido, una transacción de bitcoin se parece más a una transacción inmobiliaria (u otra transacción de propiedad) que a una transacción en efectivo.

Para "enviar" bitcoin, el remitente firma un mensaje con su clave privada, indicando a la red que el propietario legítimo de los bitcoins ha transferido su propiedad al destinatario.

Los bitcoins ahora estarán vinculados a la dirección del destinatario, dándole la propiedad de los bitcoins, de modo que solo el nuevo propietario podrá gastarlos utilizando su clave privada.

Las nuevas transacciones de Bitcoin se inician desde monederos de todo el mundo, pero no hay un procesador de pagos central. En cambio, los mineros compiten para registrar las transacciones en el libro contable.

Supongamos que Jim le debe 0.5 BTC a Eliana y está listo para pagarle. Ambos tienen monederos digitales.

1. Eliana comparte su dirección con Jim.
1. Jim utiliza el software de su monedero para crear la transacción, que incluye la dirección de Eliana, la cantidad a transferir (0.5 BTC) y una comisión para el minero. Las comisiones más altas hacen que sea más probable que un minero incluya la transacción en el siguiente bloque.
1. Después de firmar la transacción, esta se transmite a la red, donde es verificada por los nodos. Ellos comprueban si Jim tiene fondos suficientes y si es el propietario legítimo de las monedas que desea gastar. Si no es así, rechazan la transacción de inmediato.
1. Una vez que la transacción es verificada, los mineros deciden si la añaden al siguiente bloque, generalmente en función de la comisión seleccionada. Cuando la transacción entra en un bloque, se añade a la cadena de bloques y los fondos se transfieren a la dirección de Eliana.
1. La propiedad ha sido transferida a Eliana. Ahora puede usar su clave privada para gastar los fondos recibidos.

_Es importante tener en cuenta que una vez que la transacción se completa, no puede ser revertida._


> **Note – Cómo funciona una transacción de Bitcoin**
>
> 1. Alguien solicita una transacción
> 1. La transacción se transmite a computadoras P2P (nodos)
> 1. Los mineros verifican la transacción
> 1. Las transacciones se combinan para formar un bloque de datos
> 1. El nuevo bloque se añade a la cadena de bloques existente
> 1. La transacción está completa



> **Note – Recepción de transacciones de Bitcoin**
>
> Para recibir bitcoin, deberás proporcionar al remitente una dirección pública de Bitcoin. Esta es una cadena única de letras y números que representa tu monedero y se utiliza para identificarlo en la red de Bitcoin.
>
> Puedes encontrar tu dirección pública abriendo tu monedero de Bitcoin y buscando una opción para “Recibir” o “Depositar” bitcoin.
>
> Luego puedes compartir tu dirección de Bitcoin de varias maneras:
>
> 1. **Copiar y pegar la dirección**: Puedes copiar la dirección seleccionándola y presionando "Copiar" en tu teclado, luego pegarla en un correo electrónico o mensaje al remitente.
> 1. **Compartir un enlace a tu monedero de Bitcoin**: Algunos monederos de Bitcoin permiten crear un enlace a tu monedero que puedes compartir con el remitente. Luego pueden hacer clic en el enlace para acceder a tu monedero y enviar los bitcoins.
> 1. **Compartir un código QR**: Si el remitente tiene un teléfono inteligente con una aplicación de monedero de Bitcoin, puede escanear el código QR para obtener tu dirección de bitcoin.


Una vez que el remitente tiene tu dirección, puede enviarte bitcoins ingresando tu dirección y la cantidad que desea enviarte. Los bitcoins se enviarán desde su monedero al tuyo.

La transacción se confirma en la red de Bitcoin y normalmente tarda unos 10 minutos. Para mayor seguridad, se recomienda esperar dos confirmaciones, lo que toma aproximadamente 20 minutos.


> **Note – Envío de transacciones de bitcoin**
>
> Para enviar bitcoins, necesitarás algunas cosas: un monedero de Bitcoin, la dirección pública del destinatario y la cantidad de bitcoin que deseas enviar.
>
> 1. Abre tu monedero de Bitcoin.
> 1. Ve a la función "Enviar" y pega la dirección del destinatario en el campo "Para". Alternativamente, también puedes escanear el código QR si el destinatario lo proporciona.
> 1. Ingresa la cantidad de bitcoin que deseas enviar en el campo “Cantidad”.
> 1. Verifica dos veces la dirección del destinatario y la cantidad a enviar. ¡Recuerda que las transacciones son irreversibles!
> 1. Antes de hacer clic en “Confirmar y Enviar”, te recomendamos revisar los detalles de la transacción una vez más para asegurarte de que estás enviando la cantidad correcta de bitcoin a la dirección correcta.
> 1. Transmite la transacción y espera a que la red confirme la transacción.
>
> Ahora sabes cómo evaluar, seleccionar y configurar un monedero de Bitcoin de autocustodia. El envío y la recepción de bitcoin en la red de Bitcoin se denominan transacciones “on-chain”. Esto se debe a que las transacciones ocurren en la red principal de Bitcoin y quedan registradas en la cadena de bloques.
>
> Las transacciones on-chain son la forma más segura de operar con bitcoin debido a la verificación descentralizada que proporciona la red.
>
> Sin embargo, las transacciones on-chain son más lentas y pueden ser significativamente más costosas que otras opciones (que veremos en el Módulo 7) debido a la comisión del minero.



---


#### Actividad: Transacciones en acción

https://qr.myfirstbitcoin.org/transactions.pdf

**Este es un ejercicio cooperativo que simplifica los roles básicos de las personas involucradas en una transacción de Bitcoin.**

###### Puntos clave

1. En cada transacción de bitcoin hay cuatro tipos de participantes: el remitente, el destinatario, los mineros y los operadores de nodos.
1. El remitente debe aprobar (firmar criptográficamente) la **cantidad de bitcoin** a enviar Y la **dirección específica** a la que se enviará.
1. El receptor debe proporcionar una **dirección válida** al remitente Y verificar que la transacción haya sido confirmada exitosamente en el blockchain.
1. Los mineros se aseguran de que se cumplan todos los criterios antes de agregar transacciones a los futuros bloques.
1. Los operadores de nodos verifican que los bloques minados sean válidos antes de actualizar su versión del blockchain (el libro mayor).

###### Consejo para el estudiante

Rota por los cuatro roles para experimentar lo que hace cada participante.
