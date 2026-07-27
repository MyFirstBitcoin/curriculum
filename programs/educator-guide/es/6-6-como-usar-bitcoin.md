# 6 - Cómo usar Bitcoin

Duración: 90 minutos

Idea central: Usar Bitcoin en cadena enseña a los estudiantes cómo funcionan en la práctica la propiedad, la autocustodia y la verificación, convirtiendo la teoría en acción financiera directa.

#### Objetivos de aprendizaje

Al final de esta lección, los estudiantes deberían ser capaces de:

* Identificar formas comunes de adquirir e intercambiar bitcoin, incluyendo métodos entre pares y a través de exchanges centralizados.
* Explicar la diferencia entre monederos autocustodiados y custodiados, y por qué la autocustodia es importante en Bitcoin.
* Describir el propósito de las llaves privadas, direcciones públicas, frases semilla e interfaces de monederos.
* Comparar diferentes tipos de monederos y evaluar sus ventajas y desventajas en función de la seguridad, conveniencia, privacidad y control.
* Configurar un monedero móvil de Bitcoin y explicar el proceso básico de recuperación.
* Demostrar cómo recibir y enviar una transacción de bitcoin en cadena.

Aplicar el principio "No confíes, verifica" a la elección de monederos, transacciones y el uso general de Bitcoin.

#### Herramientas y recursos

##### Material visual de apoyo

* Capítulo 6 - Cómo usar Bitcoin

##### Biblioteca de apoyo

* Tarjeta de referencia de vocabulario — Capítulo 6 — Términos: monedero, llave privada, dirección pública, frase semilla, custodiado, autocustodiado, UTXO, comisión de transacción
* Cuadros comparativos y hojas de referencia — Comparación de tipos de monederos (custodiado, móvil, hardware, papel)
* Explicaciones técnicas y análisis en profundidad — Llaves públicas/privadas, modelo UTXO, confirmación de transacciones
* Análisis profundo de la seguridad de la llave privada — Frases semilla, derivación de llaves, métodos de respaldo, vectores de ataque
* Guía de anatomía de una transacción — Ejemplo paso a paso de cómo funciona una transacción de Bitcoin
* Lista de mejores prácticas de seguridad — Antes de empezar, crear monedero, recibir, enviar, prevención de phishing

#### Actividades

* Transacciones en acción
* Carrera de relevos Lightning
* Explorando el mempool

#### Enseñanza en línea

* Deja claro desde el principio si los estudiantes están viendo una demostración o configurando un monedero ellos mismos.
* Utiliza capturas de pantalla grandes y legibles para cada paso de la configuración del monedero.
* Haz una pausa después de cada paso y pide a los estudiantes que confirmen su comprensión en el chat antes de continuar.
* Da una advertencia directa antes de la sección de la frase semilla y recuerda a los estudiantes que nunca deben compartir información sensible en línea.

#### Preparación

* Descarga y prueba una aplicación de monedero móvil (Blue Wallet o Muun); prepara capturas de pantalla de los pasos clave de configuración.
* Prepara una guía de configuración de monedero (descargar → crear → respaldar semilla → recibir) para referencia.
* Asegúrate de que la red/WiFi funcione; ten una dirección de demostración y un código QR listos para mostrar.

#### Procedimiento

Esta lección pasa de la teoría a la práctica directa. Ahora coincide directamente con la estructura del Diploma para que adquisición, monederos, configuración, transacciones y verificación aparezcan bajo los mismos encabezados principales que la guía del estudiante. El apoyo docente adicional permanece anidado dentro de esas secciones.

##### 6.0 Introducción, 8 minutos

Comienza conectando este capítulo con el anterior:

* Si Bitcoin es dinero, ¿cómo lo obtiene y usa la gente realmente?
* ¿Qué significa realmente controlar tu bitcoin?
* ¿Por qué usar Bitcoin es diferente a usar una app bancaria?

Aclara que este capítulo trata sobre el uso práctico. Los estudiantes ya no solo están aprendiendo qué es Bitcoin, están aprendiendo cómo interactuar directamente con él.

##### 6.1 Adquirir e intercambiar Bitcoin, 12 minutos

Explica que las personas pueden adquirir bitcoin de diferentes maneras, incluyendo:

* recibir pagos en bitcoin
* minar bitcoin
* intercambiar dinero fiduciario por bitcoin en persona
* intercambiar dinero fiduciario por bitcoin en línea

Luego enfócate en las dos principales formas de adquisición cubiertas en el capítulo:

* entre pares, en persona
* entre pares, en línea
* intercambios centralizados

Haz que los compromisos sean claros.

Para P2P en persona, enfatiza el intercambio directo sin un banco o intermediario, pero también menciona los riesgos prácticos de reunirse con personas para intercambios en efectivo.

Para P2P en línea, explica el escrow (depósito en garantía) en términos sencillos, como una forma de reducir el riesgo de contraparte mientras se permite el intercambio directo entre pares.

Para los intercambios centralizados, deja claro que son convenientes, pero requieren que los usuarios confíen en una empresa, a menudo compartan información personal y dejen los fondos bajo control de un tercero hasta que se retiren. Este es un buen momento para reforzar que la conveniencia suele venir acompañada de compromisos en privacidad y soberanía.

##### 6.2 Una Introducción a las Carteras de Bitcoin, 35 minutos

**Qué es realmente una Cartera de Bitcoin**

Aclara un malentendido común de inmediato: el bitcoin no se almacena dentro de la aplicación de la cartera como el dinero físico en una bolsa.  
El bitcoin existe en el libro mayor mantenido por la red. Lo que el usuario controla es la capacidad de gastarlo a través de las llaves privadas.

Luego explica las dos cosas a las que la gente suele referirse con "cartera":

* el sistema de llaves privadas, del cual se generan las direcciones
* la aplicación o interfaz utilizada para interactuar con la red

Utiliza la analogía del correo electrónico del capítulo si es útil:

* dirección pública = como una dirección de correo electrónico que puedes compartir
* llave privada = como una contraseña que debes proteger

Sé muy claro aquí: quien controla las llaves privadas controla el bitcoin. Ese es el concepto central que los estudiantes deben entender.

**Carteras de Autocustodia vs Carteras de Custodia**

Esta es una de las partes más importantes del capítulo.

Explica la distinción claramente:

* Cartera de autocustodia: el usuario controla las llaves privadas
* Cartera de custodia: un tercero controla las llaves privadas en nombre del usuario

Luego explica los compromisos:

Autocustodia

* control total sobre los fondos
* sin proceso de aprobación
* protección contra confiscación arbitraria
* mayor responsabilidad
* no hay recuperación fácil si se pierde la frase semilla

Custodia

* recuperación y soporte más fáciles
* más simple para principiantes
* más expuesto a congelaciones de cuentas, hackeos y control de terceros
* el usuario realmente no posee el bitcoin

Este es el momento adecuado para enfatizar la frase:

"Si no son tus llaves, no son tus monedas."

Los estudiantes deben salir de esta sección entendiendo no solo el eslogan, sino lo que realmente significa en la práctica.

**Diferentes Tipos de Carteras y Cómo Elegir Una**

Presenta los tipos de carteras cubiertos en el capítulo:

* cartera en línea
* cartera móvil
* cartera de escritorio
* cartera de hardware
* cartera de papel

No trates una como perfecta. En cambio, explica que cada una implica compromisos entre:

* seguridad
* privacidad
* conveniencia
* compatibilidad
* comisiones
* control
* reputación

También deja claro que recomendamos prestar atención a si el software de la billetera es de código abierto, porque las herramientas de código abierto pueden ser revisadas, auditadas y continuadas por la comunidad. Esto se conecta directamente con el principio de verificación en Bitcoin.

##### 6.3 Configuración de una billetera Bitcoin móvil, 10 minutos

Guía a los estudiantes a través del proceso básico mostrado en el capítulo:

* descargar la billetera
* crear una nueva billetera
* generar y anotar la frase de recuperación
* confirmar la frase de recuperación
* agregar seguridad adicional si está disponible
* abrir la billetera y encontrar la función de recibir

Haz que la advertencia sobre la frase semilla sea muy explícita:

* si se pierde la frase semilla, se puede perder el acceso a los fondos
* si alguien más obtiene la frase semilla, puede tomar los fondos

Si los estudiantes están haciendo esto de manera práctica, el educador debe pausar en cada paso y verificar que todos entienden lo que están haciendo. Si la clase es más conceptual, esta sección puede explicarse como una demostración en lugar de realizarse en vivo. La opción de recuperación mostrada en el capítulo también es útil para explicar que las billeteras pueden restaurarse si la frase semilla fue respaldada correctamente.

##### 6.4 Recibir y enviar transacciones, 17 minutos

**Recibir y enviar transacciones en cadena**

Ahora explica cómo funcionan las transacciones en cadena.

Para recibir bitcoin:

* abrir la billetera
* tocar recibir o depositar
* copiar la dirección, compartir el enlace o mostrar el código QR

Para enviar bitcoin:

* abrir la billetera
* pegar o escanear la dirección del destinatario
* ingresar la cantidad
* verificar todos los detalles
* transmitir la transacción
* esperar la confirmación

Deja claros estos puntos clave:

* la transacción transfiere la propiedad, no monedas físicas
* las transacciones son irreversibles
* los nodos verifican la validez
* los mineros incluyen las transacciones en los bloques
* las comisiones influyen en la prioridad de confirmación
* las transacciones en cadena generalmente son seguras, pero más lentas y a menudo más caras que las transacciones Lightning

El diagrama de flujo de transacciones en el capítulo es especialmente útil aquí, porque ayuda a los estudiantes a visualizar el camino desde la solicitud de la billetera hasta la confirmación en la red.

**Transacciones en acción y práctica basada en roles**

Utiliza la estructura de ejercicio cooperativo del capítulo para reforzar la comprensión. Explica los cuatro roles involucrados:

* remitente
* destinatario
* minero
* operador de nodo

Un enfoque sencillo en el aula es asignar roles y recorrer una transacción paso a paso. Esto ayuda a los estudiantes a ver que una transacción de Bitcoin no es magia, es un proceso coordinado que implica aprobación, verificación, inclusión en un bloque y actualizaciones en el libro mayor.

El objetivo aquí no es la profundidad técnica. Es ayudar a los estudiantes a entender quién hace qué en una transacción y por qué la verificación es importante.

##### 6.5 No confíes, verifica, 8 minutos

Explica que esto aplica a:

* billeteras
* casas de cambio
* aplicaciones
* detalles de la transacción
* afirmaciones sobre "ganancias fáciles"
* proyectos que pretenden ser como Bitcoin

Deja claro que Bitcoin requiere que los usuarios piensen críticamente, verifiquen lo que están usando y eviten la confianza ciega. Explica también por qué las herramientas de código abierto son importantes en este contexto: permiten la verificación independiente.

###### Cierre y Comprobación de Comprensión

Cierra con algunas preguntas rápidas:

* ¿Cuál es la diferencia entre una billetera de custodia y una de autocustodia?
* ¿Por qué es tan importante la frase semilla?
* ¿Qué sucede cuando envías una transacción en la cadena?
* ¿Por qué las transacciones en la cadena son más lentas que algunos otros pagos con Bitcoin?
* ¿Qué significa "No confíes, verifica" en la práctica?

#### Notas para el Educador

Este capítulo es altamente práctico, así que prioriza la claridad, la seguridad y la repetición.

Los estudiantes no necesitan dominar todos los tipos de billetera en una sola clase. Los objetivos principales son:

* entender los conceptos básicos de las billeteras
* entender la autocustodia
* aprender el flujo básico de una transacción
* adoptar una mentalidad responsable de verificación

Ten especial cuidado al hablar de las frases semilla y la configuración de la billetera. Los estudiantes deben irse entendiendo que estos no son detalles menores, sino la base de la propiedad de Bitcoin.

Los recursos visuales y actividades más útiles en este capítulo son:

* la comparación entre autocustodia y custodia
* la tabla de comparación de tipos de billetera
* el ejercicio paso a paso de configuración de billetera
* el diagrama del flujo de la transacción
* la actividad de transacción basada en roles

##### Cómo se ve un buen resultado

* Es importante que los estudiantes realmente configuren una billetera o vean una demostración cuidadosa, que la frase semilla sea el centro con "Estas 12 palabras SON tu Bitcoin", probar escenarios como "¿Qué pasa si pierdes tu teléfono?" y practicar el reconocimiento de phishing.
* Los educadores deben ser guías prácticos que ya hayan hecho esto antes, ser conscientes de la seguridad sin paranoia y ser honestos sobre la curva de dificultad y el aprendizaje requerido.
* Los estudiantes sienten que han aprendido una habilidad real que pueden usar, entienden que la frase semilla es real e importante y no algo abstracto, se sienten capaces de tener su propio Bitcoin y comprenden que la descentralización requiere responsabilidad personal.
* Los resultados de aprendizaje se cumplen si los estudiantes pueden configurar una billetera y entender la diferencia entre claves públicas y privadas, comprender los compromisos entre billeteras de custodia y autocustodia, explicar cómo funciona una transacción incluyendo entradas, salidas y comisiones, demostrar conciencia de seguridad incluyendo la protección de la frase semilla, y hacer preguntas críticas sobre la propiedad y el control.

##### Gestión del Tiempo

Si el tiempo es limitado, prioriza:

* Entender los conceptos básicos de las billeteras
* Entender la autocustodia
* Aprender el flujo básico de una transacción
* Adoptar una mentalidad responsable de verificación

Si hay tiempo de sobra, dedica tiempo a:

* Tabla comparativa de autocustodia vs custodia
* Tabla de comparación de tipos de billetera
* Ejercicio paso a paso de configuración de billetera con demostración en vivo
* Diagrama del flujo de la transacción con cálculo de comisiones
* Prácticas avanzadas de seguridad y consideraciones sobre billeteras hardware

##### Si los estudiantes tienen dificultades

* Frases semilla como "reales" → "Esta frase ES tu bitcoin; no hay servicio al cliente."
* Claves públicas vs privadas → Analogía con el correo electrónico (dirección vs contraseña).
* Por qué es difícil → "Tú lo controlas; tú eres responsable." Reconoce el compromiso.
