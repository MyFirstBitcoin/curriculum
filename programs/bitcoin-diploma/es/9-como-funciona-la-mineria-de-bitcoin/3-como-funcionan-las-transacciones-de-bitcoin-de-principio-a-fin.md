# 9.3 Cómo funcionan las transacciones de Bitcoin de principio a fin

Ahora que entiendes las claves públicas y privadas, así como el papel de los nodos y los mineros, así es como funciona una transacción de Bitcoin de principio a fin.

1. Adam quiere enviar bitcoin a Gerardo. Crea una transacción con la dirección de Gerardo, la cantidad a enviar y una tarifa.
1. Adam firma la transacción con su clave privada para demostrar la propiedad.
1. Transmite la transacción a la red de Bitcoin.
1. Los nodos la reciben y verifican que cumpla con las reglas, incluyendo la verificación de la firma y que Adam tenga suficiente bitcoin.
1. Si es válida, la transacción se comparte en toda la red y se agrega al mempool, donde esperan las transacciones pendientes.
1. Los mineros seleccionan transacciones del mempool y las incluyen en un bloque que intentan minar.
1. Cuando un minero mina un bloque con éxito, lo comparte con la red y otros nodos lo verifican.
1. Si es válido, el bloque se añade a la cadena de bloques. Gerardo recibe el bitcoin.
1. A medida que se agregan más bloques, la transacción obtiene más confirmaciones, lo que la hace más segura.

Una vez incluida en un bloque, la transacción queda confirmada. Adam no puede volver a gastar ese bitcoin, y Gerardo puede gastar lo que recibió en una nueva transacción.


> **Note**
>
> Transacción y tarifa seleccionada → Firmada por la billetera y enviada → Distribuida por nodos → El minero añade la transacción al bloque → El minero gana el concurso de Prueba de trabajo → El nuevo bloque es validado → El nuevo bloque es distribuido por nodos


###### Recursos


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
