# 9.1 Una mirada más cercana a los nodos y mineros de Bitcoin

Los nodos de Bitcoin pueden sonar técnicos, pero simplemente son programas que mantienen una copia de la blockchain de Bitcoin en una computadora. La blockchain es un registro compartido de todas las transacciones de Bitcoin.

Cuando ejecutas tu propio nodo, verificas las transacciones de Bitcoin por ti mismo en lugar de confiar en otra persona. Esto te da más independencia y ayuda a mantener la red de Bitcoin descentralizada.

Puedes pensar en un nodo de Bitcoin como un agente de tránsito digital con algunas tareas importantes.

Primero, mantiene una copia de la blockchain, que es el historial de todas las transacciones de Bitcoin.

Segundo, los nodos se conectan con otros nodos alrededor del mundo y comparten información. Un ejemplo es la lista de nuevas transacciones esperando ser confirmadas, conocida como mempool.

Tercero, los nodos verifican que cada transacción cumpla con las reglas de Bitcoin. Si una transacción es inválida, el nodo la rechaza.

Los nodos también ayudan a que nuevos nodos se unan a la red compartiéndoles la blockchain. Sin embargo, cada nuevo nodo verifica todas las reglas de forma independiente.

Cualquiera puede ejecutar un nodo instalando un programa como Bitcoin Core y descargando la blockchain. Una vez configurado, el nodo sigue recibiendo nuevos bloques aproximadamente cada 10 minutos y los verifica antes de agregarlos a su copia de la blockchain.

Ejecutar un nodo ayuda a que la red de Bitcoin sea más segura y descentralizada, ya que más personas verifican el sistema de manera independiente.

#### ¿Qué es un nodo de Bitcoin?

> El propósito de la minería no es la creación de nuevos bitcoin; esa es la parte del sistema de incentivos. La minería es el mecanismo por el cual la seguridad de Bitcoin se descentraliza.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Los mineros recopilan transacciones no confirmadas, forman un bloque y gastan energía buscando una clave que agregue y asegure el bloque.


Los mineros compiten para agregar el siguiente bloque de transacciones a la blockchain. Para lograrlo, deben encontrar un número especial que genere un hash de bloque válido. Puedes imaginarlo como buscar la llave correcta entre miles de millones de posibilidades. El primer minero que encuentra el hash correcto gana la carrera y obtiene el derecho de agregar su bloque a la blockchain.

Cuando un minero encuentra un hash válido, comparte su bloque con la red. Otros mineros verifican rápidamente que la solución sea correcta. Si lo es, el bloque se agrega a la blockchain, ayudando a mantener seguro el libro mayor público de Bitcoin.

Los mineros obtienen bitcoin de dos maneras:

* **Recompensas por bloque:** Se crean nuevos bitcoin y se entregan al minero que agrega exitosamente un bloque a la blockchain.
* **Comisiones por transacción:** Cuando las personas envían bitcoin, incluyen una pequeña comisión. El minero que agrega el bloque recibe las comisiones de las transacciones incluidas en ese bloque.

#### Halvings de Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12.5 BTC | 6.25 BTC | 3.125 BTC |



> **Callout**
>
> Las recompensas de los mineros por completar un bloque se reducen a la mitad cada 210,000 bloques, aproximadamente cada cuatro años.


Bitcoin tiene un suministro máximo fijo de 21,000,000 de bitcoin, pero no todos fueron creados cuando Bitcoin comenzó. En su lugar, nuevos bitcoin se introducen gradualmente en circulación a través de **la minería**.

Cuando los mineros agregan exitosamente un nuevo bloque de transacciones a la red de Bitcoin, reciben una **recompensa por bloque** en bitcoin. En los primeros días de Bitcoin, esta recompensa era de 50 bitcoin por bloque. Esta recompensa motivaba a las personas a usar potencia informática y electricidad para ayudar a asegurar la red.

Aproximadamente cada 210,000 bloques (alrededor de cada 4 años), la recompensa por bloque se reduce a la mitad. Este evento se llama **halving**. El halving ralentiza la creación de nuevos bitcoin y ayuda a asegurar que el suministro total nunca supere los 21 millones. Con el tiempo, esto hace que bitcoin sea cada vez más escaso.


> **Definition – Suministro circulante**
>
> **El suministro circulante** se refiere a la cantidad total disponible de una moneda. En el caso de Bitcoin, el suministro circulante total es el número de monedas que se han minado y están en circulación en un momento dado.



> **Definition – Cronograma de suministro de Bitcoin**
>
> El **cronograma de suministro de Bitcoin** es el plan predeterminado y público para la liberación de nuevos bitcoins en circulación, diseñado para mantener la escasez de bitcoin con el tiempo.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/739a3085cf7a779aec7f212bd4b877568e427b43-292x200.svg)

Después de cada evento de halving, la recompensa en bitcoin que reciben los mineros por agregar un bloque se reduce a la mitad. Esto disminuye la tasa a la que se crean nuevos bitcoins.

Los mineros aún ganan comisiones por transacción de las transacciones incluidas en el bloque que minan. Con el tiempo, se espera que estas comisiones se conviertan en una parte más importante de los ingresos de los mineros.

Los halvings están incorporados en el protocolo de Bitcoin y ocurren automáticamente aproximadamente cada cuatro años. Gracias a esto, el calendario de emisión de Bitcoin es predecible y transparente.

La siguiente tabla muestra los próximos halvings, incluyendo la fecha aproximada, el número de bloque en que ocurren, la nueva recompensa por bloque y el porcentaje del suministro total de bitcoin que habrá sido minado.


| Evento | Fecha | Bloque | Recompensa | Minado |
| --- | --- | --- | --- | --- |
| Quinto Halving | 2028 | 1,050,000 | 1.5625 BTC | 98.44 % |
| Sexto Halving | 2032 | 1,260,000 | 0.78125 BTC | 99.22 % |
| Séptimo Halving | 2036 | 1,470,000 | 0.390625 BTC | 99.61 % |


A medida que se minan más bitcoin, el suministro en circulación sigue aumentando hasta alcanzar el suministro máximo de 21,000,000 de bitcoins, lo cual se espera alrededor del año 2140. Como cada vez se crean menos bitcoins nuevos, si la demanda aumenta, el precio de Bitcoin puede subir. Esto también motiva a los mineros a seguir asegurando la red al contribuir con su potencia informática.


---


#### ¿Qué es un hash de bloque válido en Bitcoin?

En Bitcoin, los mineros compiten para encontrar un código especial llamado **hash de bloque**. Este código identifica un bloque de transacciones y permite que se agregue a la blockchain.

Cada bloque contiene información sobre transacciones recientes e incluye también el hash del bloque anterior. Esto enlaza cada bloque con el anterior, formando una cadena desde el primer bloque (el Bloque Génesis) hasta el más reciente.

Un hash funciona como una **huella digital** para los datos del bloque. Si se cambiara cualquier información en el bloque, la huella digital también cambiaría. Esto facilita que cualquiera pueda verificar que el historial de transacciones de la blockchain no ha sido alterado y ayuda a mantener la red segura.


> **Callout**
>
> Satoshi Nakamoto, el creador de Bitcoin, minó el Bloque Génesis, que liberó un total de 50 bitcoin.


#### La carrera por minar un bloque

Los mineros compiten para encontrar un hash de bloque válido. El primer minero en encontrarlo puede agregar el nuevo bloque a la blockchain y recibir una recompensa en bitcoin.

Para ser válido, el hash del bloque debe ser menor que un número establecido por la red llamado objetivo de dificultad. Como los hashes son aleatorios, los mineros deben probar diferentes entradas hasta encontrar una que funcione.

Si hay demasiados mineros compitiendo, los bloques se encontrarían demasiado rápido. Si hay muy pocos mineros participando, los bloques tardarían demasiado en encontrarse. Para que el sistema funcione de manera estable, Bitcoin ajusta automáticamente la dificultad cada 2,016 bloques (aproximadamente cada dos semanas).

Este ajuste asegura que, en promedio, se agregue un nuevo bloque a la blockchain aproximadamente cada 10 minutos.


> **Definition – Definición de nivel de dificultad**
>
> El **nivel de dificultad** en la minería de Bitcoin mide cuán difícil es encontrar un hash de bloque válido. La red ajusta esta dificultad cada 2,016 bloques (aproximadamente cada dos semanas) para que los nuevos bloques se agreguen a la blockchain aproximadamente cada 10 minutos. Cuanto mayor es la dificultad, más difícil es para los mineros encontrar un bloque válido.



> **Info**
>
> Al encontrar un hash de bloque válido, un minero demuestra que ha realizado el trabajo necesario para agregar un nuevo bloque al blockchain. Este proceso se llama Prueba de Trabajo (PoW). Es el mecanismo de seguridad que permite a Bitcoin confirmar transacciones y agregar nuevos bloques a la blockchain. El minero que encuentra primero el hash válido obtiene una recompensa en bitcoin, que incluye la recompensa por bloque y las comisiones de las transacciones incluidas en ese bloque.


La Prueba de Trabajo (PoW) ayuda a mantener segura la red de Bitcoin al hacer extremadamente costoso que alguien intente hacer trampa o tomar el control de la red. En cambio, es mucho más rentable seguir las reglas.

Los mineros cumplen cuatro funciones principales:

1. **Recopilar transacciones**: Los mineros eligen transacciones que han sido enviadas a la red y las colocan en un bloque candidato.
1. **Realizar Prueba de Trabajo**: Los mineros compiten para resolver un difícil acertijo matemático encontrando un hash de bloque válido.
1. **Transmitir el bloque**: El primer minero en encontrar una solución válida comparte el nuevo bloque con la red.
1. **Obtén recompensas**: Si el bloque es válido, se agrega al blockchain y el minero recibe bitcoins recién creados más las comisiones por transacción.

Muchos mineros en todo el mundo intentan crear el siguiente bloque al mismo tiempo. Cuando un minero encuentra una solución válida, la red verifica el bloque. Si todo está correcto, se agrega al blockchain. Los demás bloques en competencia son descartados. Este proceso mantiene el consenso en la red y previene el doble gasto.

* Los mineros son computadoras que ayudan a mantener y actualizar el libro mayor de Bitcoin.
* Recopilan transacciones y las agrupan en un bloque. Luego, procesan los datos del bloque a través de un algoritmo de hash para crear un código único llamado hash.
* Los mineros repiten este proceso muchas veces, buscando un hash que cumpla con las reglas de Bitcoin. El primer minero en encontrar un hash válido obtiene bitcoins recién creados como recompensa y su bloque se agrega al blockchain.
* El hash de cada bloque también lo conecta con el bloque anterior. Si alguien intentara modificar una transacción pasada, los hashes ya no coincidirían y la red rechazaría la cadena alterada. Esto es lo que mantiene seguro el libro mayor de Bitcoin.
