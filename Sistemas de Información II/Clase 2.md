# Ver -> ==the imitation game==

## Proceso
	Proceso se refiere a una serie de acciones o pasos que se llevan a cabo de manera sistemática y organizada para lograr un objetivo específico.
---

entrada --> **Proceso** --> Salida
entrada --> **actividad 1 -> actividad 2 -> actividad 3** --> Salida
### Tipos
- Estrategicos -> Determinan la estrategia de la organización de la organización de acuerdo a su mision, vision y valores.
- Tacticos -> Dan apoyo a los sistemas productivos para asegurar que se ejecute la estrategia fijada.
- Operativos -> Llevan a cabo las actividades principales para producir y/o brindar el producto o servicio.



## Calidad
---
Dos puntos de vista:
- Cliente: Es el valor percibido y juzgado por el cliente.
- Producto: Es el grado en el que un conjunto de caracteristicas inherentes cumple con los requisitos.

ISO 9001 -> Estandar internacional, puede ser usado en el desarrollo de un sistema de gestion de calidad.

Plan de calidad
- Descripcion del producto.
- Planes del producto.
- Descripcion del proceso.
- Objetivos de calidad.
- Gestion de riesgo.

Particularidades en Software
- Dificultad para enunciar especificaciones.
- Las especificaciones integran requerimientos de varios stakeholders pero no todos de ellos pueden ser contemplados en la solucion.
- Es imposible medir ciertas caracteristicas de calidad. ej: Mantenibilidad.

## Atributos de un buen software
Seguridad - Comprensibilidad - Portabilidad
Proteccion - Traceabilidad - Usabilidad
Fiabilidad - Adaptabilidad - Reusabilidad
Resilencia - Modularidad - Eficiencia
Robusticidad - Complejidad - Aceptabilidad
## Importancia del uso de estandares
- Captura el conocimientode la organizacion que asegura las practicas mas exitosas.
- Provee un marco para definir que significa calidad en cada paso.
- Agiliza la incorporacion de personas con poca experiencia en el proceso sin tener impacto negativo en el producto.

## Tipos de estandares
- Producto: 
	- Aplica al producto a ser desarrollado.
	- Incluye estandar de documentación.
- Proceso:
	- Aplica al Proceso que deve seguirse para desarrollar al producto.
	- Constituyen las buenas practicas y los procesos para especicacion, diseño, validacion, implementacion y soporte del producto.

## Tipos de requerimientos
- **Funcional** -> Declaraciones de los servicios que el sistema debe proveer, como debe reaccionar con los input particulares y comose espera que reaccione.
- **No funcional / tecnico** -> Son restricciones que aplican al Sistema o a sus funciones.


## Modelo de cascada
![[Screenshot from 2024-03-15 21-08-19.png]]

## Modelo de espiral
![[Screenshot from 2024-03-15 21-10-47.png]]


## Modelo de desarrollo en V

## RUP (Proceso Unificado Racional)
Se describe desde tres perspectivas:
1. Una perspectiva dinámica que muestra las fases del modelo a través del tiempo.
2. Una perspectiva estática que presenta las actividades del proceso que se establecen.
3. Una perspectiva práctica que sugiere buenas prácticas a usar durante el proceso.
Fases:
1. **Concepción** La meta de la fase de concepción es establecer un caso empresarial para el sistema. Deben identificarse todas las entidades externas (personas y sistemas)que interactuarán con el sistema y definirán dichas interacciones. Luego se usa esta información para valorar la aportación del sistema hacia la empresa. Si esta aportación es menor, entonces el proyecto puede cancelarse después de esta fase.
2. **Elaboración** Las metas de la fase de elaboración consisten en desarrollar la comprensión del problema de dominio, establecer un marco conceptual arquitectónicopara el sistema, diseñar el plan del proyecto e identificar los riesgos clave del proyecto. Al completar esta fase, debe tenerse un modelo de requerimientos para elsistema, que podría ser una serie de casos de uso del UML, una descripción arquitectónica y un plan de desarrollo para el software.
3. **Construcción** La fase de construcción incluye diseño, programación y pruebas del sistema. Partes del sistema se desarrollan en paralelo y se integran durante esta fase. Al completar ésta, debe tenerse un sistema de software funcionando y la documentación relacionada y lista para entregarse al usuario.
4. **Transición** La fase final del RUP se interesa por el cambio del sistema desde la comunidad de desarrollo hacia la comunidad de usuarios, y por ponerlo a funcionar en un ambiente real. Esto es algo ignorado en la mayoría de los modelos de proceso de software aunque, en efecto, es una actividad costosa y en ocasiones problemática. En el complemento de esta fase se debe tener un sistema de software documentado que funcione correctamente en su entorno operacional.