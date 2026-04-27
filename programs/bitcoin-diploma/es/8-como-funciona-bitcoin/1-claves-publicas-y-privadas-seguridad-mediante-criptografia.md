# 8.1 Claves públicas y privadas: Seguridad mediante criptografía

> Lo que Bitcoin nos da es una promesa firme: el programa se ejecutará exactamente como está especificado.  
_Andreas M. Antonopoulos_

#### Criptografía de clave pública/privada


> **Definition – Definición de Criptografía**
>
> **Criptografía** es la práctica de convertir información en un secreto que solo las personas correctas pueden leer.


* **Encriptación** es el proceso de convertir información en una forma codificada para que solo alguien con la clave correcta pueda leerla.
* **Desencriptación** es el proceso de convertir esa información codificada de nuevo en algo legible.

En la criptografía tradicional, dos personas que quieren comunicarse en privado primero deben compartir la misma clave secreta, similar a una contraseña compartida. Una persona usa esta clave para encriptar el mensaje antes de enviarlo, y la otra persona usa la misma clave para desencriptarlo y leerlo.

El problema con este sistema es que ambas personas ya deben compartir la clave secreta. Si alguien más obtiene acceso a esa clave, puede leer cualquier mensaje interceptado.

Bitcoin resuelve este problema usando un enfoque diferente llamado criptografía de clave pública, donde los usuarios no necesitan compartir claves secretas de antemano.

La criptografía de clave pública/privada resuelve el problema de compartir secretos. En vez de compartir una contraseña, cada persona tiene dos claves: una clave pública y una clave privada.

* La **clave pública** se puede compartir con cualquiera.
* La **clave privada** siempre debe mantenerse en secreto.

Si Juan quiere enviarle algo a Ariel, puede usar la clave pública de Ariel. Solo Ariel puede desbloquearlo usando su clave privada. Incluso si alguien intercepta el mensaje, no puede leerlo ni usarlo sin la clave privada.

En Bitcoin, este sistema se utiliza para crear firmas digitales. Una firma digital prueba que el dueño de una clave privada aprobó una transacción, similar a firmar tu nombre en un documento. Esto es lo que permite que las transacciones de Bitcoin sean seguras y verificables sin confiar en un tercero.

Las transacciones de Bitcoin implican transferir la propiedad de bitcoin de una dirección a otra.

La encriptación se utiliza para asegurar que solo el verdadero poseedor del bitcoin tenga la autoridad para enviar su dinero a otra persona. Garantiza que su propiedad esté protegida contra actores maliciosos.

Como medida adicional de protección, cada transacción de Bitcoin recibe automáticamente una firma digital ÚNICA. Esta firma digital única está impulsada por tecnología a prueba de manipulaciones que ayuda a la red a verificar que el verdadero dueño del bitcoin, y no otra persona, los haya enviado.


> **Info**
>
> Cada usuario tiene dos claves: una **clave privada**, que se **mantiene en secreto**, y una **clave pública** que puede ser **compartida con otros**. La **clave privada** sirve como una forma de identificación y prueba de propiedad, confirmando: “Esta dirección me pertenece y tengo control sobre ella.”


###### Cómo funciona una transacción de Bitcoin

1. **Creación de la transacción**: Un usuario inicia una transacción de Bitcoin especificando detalles como la dirección del destinatario y la cantidad de bitcoin a enviar.
1. **Generación de la firma digital**: El remitente genera una **firma digital** única usando su **clave privada**. Esta firma es un código único que verifica la autenticidad de la transacción.
1. **Transmisión de la transacción**: La transacción firmada se transmite a la red de Bitcoin, indicando la intención de transferir la propiedad de bitcoin del remitente al destinatario.
1. **Verificación en la red**: Los nodos de la red de Bitcoin reciben la transacción y usan la **clave pública** para verificar la autenticidad de la firma de la transacción. Al mismo tiempo, utilizan la **clave pública** para verificar la **firma digital**.
1. **Confirmación en la red de Bitcoin**: Si la verificación es exitosa, la transacción se añadirá al libro mayor, que sirve como un registro seguro y transparente de todas las transacciones. Una vez confirmada, la propiedad del bitcoin se transfiere oficialmente del remitente al destinatario.


> **Callout – Resumen**
>
> La **firma digital**, creada con la **clave privada** del remitente, demuestra que la transacción fue autorizada por el dueño del bitcoin. La red de Bitcoin puede entonces verificar esta prueba y registrar la transacción.


#### Explicación del Hashing

Por favor, no te intimides por los términos técnicos y conceptos matemáticos que vienen a continuación. Entendemos que no a todos les apasionan las matemáticas, pero podrías sorprenderte y ver que incluso las ideas más complejas pueden entenderse con un poco de esfuerzo.


> **Definition – Definición de una función**
>
> Una **función** es como una máquina que toma cierta información y la convierte en algo nuevo. La información que le das a la función es la **entrada**. La nueva información que crea la función es la **salida**. Las funciones ayudan a las computadoras a realizar tareas y resolver problemas.


##### ¿Qué es una función?

Una función es un conjunto de instrucciones que toma una entrada y produce una salida. Puedes pensar en ella como una receta: sigues los pasos con ciertos ingredientes y siempre obtienes un resultado predecible.

En Bitcoin, las funciones se utilizan para procesar y verificar transacciones. Cuando alguien envía bitcoin, las funciones criptográficas ayudan a comprobar que la transacción es válida, confirman que el remitente tiene fondos suficientes y actualizan los saldos en el libro mayor de Bitcoin. Una vez verificada y añadida a un bloque, la transacción pasa a formar parte del registro permanente en la blockchain.

##### ¿Qué es una función unidireccional?

Una función unidireccional es un tipo especial de función que es fácil de calcular en una dirección pero extremadamente difícil de revertir. Por ejemplo, hacer un licuado con ingredientes es fácil, pero no puedes separar el licuado de nuevo en los ingredientes originales.

La seguridad de Bitcoin depende de las funciones unidireccionales. Se utilizan en la criptografía de clave pública y privada, permitiendo que las personas compartan una clave pública mientras mantienen su clave privada en secreto. Aunque la clave pública es visible, es imposible derivar la clave privada a partir de ella. Esto es lo que hace que las transacciones de Bitcoin sean seguras.

##### ¿Qué es una función hash?

Una **función hash** es como una máquina de códigos secretos. Toma un mensaje y lo convierte en un código.

###### Cómo funciona el Hashing en las transacciones de Bitcoin

En Bitcoin, cada transacción se convierte en un hash antes de ser añadida a la blockchain. Un hash es una huella digital única de la transacción. Si alguien intenta cambiar incluso una pequeña parte de la transacción, el hash cambiará completamente. Esto facilita que la red detecte cualquier manipulación.

###### El papel del Hashing en la seguridad de Bitcoin

El hashing ayuda a proteger la red de Bitcoin haciendo que las transacciones sean fáciles de verificar e imposibles de modificar en secreto. Como cada transacción tiene su propio hash único, la red puede detectar rápidamente si algo ha sido alterado.

Una función hash toma datos y los convierte en una cadena fija de números y letras llamada hash. La misma entrada siempre producirá el mismo hash, pero incluso un pequeño cambio en la entrada generará un resultado completamente diferente. Esta propiedad permite a las computadoras comprobar que los datos no han sido modificados.


> **Definition – Definición de Hashing**
>
> **Hashing** es como crear una huella digital para los datos digitales. Es el proceso de tomar un mensaje digital y convertirlo en un código de longitud fija, que sirve como un identificador único. Así como una huella digital puede identificar a una persona, un hash puede identificar un mensaje digital.


La **salida**, o hash, siempre tiene la misma longitud, sin importar cuán larga era la información original. Bitcoin utiliza algunos tipos específicos de función hash llamados **SHA-256** y **RIPEMD160**.

Algunos ejemplos se muestran a continuación:

* Hash SHA256 de la cadena **hola mundo**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Hash SHA256 de la cadena **hola mundo.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Observa que un pequeño cambio en la entrada cambia completamente la salida en comparación con la primera.
* Hash SHA256 del archivo iso descargable **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Esta entrada es un archivo enorme, pero la salida sigue teniendo la misma longitud fija.

También puedes pensar en el hash como una partitura musical que captura la esencia de una pieza de música. Así como una partitura es una representación única de una melodía, un valor hash es una representación única de un dato.

Al comparar la partitura de una pieza musical con la interpretación real, un músico puede determinar si la interpretación es precisa. De manera similar, al comparar el valor hash de los datos recibidos con el valor hash original, se puede determinar si los datos han sido alterados durante la transmisión.

Así como una pequeña desviación en una interpretación musical puede hacer que suene diferente, incluso el cambio más pequeño en los datos originales resultará en un valor hash diferente. Esto hace que el hash sea una herramienta poderosa para garantizar la integridad y autenticidad de una transacción de Bitcoin.

El proceso de codificar la **clave pública** mediante hashing se utiliza para mejorar la seguridad de la información convirtiéndola en un formato ilegible de longitud fija. Bitcoin utiliza los algoritmos SHA-256 y RIPEMD160 para producir direcciones públicas. El resultado sirve como un identificador único para la **clave pública** y ayuda a garantizar la integridad y seguridad de las transacciones almacenadas en el libro mayor. Al cifrar la información de esta manera, se vuelve más difícil para personas no autorizadas acceder y manipular los datos.

##### Propiedades de una función hash

* **Determinista**: Los mismos ingredientes siempre producen el mismo batido. De la misma manera, los mismos datos siempre producirán el mismo hash.
* **Resistencia a la preimagen**: Si solo tienes el batido, no puedes saber exactamente qué frutas se usaron. De manera similar, si solo tienes un hash, no puedes determinar los datos originales.
* **Efecto avalancha**: Cambiar incluso una pequeña parte de los ingredientes crea un batido completamente diferente. En el hash, un cambio muy pequeño en los datos produce un hash completamente diferente.
* **Resistencia a colisiones**: Es extremadamente difícil encontrar dos conjuntos diferentes de ingredientes que produzcan exactamente el mismo batido. De la misma manera, es extremadamente improbable que dos datos diferentes produzcan el mismo hash.
* **Fácil de verificar**: Hacer el batido es rápido, y es fácil comprobar que el resultado es un batido. Las funciones hash son rápidas de calcular y fáciles de verificar para cualquiera.

#### Actividad: Genera un hash SHA 256

https://tools.keycdn.com/sha256-online-generator

¿Tienes curiosidad sobre cómo funciona el hash? Escanea el código QR para generar al instante un hash SHA256 de cualquier palabra, frase o entrada que elijas. Las funciones hash son como huellas digitales digitales: son de una sola vía, es decir, una vez que algo se ha hasheado, no se puede revertir. ¡Pruébalo y compruébalo tú mismo!
