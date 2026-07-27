# 8 - Cómo funciona Bitcoin

Duración: 90 minutos

Idea central: La seguridad de Bitcoin depende de ideas técnicas simples pero poderosas como claves, firmas, hashing y UTXOs, que permiten la propiedad y la verificación sin una autoridad central.

#### Objetivos de aprendizaje

Al final de esta lección, los estudiantes deberían ser capaces de:

* Explicar cómo las claves públicas y privadas ayudan a asegurar la propiedad y las transacciones de Bitcoin.
* Describir qué es una firma digital y cómo demuestra que una transacción fue autorizada por el propietario legítimo.
* Explicar, en términos sencillos, qué significan criptografía, cifrado y descifrado en el contexto de Bitcoin.
* Definir hashing y describir por qué las funciones hash son importantes para la seguridad y la integridad de los datos en Bitcoin.
* Identificar propiedades básicas de una función hash, como la salida de longitud fija, el comportamiento unidireccional y la sensibilidad a pequeños cambios en la entrada.
* Explicar el modelo UTXO y cómo se gasta, recibe y devuelve el bitcoin como cambio a través de las salidas de transacción.
* Describir cómo los nodos ayudan a prevenir el doble gasto comprobando si una salida ya ha sido gastada.

#### Herramientas y recursos

##### Materiales visuales

* Capítulo 8 - Cómo funciona Bitcoin

##### Biblioteca de apoyo

* Tarjeta de referencia de vocabulario — Capítulo 8 — Términos: criptografía, hash, UTXO, firma digital, clave privada/pública, árbol de Merkle, blockchain
* Bibliotecas de conceptos erróneos — Capítulo 8 — Aborda: "la frase semilla perdida se puede recuperar", "clave privada = contraseña", "blockchain es anónima"
* Explicaciones técnicas y análisis en profundidad — Funciones hash, claves públicas/privadas, modelo UTXO, seguridad de Prueba de Trabajo

#### Actividades

* Transacciones en acción
* Explorando el Mempool

#### Enseñanza en línea

* Utiliza una pizarra digital y dibuja cada concepto en vivo en lugar de depender solo de la explicación verbal.
* Enseña una idea técnica a la vez y haz pausas frecuentes para comprobar la comprensión con preguntas.
* Utiliza materiales visuales para claves, firmas, hashes y UTXOs para que los estudiantes puedan seguir la estructura.
* Mantén el objetivo conceptual y evita profundizar demasiado en matemáticas o jerga técnica.

#### Preparación

* Prepara y plastifica diagramas: pares de claves públicas/privadas, firmas digitales, modelo UTXO, hashing (función unidireccional).
* Marca como favoritos un explorador de blockchain y una calculadora de hash SHA-256; selecciona 2-3 transacciones reales de Bitcoin para analizar paso a paso.
* Prepara notas en la pizarra para explicar entradas, salidas y cómo las transacciones se confirman en la blockchain.

#### Procedimiento

Esta lección ofrece a los estudiantes una primera mirada al lado técnico de Bitcoin sin asumir conocimientos técnicos previos. La guía ahora sigue la misma estructura comprimida que el Diploma, agrupando la criptografía bajo un encabezado y los UTXOs bajo otro.

##### 8.0 Introducción, 8 minutos

Comienza estableciendo expectativas:

* ¿Qué hace que Bitcoin sea seguro si no hay un banco central que lo controle?
* ¿Cómo puede la red saber si una persona realmente posee el bitcoin que intenta enviar?
* ¿Qué sucede realmente detrás de escena cuando alguien realiza una transacción de Bitcoin?

Aclara que este capítulo se centra en las bases técnicas básicas de Bitcoin, especialmente claves, firmas, hashing y UTXOs. También tranquiliza a los estudiantes diciéndoles que no necesitan convertirse en ingenieros para entender la lógica esencial. El propio capítulo deja esto claro al comparar Bitcoin con Internet: muchas personas lo usan todos los días sin comprender completamente cada capa que lo compone.

##### 8.1 Seguridad a través de la criptografía, 57 minutos

**Bitcoin como un libro mayor almacenado en muchas computadoras**

Comienza con la sencilla presentación del capítulo sobre la red de Bitcoin:

* Bitcoin es un registro de transacciones
* ese registro se almacena en muchas computadoras llamadas nodos
* el libro mayor es público y seudónimo
* muestra direcciones e historial de transacciones, no detalles de identidad personal

Esta sección ayuda a los estudiantes a conectar con lo que ya saben de capítulos anteriores. Bitcoin no se basa en cuentas ocultas dentro de un banco. Se basa en un libro mayor compartido que muchos participantes pueden verificar. es especialmente útil aquí porque muestra a los usuarios, monederos y la red de Bitcoin conectados al libro mayor público.

**Claves públicas y privadas**

Ahora pasa a la criptografía.

Explica que cada usuario de Bitcoin tiene:

* una clave privada, que debe permanecer secreta
* una clave pública, que se puede compartir

Aclara su propósito en términos sencillos:

* la clave privada demuestra el control y autoriza el gasto
* la clave pública ayuda a otros a verificar que la transacción fue autorizada correctamente

Un punto clave de enseñanza del capítulo es que Bitcoin utiliza criptografía de clave pública/privada, no el modelo antiguo donde dos personas primero debían compartir la misma clave secreta. Eso es importante porque permite una verificación segura sin obligar a los usuarios a revelar el secreto que protege sus fondos.

Puedes explicarlo así:

* la clave privada es como la prueba secreta de que el bitcoin te pertenece
* la clave pública es parte de lo que permite a la red verificar tu autorización
* quien controla la clave privada controla la capacidad de gastar el bitcoin

Ten cuidado aquí de no complicar demasiado el lenguaje de cifrado. El punto más importante para los estudiantes es la propiedad y la autorización.

**Firmas digitales y autorización de transacciones**

Ahora explica qué sucede cuando alguien envía bitcoin.

Utiliza la secuencia del capítulo:

* un usuario crea una transacción
* el remitente genera una firma digital usando su clave privada
* la transacción se transmite a la red
* los nodos verifican que la firma sea válida
* una vez verificada y confirmada, la propiedad se transfiere en el libro mayor

Deja claro que una firma digital no es lo mismo que escribir un nombre. Es una prueba criptográfica de que el verdadero propietario autorizó la transacción. Este es uno de los mecanismos centrales que permite que Bitcoin funcione sin una autoridad central que apruebe las transacciones manualmente. El diagrama es útil porque muestra visualmente la firma y la verificación, así como el camino de la transacción desde el remitente hasta la validación en la red.

Una buena frase para la clase es:

Las transacciones de Bitcoin no se aprueban porque lo diga un banco. Se aceptan porque la red puede verificar una prueba criptográfica válida.

**Hashing y funciones unidireccionales**

A continuación, explica el hashing.

Empieza simple:

* una función toma una entrada y produce una salida
* una función unidireccional es fácil de ejecutar en una dirección, pero prácticamente imposible de revertir
* una función hash toma datos de cualquier tamaño y los convierte en una salida de longitud fija llamada hash

Utiliza una de las analogías del capítulo, la que te parezca más clara para tu audiencia:

* la analogía del batido para funciones unidireccionales
* la analogía de la huella digital para los hashes
* la analogía de la partitura musical para comprobar si algo cambió

La analogía de la huella digital probablemente sea la más clara para la mayoría de las clases:

* un hash es como una huella digital digital para los datos
* si la entrada cambia aunque sea un poco, el hash cambia completamente
* esto ayuda a las computadoras a comprobar la integridad y detectar manipulaciones

Luego explica por qué el hashing es importante en Bitcoin:

* las transacciones se hashean
* la red utiliza hashes para ayudar a verificar la integridad
* si una transacción se modifica, el hash cambia
* esto ayuda a proteger el libro mayor de manipulaciones no detectadas

Las imágenes de las páginas 7 a 10 son muy útiles aquí. El capítulo muestra tanto la idea de la salida de longitud fija como el principio de "un pequeño cambio, un resultado completamente diferente", que es uno de los conceptos más importantes para que los estudiantes comprendan.

**Propiedades básicas de las funciones hash**

Recorre brevemente las propiedades destacadas en el capítulo, sin hacerlas sentir demasiado académicas:

* Determinista: la misma entrada da la misma salida cada vez
* Unidireccional / resistencia a preimagen: no puedes revertir el proceso de manera realista
* Sensible al cambio: incluso un pequeño cambio en la entrada crea una salida muy diferente
* Resistencia a colisiones: es extremadamente difícil encontrar dos entradas diferentes con la misma salida
* Rápido de verificar: la función es eficiente de ejecutar y comprobar

No necesitas que los estudiantes memoricen cada término, pero sí que comprendan el punto general: el hashing le da a Bitcoin una forma confiable de identificar datos y detectar cambios.

##### 8.2 El modelo UTXO, 25 minutos

**El Modelo UTXO**

Ahora pasamos a la segunda parte principal del capítulo: los UTXOs, o Salidas de Transacción No Gastadas.

Explícalo en términos sencillos usando la analogía del efectivo del capítulo:

* bitcoin no se rastrea solo como el saldo de una cuenta bancaria
* en cambio, está compuesto por piezas gastables llamadas UTXOs
* cuando gastas bitcoin, usas uno o más UTXOs existentes como entradas
* luego se crean nuevos UTXOs como salidas

Usa el ejemplo del capítulo:

* si tienes un UTXO de 10 BTC
* y envías 6 BTC
* un nuevo UTXO de 6 BTC va al destinatario
* un nuevo UTXO de cambio regresa a ti
* una pequeña parte se paga como comisión al minero

Eso ayuda a los estudiantes a ver que Bitcoin funciona más como gastar efectivo y recibir cambio que como restar números de una simple línea de cuenta. Los diagramas son especialmente útiles aquí porque muestran visualmente cómo un UTXO se divide en salida al destinatario, salida de cambio y comisión.

Haz explícitos dos puntos clave:

* el saldo de tu monedero es la suma de tus UTXOs
* cuando gastas, los UTXOs antiguos se consumen y se crean nuevos

**Prevención del Doble Gasto**

Cierra el contenido explicando una de las implicaciones más importantes del modelo UTXO.

Si alguien intenta gastar la misma salida dos veces, los nodos rechazan el segundo intento porque mantienen el libro mayor y pueden verificar si ese UTXO ya ha sido gastado. Así es como Bitcoin previene el doble gasto sin necesidad de una empresa central de pagos que gestione los registros. El ejemplo es muy útil aquí porque muestra cómo Alice combina UTXOs, envía fondos a Bob, recibe cambio y la transacción confirmada actualiza el libro mayor en todos los nodos.

Una forma clara de decirlo en clase es:

Bitcoin previene el doble gasto porque la red lleva un registro de qué salidas permanecen no gastadas y cuáles ya han sido usadas.

###### Cierre y Comprobación de Comprensión

Cierra con algunas preguntas rápidas:

* ¿Cuál es la diferencia entre una clave pública y una clave privada?
* ¿Qué prueba una firma digital?
* ¿Por qué es útil el hashing en Bitcoin?
* ¿Qué ocurre si una transacción se cambia después de ser hasheada?
* ¿Qué es un UTXO en términos sencillos?
* ¿Cómo evita la red que alguien gaste el mismo bitcoin dos veces?

#### Notas para Educadores

Este capítulo contiene un lenguaje más técnico que los anteriores, así que prioriza la claridad, la analogía y la repetición.

El objetivo no es convertir a los estudiantes en desarrolladores. El objetivo es ayudarles a entender por qué funciona la seguridad de Bitcoin.

Los puntos más importantes a priorizar, si el tiempo es limitado, son:

* clave privada vs clave pública
* firmas digitales
* qué hace el hashing
* UTXOs como piezas gastables de bitcoin
* cómo se previene el doble gasto

Los recursos visuales más útiles en este capítulo son:

* el diagrama usuario-monedero-red
* el visual de la firma digital
* los ejemplos de hashing y los diagramas de salida de longitud fija en las páginas 7 a 10
* los diagramas de UTXO en las páginas 10 a 12

##### Cómo se ve un buen resultado

* Es importante tratar la criptografía como una base y no como un misterio, usar muchos recursos visuales, evitar matemáticas profundas, conectar con capítulos anteriores y comprobar la comprensión con aplicaciones como "Si alguien cambia una transacción, ¿qué falla?"
* Los educadores deben ser pacientes con los estudiantes que tengan dificultades, pensar visualmente y dibujar todo, ser honestos sobre lo que los estudiantes no necesitan entender, estar dispuestos a decir "No lo sé, pero así es como lo averiguaríamos" y mantenerse alentadores en todo momento.
* Los estudiantes entienden por qué Bitcoin no puede ser hackeado porque está protegido por las matemáticas, respetan el diseño elegante del sistema, se sienten cómodos con la complejidad sabiendo que no necesitan cada detalle, ganan confianza para hacer preguntas sin ser juzgados y reconocen que han avanzado en la comprensión de algo que la mayoría de la gente no entiende.
* Los Resultados de Aprendizaje se cumplen si los estudiantes pueden explicar los conceptos básicos de criptografía como funciones unidireccionales y firmas digitales sin matemáticas profundas, entender el modelo UTXO mostrando que posees monedas y no cuentas, reconocer el hashing como la base de la seguridad de Bitcoin, comprender la anatomía de una transacción incluyendo firmas y confirmaciones, explicar por qué Bitcoin es inmutable y hacer preguntas críticas sobre posibles ataques o vulnerabilidades.

##### Gestión del Tiempo

Si el tiempo es limitado, prioriza:

* Clave privada vs clave pública
* Firmas digitales
* Qué hace el hash
* UTXOs como piezas gastables de bitcoin
* Cómo se previene el doble gasto

Si vas adelantado, dedica tiempo a:

* Diagrama usuario-billetera-red y modelo visual de seguridad
* Visualización de la firma digital: proceso criptográfico detallado
* Árboles de Merkle y seguridad de la cadena
* Vectores de ataque avanzados y por qué fallan

##### Si los estudiantes tienen dificultades

* La criptografía como algo amenazante → "La usas a diario; Bitcoin la usa de la misma manera."
* El hash como concepto → Analogía de la huella digital; única, no se puede cambiar sin que cambie el hash.
* Firmas digitales → "Demuestra autorización sin revelar la contraseña."
