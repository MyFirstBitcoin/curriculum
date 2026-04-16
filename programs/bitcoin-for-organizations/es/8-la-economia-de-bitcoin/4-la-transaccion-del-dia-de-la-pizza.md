# 8.4 La transacción del Día de la Pizza

Hasta ahora, este módulo se ha centrado en utilizar la naturaleza abierta del libro mayor de Bitcoin para recopilar métricas útiles a partir de datos de transacciones agregados. Sin embargo, es posible utilizar los datos del libro mayor y los exploradores de bloques para examinar transacciones reales y rastrear el movimiento de fondos dentro de la red.

Cada año, el 22 de mayo, la comunidad de Bitcoin reconoce a Laszlo Hanyecz, quien se convirtió en la primera persona de la que se tiene registro en utilizar bitcoin para comprar bienes físicos. El 18 de mayo de 2010, Hanyecz anunció en un foro de Bitcointalk.org que buscaba pizza y estaba dispuesto a pagar en BTC. Ofreció 10,000 BTC a quien estuviera dispuesto a realizar la transacción. Esperó varios días, hasta que el estudiante de 19 años Jeremy Sturdivant aceptó y envió dos pizzas grandes.

La **Pizza Day** transacción puede ser vista por cualquiera y tiene el siguiente ID de transacción:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Al ingresar este ID de transacción en [mempool.space](https://mempool.space) revela lo siguiente:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Fecha y hora de la transacción: 22 de mayo de 2010

Comisión de transacción en la red: 99,000,000 sats (en ese momento equivalía a menos de 1 centavo de dólar estadounidense. En mayo de 2025, esto equivale a $95,072.67)

Altura del bloque: 57,043

Número de confirmaciones: 838,645 (este es el número de bloques añadidos al libro mayor después de esta transacción)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Número de entradas de la transacción: 131

Número de salidas de la transacción: 1

Al hacer clic en la clave pública de salida (terminada en `XaxFyQ`) que sabemos que pertenecía a Jeremy Sturdivant, quien recibió 10,000 BTC por dos pizzas, se revela lo siguiente:

Esta dirección actualmente tiene un saldo de 0.00257879 BTC y parece que ha estado involucrada en 14 transacciones, la más reciente de las cuales fue el 13 de diciembre de 2024.



#### 8.4.1 Actividad: Discusión en grupo

1. Describe los beneficios (por ejemplo, auditoría, rendición de cuentas) o riesgos (por ejemplo, preocupaciones de privacidad) para individuos o empresas que utilizan un sistema de transacciones tan transparente y abierto.
1. ¿Cómo podría este tipo de transparencia financiera afectar a industrias como la caridad, la contratación pública, las remesas o la aplicación de la ley?
1. ¿Deberían los sistemas bancarios tradicionales ofrecer un nivel de visibilidad similar? ¿Serán obligados a hacerlo por el mercado?
