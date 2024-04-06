# Fechas
- 1er parcial: 12/6 -> Recuperatorio: 26/6
- 2do parcial: 6/11 -> Recuperatorio: 20/11
# Repaso Programación II

## Metodología orientada a objetos
	En la metodología orientada a objetos se enfatiza el estudio de los objetos en vez de la funcionalidad (análisis estructurado), porque constituye un descripción mas próxima a la realidad y facilita los cambios y adaptaciones posteriores.
#### Mecanismo de POO ->
- Objetos -> Instancia concreta de una clase.
- Métodos -> definen el comportamiento de los objetos y pueden realizar operaciones.
- Clases  -> plantilla para _objetos_ múltiples con características similares. Las _clases_ comprenden todas esas características de un conjunto particular de objetos.
- Mensajes -> La forma en la que se comunica un objeto con otro.

#### Tipos de Acceso:
- Private -> -
- Protected -> #
- public -> +
- (default) Package -> ~ 
#### Características de POO
- Abstracción -> Capacidad de representar los aspectos esenciales de un objeto y ocultar los detalles innecesarios o complejos
Debe incluir al menos un método abstracto de la siguiente forma:
`public abstract void metodoAbstracto();`
- Encapsulamiento -> Ocultación de los detalles internos de un objeto y la restricción del acceso a ciertos componentes.
- Herencia -> Permite compartir los elementos de una clase con otra.
- Polimorfismo -> permite a un objeto tomar diferentes formas o comportarse de manera diferente en función del contexto.
	- Sobrecarga de funciones: permite tener múltiples funciones con el mismo nombre en una clase, pero con diferentes tipos o cantidades de parámetros.
	- Shadowing: situación en la que una variable local en un ámbito interno tiene el mismo nombre que una variable en un ámbito externo, lo que oculta la variable externa durante la duración de ese ámbito interno. (@Override). Se resuelve en tiempo de compilación.
	- Ligadura dinámica: Se resuelve en tiempo de ejecución.
	Ej: Lista de Vehículos, un elemento de Clase hija auto, que posee un override de su claseMadre, el override se ejecuta automáticamente sin necesidad de realizar un Downcasting. Es decir, los métodos de la clase base no se castean.

#### Relaciones
- Asociación -> dos instancias A y B relacionadas entre sí existen de forma independiente.
	- Composición: agregación _fuerte_ en la que una instancia ‘parte’ está relacionada, como máximo, con una instancia ‘todo’ en un momento dado, de forma que cuando un objeto ‘todo’ es eliminado, también son eliminados sus objetos ‘parte’.
	- Agregación: asociación binaria que representa una relación todo-parte (_pertenece a tiene un, es parte de_). Por ejemplo, un centro comercial tiene clientes.


####  Static
- Ocupa un único espacio de memoria.
- Comparte el valor en todas sus instancias de cualquier clase.
Se accede: `NombreClase.setStaticAtrib()`.




```python
def hello(name):
	print("Hello", name)

if __name__ == "__main__":
	hello("Eve")

```


```c
#include <stdio.h>

printf("Hello, World!");
```