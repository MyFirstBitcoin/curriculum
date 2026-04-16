# 2.4 No está ocurriendo innovación en Bitcoin.

> La creación de mil bosques está en una sola bellota.   
_Ralph Waldo Emerson_

Los críticos a menudo intentan afirmar que Bitcoin es una tecnología 'antigua' o 'muerta' porque no cambia el protocolo de la capa base tan frecuentemente como las blockchains competidoras. Esta afirmación ignora tanto las razones por las que los cambios en Bitcoin se adoptan lentamente como la cantidad de innovación que ocurre para escalar la red en capas superiores, como la Lightning Network. También ignora que muchas de nuestras tecnologías más flexibles y duraderas tampoco escalan rápidamente en la capa base.

Por ejemplo, tampoco hay innovación en el Protocolo de Control de Transmisión (TCP), que es la base de internet. TCP se creó por primera vez en 1974. La última vez que se actualizó TCP fue en 1982. Hace lo que necesita hacer. No es perfecto, y hay debates sobre si necesitamos actualizar IPv4 para soportar futuros desarrollos de internet. Sin embargo, decir que no ha habido innovación en internet desde 1982 sería una afirmación sorprendente. Toda esta innovación ha sido 'sobre' TCP, en lugar de 'dentro' de él.

La gran mayoría de la innovación que está ocurriendo no es 'dentro' de Bitcoin sino 'sobre' Bitcoin. Algún día probablemente no habrá innovación 'dentro' de Bitcoin, y eso debería ser un objetivo y no una crítica, ya que será un reflejo de lo fundamental que se ha vuelto para apoyar la economía global al proporcionar las bases para un dinero sólido global, neutral y sin permisos. Dinero que es sólido tanto en el sentido económico, ya que hay una oferta fija y un libro mayor inmutable, como también sólido en términos tecnológicos, ya que no cambia y lo que está funcionando ha tenido años de tiempo de actividad ininterrumpido. Bitcoin ya ha logrado un 100% de tiempo de actividad en los últimos 10 años.

Sin embargo, sería preocupante si no hubiera innovación 'sobre' Bitcoin. Veamos eso en los últimos 10 años:



#### 'Dentro' de Bitcoin

Segregated Witness (SegWit) se implementó en 2017 para proteger contra la maleabilidad de las transacciones y aumentar la capacidad de los bloques. SegWit también fue un precursor necesario para que Lightning y algunas cadenas laterales funcionaran eficientemente.

Taproot se implementó en 2021 para permitir el agrupamiento y la validación de múltiples firmas mediante la incorporación de firmas Schnorr, introduciendo un lenguaje de scripts para permitir una funcionalidad más compleja y aumentando la privacidad y la resistencia a la censura de las transacciones.



#### 'Sobre' Bitcoin

##### Cadena lateral Liquid

La cadena lateral Liquid se implementó en 2018. Liquid, como otras cadenas laterales, es un libro mayor de blockchain separado que está vinculado a la blockchain principal de Bitcoin, según un conjunto de reglas predefinidas. Estas reglas son lo suficientemente flexibles como para permitir que la cadena Liquid desarrolle e incorpore mejoras de diseño y escalabilidad con el tiempo. Sin embargo, el vínculo con la blockchain de Bitcoin garantiza que el límite total de suministro de 21 millones de bitcoin sea consistente en ambas cadenas.

El activo en Liquid, L-BTC, está vinculado en dos direcciones a bitcoin en la cadena principal. Hay compensaciones de costo, velocidad, privacidad y seguridad que hacen que L-BTC sea ideal para algunas aplicaciones. El costo, la velocidad y la privacidad mejoran con L-BTC, a costa de depositar cierta confianza en las organizaciones que conforman la Federación Liquid, que entre ellas controlan un proceso multisig de 11 de 15 para vincular y desvincular L-BTC a bitcoin y viceversa.

##### Lightning Network

La red Lightning se implementó en 2018. Lightning está diseñada para ser una red de pagos entre pares en forma de un grafo de nodos conectados mediante canales; no es una blockchain. El bitcoin es bloqueado por un operador de nodo en la blockchain principal para que esté disponible para su uso en la Lightning Network, lo que garantiza que solo se use bitcoin 'real'. Los nodos pueden entonces abrir canales de liquidez mediante contratos inteligentes multisig entre sí. Los pagos encuentran rutas a través de la red desde el origen hasta el destino, optimizando el costo según el requisito de que exista suficiente liquidez en la dirección correcta entre cada paso de nodo en la ruta. La Lightning Network mejora enormemente el costo, la velocidad y la privacidad a cambio de una pérdida de seguridad (o un aumento en la confianza requerida) y un aumento en la complejidad. Sin embargo, está destinada a pagos diarios de alto volumen y bajo valor, por lo que esto se considera una compensación muy razonable para sus millones de transacciones diarias (fuente: River, 2023).

##### Chaumian eCash Mints

Fedimints puede considerarse como una red Lightning limitada a una comunidad. Están diseñados para aprovechar la confianza inherente que existe dentro de ciertas comunidades (por ejemplo, familias, aldeas, grupos de amigos) a cambio de simplificar la complejidad y mejorar la privacidad para los usuarios. Son protocolos modulares y de código abierto para custodiar y transaccionar bitcoin en un contexto comunitario. Son interoperables con la propia Lightning Network.

**Cashu** es un token al portador que puede almacenarse en un dispositivo como un teléfono móvil; el diseño está orientado a reproducir los beneficios del dinero en efectivo físico pero en forma digital. Cashu es un ejemplo de Chaumian eCash construido sobre Bitcoin y aumenta la privacidad y la resistencia a la censura y reduce la complejidad a cambio de confiar en la casa de eCash que se utiliza. Las casas de Cashu emiten tokens de eCash, que representan bitcoin, que pueden ser gastados por los usuarios sin revelar su identidad. Cashu es interoperable con la Lightning Network.

Probablemente habrá muchas más aplicaciones de capa 2 construidas en el futuro, con muchas aplicaciones de capa 3 a su vez construidas sobre cada una de ellas.

Como ejemplo de la increíble cantidad de aplicaciones que se están construyendo sobre Lightning, aquí hay un extracto de un Informe de Investigación de Lightning Network realizado por River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
