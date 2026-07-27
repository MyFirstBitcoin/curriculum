# 9.1 Nodos y mineros de Bitcoin

¿Qué es un nodo de Bitcoin?  
Los nodos de Bitcoin pueden sonar técnicos, pero simplemente son software que mantiene una copia de la blockchain de Bitcoin en una computadora. La blockchain es un registro compartido de todas las transacciones de Bitcoin.

Cuando ejecutas tu propio nodo, verificas las transacciones de Bitcoin por tu cuenta en lugar de confiar en otra persona. Esto te da más independencia y ayuda a mantener descentralizada la red de Bitcoin.

Puedes imaginar un nodo de Bitcoin como un agente de tránsito digital con algunas tareas importantes.

1. Mantiene una copia de la blockchain, que es el historial de todas las transacciones de Bitcoin.
1. Los nodos se conectan con otros nodos alrededor del mundo y comparten información. Un ejemplo es la lista de nuevas transacciones que esperan ser confirmadas, llamada mempool.
1. Los nodos comprueban que cada transacción siga las reglas de Bitcoin. Si una transacción no es válida, el nodo la rechaza.

Los nodos también ayudan a los nuevos nodos a unirse a la red compartiendo la blockchain con ellos. Sin embargo, cada nuevo nodo sigue comprobando todas las reglas de forma independiente.

Cualquier persona puede ejecutar un nodo instalando software como Bitcoin Core y descargando la blockchain. Una vez configurado, el nodo sigue recibiendo nuevos bloques aproximadamente cada 10 minutos y los verifica antes de añadirlos a su copia de la blockchain.

Ejecutar un nodo ayuda a hacer que la red de Bitcoin sea más segura y descentralizada, porque más personas verifican el sistema de forma independiente.

#### ¿Qué es un minero de Bitcoin?

> El propósito de la minería no es la creación de nuevos bitcoins; ese es el sistema de incentivos. La minería es el mecanismo mediante el cual se descentraliza la seguridad de Bitcoin.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Los mineros recopilan transacciones no confirmadas, forman un bloque y usan energía para encontrar una clave que añade y asegura el bloque.


Los mineros compiten para añadir el siguiente bloque de transacciones a la blockchain. Para hacerlo, deben encontrar un número especial que cree un hash de bloque válido. Puedes imaginarlo como buscar la llave correcta entre miles de millones de posibilidades. El primer minero que encuentra el hash correcto gana la carrera y obtiene el derecho de añadir su bloque a la blockchain.

Cuando un minero encuentra un hash válido, comparte su bloque con la red. Otros mineros verifican rápidamente que la solución sea correcta. Si lo es, el bloque se añade a la blockchain, ayudando a mantener seguro el libro contable público de Bitcoin.

Los mineros ganan bitcoins de dos maneras:

* **Recompensas de bloque:** Se crean nuevos bitcoins y se entregan al minero que añade con éxito un bloque a la blockchain.
* **Comisiones por transacción:** Cuando las personas envían bitcoin, incluyen una pequeña comisión. El minero que añade el bloque recibe las comisiones de las transacciones incluidas en ese bloque.

#### Halvings de Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12.5 BTC | 6.25 BTC | 3.125 BTC |



> **Callout**
>
> Las recompensas de los mineros por completar un bloque se reducen a la mitad cada 210,000 bloques, aproximadamente cada cuatro años.


Bitcoin tiene un suministro máximo fijo de 21,000,000 bitcoins, pero no todos fueron creados cuando Bitcoin comenzó. En cambio, nuevos bitcoins se introducen gradualmente en circulación mediante la **minería**.

Cuando los mineros añaden con éxito un nuevo bloque de transacciones a la red de Bitcoin, reciben una **recompensa de bloque** en bitcoins. En los primeros días de Bitcoin, esta recompensa era de 50 bitcoins por bloque. Esta recompensa animó a las personas a usar potencia de cómputo y electricidad para ayudar a asegurar la red.

Cada 210,000 bloques (aproximadamente cada 4 años), la recompensa de bloque se reduce a la mitad. Este evento se llama **halving**. El halving ralentiza la creación de nuevos bitcoins y ayuda a garantizar que el suministro total nunca supere los 21 millones. Con el tiempo, esto hace que bitcoin sea cada vez más escaso.


> **Definition – Oferta circulante**
>
> **La oferta circulante** se refiere a la cantidad total disponible de una moneda. Con Bitcoin, la oferta circulante total es la cantidad de monedas que se han minado y están en circulación en cualquier momento dado.



<!-- micrographic: bitcoin-supply-schedule -->



> **Definition – Calendario de emisión de Bitcoin**
>
> El **calendario de emisión de Bitcoin** es el plan predeterminado y público para la liberación de nuevos bitcoins en circulación, diseñado para mantener la escasez de Bitcoin a lo largo del tiempo.


Después de cada evento de halving, la recompensa en bitcoins que reciben los mineros por añadir un bloque se reduce a la mitad. Esto reduce el ritmo al que se crean nuevos bitcoins.

Los mineros aún ganan comisiones por transacción de las transacciones incluidas en el bloque que minan. Con el tiempo, se espera que estas comisiones se conviertan en una parte mayor de los ingresos de los mineros.

Los halvings están integrados en el protocolo de Bitcoin y ocurren automáticamente aproximadamente cada cuatro años. Por eso, el calendario de emisión de Bitcoin es predecible y transparente.

La tabla muestra los próximos halvings, incluyendo la fecha aproximada, el número de bloque en el que ocurren, la nueva recompensa por bloque y el porcentaje del suministro total de bitcoin que habrá sido minado.


| Evento | Fecha | Bloque | Recompensa | Minado |
| --- | --- | --- | --- | --- |
| 5.º halving | 2028 | 1,050,000 | 1.5625 BTC | 98.44 % |
| 6.º halving | 2032 | 1,260,000 | 0.78125 BTC | 99.22 % |
| 7.º halving | 2036 | 1,470,000 | 0.390625 BTC | 99.61 % |


A medida que se minan más bitcoin, el suministro en circulación sigue aumentando hasta alcanzar el suministro máximo de 21,000,000 bitcoins, lo cual se espera alrededor del año 2140. Debido a que con el tiempo se crean menos bitcoins nuevos, si aumenta la demanda, el precio de Bitcoin puede subir. Esto también incentiva a los mineros a seguir asegurando la red aportando su poder de cómputo.

#### ¿Qué es un hash de bloque válido en Bitcoin?

Los mineros compiten por encontrar un código especial llamado **hash de bloque**. Este código identifica un bloque de transacciones y permite que se agregue a la blockchain.

Cada bloque contiene información sobre transacciones recientes y también incluye el hash del bloque anterior. Esto enlaza todos los bloques entre sí, formando una cadena desde el primer bloque (el Bloque Génesis) hasta el más reciente.

Un hash funciona como una **huella digital** para los datos del bloque. Si se cambiara cualquier información del bloque, la huella también cambiaría. Esto facilita que cualquiera verifique que el historial de transacciones de la blockchain no ha sido alterado y ayuda a mantener segura la red.


> **Callout**
>
> Satoshi Nakamoto, el creador de Bitcoin, minó el Bloque Génesis, que desbloqueó un total de 50 bitcoin.


#### La carrera para minar un bloque

Los mineros compiten por encontrar un hash de bloque válido. El primer minero en encontrar uno puede agregar el nuevo bloque a la blockchain y recibir una recompensa en bitcoin.

Para ser válido, el hash del bloque debe ser menor que un número establecido por la red llamado objetivo de dificultad. Como los hashes son aleatorios, los mineros deben seguir probando diferentes entradas hasta encontrar una que funcione.

Si compiten demasiados mineros, los bloques se encontrarían demasiado rápido. Si participan muy pocos mineros, los bloques tardarían demasiado en encontrarse. Para que el sistema funcione sin problemas, Bitcoin ajusta automáticamente la dificultad cada 2,016 bloques (aproximadamente cada dos semanas).

Este ajuste garantiza que, en promedio, se agregue un nuevo bloque a la blockchain aproximadamente cada 10 minutos.


> **Definition – Definición de nivel de dificultad**
>
> El **nivel de dificultad** en la minería de Bitcoin mide qué tan difícil es encontrar un hash de bloque válido. La red ajusta esta dificultad cada 2,016 bloques (aproximadamente cada dos semanas) para que se agreguen nuevos bloques a la blockchain aproximadamente cada 10 minutos. Cuanto mayor sea la dificultad, más difícil será para los mineros encontrar un bloque válido.


Al encontrar un hash de bloque válido, un minero demuestra que ha realizado el trabajo necesario para agregar un nuevo bloque a la blockchain. Este proceso se llama **Prueba de trabajo** (PoW). Es el mecanismo de seguridad que permite a Bitcoin confirmar transacciones y agregar nuevos bloques a la blockchain. El minero que encuentra primero el hash válido gana una recompensa en bitcoin, que incluye la recompensa por bloque y las comisiones de transacción de las transacciones incluidas en ese bloque.

La Prueba de trabajo (PoW) ayuda a mantener seguro Bitcoin al hacer que sea extremadamente costoso para cualquiera intentar hacer trampa o tomar el control de la red. En cambio, es mucho más rentable seguir las reglas.

Los mineros desempeñan cuatro funciones principales:

1. **Recopilar transacciones**: Los mineros eligen transacciones que han sido enviadas a la red y las colocan en un bloque candidato.
1. **Realizar la Prueba de trabajo**: Los mineros compiten para resolver un difícil acertijo matemático encontrando un hash de bloque válido.
1. **Difundir el bloque**: El primer minero que encuentra una solución válida comparte el nuevo bloque con la red.
1. **Obtener recompensas**: Si el bloque es válido, se añade a la cadena de bloques y el minero recibe bitcoin recién creado más las comisiones de transacción.

Muchos mineros de todo el mundo intentan crear el siguiente bloque al mismo tiempo. Cuando un minero encuentra una solución válida, la red verifica el bloque. Si todo es correcto, se añade a la cadena de bloques. Los otros bloques en competencia se descartan. Este proceso mantiene a la red en acuerdo y evita el doble gasto.

* Los mineros son computadoras que ayudan a mantener y actualizar el libro contable de Bitcoin.
* Recopilan transacciones y las agrupan en un bloque. Luego pasan los datos del bloque por un algoritmo de hash para crear un código único llamado hash.
* Los mineros repiten este proceso muchas veces, buscando un hash que cumpla con las reglas de Bitcoin. El primer minero que encuentra un hash válido recibe bitcoin recién creado como recompensa, y su bloque se añade a la cadena de bloques.
* El hash de cada bloque también lo conecta con el bloque anterior. Si alguien intentara cambiar una transacción pasada, los hashes ya no coincidirían y la red rechazaría la cadena alterada. Esto es lo que mantiene seguro el libro contable de Bitcoin.
