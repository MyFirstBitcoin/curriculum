# 3.7 Bitcoin

Después de muchos años y varios intentos fallidos, los Cypherpunks en su mayoría habían comenzado a perder interés en la idea de una moneda digital sin permisos, cuando Adam Back recibió un correo electrónico con un enlace a un borrador de un libro blanco titulado 'dinero electrónico sin un tercero', enviado por una persona anónima que se hacía llamar Satoshi Nakamoto.

Para recapitular hasta este punto, tenemos al menos las ideas de:

* Firmas criptográficas que podrían proporcionar un nivel de privacidad y anonimato
* Concepto de una moneda sin respaldo (B-Money)
* Propuestas (pero sin medios) para limitar la emisión de nueva moneda
* Monedas digitales cuya propiedad se atribuía mediante claves públicas (B-Money) y podían transferirse firmando y reasignarse según la dirección del destinatario (RPOW y Hashcash)
* Todos los nodos mantienen una copia de un libro mayor totalmente distribuido (B-Money) (descartado en ese momento por considerarse poco práctico)
* Protocolo de sellado de tiempo: utilizando el hash de árbol de Merkle para proporcionar una cronología de eventos matemáticamente comprobable que es difícil de falsificar si todos los usuarios mantienen los mismos registros
* Prueba de trabajo para vincular el esfuerzo del mundo real al sistema (pero usando el hash en sí como la moneda)
* Redes totalmente descentralizadas donde todos los pares son iguales y pueden entrar y salir de la red (BitTorrent)
* Concepto de vincular nuevos hashes a hashes anteriores (Bit Gold y sellado de tiempo)

Lo que faltaba en ese momento incluía:

* Una solución viable para resolver el problema de los 'generales bizantinos'
* Un método para limitar la cantidad de dinero en circulación a pesar de las mejoras continuas en el hardware
* Un esquema de incentivos para que las personas participen (problema del huevo y la gallina)

La otra gran diferencia entre los intentos recientes y Bitcoin fue que Satoshi había estado trabajando en el código durante algún tiempo, en el verdadero espíritu original de 'los Cypherpunks escriben código', antes de anunciarlo en las listas de correo, a diferencia de Bit Gold y B-Money, que eran más conceptuales.

¿Cuál fue la innovación que diferenció a Bitcoin de los intentos anteriores de dinero electrónico?

La prueba de trabajo se utilizaría como un mecanismo de consenso y una forma de proporcionar seguridad e inmutabilidad: en lugar de usar el hash como una forma de dinero, se utilizaría en un nuevo proceso conceptual llamado minería, donde un nodo agruparía un conjunto de transacciones, añadiría un número aleatorio y luego aplicaría el hash al 'bloque' de datos. Un bloque válido que cumpliera con el requisito del hash sería entonces anunciado a la red. Estos bloques se vincularían entre sí utilizando el hash del bloque anterior en cada uno, y la cadena de bloques más larga se utilizaría en caso de un desempate donde diferentes nodos validaran y anunciaran diferentes bloques al mismo tiempo, creando divisiones en la cadena. La prueba de trabajo se convirtió en el desempate distribuido para resolver el problema de los generales bizantinos.

Estos mineros también recibieron un incentivo para proporcionar la CPU necesaria para realizar la prueba de trabajo, al recibir nuevos bitcoin por cada bloque. La cantidad de Bitcoin que se les otorga también está programada para disminuir aproximadamente cada 4 años hasta que se hayan creado todos los Bitcoin, estableciendo un límite máximo a la cantidad total de Bitcoin que existirá en circulación, de 21 millones.

La idea más original fue la forma en que resolvió el problema de cuánto dinero se crea a medida que mejora el hardware y se puede aplicar más potencia a la red. Las marcas de tiempo de un número determinado de bloques (2016) se promediarían, y si se están creando demasiado rápido, el hash necesario para crear un nuevo bloque se haría más difícil; si es demasiado lento, se haría más fácil. Esto se incorporó al protocolo descentralizado que ejecutan todos los nodos, por lo que cualquier minero que lo ignore gastaría energía para minar un bloque sin beneficio, ya que sería rechazado por el resto de la red. Este ajuste garantiza que la creación de nuevos bloques se mantenga en el calendario previsto de emisión y proporciona incentivos para que los mineros 'jueguen según las reglas'.

####   
Resumen

Muchas de las piezas del rompecabezas necesarias para construir un sistema de dinero electrónico descentralizado entre pares basado en principios de dinero sólido ya estaban en su lugar antes de que Satoshi publicara su libro blanco y poco después del lanzamiento inicial del código.

> La naturaleza de Bitcoin es tal que, una vez que se lanzó la versión 0.1, el diseño central quedó grabado en piedra para el resto de su existencia  
_Satoshi Nakamoto_

Aunque se han propuesto y adoptado muchas ideas de mejora (BIPs), Bitcoin ha estado funcionando en segundo plano desde 2009 siguiendo el protocolo diseñado en la versión inicial y con apenas ninguna interrupción. Todas las mejoras se han realizado manteniendo la compatibilidad hacia atrás con todas las versiones anteriores.



##### Notas

1. Para una explicación del problema de los Generales Bizantinos, véase [https://es.wikipedia.org/wiki/Fallo_bizantino](https://en.wikipedia.org/wiki/Byzantine_fault)
