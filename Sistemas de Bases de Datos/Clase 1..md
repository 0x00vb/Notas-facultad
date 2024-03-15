Herramienta: SQL server 
## Fechas
#### 1er 
Parcial -> 13/Junio
Recupertorio -> 22/Agosto
#### 2do
Parcial -> 31/Octubre
Recuperatorio -> 14/Noviembre

## Tipos de bases de datos
- Relacionales -> Almacena datos estructurados en tablas relacionadas entre si.
La tabla, posee columnas, campos (pueden poseer un tipo). Estructura escalable y flexible. Se suelen utilizar cuando se requieren transacciones en tiempo real.
Ej: Oracle, postgress, mySql, SqlServer.

- No Sql -> MongoDB.
No utilizan tablas ni claves, sino que utilizan un conjunto de datos, y son muy escalables, y se suelen utilizar cuando tenemos un gran conjunto de datos no estructurados.

- De objetos (NoSQL) -> Almacenan los datos como objetos. Este tipo de datos, se suele utilizar para almacenar y manipular objetos complejos y jerárquicos.
- Grafos -> Pensados para relacionar relaciones de datos complejos. Se suelen utilizar cuando se trabaja con patrones en grandes volúmenes de datos.
- En Memoria -> Almacenan datos en la memoria del hardware.
- En archivos -> 
	Inconvenientes:
	- Redundancia de datos.
	- Dificultad de acceso.
	- Dependencia de los datos.
	- Problema de Integridad.
	- Problemas de atomicidad.
	- Acceso concurrente.
	
## Que es una base de datos
	Conjunto de datos almacenados entre los que existe relaciones lógicas y ha sido diseñado par satisfacer los requerimientos de información de un empresa u organización.


## Sistemas de gestión de Bases de Datos
	Conjunto de programas que le permite a los 'Usuarios' definir, crear y mantener la base de datos, y a su vez proporcionar un acceso controlado a la misma.

### Quienes son los usuarios
	- El usuario final: Es quien utiliza la aplicación.
	- Diseñadores: Realizan el diseño logico de la DB. Identificando que datos hay que guardar, y que relaciones deben tener.
	- Diseñadores de aplicaciones: Realizan las consultas para el acceso de los datos.
	- Admin de base de datos: Conoce a la perfección el almacenamiento fisico de los datos, y es quien administra la seguridad.
	
## Características
- Relaciones -> Reglas de negocio de la aplicación.
- Independencia Lógica y Física -> Independencia entre la estructura y donde se guarda.
- Integridad -> Mecanismos de seguridad que manejan la integridad de los datos.
- Redundancia.
- Consistencia.
- Atomicidad. -> Las transacciones se deshacen ante una interferencia externa.
- Concurrencia.

## Arquitectura
	Buscan proveer a los usuarios una vista abstracta de los datos.
	Se buscara ocultar el detalle de como es almacenada esa información.
	Los niveles de abstraccion de la informacion son:
		- Fisico: Como estan almacenados los datos a nivel fisico.
		- Logico: Que datos estan almacenados y las relaciones entre ellos.
		- Vista: Detalle de una parte de la DB.
	- Instancias:
		Es un estado que presenta una DB en un momento dado.
	- Esquema: Descripcion logica de la DB. Proporciona nombres de las entidades, tablas (y atributos), vistas, funciones.
	Este no cambia, lo que cambia son los datos.

### Independencia lógica-física
#### interfaces de acceso
- DML (data manipulation language) -> Sentencias de manipulación de datos.
- DDL (data definition language) -> Sentencias que manipulas la estructura. (Crear tablas, relaciones, indices)

### Administración de transacciones
	Existe para poder soportar el acceso a un conjunto de datos como unica unidad de trabajo. Propiedades (ACID):
	- Atomicidad. -> Los cambios aplicados en la transaccion se aplican todos o ninguno.
	- Consistencia. -> Las reglas y las variaciones definidas en la DB deben mantenerse luego ejecutada la transacción.
	- Aislamiento. -> La ejecución de la transaccion sobre un conjunto de datos, debe ser independiente de otra transaccion sobre el mismo conjunto.
	- Durabilidad. -> Luego de ejecutar una transacción los atos debes ser persistentes, mas alla de un posible fallo.

	Se denomina ACID complete al sistema que cumple con las 4 caracteristticas.


Administrador de procesamiento -> Componente que provee una interfaz entre los datos almacenados de bajo nivel y los programas y aplicaciones del sistema.
Responsable de guardar, recuperar y actualizar; Y traduce consultas DML a otro nivel.
Dentro de este hay subcomponentes:
- Admin de Autorizaciones e integridad
- Admin de transacciones
- Admin de archivos
- Admin de Almacenamiento 

Procesador de consultas -> Componente dentro del sistema de gestión, encargado de proveer una interfaz de alto nivel para el acceso de los datos atraves de consultas. Componentes:
- Interpretador DDL
- Copilador DML
- ingeniería de consultas (evaluación de querys)

## Inconvenientes de un gestor de bases de datos
- Complejidad.
- Tamaño.
- Costos.
	- Económico.
	- Equipamiento adicional.
	- 

## Base de datos optima
- Diseño adecuado en base a la necesidad. -> Normalizado, no redundante.
- Uso adecuado de indices.
- Optimización de consultas.
- Configuración adecuada del servidor de la DB.
- Optimización de almacenamiento de datos.
- Correcto mantenimiento de la DB. -> Eliminación de datos obsoletos, backups, updates, etc.