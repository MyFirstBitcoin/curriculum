# 6.4 Recibir y enviar transacciones

Una transacción de Bitcoin es una transferencia de propiedad de bitcoin a un nuevo dueño. Ten en cuenta que no se transfieren las monedas en sí, sino la propiedad de las mismas: es decir, el derecho a gastarlas. Cada vez que una transacción es aceptada en un bloque, todos los nodos de la red actualizan su copia local del libro público para reflejar el cambio de propiedad. En este sentido, una transacción de Bitcoin se parece más a una transacción inmobiliaria (u otra transacción de bienes) que a una transacción en efectivo.

Para "enviar" bitcoin, el remitente firma un mensaje con su clave privada, señalando a la red que el legítimo propietario del bitcoin ha transferido su propiedad al destinatario.

El bitcoin ahora estará vinculado a la dirección del destinatario, dándole la propiedad del bitcoin, de modo que solo el nuevo dueño podrá gastarlos usando su clave privada.

Nuevas transacciones de Bitcoin se inician desde billeteras en todo el mundo, pero no existe un procesador de pagos central. En su lugar, los mineros compiten para registrar las transacciones en el libro contable.

Supongamos que Jaime le debe a Eliana 0.5 BTC y está listo para pagarle. Ambos tienen billeteras digitales.

1. Eliana comparte su dirección con Jaime.
1. Jaime usa el software de su billetera para crear la transacción, que incluye la dirección de Eliana, la cantidad a transferir (0.5 BTC) y una comisión para el minero. Comisiones más altas hacen más probable que un minero incluya la transacción en el siguiente bloque.
1. Después de firmar la transacción, se transmite a la red, donde es verificada por los nodos. Ellos revisan si Jaime tiene fondos suficientes y es el legítimo propietario de las monedas que quiere gastar. Si no lo es, rechazan la transacción de inmediato.
1. Una vez que la transacción es verificada, los mineros deciden si agregar la transacción al siguiente bloque, usualmente según la comisión seleccionada. Cuando la transacción entra en un bloque, se añade a la blockchain y los fondos se transfieren a la dirección de Eliana.
1. La propiedad ha sido transferida a Eliana. Ahora ella puede usar su clave privada para gastar los fondos.

_Es importante notar que una vez que la transacción se completa, no puede ser revertida._


> **Note – Cómo funciona una transacción de Bitcoin**
>
> 1. Alguien solicita una transacción
> 1. La transacción se transmite a computadoras P2P (nodos)
> 1. Los mineros verifican la transacción
> 1. Las transacciones se combinan para formar un bloque de datos
> 1. Nuevo bloque añadido a la blockchain existente
> 1. La transacción está completa



> **Note – Recibiendo transacciones de Bitcoin**
>
> Para recibir bitcoin, necesitarás proporcionar al remitente una dirección pública de Bitcoin. Esta es una cadena única de letras y números que representa tu billetera y se usa para identificarla en la red de Bitcoin.
>
> Puedes encontrar tu dirección pública abriendo tu billetera de Bitcoin y buscando una opción para “Recibir” o “Depositar” bitcoin.
>
> Luego puedes compartir tu dirección de Bitcoin de varias maneras:
>
> 1. **Copiar y pegar la dirección**: Puedes copiar la dirección seleccionándola y presionando "Copiar", luego pegarla en un correo electrónico o mensaje.
> 1. **Compartir un enlace a tu billetera de Bitcoin**: Algunas billeteras de Bitcoin te permiten crear un enlace a tu billetera que puedes compartir con el remitente. Luego, pueden hacer clic en el enlace para acceder a tu billetera y enviarte bitcoin.
> 1. **Compartir un código QR**: Si el remitente tiene un teléfono inteligente con una aplicación de billetera de Bitcoin instalada, puede escanear el código QR para obtener tu dirección de Bitcoin.


Una vez que el remitente tiene tu dirección, puede enviarte bitcoin ingresando tu dirección y la cantidad que desea enviar. El bitcoin se envía desde su billetera a la tuya.

La transacción es confirmada por la Red de Bitcoin y usualmente toma alrededor de 10 minutos. Para mayor seguridad, se recomienda esperar dos confirmaciones, lo que toma aproximadamente 20 minutos.


> **Note – Enviando transacciones de Bitcoin**
>
> Para enviar bitcoin, necesitarás algunas cosas: una billetera de Bitcoin, la dirección pública del destinatario y la cantidad de bitcoin que deseas enviar.
>
> 1. Abre tu billetera de Bitcoin.
> 1. Navega al botón “Enviar” y pega la dirección del destinatario en el campo "Para". Alternativamente, también puedes escanear el código QR si el destinatario proporciona uno.
> 1. Ingresa la cantidad de bitcoin que deseas enviar en el campo “Cantidad”.
> 1. Verifica dos veces la dirección del destinatario y la cantidad a enviar. ¡Recuerda que las transacciones son irreversibles!
> 1. Antes de hacer clic en “Confirmar y Enviar”, te recomendamos revisar los detalles de la transacción una vez más para asegurarte de que estás enviando la cantidad correcta de bitcoin a la dirección correcta.
> 1. Transmite la transacción y espera a que la red confirme la transacción.
>
> Ahora sabes cómo evaluar, seleccionar y configurar una billetera de Bitcoin de autocustodia. Enviar y recibir bitcoin en la red de Bitcoin se conoce como transacciones “on-chain”. Esto se debe a que las transacciones ocurren en la red principal de Bitcoin y se registran en la blockchain.
>
> Las transacciones on-chain son la forma más segura de transaccionar con bitcoin debido a la verificación descentralizada que proporciona la red.
>
> Sin embargo, las transacciones on-chain son más lentas y pueden ser significativamente más caras que otras opciones (que veremos en el Módulo 7) debido a la comisión del minero.


#### Actividad: Transacciones en acción

https://qr.myfirstbitcoin.org/transactions.pdf

**Este es un ejercicio cooperativo que simplifica los roles básicos de las personas involucradas en una transacción de Bitcoin.**

###### Puntos clave

1. Hay cuatro tipos de participantes en cada transacción de bitcoin: el remitente, el destinatario, los mineros y los operadores de nodos.
1. El remitente debe aprobar (firmar criptográficamente) la **cantidad de bitcoin** a enviar Y la **dirección específica** a la que se enviará.
1. El destinatario debe proporcionar una **dirección válida** al remitente Y verificar que la transacción fue confirmada exitosamente en la blockchain.
1. Los mineros se aseguran de que todos los criterios sean válidos antes de agregar transacciones a los bloques futuros.
1. Los operadores de nodos verifican que los bloques minados sean válidos antes de actualizar su versión de la blockchain (el libro mayor).

###### Consejo para estudiantes

Rota entre los cuatro roles para experimentar lo que hace cada participante.
