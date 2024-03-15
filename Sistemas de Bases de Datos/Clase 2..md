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



