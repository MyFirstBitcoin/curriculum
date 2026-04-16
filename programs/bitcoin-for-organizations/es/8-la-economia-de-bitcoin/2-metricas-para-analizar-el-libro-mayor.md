# 8.2 Métricas para analizar el libro mayor

Debido a que la transparencia de Bitcoin es diferente a la de los sistemas financieros tradicionales —donde gran parte del flujo monetario ocurre a puertas cerradas en instituciones—, surge un campo rico de análisis en cadena, donde los datos a nivel de red se convierten en una lente para comprender el comportamiento de los usuarios, los flujos monetarios y las tendencias a largo plazo. Estas métricas pueden ayudar a responder preguntas específicas, como cuán activamente se está utilizando la red, si las monedas se están acumulando o vendiendo, y si la red se está volviendo más segura.

Comprender estas métricas es útil no solo para los usuarios de Bitcoin, sino también para investigadores o responsables de políticas que buscan obtener información sobre este sistema financiero singularmente transparente.

Esta sección contiene algunas métricas comúnmente utilizadas para analizar la actividad de Bitcoin agrupadas en subcategorías. No es una lista exhaustiva. Visita [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) para una lista más completa y descripciones.



#### 8.2.1 Métricas de Direcciones

Las métricas de direcciones son útiles para monitorear a lo largo del tiempo, ya que indican el nivel de actividad en la red de Bitcoin. Por ejemplo, a medida que Bitcoin es más adoptado, el número de direcciones activas aumenta. Podemos examinar esto más a fondo destilando el número de direcciones que poseen una cantidad mínima especificada de Bitcoin, digamos 0.1 BTC, en un determinado período de tiempo, como un año. Si bien esto proporciona una visión de la adopción de Bitcoin a lo largo del tiempo, es imperfecto, ya que un individuo puede tener múltiples direcciones de Bitcoin. Por el contrario, los exchanges o ETFs pueden aparecer como entidades únicas cuando en realidad mantienen fondos para un gran número de personas.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Direcciones que mantienen Bitcoin > X BTC por año. Fuente: Bitcoin Magazine Pro._

Al comparar las direcciones con el precio de mercado actual de BTC es posible ver el porcentaje total de direcciones de Bitcoin que están en ganancia. Esto nos permite rastrear el sentimiento del mercado, ya que podemos ver qué proporción del mercado mantiene BTC con ganancia o pérdida.

Por ejemplo, el **Porcentaje de Ganancia No Realizada** en el gráfico a continuación muestra la proporción de todas las direcciones del libro mayor con una ganancia no realizada medida en dólares estadounidenses. Ten en cuenta que, dado que el gráfico a continuación fue tomado cerca del máximo histórico de Bitcoin, el porcentaje de direcciones que muestran una ganancia no realizada está cerca del cien por ciento. También podemos ver que los períodos prolongados de Porcentaje de Ganancia No Realizada por debajo de una desviación estándar de la media son inusuales. Por lo tanto, una caída por debajo de esta línea puede sugerir un buen punto de entrada para compradores.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Porcentaje de Ganancia No Realizada. Fuente: checkonchain.com_



#### 8.2.2 Indicadores en Cadena

Los indicadores en cadena son útiles porque ofrecen una visión del comportamiento de la red, más allá de lo que pueden mostrar solo el precio y las métricas de direcciones. Ayudan a los analistas a comprender las acciones y el sentimiento de diferentes tipos de participantes, como los tenedores a largo plazo frente a los operadores a corto plazo, al rastrear cómo se mantienen, mueven o valoran las monedas a lo largo del tiempo. Estos indicadores aprovechan la naturaleza transparente del libro mayor para revelar dinámicas de mercado ocultas como acumulación, distribución o incluso la convicción de los inversores. Esto los hace especialmente útiles para identificar tendencias estructurales, evaluar si el mercado está sobrecalentado o infravalorado y anticipar puntos de inflexión en un ciclo de mercado.

Por ejemplo, al examinar el valor de las tenencias de BTC desde la última vez que se transaccionaron, podemos deducir si el mercado está o no bajo estrés (como podría estarlo durante un mínimo importante del ciclo). Esta métrica se conoce como **Precio Realizado** y nos da una 'base de costo promedio' de todo el BTC en circulación. Si el precio de mercado cae por debajo del Precio Realizado, esto muestra que en conjunto la mayoría de las direcciones mantienen una pérdida no realizada.

Agrupando aún más los datos del libro mayor en bandas de antigüedad, podemos mostrar cómo la cantidad de BTC se mueve entre direcciones a lo largo del tiempo, lo que crea patrones ondulatorios en un gráfico conocidos como **Ondas HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Ondas HODL de Bitcoin. Fuente: Bitcoin Magazine Pro._

Las ondas HODL muestran lo que los tenedores a largo, mediano y corto plazo están haciendo con su BTC. Por ejemplo, en el gráfico anterior, los tenedores a corto plazo se muestran en rojo y naranja y podemos ver picos de actividad cuando este grupo se apresura a comprar cerca de los máximos del mercado. En el otro extremo, podemos ver que los tenedores a muy largo plazo (en púrpura y azul) están aumentando constantemente su participación total en la red, lo que indica una alta convicción entre estos grupos. El gráfico es imperfecto, ya que algunas monedas pueden moverse de direcciones antiguas a nuevas bajo el control del mismo usuario. Sin embargo, proporciona una visión interesante de la convicción de los tenedores a largo plazo.

Otra forma de examinar el 'dinero inteligente' de los tenedores a largo plazo es analizar los **Días de Moneda Destruidos** (CDD). El concepto de 'Días de Moneda' es el resultado de multiplicar el número de BTC por los días desde la última vez que se movieron las monedas. Por ejemplo, 5 BTC que no se han movido en 100 días han acumulado 500 días de moneda y 10 BTC que no se han movido en 10 días han acumulado 100 días de moneda. De esta manera, damos mayor peso a las monedas mantenidas por más tiempo. Cuando esas monedas se mueven, esos días de moneda se 'destruyen'. Este indicador muestra aumentos en el CDD en momentos de movimientos significativos de precio, lo que proporciona a los analistas una forma de separar la actividad rutinaria del mercado de cambios significativos en el sentimiento de los tenedores a largo plazo.

Otra métrica que puede ayudar a identificar si el mercado está subvalorando o sobrevalorando BTC es la Relación Valor de Mercado a Valor Realizado o **MVRV**. Se calcula simplemente como la relación entre el Valor de Mercado (número de BTC en circulación multiplicado por el precio de mercado) dividido por el Valor Realizado (la suma de todos los BTC desde la última vez que se movieron). Un MVRV alto sugiere que más monedas están en ganancia (a menudo visto cerca de los máximos del mercado) y un MVRV bajo indica que muchas monedas se mantienen en pérdida (visto cerca de los mínimos del mercado).



#### 8.2.3 Métricas de Minería

Las métricas de minería son útiles para comprender la seguridad, los incentivos económicos y la salud general de la red de Bitcoin. Métricas como el hashrate, los ingresos de los mineros, la dificultad y las proporciones de comisiones revelan cuánta potencia computacional está asegurando la cadena de bloques y cuán bien están siendo compensados los mineros por sus actividades.

El **Hashrate** de la red de Bitcoin es quizás el indicador más comúnmente mencionado de la salud de la red y la fortaleza de su seguridad. Dado que el proceso de minería asegura la red y confirma que las transacciones en el libro mayor son válidas, cuanto mayor sea el nivel de poder de cómputo (o hash), más difícil será para un actor malicioso sobrepasar y atacar la red.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate de Bitcoin. Fuente: Bitcoin Magazine Pro._

El gráfico anterior muestra que, en mayo de 2025, la potencia de cómputo total de la red se sitúa en torno a 900 TeraHash/s (900 billones de cálculos criptográficos de 'hash' por segundo). Si el hashrate está aumentando, muestra que la red se está volviendo más segura, lo cual es tranquilizador para los usuarios.

El Múltiplo de Puell (ideado por David Puell) observa el ciclo de mercado desde la perspectiva de los mineros y sus ingresos. La métrica se calcula dividiendo la emisión diaria de BTC (en USD) por el promedio móvil de 365 días del valor de emisión diaria. La métrica ayuda a identificar períodos de estrés o alivio para los mineros. Históricamente, un múltiplo superior a 3 ha precedido una caída en el valor de mercado de BTC, ya que indica que los mineros son altamente rentables. Un valor inferior a 0.5 indica estrés y ha señalado históricamente mínimos de mercado para el valor de BTC.
