## Arquitectura de un SGBD
- Storage Manager ->
	- Se encarga del manejo de disco.
	- Provee una interfaz entre los datos almacenados y los programas de aplicacion y consultas.
		Subvomponentes:
		- Transaction manager
		- File manager
		- Buffer manager
		- Auth and integrity manager


- Query Procesor -> Se encarga de interactuar con la aplicacion
	Subcomponentes:
	- DDL INTERPRETER
	- DML COMPILER
	- QUERY EVALUATION ENGINE

# ==Ejercicios Tarea==
1. Describir las propiedades ACID con el ejemplo de una transferencia bancariade $100 de una cuenta A hacia una cuenta B.
   
**Atomicidad**: La atomicidad garantiza que si la transferencia comienza, entonces se completará con éxito, es decir, se deducirán $100 de la cuenta A y se añadirán $100 a la cuenta B, o bien, si algo falla durante la transferencia, no se realizará ningún cambio en ninguna de las cuentas.

**Consistencia**: La consistencia asegura que, después de la transferencia, tanto la cuenta A como la cuenta B mantengan saldos corespondientes y cumplan con las restricciones y reglas de integridad de la base de datos. Por ejemplo, asegura que no se creen ni se destruyan dinero de la nada durante la transferencia.

**Aislamiento**: El principio de aislamiento garantiza que ninguna otra transacción (como otra transferencia o consulta de saldo) afecte la integridad de los datos de las cuentas A y B mientras la transferencia de $100 está en proceso. Esto evita problemas como la lectura de datos intermedios o no confirmados.

**Durabilidad**: La durabilidad asegura que una vez que se ha deducido $100 de la cuenta A y se han añadido $100 a la cuenta B, esos cambios persistirán en la base de datos incluso si ocurriera un fallo en el sistema, como un corte de energía o un reinicio no planificado.
   
2. A partir del diagrama 2-tier y 3-tier describir un ejemplo de cada tipo de aplicación.
**Aplicación de 2-tier**:
- **Ejemplo**: Una aplicación de escritorio de procesamiento de texto.
- **Descripción**: En una arquitectura de 2-tier, la aplicación consiste en dos capas principales: la capa de presentación (interfaz de usuario) y la capa de datos (base de datos). En el caso de una aplicación de procesamiento de texto, la interfaz de usuario (capa de presentación) proporciona las herramientas y controles necesarios para que el usuario cree y edite documentos. La capa de datos maneja el almacenamiento y recuperación de los documentos en la base de datos local o en el sistema de archivos del dispositivo. La lógica de negocio, como el formato del texto o la funcionalidad de impresión, generalmente reside en la misma máquina que la interfaz de usuario o en una parte integrada en la capa de datos.

 **Aplicación de 3-tier**:
- **Ejemplo**: Un sistema de e-commerce.
- **Descripción**: En una arquitectura de 3-tier, la aplicación se divide en tres capas principales: la capa de presentación, la capa de lógica de negocio (o aplicación) y la capa de datos. Para un sistema de comercio electrónico, la capa de presentación es la interfaz de usuario que ve el cliente, donde puede buscar productos, agregarlos al carrito y realizar el pago. La capa de lógica de negocio maneja las reglas comerciales y las operaciones relacionadas con la gestión de pedidos, como calcular el total del carrito, procesar el pago y actualizar el inventario. La capa de datos gestiona la persistencia de los datos, como la información del producto, los detalles del cliente y el historial de pedidos, en una base de datos centralizada. En este modelo, la capa de lógica de negocio actúa como un intermediario entre la interfaz de usuario y la base de datos, garantizando una mayor separación de preocupaciones y flexibilidad en el desarrollo y mantenimiento de la aplicación.
   
3. A partir del diagrama de arquitectura de un SGBD describir la secuencia que se lleva a cabo desde que un usuario accede a un sitio web a realizar una búsqueda hasta que obtiene los resultados en pantalla.

El usuario utiliza la interfaz de la aplicacion, 