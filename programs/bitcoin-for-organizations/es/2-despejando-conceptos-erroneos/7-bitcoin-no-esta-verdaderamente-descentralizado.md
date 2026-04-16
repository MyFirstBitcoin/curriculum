# 2.7 Bitcoin no está verdaderamente descentralizado.

> La complejidad de las criptomonedas surge de los intentos de descentralización: al distribuir el poder y la gobernanza en el sistema, teóricamente no hay necesidad de intermediarios de confianza como las instituciones financieras. Esa fue la premisa del documento fundacional de Bitcoin, que ofrecía una solución criptográfica destinada a permitir que los pagos se enviaran sin involucrar a ninguna institución financiera u otro intermediario de confianza. Sin embargo, Bitcoin se centralizó muy rápidamente y ahora depende de un pequeño grupo de desarrolladores de software y pools de minería para funcionar  
_Fondo Monetario Internacional_

Como muestra la cita anterior de una publicación bastante reciente del Fondo Monetario Internacional, la industria financiera tradicional sigue afirmando que Bitcoin no está descentralizado, además de confundir Bitcoin con otros criptoactivos.

##### Introducción

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/21bcaa106319f91359b6b6df74bfecf824f73f5e-161x167.svg)

La descentralización es un aspecto fundamental de Bitcoin. La capacidad de mantener las reglas del protocolo, como la escasez y la distribución, sin una autoridad central, garantiza que pueda funcionar como dinero sin permisos para una sociedad global.

Como señaló Satoshi en su correspondencia en línea, servicios descentralizados como BitTorrent estaban 'manteniéndose por sí mismos' frente a las restricciones gubernamentales, en comparación con servicios con propietarios identificados y servidores centralizados. Claramente le preocupaba el riesgo potencial de que los gobiernos u otros intereses cerraran o afectaran negativamente a Bitcoin.

En este contexto, nos interesa la descentralización de:

* El desarrollo y la gestión del código que ejecuta el protocolo; ¿quién puede cambiar las reglas?
* La función de minería que crea nuevos bloques de acuerdo con las reglas y valida contra el doble gasto
* Los nodos que validan las transacciones para comprobar su validez y mantienen una copia de la blockchain

##### Desarrolladores

Bitcoin es un protocolo de código abierto que cualquiera puede consultar, descargar, copiar o sugerir cambios. Está disponible en una biblioteca de GitHub, y el código fuente fue lanzado originalmente en 2009 por Satoshi Nakamoto. Cualquiera es libre de descargar el código y ejecutar un nodo, la mayoría de los cuales ejecutan el software original de Bitcoin Core, que se ha actualizado con el tiempo.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Fuente: https://river.com/learn/what-is-bitcoin-core/_

El desarrollo de Bitcoin Core sigue las mejores prácticas del desarrollo de código abierto. En cualquier momento, puede haber cualquier número de desarrolladores escribiendo o revisando cambios en el código. Deben escuchar las preocupaciones de los operadores de nodos y mineros, así como de la base de usuarios antes de realizar cualquier cambio crítico en el código, el cual será revisado y acordado como se muestra en el diagrama de flujo anterior antes de incorporarse al código.

Las reglas de Bitcoin están entonces codificadas en este software Bitcoin Core, que se ejecuta en cada nodo. Cualquiera puede sugerir un cambio en las reglas: las reglas son código, pero no son_solo_código, son_acordadas_reglas codificadas. Si se cambian unilateralmente, el nuevo código ya no forma parte del consenso y deja de ser parte de Bitcoin. Cambiar algo en Bitcoin y seguir en consenso es complicado. Los cambios sugeridos al código caen en una de tres categorías:

* Dentro de las reglas existentes: Mejoras menores como errores ortográficos, una interfaz de usuario más agradable o gestión de datos pueden entrar en esta categoría y son relativamente triviales de aprobar.
* Agregar una nueva regla que añada restricciones a las reglas, como reducir el tamaño del bloque. Esto se conoce como una 'bifurcación suave' (soft fork). Los nodos que decidan no implementar el cambio de código y permanezcan en la versión anterior aún podrán participar en la red.
* Agregar una nueva regla que rompa las reglas actuales, por ejemplo, un aumento en el tamaño del bloque. Los nodos que no actualicen al nuevo código descartarán un bloque creado con el tamaño mayor como inválido. Esto se conoce como una 'bifurcación dura' (hard fork) y creará una división de la cadena entre los nodos que ejecutan el código original y el nuevo, y crea una nueva moneda. Esto ha sucedido anteriormente, pero no ha llevado a ningún éxito a largo plazo para la nueva moneda, ya que la mayoría de los nodos decidieron mantener el código original.

Por lo tanto, una sola parte o grupo de personas no puede cambiar unilateralmente el código de Bitcoin sin lograr un acuerdo de consenso, o corren el riesgo de una división de la cadena y la creación de una nueva moneda siguiendo un conjunto diferente de reglas.

##### Minería

La función de minería valida las transacciones igual que cualquier otro nodo en la red, pero luego gasta la energía necesaria para crear un nuevo bloque que cumpla con las reglas de consenso en el código. El éxito permite al minero obtener las recompensas en forma de comisiones de transacción y recompensas de Bitcoin (al momento de escribir esto, 3.125 monedas por bloque).

La minería normalmente se realiza en 'pools' de minería donde las personas consolidan el poder de minado o tasa de hash para aumentar las posibilidades de minar un bloque con éxito y compartir las recompensas. Existe el peligro de que uno o más de estos pools de minería puedan combinarse para lograr un dominio del 51% en la minería y, esencialmente, invalidar el protocolo de validación de la red a su favor para gastar monedas dos veces. Esto requeriría una enorme cantidad de recursos a un gran costo, y los mineros individuales pueden cambiar fácilmente a otro pool de minería en cualquier momento. Tal ataque probablemente también colapsaría el valor de bitcoin, ya que sería obvio que la integridad de la red ha sido comprometida. Por lo tanto, un atacante tendría que convertir rápidamente cualquier bitcoin obtenido a dinero fiduciario antes de que el valor se erosione. Esto haría aún más difícil sostener un ataque durante mucho tiempo, y por lo tanto hace más rentable para un minero o un operador de pool adherirse a las reglas e intentar minar bloques válidos.

La distribución geográfica de la función de minería también es importante para evitar que, por ejemplo, los gobiernos tomen el control de la capacidad de minería o la cierren. Por ejemplo, una prohibición reciente de la minería por parte de China demostró la capacidad de Bitcoin para adaptarse y sobrevivir a tal intervención gubernamental, adaptándose y recuperándose rápidamente de la pérdida resultante de poder de hash.

##### Nodos

A diferencia de la minería, que requiere una inversión financiera significativa para competir eficazmente en la carrera por minar nuevos bloques, o el desarrollo de código que requiere experiencia en programación, ejecutar un nodo es algo que cualquiera interesado en ayudar a mantener la descentralización de Bitcoin puede hacer.

Los nodos ejecutan el software Bitcoin Core y hacen cumplir las reglas que incluye el código para asegurar que los mineros no hagan trampa, por ejemplo, asignándose a sí mismos una recompensa de bloque mayor a la permitida. También hacen cumplir el límite de suministro de 21 millones, que es fundamental para mantener la escasez de Bitcoin. Para que un gobierno o actor malicioso detenga Bitcoin, tendría que destruir cada copia de la blockchain, que actualmente se ejecuta en miles de nodos distribuidos globalmente, una tarea casi imposible.

##### Personas

Otro aspecto de la posible centralización son las personas. Cada otra 'altcoin' tiene una figura visible: alguien que podría ser potencialmente coaccionado para abogar por cambios que no estén en el mejor interés de Bitcoin. Satoshi Nakamoto permaneció el tiempo suficiente para asegurar que Bitcoin estuviera en el camino del éxito antes de desaparecer para siempre, dejándolo en manos de otros para mejorar y adaptar el software.

¿Qué pasa con los poseedores de grandes cantidades de Bitcoin? Los primeros inversores, que han mantenido sus monedas y no las han perdido, serán extremadamente ricos en este momento. Es importante señalar que esto puede ser cierto, pero eso no les da más influencia en el sistema que a cualquier otra persona, a diferencia de las monedas de 'prueba de participación' donde los primeros adoptantes, que ya son ricos en esa moneda, obtienen ventajas en la toma de decisiones y en la distribución de futuras monedas. Esto ha llevado o inevitablemente llevará a la centralización con el tiempo.

##### Conclusión

¿Cuáles son las amenazas potenciales que la descentralización puede intentar mitigar?

* El gobierno cerrando o prohibiendo Bitcoin
* Cambios no deseados en el código que favorecen a un conjunto de intereses en Bitcoin, por ejemplo, aumentar la recompensa de bloque
* Coerción del protocolo por parte del gobierno o actores maliciosos para influir en la dirección del protocolo
* Capacidad de un pool de mineros para tomar el control de la red y 'gastar dos veces' Bitcoin – un ataque del 51%

Como podemos ver, la combinación de nodos, desarrolladores de código y mineros, así como el uso del mecanismo de 'prueba de trabajo', descentraliza Bitcoin a un nivel suficiente donde estas amenazas potenciales no se consideran de gran preocupación. La comunidad deberá seguir monitoreando la situación para asegurar que esto siga siendo así.
