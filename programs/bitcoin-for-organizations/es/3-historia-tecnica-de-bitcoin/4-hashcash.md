# 3.4 Hashcash

Hashcash fue creado por Adam Back, otro de los primeros innovadores en este ámbito. Adam tenía un gran interés en los mercados libres y la privacidad en internet, y se topó con la lista de correo de los Cypherpunks, a la que se unió y de la que se convirtió en un participante activo.

Estaba muy interesado en el dinero digital, e hizo algunas sugerencias sobre cómo el grupo podría trabajar más estrechamente en DigiCash con Chaum, pero estas no llegaron a nada. Luego centró su atención en otro problema emergente: el spam de correo electrónico. Él y el resto de los Cypherpunks querían encontrar una solución al problema del spam, donde era trivial para los spammers crear y enviar miles de correos electrónicos que saturaban las redes. Su solución innovadora se basó en el hashing: la capacidad, mediante criptografía, de convertir cualquier dato en una cadena única y aleatoria de una longitud específica, para crear el equivalente a un ‘sello’ digital que debía añadirse al correo electrónico para que se considerara válido y pudiera transmitirse por la red. Un coste trivial para un correo legítimo, pero prohibitivo para un spammer.

La innovación clave que creó Hashcash fue vincular recursos del mundo real —el poder computacional— a una red digital. Mientras que los recursos digitales hasta ese momento podían replicarse sin límites, la cantidad de ‘hashcash’ creada estaba limitada por cuánta energía estuvieran dispuestas las personas a invertir en ello.

Aunque la solución cumplía con algunos de los criterios que Adam creía necesarios en un sistema de dinero digital; era anónima, resistente y sin necesidad de confianza, cada hashcash no era reutilizable ni verdaderamente escaso. Sugirió otras formas en que estos problemas podrían abordarse utilizando terceros externos.

##### BitGold

Nick Szabo desarrolló el concepto de Hashcash y la prueba de trabajo para proponer una solución alternativa, que describió en una lista de correo un año después de que se publicara Hashcash, en 1998.

Aunque se acercaba más a una solución, esta propuesta aún presentaba varios desafíos.

* ¿Quién gestionaría el Registro de propiedad de los hashes y cómo se podría confiar en ellos?
* El hashing generalmente se volvería más barato con el tiempo, un desafío también para HashCash.

Como los hashes enlazados estarían sellados en el tiempo, propuso alguna forma de seguimiento histórico de la dificultad del hashing en ese momento; un hash anterior requeriría más costes de procesamiento que uno posterior, ya que los costes han disminuido. Desafortunadamente, esto significaba que los hashes no serían ‘fungibles’, es decir, de igual valor, considerado un atributo clave del dinero digital. Para ayudar a resolver esto, Nick sugirió alguna forma de ‘banca libre’ funcionando sobre BitGold que pudiera agrupar diferentes grupos de hashes que serían valorados de la misma manera.

##### B-Money

Poco después de la propuesta de Bit Gold, Wei Dai propuso una solución similar. Ya había desarrollado varias otras herramientas para los Cypherpunks, y tenía sus propias ideas sobre el dinero digital.

Su propuesta se parecía a Bit Gold en que utilizaba firmas digitales para transferir dinero, y los registros de las transacciones se almacenarían en un libro mayor, que contenía claves públicas y la cantidad de unidades de moneda atribuidas a cada una. Al igual que en Bit-Gold, los terceros de confianza se consideraban vulnerabilidades de seguridad, y se creía que un sistema de dinero electrónico no debía depender de una sola entidad para rastrear saldos, transacciones o para evitar el doble gasto.

Wei-Dai propuso varias soluciones a estos problemas, una de las cuales era que, en lugar de que una entidad central (o varias) mantuviera el libro mayor, TODOS los nodos mantendrían una copia. Si todos los usuarios verificaban su propio libro mayor y la validez de cada transacción, mientras todos los nodos se mantuvieran actualizados, los libros mayores deberían permanecer sincronizados en toda la red. Este sistema altamente distribuido sería difícil de corromper.

Wei Dai reconoció que esto no resolvía el problema de los generales bizantinos (1), ya que los nodos podían perder la sincronización fácilmente o simplemente mentir. Sugirió métodos alternativos, como tener un subconjunto de servidores ‘de confianza’ que mantuvieran el libro mayor, y crear incentivos financieros para mantener honestos a estos servidores.

Para la política monetaria, propuso vincular el poder adquisitivo de B-Money a algún tipo de índice de precios al consumidor externo. Quería que la misma cantidad de B-Money pudiera comprar una parte igual del índice a lo largo del tiempo, proporcionando cierta estabilidad de precios. Así, cualquiera podría generar nuevas unidades de moneda proporcionando un hash válido, pero la dificultad de generar un hash podría cambiar con el tiempo según los costes de CPU y el índice de precios, de modo que cada unidad sería ‘inmutable’.
