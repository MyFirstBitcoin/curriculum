# 8.1 La naturaleza del libro mayor de Bitcoin

El libro mayor de transacciones de Bitcoin (también llamado timechain o blockchain) es un registro de acceso público y con sello de tiempo de cada transacción válida que ha ocurrido en la red. Dentro del sistema financiero tradicional, las transacciones internas solo son visibles para participantes autorizados, como bancos, reguladores u operadores de datos como SWIFT, BACS o SEPA. El acceso a los datos de pagos en los sistemas tradicionales puede estar altamente restringido y ser costoso.

En contraste, dentro de la red de Bitcoin, cualquier persona con conexión a internet puede ver cada transacción, desde la mayor cantidad de valor hasta el Satoshi individual. Los participantes pueden rastrear el suministro total de bitcoin en tiempo real, monitorear la actividad de direcciones y monederos, y ver las recompensas de los mineros y el comportamiento de las comisiones. Aunque la actividad visible en el libro mayor está vinculada a direcciones de clave pública y no a identidades individuales, es posible agregar grandes conjuntos de datos sobre el comportamiento de gasto, permitiendo que todos recopilen e investiguen la actividad económica en tiempo real. A medida que la red crece y se acepta más como fuente de verdad económica, podríamos ver una menor dependencia de organismos gubernamentales y proveedores externos para la producción de análisis estadísticos e informes sobre el comportamiento de gasto.



#### 8.1.1 Nodos y Exploradores de Bloques

Cualquier persona que desee verificar de forma independiente el libro mayor de Bitcoin y acceder a sus datos debe ejecutar un nodo completo. El nodo completo suele describirse como la forma más fundamental de participar y verificar la economía de Bitcoin. Está disponible globalmente como software de código abierto que, al ejecutarse, descargará y validará todo el libro mayor de Bitcoin desde el ‘Bloque Génesis’, publicado en enero de 2009, hasta el día de hoy. También apoya la seguridad de la red de Bitcoin ayudando a verificar las nuevas transacciones que se agregan al libro mayor. Al acceder al libro mayor de Bitcoin de esta manera, el nodo completo sirve como fuente de verdad para investigadores y auditores de la red. Y, para los usuarios de Bitcoin, el nodo completo actúa como una puerta de entrada ‘autosoberana’ a la información transaccional de la economía de Bitcoin porque mejora la privacidad y la seguridad al eliminar la dependencia de servicios de terceros.

Mientras que los nodos completos descargan los datos en bruto, los exploradores de bloques como mempool.space o blockstream.info ofrecen una interfaz visual para buscar e interpretar la actividad del libro mayor. El explorador de bloques permite rastrear transacciones individuales y ver saldos e historiales de monederos. También muestra métricas de actividad de los mineros, como recompensas de bloque y datos de comisiones de transacción.

Juntos, los nodos completos y los exploradores de bloques son las herramientas que hacen utilizable la transparencia de la red de Bitcoin.



#### 8.1.2 Actividad: Explorando el Libro Mayor de Bitcoin

1. Abre [mempool.space](https://mempool.space) y explora la página principal.
  * ¿Cuál es la altura del último bloque?
  * ¿Cuál es la comisión de transacción actual (Baja, Media y Alta Prioridad)?
  * ¿Cuántas transacciones están esperando en el mempool para el próximo bloque?
1. Accede al último bloque en el libro mayor.
  * ¿Cuántas transacciones fueron incluidas?
  * ¿Quién es el minero del bloque?
  * ¿Cuál fue la recompensa del bloque?
1. Accede a una transacción en el bloque.
  * ¿Cuántas entradas y salidas tiene la transacción?
  * ¿Cuál es el valor de la transacción en BTC y USD?

Comenta las diferencias entre cómo se mueve el dinero dentro del sistema tradicional y cómo una empresa o gobierno utiliza este tipo de transparencia.
