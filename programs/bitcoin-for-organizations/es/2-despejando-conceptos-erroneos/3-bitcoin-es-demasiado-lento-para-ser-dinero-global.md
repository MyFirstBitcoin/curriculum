# 2.3 Bitcoin es demasiado lento para ser dinero global.

> Los visionarios ven un futuro de trabajadores que teletrabajan, bibliotecas interactivas y aulas multimedia. Hablan de reuniones municipales electrónicas y comunidades virtuales... La verdad es que ninguna base de datos en línea reemplazará tu periódico diario, ningún CD-ROM puede sustituir a un maestro competente y ninguna red informática cambiará la forma en que funciona el gobierno.  
_Clifford Stroll_

17 años después, Newsweek dejó de publicarse en papel y pasó a estar disponible exclusivamente en línea. Imagina estar vivo en 1974 cuando se creó por primera vez el Protocolo de Control de Transmisión (TCP).

Nadie previó el teléfono inteligente, con todas sus aplicaciones, en la palma de tu mano. Nadie imaginó el sistema de navegación por satélite en tu coche.

Internet no surgió de una sola vez, sino gradualmente como una evolución de protocolos y capas. Estas evoluciones se han construido sobre TCP, pero en su mayoría no lo han cambiado.

> Así que, al considerar la transición hacia las plataformas de comunicación del futuro, veo que la belleza de los protocolos de Internet es que permiten la separación de las capas entre el servicio y la tecnología.  
_Michael K Powell_



##### Compara la evolución de Bitcoin con la de Internet

TCP fue necesario pero no suficiente para la aparición de todo lo demás en Internet. La evolución de Bitcoin parece estar siguiendo un camino similar. Los sistemas abiertos parecen ser más resilientes y exitosos cuando se desarrollan en capas, aunque puede pasar mucho tiempo entre la colocación de los bloques iniciales y la adopción generalizada. Las soluciones todo en uno no parecen ser tan efectivas en sistemas abiertos como aquellas construidas en capas sobre protocolos. Así como nadie ha necesitado reconstruir Internet porque no se podían transmitir películas usando TCP, es probable que ocurra lo mismo con Bitcoin.

Ya existen varios protocolos de capa 2 sobre Bitcoin, y hay muchas aplicaciones que funcionan sobre estos protocolos de capa 2 (ver la sección 201.4 para más detalles sobre estos).

En lugar de enfocarte en lo que bitcoin y la red de Bitcoin no pueden hacer hoy, piensa en lo que ya se puede hacer hoy y compáralo con lo que podía hacer hace 10 años. Haz este ejercicio con Internet desde 1985 hasta 1995, y luego observa lo mucho más rápido que se volvió Internet en los siguientes 30 años y las aplicaciones que se hicieron posibles. Usa esa perspectiva para proyectar Bitcoin hacia adelante e imagina cómo podría ser en solo otros 10 años, o 30 si tu imaginación puede llegar tan lejos.



##### Compara Bitcoin con el sistema monetario global existente

La afirmación central de que Bitcoin es demasiado lento para ser dinero global es discutiblemente cierta si nos restringimos a la capa base de Bitcoin. También es cierto que la capa base de nuestros sistemas monetarios actuales es demasiado lenta para ser dinero global, si una restricción similar significara que no existiera infraestructura de pagos construida sobre ella por bancos privados y servicios de pago como Visa y Mastercard. Nuestro sistema actual está construido en capas, por lo que podríamos esperar que el futuro sea similar. Algunos compromisos de diseño, como entre confianza, velocidad y costo, pueden trasladarse entre sistemas que ofrecen las mismas soluciones, aunque estén construidos para mover diferentes tipos de valor.

Algunas de las capas 2 existentes en Bitcoin abordan directamente el problema de la velocidad, por ejemplo Liquid y la Lightning Network (ver la sección 201.4 para más detalles). Liquid es más rápida y barata que la blockchain de Bitcoin, y la Lightning Network es aún más rápida y barata que Liquid. Se espera una proliferación de capas 2, cada una con diferentes compromisos, y esto es saludable.

Probablemente habrá más capas 2 y 3 y una explosión de aplicaciones que las utilicen, tal como ocurrió con la evolución de Internet.



##### Motivación

Cuando surge esta crítica, vale la pena considerar si el crítico tiene otras motivaciones. Por ejemplo, ¿tienen un proyecto de blockchain nuevo o diferente? Esto puede ser análogo a intentar vender un Protocolo de Control de Transmisión mejorado.

El Trilema de la Escalabilidad, o de la Blockchain, fue planteado por primera vez por Vitalik Buterin en 2017. Afirma que siempre hay un compromiso en el diseño de blockchain entre las propiedades de descentralización, seguridad y escalabilidad. Cualquiera que critique que Bitcoin es demasiado lento y que tiene una solución más rápida en una blockchain de capa 1 estará sacrificando algo de seguridad o descentralización para lograrlo. Aunque tal compromiso puede tener sentido para una blockchain diseñada para otros usos, el orden de prioridad para un dinero global debe ser:


> **Note**
>
> * **Descentralización**
>   * Hace posible eliminar a las partes de confianza
> * **Seguridad**
>   * Impide que actores malintencionados manipulen las transacciones o el libro mayor
> * **Escalabilidad**
>   * Permite que el sistema escale económicamente en usuarios y velocidad


Las dos primeras características crean el entorno para la emisión sin creadores, pagos sin intermediarios y custodia sin gestores.

Bitcoin realiza el compromiso correcto entre las tres características de diseño de blockchain, dado que su caso de uso objetivo es como dinero global, y mitiga los compromisos de escalabilidad y velocidad utilizando capas.

> Satoshi descubrió cómo proteger la integridad del dinero digital sin partes de confianza: no se necesitan creadores, intermediarios ni gestores.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
