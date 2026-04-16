# 7.1 La Red Lightning

La red Lightning es un sistema de pago que permite a los usuarios enviar y recibir pagos de forma rápida y económica utilizando bitcoin. Funciona creando un monedero compartido en el que ambas personas almacenan sus bitcoins y luego realizan transacciones ilimitadas entre sí sin necesidad de registrar cada una en la blockchain principal. De este modo, se evita la necesidad de verificar e incluir cada transacción individual en un bloque, lo que hace que el proceso sea rápido y rentable. Las tarifas más bajas permiten que la red Lightning se utilice para pagos pequeños que no siempre son viables en la cadena principal. Cuando las partes deciden finalizar su colaboración, solo el saldo final se registra en la blockchain.

Imagina un día en el que trabajas en una cafetería. Planeando quedarte un buen rato, abres una cuenta y pagas por adelantado en lugar de pagar cada vez que haces un pedido. Al final del día, tú y el dueño revisan la cuenta para liquidar la factura. Si tu depósito es mayor que lo que consumiste, te devuelven la diferencia; si gastaste más, pagas lo que aún debes.

Este esquema puede ampliarse para incluir a más participantes. Por ejemplo, en una de tus visitas a la cafetería, llevas a un amigo que el camarero no conoce y no puede abrir una cuenta. Tú le ofreces a tu amigo usar tu cuenta existente para cubrir sus gastos y acuerdan que él te pagará después en privado. Ahora imagina a miles de personas haciendo lo mismo simultáneamente, permitiendo que otros utilicen cuentas existentes para conectarse con aún más personas: ¡así es como funciona la Red Lightning!

Con Lightning, puedes hacer pagos a cualquier persona en la red, no solo a la persona con la que compartes una cuenta directa, siempre que exista una ruta entre ambas partes. Tu pago puede navegar a través de la red hasta llegar a su destino, incluso si no tienes un canal abierto directamente con el destinatario.

Echemos un vistazo a la diferencia entre las transacciones en cadena y las transacciones fuera de cadena.

##### Transacciones en cadena

Estas son transacciones que ocurren directamente en la cadena de bloques de Bitcoin. Tardan unos 10 minutos en confirmarse y las tarifas dependen del tamaño de la transacción en bytes virtuales. Son más seguras pero más lentas, ya que requieren el consenso de la red.

##### Transacciones en la Red Lightning

Estas transacciones ocurren en una red separada construida sobre la cadena de bloques de Bitcoin. Se liquidan más rápido y con tarifas más bajas. Se utilizan comúnmente cuando la velocidad y el costo de las transacciones son más importantes. En comparación con las transacciones en cadena, son menos seguras.


|  | Red de Bitcoin | Red Lightning |
| --- | --- | --- |
| Definición | Una red digital descentralizada que utiliza criptografía para asegurar las transacciones financieras. | Un protocolo de pagos de segunda capa que opera sobre la cadena de bloques de Bitcoin, permitiendo transacciones más rápidas y económicas. |
| Ventajas | Descentralizada y segura. Sin contracargos ni fraudes. Puede usarse de forma seudónima. Aceptación global. | Transacciones más rápidas y económicas. Mayor escalabilidad. Las transacciones fuera de cadena no congestionan la blockchain. |
| Desventajas | Tiempos de transacción lentos. Tarifas altas para ciertos tipos de transacciones. Complejo para principiantes. | Puede requerir confianza en los operadores de los canales. Requiere una transacción en cadena para abrir y cerrar canales. |
