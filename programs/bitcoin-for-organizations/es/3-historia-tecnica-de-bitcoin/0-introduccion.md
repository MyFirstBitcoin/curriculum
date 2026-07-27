# 3.0 Introducción

> **Dark – Resumen del White Paper de Bitcoin**
>
> **Una versión puramente entre pares de dinero electrónico** permitiría que los pagos en línea se envíen directamente de una parte a otra sin pasar por una institución financiera. **Las firmas digitales proporcionan parte de la solución**, pero los principales beneficios se pierden si todavía se requiere una **tercera parte confiable** para evitar el doble gasto. Proponemos una solución al problema del doble gasto utilizando una **red entre pares**. La **red sella las transacciones con marcas de tiempo** al incluirlas en una cadena continua de **prueba de trabajo basada en hash,** formando un registro que no puede ser modificado sin rehacer la **prueba de trabajo**. La cadena más larga no solo sirve como prueba de la secuencia de eventos presenciados, sino también como prueba de que proviene del mayor grupo de poder de CPU. Mientras la mayoría del poder de CPU esté controlado por nodos que no cooperan para atacar la red, ellos generarán la cadena más larga y superarán a los atacantes. **La propia red requiere una estructura mínima. Los mensajes se transmiten con el mejor esfuerzo posible, y los nodos pueden salir y volver a unirse a la red cuando lo deseen**, aceptando la cadena de prueba de trabajo más larga como prueba de lo que ocurrió mientras estaban ausentes.


Bitcoin no apareció en un vacío, sino que se construyó sobre el trabajo de muchos en las décadas anteriores. Este módulo explorará los fundamentos de internet sobre los que se apoya Bitcoin, así como la investigación y el desarrollo reconocidos en el whitepaper.

En los años 70, un grupo de personas observó cómo el gobierno de los Estados Unidos, en particular, intentaba restringir el acceso a la criptografía, y se propuso asegurar que esta tecnología estuviera disponible para todas las personas para proteger su privacidad en línea. Algunos de estos primeros pioneros también se enfocaron en los posibles beneficios de un sistema digital de 'dinero sólido' que pudiera usarse para almacenar e intercambiar valor a través del incipiente internet. Friedrich Hayek, un destacado contribuyente a la economía austriaca, imaginó cómo sería una moneda ideal basada en la competencia del libre mercado mucho antes de la era de internet, pero consideró que era técnica y políticamente inviable. Además de la privacidad digital, este grupo, que evolucionó hasta convertirse en los Cypherpunks, intentó hacer realidad la visión de Hayek para el dinero digital, pero estos intentos fracasaron hasta que Satoshi publicó sus ideas en la lista de correo.

* Protocolo TCP/IP (1976)
* Protocolos para Criptosistemas de Clave Pública - Ralph Merkle (1980)
* Digicash - David Chaum (1989)
* Sellado digital de tiempo (años 90)
* Hashcash - Adam Back (1997)
* BitTorrent - Bram Cohen (2001)
* POW reutilizable - Hal Finney (2004)
* Whitepaper de Bitcoin - Satoshi Nakamoto (2008)

Una influencia clave en el desarrollo de Bitcoin fue la aparición de este movimiento Cypherpunk en los años 90. Desarrollaron varias tecnologías criptográficas, incluida la criptografía de clave pública, para permitir a los usuarios comunicarse y compartir información de forma segura y privada. Muchos de los desarrollos aquí descritos y las personas involucradas formaban parte de este grupo.

También se identificó la necesidad de dinero digital y se hicieron varios intentos para crearlo, pero estos tenían limitaciones que les impidieron tener éxito. El genio de Satoshi Nakamoto fue reunir estas capacidades y, junto con algunas innovaciones propias, construir sobre ellas para crear el protocolo de Bitcoin que se utiliza hoy en día. En las siguientes secciones exploraremos algunos de estos desarrollos y explicaremos cómo ayudaron a informar el diseño de Bitcoin. También discutiremos cuáles eran las piezas faltantes del rompecabezas que Satoshi logró resolver.
