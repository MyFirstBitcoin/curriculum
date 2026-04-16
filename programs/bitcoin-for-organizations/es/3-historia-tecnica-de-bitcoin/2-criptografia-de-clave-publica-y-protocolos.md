# 3.2 Criptografía de clave pública y protocolos

Internet hoy en día, y la mayoría de los sistemas informáticos modernos, dependen de la criptografía, un método para ocultar información de modo que solo el destinatario pueda descifrarla. Los fundamentos de la criptografía utilizada para asegurar Bitcoin se remontan a los años 70.

El primer problema a resolver es: ¿cómo enviar un secreto compartido a través de un medio no seguro?

Esto fue estudiado por primera vez por Whitfield Diffie y Martin Hellman.

El problema: las dos partes —normalmente llamadas Alicia y Bob— quieren compartir información secreta a través de una red donde otros pueden estar escuchando. Para lograr esto, crearon el proceso de intercambio de claves Diffie-Hellman.

Este secreto compartido puede usarse como valor semilla para crear numerosas claves simétricas para cifrar y descifrar mensajes entre sí sin compartir la clave abiertamente.

Como la clave privada nunca tiene que compartirse, y se usan diferentes claves en cada extremo para cifrar y descifrar, esto se conoce como un algoritmo de cifrado asimétrico.

Casos de uso:

* Alicia firma un mensaje con la clave pública de Bob — quien es la única persona que puede descifrarlo usando su clave privada
* Alicia firma un mensaje con su clave privada — al descifrarlo con su clave pública, cualquiera puede verificar que el mensaje fue enviado por Alicia, sin conocer su clave privada
* Combinando estos dos enfoques con dos capas de cifrado, se puede enviar un mensaje cifrado de modo que solo Bob pueda descifrarlo, y él puede entonces verificar que la remitente fue realmente Alicia

Aunque no fue acreditado en el artículo, Ralph Merkle fue fundamental para ayudar a resolver lo que hasta entonces se consideraba un enigma irresoluble: cómo establecer o restablecer comunicación privada a través de una red abierta y potencialmente hostil.

Este enfoque por sí solo es susceptible a un ataque de fuerza bruta, donde un atacante puede tomar los números compartidos y eventualmente recrear una clave compartida si dispone de suficiente tiempo y recursos, por lo que no es la solución completa por sí misma.

##### Protocolos para Criptosistemas de Clave Pública

Además de contribuir al sistema de clave pública Diffie-Hellman descrito arriba, **Ralph Merkle** continuó contribuyendo en este campo durante muchos años, y fue fundamental en el desarrollo de algunos componentes clave utilizados por Bitcoin.

Una función hash criptográfica es un algoritmo matemático que toma entradas de cualquier tamaño y realiza cálculos complejos para devolver un valor hash en bits, que normalmente se representa como una salida alfanumérica de longitud fija usando formato hexadecimal.

* Las entradas pueden ser de cualquier tamaño
* La salida siempre es de longitud fija y determinista (la misma entrada genera el mismo hash cada vez)
* Es fácil de verificar pero extremadamente difícil revertir el proceso para determinar la entrada
* Una pequeña modificación de los datos altera completamente las salidas

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/1f232fdbe6e4714ed8b683ab9dc630e0b1d705ce-515x331.svg)

El hashing es una parte integral del protocolo de Bitcoin. SHA-256, utilizado en Bitcoin, fue creado por la NSA y es un ejemplo de un algoritmo de hash criptográfico.

* Cada bloque en la cadena se hashea para que los datos no puedan ser modificados — asegurando la integridad del libro mayor distribuido
* El hash generado debe cumplir con los criterios de 'Prueba de trabajo' para ser considerado un bloque válido
* Árboles de Merkle — al emplear ramificaciones y hashes de hashes, los árboles hash permiten la verificación de grandes conjuntos de datos con almacenamiento mínimo
* Firmas y claves basadas en hash pueden usarse para monederos, direcciones y autorización de transacciones

La verificación distribuida de los estados de la blockchain y los modelos de libro mayor solo-adición resistentes a la revisión son posibles gracias al hash unidireccional. Las funciones hash proporcionan el método confiable y determinista para verificar eventos en libros mayores públicos como Bitcoin en ausencia de un modelo de confianza centralizado.

Se esperaba que estas nuevas capacidades en el campo de la criptografía dieran paso, según sus creadores, a una nueva ola de innovación en este ámbito.

##### Criptografía de curva elíptica

Una de estas innovaciones posteriores llegó en forma de la criptografía de curva elíptica.

La criptografía de curva elíptica fue introducida en 1985 por dos científicos, N. Koblitz y V. Miller. Propusieron la idea de usar puntos definidos por curvas elípticas en lugar de los campos primos finitos, de modo que se mantenga la suposición del problema del logaritmo discreto, como se usa comúnmente en el protocolo estándar de intercambio de claves Diffie-Hellman. Los detalles de cómo funciona esto están fuera del alcance de esta sección, pero a grandes rasgos, una curva elíptica es el conjunto de puntos que satisfacen una ecuación matemática específica.

La ecuación para una curva elíptica se ve algo así:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Esto tiene algunas propiedades útiles:

* Simetría horizontal. Cualquier punto en la curva puede reflejarse sobre el eje x y sigue perteneciendo a la misma curva.
* cualquier línea no vertical intersectará la curva en como máximo tres puntos.
* Los tamaños de clave compactos son esenciales para el almacenamiento y transmisión eficiente de claves públicas en la blockchain.

Estas propiedades pueden usarse para crear pares de claves de manera similar al algoritmo Diffie-Hellman. Bitcoin utiliza ECDSA, que significa Algoritmo de Firma Digital de Curva Elíptica. Es un proceso que utiliza una curva elíptica y un campo finito para “firmar” datos de tal manera que terceros puedan verificar la autenticidad de la firma mientras que el firmante conserva la capacidad exclusiva de crear la firma. En bitcoin, los datos que se firman son la transacción que transfiere la propiedad.

La parte 'finita' es similar al enfoque 'mod' con Diffie-Hellman, donde la salida de la ecuación se divide y el residuo se usa para asegurar que encaje dentro de un rango de números.
