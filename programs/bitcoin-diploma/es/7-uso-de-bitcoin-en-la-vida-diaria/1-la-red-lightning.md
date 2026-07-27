# 7.1 La red Lightning

Lightning Network es un sistema de pagos que permite a los usuarios enviar y recibir bitcoin de forma rápida y económica. Funciona creando una billetera compartida donde ambas partes guardan parte de sus bitcoin. Luego pueden realizar transacciones ilimitadas entre sí sin necesidad de registrar cada una en la blockchain principal. Al hacerlo, evitan la necesidad de verificar e incluir cada transacción individual en un bloque, lo que hace que el proceso sea rápido y rentable. Las comisiones más bajas significan que Lightning Network puede usarse para pagos pequeños que no siempre son viables en cadena. Una vez que las partes deciden poner fin a su colaboración, solo el saldo final se registra en la blockchain.

Imagina un día trabajando en un café. Como planeas quedarte un buen rato, abres una cuenta y pagas por adelantado en lugar de pagar cada pedido. Al final del día, tú y el dueño revisan la cuenta para saldar lo adeudado. Si tu depósito es mayor que lo que gastaste, te devuelven la diferencia; si gastaste más, pagas lo que aún debes.

Este esquema puede escalar para incluir a más participantes. Por ejemplo, en una de tus visitas al café, llevas a un amigo a quien el barista no conoce y no puede abrirle una cuenta. Le ofreces a tu amigo usar tu cuenta existente para cubrir sus gastos y acuerdan que te lo pagará en privado. Ahora imagina a miles de personas haciendo lo mismo simultáneamente, permitiendo que otros usen cuentas existentes para conectarse con aún más personas: ¡así es como funciona Lightning Network!

Con Lightning, puedes hacer pagos a cualquier persona de la red, no solo a la persona con la que compartes una cuenta directa, siempre que se pueda encontrar una ruta entre ambas partes. Tu pago puede navegar por la red hasta llegar a su destino, incluso si no tienes un canal abierto directamente con el destinatario.

Veamos la diferencia entre las transacciones en cadena y fuera de cadena.

##### Transacciones en cadena

Estas son transacciones que ocurren directamente en la blockchain de Bitcoin. Tardan unos 10 minutos en confirmarse, y las comisiones dependen del tamaño de la transacción en bytes virtuales. Son más seguras, pero más lentas, ya que requieren el consenso de la red.

##### Transacciones de Lightning Network

Estas transacciones ocurren en una red separada construida sobre la blockchain de Bitcoin. Se liquidan más rápido y con comisiones más bajas. Se usan comúnmente cuando consideraciones como la velocidad y el costo de las transacciones son más importantes. En comparación con las transacciones en cadena, son menos seguras.


|  | Red Bitcoin | Lightning Network |
| --- | --- | --- |
| Definición | Una red digital descentralizada que utiliza criptografía para asegurar transacciones financieras. | Un protocolo de pagos de segunda capa que opera sobre la blockchain de Bitcoin y permite transacciones más rápidas y baratas. |
| Ventajas | Descentralizada y segura. Sin contracargos ni fraude. Puede usarse de forma seudónima. Aceptación global. | Transacciones más rápidas y baratas. Mayor escalabilidad. Las transacciones fuera de cadena no congestionan la blockchain. |
| Desventajas | Tiempos de transacción lentos. Comisiones altas para ciertos tipos de transacciones. Compleja para principiantes. | Puede requerir confiar en los operadores de canales. Requiere una transacción en cadena para abrir y cerrar canales. |
