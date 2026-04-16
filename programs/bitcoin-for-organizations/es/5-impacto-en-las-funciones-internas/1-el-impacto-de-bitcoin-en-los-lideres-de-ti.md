# 5.1 El impacto de Bitcoin en los líderes de TI

> Toda persona informada necesita saber sobre Bitcoin porque podría ser uno de los desarrollos más importantes del mundo.  
_Leon Luow_



#### 5.1.0 Introducción

Los líderes de TI tienen responsabilidades con el negocio, utilizando la tecnología tanto para impulsar la innovación y la competitividad de sus empresas, como para encontrar formas de mejorar la eficiencia interna y reducir costos.

Existen varios riesgos y conceptos erróneos comunes sobre Bitcoin que es útil comprender y sobre los cuales se puede orientar:

* A menudo se ve como parte de una industria ‘cripto’ más grande, y soluciones basadas en una de las innovaciones clave utilizadas, la blockchain.
* Se percibe que ‘desperdicia energía’ para operar la red.
* Existe un riesgo para los usuarios de la Nube Pública de que el entorno pueda ser hackeado y utilizado para ‘minar’ Bitcoin u otras criptomonedas por un actor malicioso, lo que puede llevar a una factura muy grande e inesperada, así como a impactos en el rendimiento de las aplicaciones empresariales.
* Existe una falta de conocimiento sobre la tecnología detrás de Bitcoin.

En el lado positivo, Bitcoin podría beneficiar a cualquier empresa mediante:

* Ser añadido a la tesorería como un activo, ya sea minado directamente o comprado en el mercado abierto.
* Utilizar recursos que de otro modo estarían inactivos para minar Bitcoin para la empresa.
* Proporcionar justificación para inversiones en soluciones de IA que requieren recursos informáticos de alto rendimiento similares.
* Agregar un método de pago alternativo para la compra de servicios o productos de la empresa.
* Reducir las comisiones globales por transacciones en divisas extranjeras.
* Ofrecer un beneficio adicional a los empleados a través de incentivos basados en pagos Lightning.
* Construir nuevas fuentes de ingresos para la empresa basadas en Bitcoin.

Cualquier líder de TI debe tomarse el tiempo para entender Bitcoin, el impacto potencial y los riesgos asociados, así como los posibles beneficios, para poder proporcionar orientación y liderazgo al negocio.

> Bitcoin es un logro criptográfico notable. La capacidad de crear algo que no se puede duplicar en el mundo digital tiene un valor enorme. Muchas personas construirán negocios sobre eso.  
_Eric Schmidt_



#### 5.1.1 Riesgos y conceptos erróneos sobre Bitcoin

##### Bitcoin como parte de una industria ‘cripto’ más grande.

Bitcoin fue el primer intento exitoso de crear un activo digital finito y ha dado lugar a toda una industria de ‘alt-coins’ que intentan utilizar parte de la tecnología subyacente para ‘mejorar’ Bitcoin o construir una solución para abordar otras oportunidades potenciales de mercado.

Los proveedores de nube pública han creado plataformas de blockchain para permitir a las empresas construir estas soluciones, sin embargo, el interés en ellas tiende a subir y bajar en línea con el bombo de la industria; de hecho, Microsoft descontinuó su servicio de blockchain en 2021.

* Hasta 2017, Bitcoin representaba hasta el 95% de la capitalización total del mercado cripto.
* La primera ola de ICOs cripto ‘alternativas’ hizo que la dominancia cayera a un mínimo histórico del 37,6%.
* A medida que estas no lograron aportar beneficios reales al negocio y comenzaron a desaparecer, la dominancia de Bitcoin empezó a aumentar nuevamente.
* En 2021, a medida que el precio de Bitcoin aumentó, apareció en el mercado una nueva ola de soluciones alternativas basadas en NFT que volvió a reducir la dominancia de Bitcoin.
* Después de que este bombo tampoco lograra aportar beneficios reales, la dominancia de Bitcoin ha comenzado a subir de nuevo.
* Cuando Bitcoin entre en otro mercado alcista, es posible que surja una nueva ola de ‘alt-coins’ para capitalizar una nueva tendencia, pero probablemente tendrán un destino similar.

Si el negocio acude al líder de TI con el último ‘objeto brillante’ que se promociona para una aplicación particular de la blockchain, o como alternativa a Bitcoin, es importante tener en cuenta esta tendencia y preguntar:

* ¿Cuál es el propósito de la blockchain?
* ¿Se necesita o es deseable una blockchain, dado sus inconvenientes de rendimiento en comparación con una base de datos relacional centralizada?
* ¿Quién puede cambiar el protocolo y cuál es el impacto en la solución?
* ¿Qué sacrificios se han hecho en seguridad o descentralización para proporcionar el rendimiento declarado?
* ¿Qué beneficio puede aportar que no pueda ser entregado usando Bitcoin y los protocolos asociados, como Lightning?

##### Implicaciones de operar Bitcoin

Dependiendo del sector en el que opere la empresa, puede haber beneficios potenciales de la actividad de minería de Bitcoin, típicamente donde el calor generado puede ser aprovechado. Sin embargo, a menudo hay resistencia debido a la percepción de que Bitcoin es malo para el medio ambiente, desperdicia energía o tiene poco beneficio.

Como líder de TI, comprender esta dinámica y si existen beneficios potenciales para la empresa es necesario para proporcionar una orientación efectiva. El consenso general ha sido que Bitcoin no es ‘bueno para el medio ambiente’ y ‘desperdicia energía’. Sin embargo, esto está cambiando rápidamente, se están publicando informes más positivos y se espera que esta narrativa cambie a una en la que la minería de Bitcoin pueda verse como positiva para el medio ambiente y la transición a fuentes de energía renovable. Esto es algo en lo que muchas empresas se enfocan en sus iniciativas ESG.

##### Comprender los riesgos potenciales de la minería cripto

Ha habido ejemplos en el pasado donde el entorno de nube pública gestionado por una empresa ha sido tomado por hackers, quienes pueden habilitar rápidamente recursos informáticos adicionales para minar cripto. Cuantos más recursos se habiliten del perfil de mayor rendimiento (más costoso), mayores serán las posibilidades de que el hacker mine Bitcoin u otra cripto. Esto se conoce como ‘Crypto-Jacking’ - según AWS:

‘Este es un tipo de ciberdelito que implica el uso no autorizado de dispositivos (computadoras de borde, teléfonos inteligentes, tabletas o incluso servidores) para minar criptomonedas. A medida que los precios de las criptomonedas suben y se utilizan dispositivos de borde más potentes con capacidades de GPU para ejecutar casos de uso de Machine Learning en el borde, existe una amenaza creciente de que los criptojackers exploten vulnerabilidades de seguridad en los dispositivos de borde. Cuando esto sucede, los recursos de computación de borde se utilizan para minar criptomonedas, lo que resulta en un mayor uso de CPU/GPU, una degradación en el rendimiento de las aplicaciones de borde y un aumento en los tiempos de procesamiento de inferencia de ML en el borde.’

Por lo tanto, es fundamental que cualquier uso de recursos de nube pública esté correctamente diseñado siguiendo las mejores prácticas. Estas suelen estar descritas en algún tipo de Marco de Adopción de la Nube, que describe recomendaciones sobre seguridad, rendimiento, monitoreo, resiliencia y operaciones. El líder de TI debe asegurarse de que se sigan estas recomendaciones y que se habilite algún tipo de monitoreo en tiempo real para identificar y mitigar estos ataques antes de que se generen facturas elevadas.

##### Falta de conocimiento de la tecnología utilizada por Bitcoin

Existen muchos conceptos erróneos sobre la tecnología detrás de Bitcoin, lo que lleva a preguntas sobre si puede ser hackeado, la energía que utiliza o si será superado por una nueva versión como ha sucedido a menudo con la tecnología. Como líder técnico, tener un entendimiento de la tecnología subyacente sería útil para posicionar correctamente a Bitcoin internamente y mitigar estas preocupaciones.



#### 5.1.2 En el lado positivo.

##### Bitcoin como activo de tesorería

Existen posibles beneficios financieros para una empresa que pone Bitcoin en sus libros como un activo de tesorería.

* Reserva de valor y cobertura contra la inflación
* La confianza menguante en las monedas fiduciarias como reserva de valor
* Riesgo de contraparte en el sector bancario
* Ventaja del primer movimiento para las empresas que añaden Bitcoin a su tesorería

Si bien las implicaciones financieras de hacer esto desde una perspectiva contable no son responsabilidad del líder de TI, sí lo es entender cómo podría funcionar, cómo se puede comprar, almacenar y asegurar el Bitcoin.

Existen servicios disponibles en el mercado que ayudan a comprar, custodiar y ofrecer servicios de préstamo contra los activos almacenados. Si esto se convierte en un tema de discusión dentro de la empresa, como debería ser, el líder de TI puede ayudar a calificar a las posibles empresas externas que ofrezcan estos servicios. La debida diligencia para asegurar que los servicios ofrecidos cumplan con las necesidades de seguridad, transparencia y características necesarias ayudará a garantizar la selección de un socio confiable.

##### Beneficios de la minería de Bitcoin

Se espera que el uso de los centros de datos solo crezca en el futuro, y un gran porcentaje de los costos de operar un centro de datos es disipar el calor generado. Esto es especialmente cierto para aplicaciones que utilizan computación de alto rendimiento, como IA/ML y la minería de Bitcoin.

Empresas de diferentes sectores a nivel mundial han identificado cómo este aumento en la generación de calor puede convertirse en un beneficio neto para el negocio en lugar de un costo, utilizando el calor generado para:

* Piscinas/Spas
* Centros acuáticos
* Cultivo de flores/verduras en invernaderos
* Calefacción de las propias instalaciones del negocio y sistemas de agua caliente

Esto se puede lograr trabajando en conjunto con una empresa de minería de Bitcoin que utilice las instalaciones del negocio para minar Bitcoin con fines de lucro y proporcione el calor para uso general, o

el propio negocio podría realizar esta función para construir directamente una tesorería de Bitcoin. Este enfoque también puede ayudar a la empresa con cualquier iniciativa ESG.

Un método más indirecto para obtener algunos de estos beneficios puede lograrse trasladando los requerimientos de computación a centros de datos que adopten este enfoque y ofrezcan espacio en racks o infraestructura como parte de un servicio gestionado, y que transfieran parte de estos ahorros de costos al negocio.

Como líder de TI, mantenerse al tanto de esta área le ayudará a proporcionar orientación a la empresa en la adopción de soluciones que puedan beneficiar al negocio.

##### Bitcoin e IA

Se espera que el uso de IA y ML crezca sustancialmente en los próximos años. La intersección de Bitcoin e Inteligencia Artificial está liderando una nueva era de innovación digital, destacada particularmente por la integración de la IA con la Lightning Network de Bitcoin. Esta unión está preparada para revolucionar aspectos de Internet, desde micropagos hasta agentes económicos en línea impulsados por IA.

* El ajuste fino de modelos de IA es un paso esencial en el desarrollo de la inteligencia artificial: los micropagos usando Lightning pueden permitir que personas de todo el mundo sean remuneradas por tarea en Bitcoin, fomentando la participación.
* En escenarios donde entidades de IA realizan transacciones por servicios, la red Lightning es una herramienta indispensable para actividades económicas impulsadas por IA donde la velocidad es clave.
* Una vez desarrollado el sistema de IA, los micropagos podrían facilitar un modelo de pago por uso más equitativo, donde los usuarios solo pagan por los recursos de IA que utilizan.

Para cualquier empresa que considere el uso de IA, ya sea como un servicio que necesita pagar o en el desarrollo de su propia solución de IA, es importante entender cómo Bitcoin y Lightning se integran y aportan valor a cualquier solución.

Fuente:[https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/](https://www.forbes.com/sites/digital-assets/2023/12/08/ai-and-bitcoin--a-synergy-for-the-future/)

##### Nuevas opciones de pago minorista

Cualquier empresa que acepte pagos por servicios, ya sea directamente en tiendas físicas o en línea, podría beneficiarse de aceptar pagos en Bitcoin de las siguientes maneras:

* Aumento del tráfico y crecimiento del negocio al dirigirse a clientes que usan Bitcoin
* Comisiones de pago bajas o nulas
* Liquidación instantánea
* Sin contracargos

Desde una perspectiva contable, existen diferentes formas de gestionar el Bitcoin recibido, manteniéndolo como parte de la tesorería o convirtiéndolo directamente a moneda fiduciaria, o alguna combinación según lo acordado. Dependiendo del negocio, puede haber algunas implicaciones técnicas para lograr esto, como nuevos terminales POS o integración con una solución de software para pagos en línea, cuyo impacto técnico el líder de TI debe comprender si se acuerda como objetivo para la empresa.

##### Reducción de comisiones por transferencias FX globales

Para las empresas que transfieren grandes sumas de dinero a nivel global, los costos y la complejidad de hacerlo pueden ser un desafío. Se están ofreciendo en el mercado nuevas soluciones basadas en Bitcoin que reducen estos costos y proporcionan una liquidación más rápida e inmediata. Adoptar estos servicios podría ser beneficioso para el negocio, y comprender este mercado, los servicios ofrecidos y trabajar con el equipo de cuentas para implementar la mejor solución requiere un nivel de conocimiento técnico y comprensión que el líder de TI puede aportar.

##### Beneficios para empleados

La mayoría de las empresas están buscando cómo pueden ofrecer beneficios e incentivos a sus empleados para mejorar la contratación y la retención. Recientemente, varios atletas profesionales y políticos de alto perfil han anunciado que recibirán la totalidad o parte de sus salarios en Bitcoin. La capacidad de pagar partes del salario en Bitcoin será importante para los empleadores cuando esto marque la diferencia en contrataciones clave, o cuando miembros fundamentales del equipo empiecen a solicitar esta opción o busquen empleadores que la ofrezcan en otros lugares.

* Integrar la opción de compensación total o parcial en Bitcoin da a una organización una ventaja competitiva para adelantarse a la curva. Las soluciones de nómina en Bitcoin hacen que integrar este proceso sea sencillo.
* Empresas como MicroStrategy están buscando formas de incentivar el rendimiento o incluso la asistencia a reuniones con micropagos basados en Lightning.

Aunque la decisión de implementar tales beneficios para los empleados no recae directamente en el líder de TI, sí puede ser su responsabilidad proporcionar una comprensión de por qué esto podría ser beneficioso, las soluciones disponibles para lograrlo y las implicaciones técnicas de la implementación. Los directores de TI que proactivamente proponen ideas a sus pares pueden demostrar su valor estratégico más amplio para la empresa.

##### Nuevas oportunidades de mercado

Como dijo la cita de Google, muchas empresas buscarán construir nuevas fuentes de ingresos basadas en el creciente ecosistema de Bitcoin. Esto puede abrir nuevos mercados para que la empresa los considere, y el líder de TI puede ser fundamental en la evaluación de la idoneidad, los desafíos técnicos y las oportunidades potenciales que puedan ofrecer.



#### 5.1.3 Resumen

Se espera que Bitcoin continúe su camino de adopción, volviéndose cada vez más importante para las empresas con el tiempo, afectando tanto las estrategias empresariales como técnicas e iniciativas en varias áreas. Como líder técnico de la empresa, el líder de TI se beneficiará al adelantarse a estos desarrollos, proporcionando orientación a la empresa y asegurando que obtenga el mayor beneficio de la implementación de soluciones de Bitcoin en toda la organización.
