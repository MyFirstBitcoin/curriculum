# 6.1 El descubrimiento de la escasez digital

> Con Bitcoin, se ha descubierto un nuevo tipo de mercancía... una especie de mercancía digital, generada por computadoras y en parte hecha para computadoras. La humanidad tiene una historia de inventos significativos. En los libros de historia que se escribirán en el futuro, Bitcoin será listado como uno de ellos.  
_Prof. Dr. Philipp Sander_



#### 6.1.0 Escasez en la Economía

Dentro del ámbito de la economía, se entiende bien que la escasez es un principio clave que impulsa el valor. Los bienes y servicios que experimentan una demanda significativa se vuelven más valiosos si la oferta es limitada hasta el punto de que la demanda no puede ser satisfecha fácilmente. Además, la escasez alimenta la competencia y es un motor para el descubrimiento de precios en el mercado. En un mercado de competencia libre, justa y abierta, los precios deberían establecerse en el punto donde la oferta y la demanda se encuentran.

Los recursos que experimentan una demanda significativa pueden considerarse más valiosos si son finitos o más difíciles de adquirir. Esto puede estimular una mayor demanda de ese recurso a medida que los participantes del mercado compiten por asegurarse el acceso al mismo. Esta dinámica puede observarse con recursos naturales como metales preciosos, petróleo o los llamados 'commodities blandos' como los alimentos. La escasez, por lo tanto, sustenta la toma de decisiones económicas, la asignación de recursos y el costo de oportunidad. En un mundo de recursos ilimitados, todo sería igualmente accesible y de muy bajo valor. Por el contrario, la escasez otorga valor y promueve el comercio, la inversión y la innovación, ya que obliga a las sociedades a gestionar eficazmente los recursos limitados.



#### 6.1.1 El Desafío de la Escasez Digital

El desafío en torno a la escasez digital radica en la facilidad con la que la información digital puede ser copiada y distribuida. La información digital es inherentemente más difícil de asegurar que la información física porque, a diferencia de los bienes físicos - algunos de

los cuales poseen escasez de forma natural debido a limitaciones materiales - los elementos digitales como archivos de música, documentos o imágenes pueden duplicarse infinitamente a prácticamente ningún costo.

Tradicionalmente, la capacidad de replicar datos digitales ha significado que estos activos no podían tener un valor económico similar al de los bienes físicos porque carecían de cualquier forma de escasez exigible. Para el dinero digital, esto es particularmente problemático y se caracteriza como el problema del 'doble gasto', donde una sola unidad digital (por ejemplo, un token o moneda) podría ser copiada y gastada varias veces, devaluándola. Si es posible gastar dos veces una moneda, se devalúa al hacerla indistinguible de fondos falsificados o fraudulentos.

Tradicionalmente, las instituciones financieras centralizadas como los bancos mitigan este riesgo manteniendo un libro mayor que verifica cada transacción y deduce los saldos en consecuencia, asegurando que una vez que el dinero se gasta, no pueda ser reutilizado por el mismo titular de la cuenta. Sin embargo, este enfoque requiere una autoridad central de confianza u 'oráculo' para gestionar y verificar las transacciones, lo que impone dependencia y un único punto de control. Tener un oráculo centralizado de información deja los activos digitales vulnerables a la manipulación y la censura.

Para un sistema descentralizado y minimizado en confianza como Bitcoin, donde no existe una autoridad central que supervise las transacciones, prevenir el doble gasto es un desafío monumental. Sin un mecanismo para asegurar la unicidad de cada transacción, Bitcoin estaría abierto a la explotación, haciéndolo impráctico como reserva de valor y medio de intercambio confiable. Bitcoin resuelve el problema del doble gasto a través de un libro mayor descentralizado, donde las transacciones son confirmadas por miles de participantes de la red simultáneamente. Este mecanismo permite a Bitcoin mantener un registro inmutable de cada transacción, asegurando que cada moneda solo pueda gastarse una vez.

Esta solución genera escasez digital sin depender de un control central. Bitcoin introduce la primera solución exitosa a la escasez digital, allanando el camino para un ecosistema de activos digitales escasos y minimizados en confianza de una manera que antes se consideraba imposible.



#### 6.1.2 Haciendo Cumplir la Escasez Digital con Bitcoin

> Proponemos una solución al problema del doble gasto utilizando un servidor de marcas de tiempo distribuido entre pares para generar prueba computacional del orden cronológico de las transacciones. El sistema es seguro mientras los nodos honestos controlen colectivamente más poder de CPU que cualquier grupo cooperativo de nodos atacantes.  
_Satoshi Nakamoto_

Satoshi Nakamoto creó Bitcoin como una solución de ingeniería a los problemas asociados con el dinero fiduciario. Sin embargo, esa solución requería que Satoshi descubriera una forma de hacer cumplir la escasez digital absoluta. Para lograrlo, Satoshi desarrolló un protocolo de comunicación de código abierto que se ejecuta en una red descentralizada de computadoras o nodos. Cada uno de estos nodos mantiene una copia localmente verificable de un libro mayor inmutable, la llamada blockchain o timechain. El protocolo de Bitcoin define las reglas y la red descentralizada verifica las transacciones de forma independiente, adhiriéndose a las mismas reglas sin requerir una autoridad central.

La escasez de Bitcoin contribuye a su papel como reserva de valor. Al igual que el oro, Bitcoin es valioso no solo por su oferta limitada, sino también por el esfuerzo requerido para 'minar' o producir nuevas monedas. La minería de Bitcoin (el proceso que mantiene el libro mayor y emite nuevas monedas) es un proceso costoso y que consume mucha energía, que refleja el acto físico de extraer minerales de la tierra. Esta 'prueba de trabajo' digital impone una restricción de producción que alinea a Bitcoin con los commodities tangibles, dándole propiedades de durabilidad y verificabilidad que los bienes digitales tradicionales no tienen. La dificultad incorporada y la tasa decreciente de emisión de nuevas monedas a través de 'halvings' periódicos crean una estructura económica donde la oferta de Bitcoin se vuelve cada vez más escasa con el tiempo, aumentando su atractivo como reserva de valor a largo plazo.

##### ¿Cómo se hace cumplir la escasez digital?

La solución de Bitcoin al problema del doble gasto radica en su uso de un libro mayor descentralizado y públicamente visible. El libro mayor de Bitcoin puede considerarse como una base de datos inmutable que registra cada transacción en una cadena secuencial de lotes con marcas de tiempo, llamados bloques. Cada bloque es estrictamente cronológico y contiene transacciones que han sido verificadas y aceptadas por los participantes de la red. Cada bloque está conectado al anterior, creando un registro permanente que se distribuye a través de miles de nodos en todo el mundo. Al almacenar y compartir este libro mayor en una red descentralizada, Bitcoin elimina la necesidad de una autoridad central para confirmar transacciones. Cuando ocurre una transacción de Bitcoin, los nodos de la red la validan de forma independiente, asegurando que cada una solo se gaste una vez. Este libro mayor compartido también hace extremadamente difícil que los atacantes hackeen la red o alteren transacciones pasadas, ya que cualquier cambio requeriría la aprobación de la mayoría de los participantes de la red.

El mecanismo de Prueba de Trabajo (PoW) de Bitcoin refuerza aún más su protección contra el doble gasto al requerir que los mineros resuelvan un problema criptográfico para tener permiso de validar nuevas transacciones y crear un nuevo bloque. Este proceso, conocido como minería, exige poder computacional y añade un nivel de dificultad y costo a la alteración del libro mayor. Cada bloque añadido al libro mayor debe contener un enlace criptográfico al bloque anterior, lo que solidifica la integridad de la cadena y previene la manipulación.

El papel de un nodo es almacenar la copia más actual del libro mayor, que contiene un historial completo de transacciones. Los nodos mantienen a los mineros 'honestos', ya que verifican que no haya ocurrido un doble gasto y, lo que es más importante, que todas las monedas hayan sido creadas de acuerdo con el calendario de emisión de Bitcoin. Cualquier usuario de Bitcoin puede ejecutar un nodo y verificar la propiedad de sus monedas sin necesidad de confiar en un tercero. No es necesario que las autoridades resuelvan disputas en Bitcoin porque cualquier transacción incluida en un bloque es objetivamente válida.

##### ¿Cómo podría un atacante controlar la red de Bitcoin?

Si un atacante quisiera alterar una transacción pasada para tener éxito en un ataque de doble gasto, necesitaría rehacer la Prueba de Trabajo para ese bloque y todos los bloques posteriores, compitiendo contra el poder computacional combinado de toda la red. Este mecanismo de seguridad asegura que, si alguien intentara un doble gasto, necesitaría controlar más del 50% del poder de minería de la red para tener éxito. Esto se conoce como un ataque del 51%.

En los primeros años de Bitcoin, cuando era posible que participantes individuales crearan o minaran nuevos bloques usando hardware informático generalmente disponible, al menos teóricamente era posible desplegar suficiente poder de cómputo para tener éxito en un ataque del 51%. Hoy en día, el poder computacional combinado de la red de Prueba de Trabajo supera los 700 ExaHash/s. Esto significa que, en conjunto, las computadoras de minería están calculando más de 700 quintillones de hashes (cálculos criptográficos) cada segundo. Hemos llegado a un punto en el que el inmenso costo y la coordinación requeridos para reescribir el libro mayor y tener éxito en un ataque del 51% hacen que el doble gasto sea inviable en la práctica.

##### Confirmaciones y Reorganizaciones

Otra capa de protección (que a veces se pasa por alto) proviene del proceso de confirmación de transacciones de Bitcoin. Cuando una transacción se transmite por primera vez, se considera no confirmada y se recoge en el 'mempool' mientras espera ser incluida en un bloque y validada por los mineros. Una vez que una transacción se añade a un bloque, se considera 'confirmada'. Cada bloque añadido después de eso se cuenta como una confirmación adicional para la transacción. Aunque una transacción se considera oficial una vez que tiene una sola confirmación, no se considera final hasta que se añaden más confirmaciones.

Para una seguridad total, los usuarios de Bitcoin suelen esperar múltiples confirmaciones (típicamente seis), ya que cada bloque adicional añadido a la blockchain asegura aún más la transacción, reduciendo drásticamente la probabilidad de un intento exitoso de doble gasto. Este proceso de confirmación establece una ventana de tiempo durante la cual las transacciones se finalizan.

##### ¿Por qué esperar seis confirmaciones?

Los usuarios de Bitcoin esperan más confirmaciones porque es posible que el bloque más reciente de transacciones pueda ser eliminado de la cadena de bloques si ya no forma parte de la cadena más larga. Es importante notar que la minería es una competencia entre grandes grupos de poder computacional. Por lo tanto, es posible que dos mineros competidores encuentren una solución criptográfica válida y se añadan bloques separados a la cadena casi al mismo tiempo. Si eso ocurre, la cadena se divide esencialmente. Los mineros continuarán intentando añadir bloques a cada rama de la cadena. Sin embargo, una vez que se mina el siguiente bloque, la cadena más larga1 (definida como la cadena que tiene la mayor prueba de trabajo invertida en ella) es la que prevalece y el bloque en la cadena más corta queda 'huérfano' y es inválido. Todas las transacciones en el bloque huérfano se devuelven al mempool para su inclusión en un bloque válido posterior. Este proceso se llama reorganización o simplemente, un 'reorg'.

Un actor malicioso, que intente un doble gasto, debe tomar el control de la red el tiempo suficiente para 'reorganizar' la cadena. Como hemos visto anteriormente, obtener el control total requiere una enorme cantidad de poder computacional, pero ¿qué pasa si una gran operación minera - que hipotéticamente controla poco más de un tercio de todo el poder computacional de la red - intenta un doble gasto de monedas?

Veamos un ejemplo:

Supongamos, por ejemplo, que la potencia total de minado de la red de Bitcoin es de 550 ExaHash/s. Rogue Inc, que controla 200 ExaHash/s, realiza una gran compra inmobiliaria y planea pagar en Bitcoin. Sin embargo, Rogue también planea intentar un doble gasto con las mismas monedas. El vendedor le dice a Rogue que esperará seis confirmaciones antes de entregar las escrituras. Para llevar a cabo un ataque de doble gasto, Rogue debe construir en secreto una rama alternativa en la cadena, minando una cadena más larga que contenga la transacción de doble gasto. Una vez que el vendedor ha visto seis confirmaciones que incluyen su transacción y ha entregado el activo, Rogue debe entonces publicar todos los bloques que minó en la nueva rama, convirtiéndola en la cadena más larga. ¿Qué tan posible es esto?

En cualquier momento, la probabilidad de que Rogue mine el siguiente bloque es 200/550 = 0,36. Incluso si Rogue es el mayor pool de minería, la probabilidad de que los mineros honestos encuentren el siguiente bloque es 1 - 0,36 = 0,64. Los bloques deberían minarse mucho más rápido en la cadena honesta. Pero supongamos que Rogue tiene suerte, mina un bloque y lo mantiene en secreto. Luego intenta minar otro en esta rama secreta. Sin embargo, la cadena honesta mina un bloque y se adelanta minando otro más, antes de que Rogue mine su segundo bloque.

Entonces Rogue se rinde. ¿Por qué?


| Bloques por alcanzar | 1% | 10% | 36% (Rogue) | 51% |
| --- | --- | --- | --- | --- |
| 1 | 0.010101 | 0.111111 | 0.562500 | 1.0 |
| 2 | 0.010102 | 0.012346 | 0.316406 | 1.0 |
| 3 | 1.0e-06 | 0.001372 | 0.177919 | 1.0 |
| 4 | 1.0e-08 | 0.000152 | 0.100113 | 1.0 |
| 5 | 1.0e-10 | 0.000017 | 0.056314 | 1.0 |
| 6 | 1.0e-12 | 1.9e-06 | 0.031676 | 1.0 |


**Fuente**: Basado en una tabla de Grokking Bitcoin por Kalle Rosenbaum

Rogue se da cuenta de que no tiene suficiente tasa de hash para lograr el doble gasto, a pesar de controlar el 36% de la tasa de hash de Bitcoin. Para tener éxito, debe minar cuatro bloques adicionales para adelantarse a la cadena honesta. A pesar de su enorme poder de cómputo y de controlar el 36% de la red, las probabilidades de éxito de Rogue son solo de 0.100113.


> **Dark – La teoría de juegos entra en acción**
>
> Las probabilidades de éxito de Rogue son pésimas, pero aún puede empeorar. Por cada minuto que siga intentándolo, Rogue consume una enorme cantidad de electricidad. Todo esto habrá sido en vano. Además, por cada bloque que no logre minar honestamente, Rogue pierde la recompensa del bloque, que actualmente es de 3.125 monedas por bloque, valoradas actualmente en más de $300,000.
>
> La razón principal del fracaso de Rogue fue que el vendedor del inmueble exigió seis confirmaciones. Cuantas más confirmaciones se requieran, más difícil será para los mineros deshonestos construir cadenas alternativas de bloques. De hecho, para una transacción muy grande, un vendedor puede exigir más confirmaciones. Por ejemplo, diez confirmaciones (que deberían tomar alrededor de 100 minutos) reducirían las probabilidades de éxito de Rogue a solo 0.003.
>
> De esta manera, la teoría de juegos en torno a la minería asegura que todos estén incentivados a actuar honestamente y no desperdiciar recursos computacionales ni renunciar a las recompensas de bloque. Además, es de interés para todos los mineros que la red de Bitcoin sea segura y confiable. Esto garantiza que su enorme inversión en poder de cómputo esté protegida. Si la red es atacada con éxito, el valor de mercado de las monedas caerá drásticamente, ya que la confianza en la red se verá disminuida.




#### 6.1.3 ¿Es la centralización de la minería una amenaza?

Como se ve en la tabla anterior, la centralización de la minería puede representar una amenaza potencial para la protección contra el doble gasto de Bitcoin, ya que aumenta la probabilidad de un ataque del 51%: un escenario en el que un solo minero o grupo de mineros controla más de la mitad de la potencia computacional de la red. Si esto ocurriera, la entidad controladora podría, en teoría, alterar transacciones recientes o intentar un doble gasto reescribiendo el libro mayor, permitiéndole gastar las mismas monedas más de una vez.

Tal situación socava la integridad de la red de Bitcoin al otorgar una influencia desproporcionada sobre la validación de transacciones a unos pocos actores. Sin embargo, aunque teóricamente posible, ejecutar un ataque del 51% seguiría siendo altamente complejo y costoso, requiriendo enormes recursos computacionales, electricidad y coordinación, lo que probablemente superaría los posibles beneficios de intentar un doble gasto.

Existen salvaguardas que ayudan a limitar los riesgos de la centralización de la minería. Los pools de minería, por ejemplo, permiten que los mineros más pequeños combinen recursos y compartan las recompensas de bloque, reduciendo el dominio de cualquier entidad individual. Si bien esta es una forma útil para que los pequeños mineros participen en la red, existe el riesgo de que la entidad que controla el pool se comporte de manera indebida e intente atacar la red. Sin embargo, la transparencia del libro mayor de Bitcoin también significa que cualquier concentración de poder de minado es visible, alertando a la comunidad sobre posibles riesgos y permitiendo tomar contramedidas. Los mineros son muy conscientes de que cualquier ataque a la red de Bitcoin pone en serio riesgo su propuesta de valor, por lo que es muy sencillo para los pequeños mineros cambiarse a un nuevo pool para evitar que su poder de minado sea utilizado de manera nefasta. Si bien el riesgo no es cero, la naturaleza abierta y distribuida del ecosistema de Bitcoin, combinada con el alto costo de un ataque, hace que la centralización de la minería sea más una amenaza teórica que inminente, ya que mantener tal control durante períodos prolongados sería financieramente inviable para cualquier atacante.



#### 6.1.4 El impacto más amplio de la escasez digital

Bitcoin ha transformado la manera en que pensamos sobre la escasez en el ámbito digital. Debido a que los bienes digitales —como el software, archivos de música, libros electrónicos y contenido en línea— poseen características que los diferencian de los bienes físicos, pueden reproducirse a un costo insignificante y compartirse al instante. A diferencia de los objetos físicos, que están limitados por restricciones materiales como los costos de producción y las limitaciones de almacenamiento, los bienes digitales existen como datos que pueden duplicarse infinitamente sin degradación en la calidad. Esto significa que, mientras los bienes físicos son inherentemente escasos debido a estas restricciones materiales, los bienes digitales han sido tradicionalmente abundantes, careciendo de mecanismos incorporados para limitar su oferta.

Es importante destacar que los bienes digitales son no rivales. Esto significa que el consumo de un bien digital por parte de una persona no disminuye la disponibilidad de ese bien para los demás. Por ejemplo, cuando se descarga una canción, puede copiarse y distribuirse un número ilimitado de veces sin perder utilidad. Históricamente, esta abundancia supone un desafío para la creación de valor, ya que el modelo económico tradicional de oferta y demanda se distorsiona cuando la oferta es, al menos teóricamente, ilimitada. En respuesta a esto, la gestión de derechos digitales (DRM) y otras medidas de escasez artificial han intentado restringir el acceso. Sin embargo, estos mecanismos pueden ser eludidos y delegan la confianza en autoridades centralizadas. La innovación de Bitcoin radica en cómo aborda este problema de forma nativa, convirtiéndose en el primer activo digital en incorporar escasez mediante tecnología descentralizada sin depender de estas limitaciones tradicionales.

Bitcoin desempeña un papel transformador al establecer la escasez digital mediante la introducción de un protocolo que impone una oferta finita. Un límite de 21 millones de monedas está codificado en el protocolo y este límite no puede cambiarse sin el consenso de la red, es decir, todos los miles de participantes distribuidos globalmente que ejecutan nodos de Bitcoin. De esta manera, Bitcoin ha creado un activo que imita la naturaleza finita de las materias primas físicas, como el oro, mientras existe completamente en el ámbito digital. El límite de suministro es fundamental para la propuesta de valor de Bitcoin y se sostiene mediante una combinación de criptografía, mecanismos de consenso y código abierto y transparente. Esto garantiza que todos los participantes de la red sigan las mismas reglas, además de estar impulsados por el incentivo económico clave de asegurar que la oferta de monedas sea absolutamente y comprobablemente finita.

Al resolver el problema del doble gasto, Bitcoin previene la inflación o duplicación del activo, un desafío que ha afectado a experimentos previos de dinero digital. Dentro de Bitcoin, ninguna autoridad única controla la oferta, lo que lo hace inmune a la manipulación centralizada del tipo que se observa en el sistema monetario fiduciario, como la impresión arbitraria de moneda o la devaluación. Esta innovación permite que Bitcoin funcione como reserva de valor y cobertura contra la inflación, permitiéndole ocupar una posición única similar al 'oro digital': un recurso digital escaso con valor verificable.



#### 6.1.5 Conclusión

En conclusión, cada vez se comprende más ampliamente que la innovación de Bitcoin en cuanto a la escasez digital ha redefinido el concepto de dinero. Sin embargo, a veces se pasa por alto que Bitcoin también transformó el panorama digital al resolver el antiguo problema de crear escasez en un mundo digital inherentemente abundante. Bitcoin ha introducido efectivamente una nueva categoría de activo digital que refleja las cualidades de las materias primas físicas.

Este avance demuestra que un sistema descentralizado puede establecer escasez, inmutabilidad y valor independientemente de cualquier autoridad central. Además, puede tener usos más allá del dinero, ya que ha inspirado todo un campo de investigación y desarrollo en torno a esta tecnología.

De cara al futuro, el modelo de escasez digital de Bitcoin está moldeando el futuro del dinero y del almacenamiento de valor. A medida que las preocupaciones sobre la inflación y las preguntas sobre la gestión de la moneda fiduciaria se reconocen más ampliamente, la oferta fija de Bitcoin lo hace cada vez más atractivo como cobertura frente a la inestabilidad financiera tradicional.

En última instancia, el descubrimiento de la escasez digital por parte de Bitcoin puede marcar el inicio de un cambio de paradigma, donde los activos digitales con escasez reconocida y confianza verificable ganan reconocimiento como componentes valiosos de la economía moderna, estableciendo una base para el futuro de las finanzas descentralizadas y la propiedad digital. Esto tiene implicaciones significativas para el campo de la economía: Bitcoin ha proporcionado el modelo de cómo la escasez y el valor pueden existir en forma digital.

> Más allá de la escasez digital, Bitcoin es también el primer ejemplo de escasez absoluta, la única mercancía líquida (digital o física) con una cantidad fija establecida que no puede aumentarse de ninguna manera concebible. Hasta la invención de Bitcoin, la escasez siempre fue relativa, nunca absoluta.  
_Saifedean Ammous_



###### Notas

1. La cadena más larga es aceptada por los nodos de Bitcoin como la versión más válida del libro mayor y se define como la cadena que requirió más esfuerzo (o la mayor prueba de trabajo) para construirse. Más información aquí: [https://learnmeabitcoin.com/technical/blockchain/longest-chain/](https://learnmeabitcoin.com/technical/blockchain/longest-chain/)
