# 3.1 El desarrollo de TCP/IP

La mayoría de nosotros estamos familiarizados con los protocolos TCP/IP que se utilizan hoy en día como la base de internet. Sus orígenes se remontan a finales de los años 70, cuando los científicos exploraban diseños alternativos a Arpanet, una red aún más antigua concebida por el Departamento de Defensa de EE. UU. para permitir el intercambio de recursos entre computadoras remotas. TCP/IP se convirtió en el estándar de protocolo para Arpanet en 1983, lo que llevó a que se convirtiera en el modelo de red dominante a finales de los años 90 y en la base de internet sobre la que funciona Bitcoin hoy en día.


| Modelo OSI | TCP/IP |
| --- | --- |
| Aplicación | Aplicación |
| Presentación | Aplicación |
| Sesión | Aplicación |
| Transporte | Transporte |
| Red | Red |
| Enlace de datos | Enlace de datos |
| Físico | Físico |


Al mismo tiempo que se desarrollaba el modelo TCP/IP, la Organización Internacional de Normalización (ISO) y la industria de las telecomunicaciones (CCITT) estaban desarrollando un marco similar pero más completo. El proceso para desarrollar nuevos protocolos o sugerir cambios era lento y poco manejable en comparación con el enfoque más descentralizado utilizado para desarrollar TCP/IP, lo que llevó a la dominancia de este último enfoque hoy en día.

##### Solicitud de Cambio

Cualquier desarrollo sugerido a los protocolos existentes o ideas para nuevos pueden ser propuestos en el modelo TCP/IP a través de una **Solicitud de Cambio** . Estas pasan por un proceso de aprobación, gestionado por el Grupo de Trabajo de Ingeniería de Internet (IETF), y se vuelven de código abierto una vez aprobadas para permitir que cualquiera las implemente y adopte. Algunos ejemplos destacados:

* 1969 RFC 1 Documentó cómo se enviarían los paquetes en Arpanet
* 1981 RFC791 definió el protocolo de Internet V4 – aún ampliamente adoptado hoy en día
* 1982 RFC 821 Protocolo simple de transferencia de correo
* 1987 Sistema de Nombres de Dominio – cómo los nombres de dominio se resuelven a direcciones IP
* 1999 RFC 2616 Protocolo de transferencia de hipertexto – esencial para navegar por la web


> **Callout**
>
> La **Propuesta de Mejora de Bitcoin** (BIP) sigue un enfoque similar al RFC, pero enfocado únicamente en mejoras para Bitcoin en sí mismo en lugar del desarrollo de nuevos o alternativos protocolos. Bitcoin también toma prestado de este modelo por capas, y verás protocolos adicionales descritos como capa dos o tres.


De la misma manera que las capas base del modelo TCP/IP han cambiado relativamente poco en las últimas décadas, con la innovación ocurriendo en capas superiores, se espera que la capa base de Bitcoin cambie muy lentamente en este punto, con soluciones de escalabilidad como Lightning y Liquid ocurriendo por encima.

Un buen ejemplo de cómo los protocolos de capa base se vuelven difíciles de cambiar con el tiempo es IPv6. El agotamiento esperado del espacio de direcciones en IPv4 creó la demanda de un nuevo protocolo. El primer borrador del estándar se creó en 1998, pero no fue ratificado como estándar de internet hasta 2017. Aunque resolvió muchos problemas de IPv4 y es mucho más preparado para el futuro, aún ha visto una adopción muy lenta en la industria hoy en día. Durante este tiempo, se han definido muchos nuevos protocolos en las capas superiores para habilitar multimedia, correo electrónico, etc.

##### Los bloques de construcción utilizados por Bitcoin

Esta separación de los problemas de interconectividad permite que los protocolos se desarrollen de forma independiente de las capas superiores e inferiores. En lugar de tener que reinventar soluciones para cada capa, Bitcoin como red puede confiar en las capacidades subyacentes de la red proporcionadas en las capas física y de enlace de datos.


| Capa | TCP/IP Original |
| --- | --- |
| Aplicación | Utiliza el Sistema de Nombres de Dominio (DNS) para identificar nodos vecinos. El puerto 8333 señala el protocolo Bitcoin. |
| Transporte | UDP para comunicaciones FIBRE entre mineros para baja latencia. TCP para comunicaciones P2P entre nodos. |
| Transporte | Enrutamiento TOR: Permite anonimato y privacidad. Protocolo de difusión: Rutea el tráfico a través de la red. |
| Enlace | Opera sobre cualquier medio (por ejemplo, Ethernet, Wi-Fi, etc.) |
| Físico | Transmisión física vía inalámbrica, Ethernet u otras interfaces de hardware. |


##### Bitcoin es un protocolo neutral para transferir valor, así como HTTPS es un protocolo para transferir información

* **HTTPS**: Sitios web seguros
* **SMTP**: Enviar correos electrónicos
* **FTP**: Transferir archivos
* **DNS**: Gestionar nombres de dominio
* **BTC**: Almacenar y transferir valor

Bitcoin permite transportar valor de manera confiable y sin requerir un tercero entre personas o dispositivos a través de Internet. Se espera que esto libere un valor tremendo.
