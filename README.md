# Web3_M1S2

# Fundamentos de blockchain y Ethereum 

>#### ¡Hola, futuro desarrollador de blockchain! En este primer segmento de la semana, vamos a sumergirnos en los fundamentos de esta tecnología. A continuación te presentamos el indice y contenido de la semana 2.

# Tabla de contenido

1. Fundamentos de blockchain y Ethereum
     1. Fundamentos de la tecnología blockchain
     2. Ethereum y smart contracts
     3. Fundamentos de Ethereum

# i. Fundamentos de la tecnología blockchain 
Iniciemos planteandonos algunas preguntas clave como las siguientes:

**¿Que es Blockchain?**
La blockchain, o cadena de bloques, es una tecnología que permite la transferencia de datos con una encriptación muy sofisticada y de una manera completamente segura. Imagina una enorme hoja de Excel que se copia, se pega y se asegura con encriptación en una red de computadoras y se actualiza de manera constante. En esencia, esto es blockchain.

**¿Y por qué es tan importante?** 
Blockchain es la tecnología subyacente a criptomonedas como bitcoin y ethereum, pero sus aplicaciones van más allá. Puede ser utilizada para cualquier tipo de transacción que involucre valor: bienes inmuebles, productos, servicios e incluso, votos en una elección.
Te dejamos un video que te dará una explicación más detallada: https://www.youtube.com/watch?v=V9Kr2SujqHw&t=3s  (23:19)

### Ponte a prueba - Blockchain

Ahora que sabes el valor agregado de bitcoin, te proponemos una pequeña actividad práctica.

Visita https://blockexplorer.com . Allí podrás ver en tiempo real cómo se forman los bloques en una blockchain y cómo se añaden a la cadena existente.
Para referencias adicionales, te recomiendo el libro [Mastering Blockchain](https://www.amazon.com.mx/Mastering-Blockchain-Second-Imran-Bashir/dp/1788839048), de Imran Bashir. Es un recurso muy completo para entender los detalles técnicos detrás de blockchain (I. Bashir, 2017, Mastering Blockchain. Packt Publishing). 

Continuemos analizando los elementos fundamentales que componen una blockchain.

**Transacciones**

Las transacciones en la blockchain son acciones que se registran en la cadena de bloques. En términos simples, una transacción representa una transferencia de datos de un usuario a otro en la red de blockchain. Por ejemplo, en el caso de las criptomonedas, una transacción representa una transferencia de la criptomoneda entre los usuarios de la red de blockchain. En escenarios de negocio a negocio, una transacción podría ser una forma de registrar actividades que ocurren en activos digitales o físicos. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Cada bloque en una blockchain puede contener cero o más transacciones. Para algunas implementaciones de blockchain, un suministro constante de nuevos bloques (incluso con cero transacciones) es crítico. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Las transacciones se añaden a la blockchain cuando un «nodo publicador» publica un bloque. Éste contiene un encabezado de bloque y datos de bloque. El encabezado contiene metadatos para este bloque. Los datos contienen una lista de transacciones validadas y auténticas que se han enviado a la red de blockchain. La validez y autenticidad se asegura comprobando que la transacción es correcta. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Un aspecto crítico de la tecnología blockchain es cómo los participantes acuerdan que una transacción es válida. Esto se llama «alcanzar el consenso», y hay muchos modelos para hacerlo, cada uno con ventajas y desventajas para casos de negocio particulares. NIST (2018), p7. Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Es importante destacar que, bajo la operación normal de la red de blockchain, ninguna transacción puede ser cambiada una vez publicada. Esto se debe a que los bloques y transacciones posteriores actúan como actualizaciones o modificaciones a los bloques y transacciones anteriores, asegurando que los datos de la blockchain no puedan ser alterados. Esta abstracción de software permite modificaciones a los datos de trabajo, mientras proporciona un historial completo de cambios. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Para entender mejor el concepto de las transacciones en una red blockchain, puedes acceder al siguiente demo enfocado solamente en transacciones:

https://coindemo.io/

### Ponte a prueba - Transacciones

Te invito a que realices los siguientes pasos:

1. Dar clic en el botón MINE NEW BLOCK. En este paso te pondrás en los zapatos de un minero con el nombre de Satoshi. Los mineros son los encargados de «minar» o confirmar un bloque con diferentes transacciones. Cada vez que se hace este proceso de minado, la red recompensa al minero con cierta cantidad del mismo token o moneda de la red en la que se está trabajando. En este caso, el minero será recompensado con 100 monedas. A estas recompensas se les conoce como «recompensas de bloque». En esta demo se mina el primer bloque de la red, después del «bloque génesis».
 
Puedes aprender mas sobre el bloque génesis aquí: https://academy.bit2me.com/que-es-bloque-genesis/

2. Confirmación de registro en la red. En este paso visualizarás cómo las recompensas de 100 monedas también son registradas en la misma red blockchain. Estas recompensas pasan a aportar liquidez a la red, siendo decisión del minero qué hacer con las mismas, ya sea mantenerlas, transferirlas, venderlas, hacer staking, etcétera. Estas «recompensas de bloque» son registradas en el mismo bloque que el minero «mina», siendo estas las primeras transacciones de cada bloque (un bloque contiene múltiples transacciones). A estas transacciones de carácter especial se les llama «transacción de coinbase».

Puedes aprender sobre transacciones coinbase aquí: https://economia3.com/comisiones-coinbase-cuales-son/

3. Salidas de transacciones. Una transacción normalmente consta de una o varias entradas y de una o varias salidas. A estas se les llama UTXOs por sus siglas en inglés (Unspent Transaction Output) y son los elementos en las transacciones que permiten que blockchain dé solución a uno de los principales problemas que el dinero digital tenía: el doble gasto. Este es el problema que tiene una moneda digital al ser duplicada y usada más de una vez. Pues bien, las UTXOs sirven para evitar este problema.

Si quieres indagar más acerca de las UTXOs, puedes encontrar información adicional en este enlace: https://academy.bit2me.com/que-es-una-utxo/

Por ahora solo hace falta entender que son un mecanismo para asegurar el correcto funcionamiento de la red.

Por tanto, y volviendo a la demo, estas UTXOs son representadas con la salida de 100 monedas que Satoshi posee con la etiqueta «unspent», ya que aún no han sido utilizadas. Recuerda que, en esta demo, Satoshi es quien paga a los mineros, representados por un peer en la demo. Este se encarga de minar un bloque y al hacer esto se le hará una transacción con las recompensas desde Satoshi.

NOTA: El peer puede adquirir diferentes nombres en la demo, como «Rita», «Earl», etcétera.

Una vez que se ejecuta todo este proceso, podemos ver que en el Balance se tienen 100 monedas. Con el importe de este balance podremos crear nuevas transacciones. 
En el paso de «create transaction» podemos seleccionar a algún participante de la red (peer), ya que a este se le pagará por haber minado este bloque. Por tanto, seleccionamos el peer deseado, el fee que obtendrá por minar y los inputs de las transacciones (100 monedas por recompensas de bloque).

Nota: Los fees son utilizados para incentivar a que los mineros seleccionen tu transacción en vez de otra. Una transacción sin fee tiene pocas (por no decir casi ninguna) probabilidades de ser minada. Por tanto, el minero obtendrá tanto la recompensa del bloque como los fees del minado.

Puedes aprender más sobre los fees de minado aquí: https://academy.bit2me.com/que-es-comision-fee-de-mineria/

Una vez que has dado clic en «pay», verás cómo la transacción se ha ido al memory pool. Este es un pool de transacciones por realizar. En este paso podrás elegir la transacción creada y minarla.
Ahora has creado un nuevo bloque con esta transacción y, cómo podrás ver, las 100 monedas iniciales ahora tienen la etiqueta “spent” para indicar que estas han sido utilizadas.
En el nuevo bloque podemos ver cómo esta nueva transacción ha sido registrada correctamente en la red y cada actor ha recibido tanto la transacción como los fees correspondientes.

**Bloques**

Los bloques en la blockchain son como las páginas de un libro de contabilidad. Cada bloque contiene un número de transacciones y una vez que un bloque está lleno se añade a la cadena de bloques. Lo interesante es que estos bloques no se agregan aleatoriamente al libro, sino que están enlazados en una cadena. Cada bloque contiene un código especial llamado «hash», que es como una huella digital única. Además, cada uno tiene también una referencia al bloque anterior en la cadena. Dicho de otra manera, un bloque en la blockchain contiene un encabezado de bloque y datos de bloque. El encabezado contiene metadatos para este bloque. Los datos contienen una lista de transacciones validadas y auténticas que se han enviado a la red de blockchain. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Cada bloque en una blockchain está criptográficamente vinculado al anterior, lo que lo hace evidente de manipulaciones. A medida que se añaden nuevos bloques, los bloques más antiguos se vuelven más difíciles de modificar, creando resistencia a la manipulación. Los nuevos bloques se replican a través de copias del libro de contabilidad dentro de la red, y cualquier conflicto se resuelve automáticamente utilizando reglas establecidas. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Es importante destacar que los datos de la blockchain no pueden ser alterados haciendo que los bloques y transacciones posteriores actúen como actualizaciones o modificaciones a los bloques y transacciones anteriores. Esta abstracción de software permite modificaciones a los datos de trabajo, mientras proporciona un historial completo de cambios. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf
Para añadir un nuevo bloque a la blockchain, todos los nodos deben llegar a un acuerdo común con el tiempo. Este proceso se conoce como consenso. NIST (2018). Blockchain Technology Overview. https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf
 
El resultado de todo esto es una cadena de bloques que registra y mantiene un historial de todas las transacciones realizadas. Esta tecnología es utilizada en las criptomonedas como bitcoin, pero también se puede aplicar a otros casos de uso donde se requiere un registro transparente, seguro e inmutable de la información.

###  Ponte a prueba - Bloques

A continuación presentamos una demo de blockchain. En la sección «Block» del enlace, podemos ver los diferentes elementos de un bloque.

https://andersbrownworth.com/blockchain/block

Número de bloque: se refiere literalmente al número de bloque en la cadena de bloques. El bloque Génesis podríamos verlo como el bloque cero y el siguiente bloque como el uno.
Nonce: número aleatorio que se modifica repetidamente hasta encontrar la solución al problema matemático que los mineros deben de hallar durante el proceso de minado. En esta demo, el nonce es el único campo que se modifica para encontrar la solución matemática de minado, no obstante, cabe destacar que en la realidad el nonce y el timestamp del bloque son los únicos elementos que se modifican.

Puedes encontrar mas información respecto al nonce aquí: https://academy.bit2me.com/que-es-nonce/

NOTA: Este nonce es utilizado principalmente en el protocolo de consenso prueba de trabajo o POW, por sus siglas en inglés.

Data: se refiere a la data que se va a registrar en un bloque dentro de la red. En este demo, podemos escribir texto, no obstante, la realidad es que esta sección se refiere a las transacciones mismas de los usuarios de la red.
Hash: representación alfanumérica del bloque. Surge a partir de aplicar algoritmos de encriptación al bloque entero, es decir, se aplica un proceso de encriptación a todos los elementos del bloque incluidos el nonce, el número del bloque y los datos del bloque.

Una vez que modifiques y juegues con los diferentes elementos del bloque, puedes darle clic al botón Mine para minar y registrar en la red blockchain ese bloque en específico.

**Protocolos de consenso**

Los protocolos de consenso son una parte esencial de la tecnología blockchain. Son los métodos que se utilizan para acordar qué bloques se añaden a la cadena. En otras palabras, un mecanismo de consenso es un conjunto de reglas y procedimientos que mantiene un conjunto coherente de hechos entre los nodos participantes. KPMG (2016). Blockchain Consensus - Immutable agreement for the Internet of value. https://assets.kpmg.com/content/dam/kpmg/pdf/2016/06/kpmg-blockchain-consensus-mechanism.pdf

Existen varios protocolos de consenso, algunos de los cuales son:

**Prueba de trabajo (Proof of Work, PoW)**. Este protocolo requiere que los nodos de la red resuelvan problemas matemáticos complejos para añadir un nuevo bloque a la cadena. Este proceso consume una gran cantidad de energía y recursos computacionales.

**Prueba de participación (Proof of Stake, PoS)**. En este protocolo, el creador del próximo bloque se elige en función de su participación o cantidad de monedas que posee. Este protocolo es más eficiente en términos de energía que la prueba de trabajo. Cabe destacar que en caso de actuación maliciosa, el participante en cuestión podría perder las monedas puestas como garantía por participar en el consenso.

**Prueba de autoridad (Proof of Authority, PoA)**. Este protocolo se basa en la reputación de los nodos. Los nodos con una alta reputación tienen más probabilidades de ser elegidos para crear el próximo bloque.

**Prueba de tiempo transcurrido (Proof of Elapsed Time, PoET)**. Este protocolo se basa en un enfoque de «lotería». Cada nodo espera un tiempo aleatorio y el primero en terminar la espera tiene derecho a crear el próximo bloque.

**Prueba de importancia (Proof of Importance, PoI)**. Este protocolo no solo tiene en cuenta la cantidad de monedas que posee un nodo, sino también su actividad en la red. Los nodos que son más activos en la red tienen más probabilidades de ser elegidos para crear el próximo bloque. KPMG (2016). Blockchain Consensus - Immutable agreement for the Internet of value. https://assets.kpmg.com/content/dam/kpmg/pdf/2016/06/kpmg-blockchain-consensus-mechanism.pdf

Es importante tener en cuenta que no todos los mecanismos de consenso son blockchains. Algunos también pueden funcionar «fuera de la cadena», como acuerdos bilaterales. KPMG (2016). Blockchain Consensus - Immutable agreement for the Internet of value. https://assets.kpmg.com/content/dam/kpmg/pdf/2016/06/kpmg-blockchain-consensus-mechanism.pdf, p. 5.

Aquí puedes encontrar información adicional para aprender más sobre esos protocolos de consenso:
https://www.youtube.com/watch?v=NxFPqsLNCJY (3:59)
https://ethereum.org/en/developers/docs/consensus-mechanisms/pow/#visual-learner

### Ponte a prueba - Protocolos de consenso

A continuación presentamos un demo sobre el protocolo de consenso de Avalanche. Avalanche es una blockchain de consenso que busca lograr altos niveles de escalabilidad, seguridad y descentralización. Fue creado por la empresa Ava Labs y se basa en un algoritmo de consenso llamado Protocolo Avalanche. Después de este, la empresa ha desarrollado diferentes implementaciones del protocolo como SnowFlake o SnowBall. Puedes ver el siguiente demo de este último en el siguiente enlace:

https://tedyin.com/archive/snow-bft-demo/#/snow

En el demo podrás ver cómo funciona el protocolo SnowBall. Para entenderlo, veamos la siguiente explicación intuitiva del protocolo:

Imagina una sala llena de personas tratando de ponerse de acuerdo sobre qué pedir para el almuerzo. Supongamos que es una elección binaria entre pizza y barbacoa. Algunas personas pueden preferir inicialmente la pizza, mientras que otras prefieren inicialmente la barbacoa. Sin embargo, en última instancia, el objetivo de todos es lograr el consenso.

Todos preguntan a un subconjunto aleatorio de personas en la sala cuál es su preferencia para almorzar. Si más de la mitad dice pizza, la persona piensa: "Está bien, parece que las cosas se están inclinando hacia la pizza". “Prefiero la pizza ahora". Es decir, adoptan la preferencia de la mayoría. Del mismo modo, si la mayoría dice barbacoa, la persona la adopta como su preferencia.

Todos repiten este proceso. Cada ronda, más y más personas tienen la misma preferencia. Esto se debe a que cuantas más personas prefieran una opción, es más probable que alguien reciba una respuesta mayoritaria y adopte esa opción como su preferencia. Después de suficientes rondas, llegan a un consenso y deciden sobre una opción, que todos prefieren.

# ii. Ethereum y smart contracts

Los contratos inteligentes, o smart contracts, son códigos que se ejecutan en la blockchain y se activan por transacciones. Puedes pensar en ellos como programas de computadora que ejecutan ciertas acciones cuando se cumplen condiciones específicas. Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.

https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

Los contratos inteligentes tienen su origen en la creación de la blockchain de ethereum, no obstante, en la actualidad existen diferentes plataformas blockchain que también permiten el desarrollo de estos programas, tal es el caso de las siguientes redes:

1. BNB Smart Chain (BSC): cadena paralela a la red de Binance que ofrece compatibilidad con contratos inteligentes. Utiliza un lenguaje de programación similar a Solidity y es compatible con muchas de las herramientas y aplicaciones de ethereum. https://academy.binance.com/es/articles/an-introduction-to-binance-smart-chain-bsc
 
2. Cardano: plataforma blockchain que utiliza un lenguaje de programación funcional llamado Plutus para desarrollar contratos inteligentes. Se centra en la seguridad y la verificación formal de los contratos.
        https://cardano.org/

 
3. Polkadot: red de blockchain multi-cadena que permite la interoperabilidad entre diferentes blockchains. Utiliza el lenguaje de programación Rust y su framework Substrate para crear contratos inteligentes.
        https://polkadot.network/
 
4. Tezos: plataforma blockchain que utiliza el lenguaje de programación Michelson para desarrollar contratos inteligentes. Se enfoca en la gobernanza y la actualización autónoma de su protocolo.
        https://tezos.com/
   
Aun teniendo diferentes posibilidades para crear contratos inteligentes, ethereum se ha posicionado como la plataforma líder en este campo por su flexibilidad para desarrollar aplicaciones descentralizadas. Por esto, a lo largo de este curso nos enfocaremos en esta blockchain.

**Los elementos principales de un contrato inteligente en Ethereum son los siguientes:**

Reglas preespecificadas arbitrariamente. Los contratos inteligentes permiten mover activos digitales de acuerdo con reglas preespecificadas arbitrariamente. Por ejemplo, un contrato puede especificar que «A puede retirar hasta x unidades de moneda por día; B puede retirar hasta y por día, A y B juntos pueden retirar cualquier cosa y A puede apagar la capacidad de B para retirar» . Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.

https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

**Lenguaje de programación Turing-completo**. Ethereum proporciona una blockchain con un lenguaje de programación Turing-completo incorporado, que se puede utilizar para crear «contratos» que pueden codificar funciones de transición de estado arbitrarias. Esto permite a los usuarios crear cualquier sistema simplemente escribiendo la lógica en unas pocas líneas de código. Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.
https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

**Cuentas de Ethereum**. En Ethereum, el estado está compuesto por objetos llamados "cuentas", cada una con una dirección de 20 bytes. Las transiciones de estado son transferencias directas de valor e información entre cuentas. Una cuenta de Ethereum contiene cuatro campos: el nonce (un contador utilizado para asegurar que cada transacción solo se puede procesar una vez), el saldo actual de ether de la cuenta, el código del contrato de la cuenta (si está presente) y el almacenamiento de la cuenta (vacío por defecto). Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.
https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

**Aplicaciones de contratos inteligentes**. Los contratos inteligentes pueden ser utilizados en una variedad de aplicaciones, desde derivados financieros hasta monedas de valor estable. Por ejemplo, un contrato inteligente puede ser utilizado para implementar un contrato de diferencia financiera que requiere referencia a un ticker de precio externo. Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.
https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

Si quieres profundizar más sobre contratos inteligentes, te dejamos estos videos que hablan sobre la importancia y funcionamiento de estos:

https://www.youtube.com/watch?v=pA6CGuXEKtQ (17:36)
https://www.youtube.com/watch?v=pWGLtjG-F5c&t=4s (15:59)

## Ponte a prueba - Contratos inteligentes
¡Ahora pasemos a la práctica!

En este ponte a prueba, ejecutaremos un contrato que nos permitirá (En una red blockchain de prueba), un contrato inteligente. 

Accede al siguiente enlace: https://chainide.com/

Haz clic en el botón Try now.

Haz clic en Continue as Guest o accede con tus credenciales de GitHub.

En la parte superior de la pantalla puedes cambiar el lenguaje a español si así lo deseas.

Haz clic en el + de New Project.

Verás que existen multitud de proyectos predefinidos para diferentes blockchains y que, por defecto, nos posicionamos en Ethereum. Haz clic en el proyecto llamado «Hello world».

Una vez que se haya creado el nuevo proyecto, en la parte superior derecha da clic sobre el botón Connect wallet y selecciona JavaScript VM; esto creará virtualmente una billetera o wallet para poder desplegar el contrato inteligente que has seleccionado. Si quieres aumentar la dificultad del ejercicio, puedes probar con la opción de Injected Web3 provider. Ten en cuenta que si seleccionas esta opción deberás tener instalada tu wallet Metamask o Wallet connect.

Una vez conectada tu billetera, da clic sobre el fichero .sol, ubicado en la parte izquierda de tu pantalla, titulado «HelloWorld». Verás que en la parte de la derecha de tu pantalla se ha puesto en azul el botón Compile HelloWorld.sol. Da clic en este para compilarlo.

Si el programa se ha ejecutado correctamente, verás en la consola el siguiente mensaje: «Upload file [.build/HelloWorld.sol.compiled] successfully!».
Verás que se han creado dos elementos: ABI y Bytecode dentro de la sección HelloWorld y debajo del botón de compilar. ABI se refiere a la instancia ABI o "interfaz binaria de aplicación", la cual es una representación formal que define cómo interactuar con un contrato en la cadena de bloques de Ethereum. Incluye los métodos del contrato, los tipos de entrada y salida de cada método, así como otros detalles técnicos. 

Una vez que compilas y despliegas el contrato HelloWorld en Ethereum, el compilador de Solidity genera una ABI para el contrato. Esta es necesaria para interactuar con tu contrato desde una aplicación externa. Por ejemplo, si estás utilizando la biblioteca web3.js en una aplicación de front-end, necesitarías proporcionar la ABI del contrato y la dirección del contrato desplegado para crear una instancia del contrato y llamar a sus funciones. En este caso, dentro del mismo ChainIDE se está generando esta integración que te permite interactuar con tu contrato. No te preocupes si no entiendes esto, en los módulos posteriores profundizaremos en estos conceptos.
 
Por otro lado, tenemos el elemento ByteCode, el cual es la representación de código de bajo nivel de tu contrato Solidity una vez que ha sido compilado. Es el código que se ejecuta en la Máquina Virtual de Ethereum (EVM). En otras palabras, cuando escribes un contrato en Solidity (o cualquier otro lenguaje de alto nivel que se compila a bytecode de EVM), un compilador traduce tu código fuente a un formato que la EVM puede entender y ejecutar. Este formato es el bytecode. Este es el que realmente se almacena en la cadena de bloques y se ejecuta cuando interactúas con el contrato en la cadena de bloques Ethereum.

Una vez explorados estos dos elementos, puedes darle clic a Deploy & interaction, ubicado en la parte lateral derecha de tu pantalla, justo debajo de la selección actual Solidity compiler. Verás que te permite darle clic al botón Deploy. Esto permitirá desplegar tu contrato compilado (ABI + bytecode) en la blockchain. Si todo ha salido bien, verás el siguiente mensaje: «Uploaded file [.build/HelloWorld.HelloWorld.d9145cce52d386f2.eth.deployed] successfully!».
Verás que se ha creado una nueva sección llamada Interact. Esta sección contiene dos botones, uno por cada función de nuestro contrato ( Get() y test()). 

Al darle clic al botón Get, el resultado de esta interacción con tu contrato devuelve «Hello, world», no obstante, si das clic sobre el botón Submit no verás nada. Esto es debido a que el mensaje «Hello EVM!» es emitido en un evento de Solidity (Log), mientras que «Hello, world!» se retorna directamente desde una función (get). Aunque ambos son mensajes, la forma en que son creados y accedidos es diferente, por tanto, para ver el mensaje «Hello EVM!» necesitas acceder al registro de transacciones y buscar el evento Log emitido por hacer clic en el botón Submit. Esto lo puedes hacer accediendo a la sección llamada Internal transactions, ubicado en la parte lateral derecha de tu pantalla. Verás que tienes dos transacciones (si solo has hecho clic una vez en cada botón). Si haces clic sobre ambos botones More, verás que se despliega el log de ambos eventos, pues bien, en la segunda transacción, en la parte llamada log, podrás desplegar todos los elementos de este para encontrar ahí el mensaje «Hello EVM!» bajo el desplegable «args».

**!Felicidades¡**, has compilado, desplegado e interactuado con tu primer contrato inteligente. Si bien no entramos en materia aún de explicar el código de un contrato inteligente, te invitamos a que explores por tu cuenta este contrato.

A medida que exploras y te familiarizas con este contrato inteligente, verás que hay varios conceptos y componentes subyacentes que forman su núcleo. Estos conceptos serán importantes a la hora de desarrollar otros contratos inteligentes, no obstante, otro concepto que merece especial atención, debido a su importancia en la integridad y seguridad de las transacciones, es el de la criptografía de hashing. Hablemos entonces sobre el hashing, un componente esencial de la tecnología blockchain, usado extensamente en el funcionamiento de contratos inteligentes.

**Hashing: Criptografía**

El hashing es un componente fundamental en la tecnología blockchain. En términos sencillos, es el proceso de tomar una entrada (en el caso de blockchain, esta puede ser una transacción o un bloque de transacciones) y devolver una cadena de caracteres de longitud fija, que es única para cada entrada única. Este proceso se realiza mediante el uso de una función hash, es decir, la aplicación de un algoritmo de encriptación.

En el contexto de la criptografía, el hashing se utiliza para asegurar la integridad de los datos. En otras palabras, asegura que estos no han sido alterados de ninguna manera. Esto se debe a que cualquier cambio, por pequeño que sea, en los datos de entrada dará como resultado un hash completamente diferente. Por lo tanto, si los datos se alteran de alguna manera, el hash cambiará, lo que indicará que los datos han sido manipulados.

Un algoritmo de hash comúnmente utilizado en la tecnología blockchain es el SHA-256, conocido por su seguridad. Se utiliza en varias blockchains, incluyendo bitcoin. En el caso de ethereum, se utiliza el algoritmo Keccak-256. Cuando se aplica el algoritmo SHA-256 a una entrada, se obtiene un hash de 64 caracteres. Por ejemplo, si lo aplicamos a la frase "Aprendamos blockchain", obtenemos el siguiente hash: ef5549386b27a9af7d13101f0b3bc5b081574a85373e89a7a0052948463fb3df. Cada vez que apliquemos el algoritmo SHA-256 a esta misma frase, obtendremos el mismo hash. Sin embargo, si cambiamos, aunque sea un solo carácter de la frase, el hash resultante será completamente diferente.

En resumen, el hashing es una técnica criptográfica esencial en la tecnología blockchain que se utiliza para asegurar la integridad de los datos. A través del uso de algoritmos de hash como el SHA-256, podrás asegurarte de que los datos no han sido alterados de ninguna manera, aspecto fundamental para mantener la seguridad y la confiabilidad de la blockchain.

A continuación, te presentamos este demo en el que puedes jugar con el algoritmo SHA256 para que comprendas en su totalidad cómo funciona el hashing. Prueba a escribir cualquier texto que quieras y cambia una letra. Comprobarás cómo el algoritmo cambia por completo el hash de esta transacción, haciendo que este método de encriptación sea perfecto para asegurar la inmutabilidad de los datos encriptados en una blockchain.

https://academo.org/demos/SHA-256-hash-generator/

Tras jugar y experimentar con el algoritmo SHA256 en la demo proporcionada, puedes haber notado cómo un mínimo cambio en el input genera una gran variación en el hash resultante. Este comportamiento de alta sensibilidad es crucial para mantener la inmutabilidad y seguridad de las transacciones en la blockchain. Este concepto de inmutabilidad se manifiesta en gran medida en el proceso de minería de bloques del que pasaremos ahora a hablar.

**Minería de bloques**

En la minería de bloques, un minero tiene que realizar un proceso para registrar un nuevo bloque con nuevas transacciones y datos. 
Este proceso inicia cuando un usuario A de la red blockchain solicita una transacción a un usuario B: la solicitud del usuario A es transmitida a un mempool. Este actúa como centralita para juntar múltiples solicitudes de múltiples usuarios. Cuando se mina un bloque, en realidad se minan múltiples transacciones al mismo tiempo. Una vez paquetizadas las transacciones, la red debe asignar el derecho de minar un nuevo bloque a la cadena de bloques existente (blockchain) a un minero específico. El mecanismo para asignar este derecho depende del tipo de protocolo de consenso que se utilice. Algunos protocolos de consenso son Proof of Work (PoW) o Proof of Stake (PoS), protocolos usados por bitcoin y ethereum, respectivamente.

En el caso de PoW, el primer minero que sea capaz de resolver un problema matemático tendrá el derecho a minar ese bloque nuevo.

Cuando un minero termine con el trabajo de minar, la red de nodos distribuidos validará la veracidad de dichas transacciones, ya que todos los nodos disponen del mismo historial de transacciones por medio de métodos criptográficos sobre el histórico de movimientos. En caso de encontrar diferencias o errores, se eliminará el bloque y ese nodo minero será eliminado de la red, y cuando no se encuentren diferencias y validación de los datos, ese nuevo bloque será adicionado a la red blockchain existente. 

# iii. Fundamentos de Ethereum

Ethereum, como plataforma, es una evolución de la tecnología blockchain que va más allá de ser solo una criptomoneda. Fue concebido como una versión mejorada de una criptomoneda, proporcionando características avanzadas como el depósito en garantía en la cadena de bloques, límites de retiro, contratos financieros o mercados de diferentes instrumentos y similares a través de un lenguaje de programación de alto nivel (Solidity) Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.

https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

Ethereum ha sido desarrollado con el objetivo de ser una plataforma Turing complete (al contrario de Bitcoin) para ejecutar aplicaciones descentralizadas de cualquier tipo, las cuales no dependen de ningún servidor central. En Ethereum, las aplicaciones se ejecutan en cada nodo de la red. Los resultados de las computaciones derivadas de las transacciones de la misma red se codifican en bloques, que, a través del protocolo de consenso prueba de participación o Proof of Stake (antes Proof of Work), son validados por cada nodo de la red. Además, estas operaciones (transacciones) se llevan a cabo en nombre de los usuarios. Estos deben firmar cada transacción con su clave privada, lo que hace posible rastrear si un usuario determinado puede realizar ciertas operaciones o no. En particular, las transacciones tienen un costo y los usuarios deben poder pagarlo gastando la criptomoneda de rehereum: ether. Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform. https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

Como podemos ver, Ethereum no difiere en su funcionamiento de una blockchain, como Bitcoin, por esto, la minería en esa red es un componente esencial, igual que Bitcoin. Sin embargo, a diferencia de esta última, Ethereum está diseñada para facilitar la minería incluso en redes privadas.
Otro componente que diferencia a Ethereum de Bitcoin son los contratos inteligentes (previamente explicados); estos son el elemento clave de la red. En ellos se puede codificar cualquier algoritmo. Los contratos inteligentes pueden llevar un estado arbitrario y pueden realizar cualquier cálculo arbitrario. Incluso, son capaces de llamar a otros contratos inteligentes. Esto da a Ethereum una flexibilidad tremenda. Los contratos inteligentes son ejecutados por cada nodo como parte del proceso de creación de bloques. Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.
https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

# Reto semanal (básico) 

Navegación básica del explorador de bloques de bitcoin

¡Felicidades por completar la semana 2! Para terminar, te proponemos reforzar lo aprendido mediante la siguiente práctica.

El objetivo es que te familiarices con el uso básico del explorador de bloques de Bitcoin. Te pedimos que realices lo siguiente:

Accede al explorador de bloques de Bitcoin (https://www.blockchain.com/es/explorer).

Busca el bloque más reciente y anota el número de transacciones que contiene.

Selecciona una transacción al azar de este bloque y toma nota del hash de transacción, la cantidad de bitcoins enviados y las direcciones de origen y destino.

Contesta la siguiente pregunta: ¿qué es el hash de la transacción y por qué es importante?

**Rescatando lo importante**

Los fundamentales de Ethereum no distan de los fundamentales de cualquier tecnología blockchain, aunque con una diferencia clave: la capacidad de crear aplicaciones Turing complete gracias a los contratos inteligentes, algo que, si bien se tiene actualmente también en otras redes, Ethereum fue la precursora de este tipo de aplicaciones, lo que ha permitido que esta red se mantenga en el top de la construcción de aplicaciones descentralizadas por medio de su lenguaje de programación Solidity.

**Referencias**

National Institute of Standard and Technology [NIST]. (2018). Blockchain Technology Overview.
https://nvlpubs.nist.gov/nistpubs/ir/2018/nist.ir.8202.pdf

Blockchain Consensus - Immutable agreement for the Internet of value, KPMG, 2016.
https://assets.kpmg.com/content/dam/kpmg/pdf/2016/06/kpmg-blockchain-consensus-mechanism.pdf

Vitalik Buterin (2014). Ethereum: A Next-Generation Smart Contract and Decentralized Application Platform.
https://ethereum.org/669c9e2e2027310b6b3cdce6e1c52962/Ethereum_Whitepaper_-_Buterin_2014.pdf

Nota bene: las marcas aquí mencionadas son única y exclusivamente de carácter educativo y de investigación, sin fines lucrativos ni comerciales.
