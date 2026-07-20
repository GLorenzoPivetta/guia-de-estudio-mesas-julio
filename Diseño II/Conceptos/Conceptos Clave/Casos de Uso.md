---
title: Casos de Uso
tags:
  - uda/diseno-ii
  - unidad-ii
  - repaso-oral
aliases:
  - CU
  - Caso de uso
  - Modelo de casos de uso
---

# Casos de Uso

Un caso de uso describe ==una forma en que un actor obtiene un resultado de valor al interactuar con el sistema==. Expresa un requisito funcional desde la perspectiva de quien usa o se relaciona con el sistema; por eso explica **qué debe lograr el sistema**, sin adelantar todavía cómo estará programado internamente.

La idea clave es que un caso de uso no es una pantalla, una clase ni un botón. Es un objetivo con sentido para un actor. Por ejemplo, en un sistema de turnos médicos, `Solicitar turno` es un caso de uso porque el paciente busca concretar una reserva; la pantalla donde elige la fecha es solo una parte de ese recorrido.

## Elementos fundamentales

- **Actor:** rol externo que interactúa con el sistema. Puede ser una persona, una organización o incluso otro sistema. No se define por el nombre de una persona, sino por su rol: `Paciente`, `Secretaría`, `Sistema de pagos`.
- **Objetivo:** resultado que el actor quiere alcanzar.
- **Sistema bajo estudio:** límite que separa lo que resuelve nuestro sistema de lo que pertenece al entorno.
- **Flujo principal:** secuencia normal de interacciones que lleva al objetivo.
- **Flujos alternativos y excepciones:** caminos que aparecen cuando hay una elección distinta, una condición especial o un error.
- **Precondiciones:** condiciones que deben cumplirse antes de comenzar, por ejemplo, que el paciente esté autenticado.
- **Postcondiciones:** estado que debe quedar garantizado al finalizar, por ejemplo, que el turno quede registrado.

> [!important] Para el oral
> Un caso de uso se centra en la **intención del actor y el valor obtenido**. Si la explicación se concentra en tablas, clases, pantallas o algoritmos, ya se está entrando en análisis, diseño o implementación.

## Modelo y especificación

El modelo de casos de uso suele representarse con un diagrama UML. Sirve para mostrar de forma global qué actores existen y qué objetivos pueden realizar con el sistema.

Sin embargo, el diagrama no alcanza para describir el comportamiento con precisión. Cada caso de uso importante necesita una especificación textual que detalle el flujo principal, alternativas, reglas de negocio y excepciones. El diagrama da la vista panorámica; la especificación permite analizar y validar el requisito.

Ejemplo breve de especificación:

| Elemento | Ejemplo: `Solicitar turno` |
| --- | --- |
| Actor principal | Paciente |
| Objetivo | Reservar un turno con un profesional |
| Precondición | El paciente inició sesión |
| Flujo principal | Elige especialidad, profesional y horario; el sistema valida disponibilidad y confirma la reserva |
| Alternativa | El horario ya no está disponible; el sistema ofrece otros horarios |
| Postcondición | El turno queda registrado y el paciente recibe confirmación |

## Relación con requisitos

Los casos de uso capturan principalmente **requisitos funcionales**: servicios o comportamientos que el sistema debe ofrecer a sus actores. No reemplazan a los requisitos no funcionales, como seguridad, rendimiento, disponibilidad, accesibilidad o privacidad.

En el ejemplo del turno médico, `Solicitar turno` expresa el comportamiento funcional. Que la confirmación tarde menos de dos segundos, que los datos estén protegidos o que una persona mayor pueda completar el flujo son restricciones de calidad que acompañan al caso de uso, pero no son casos de uso en sí mismos.

## Casos de uso en el Proceso Unificado

El [[Proceso Unificado de Desarrollo]] es guiado por casos de uso. Esto significa que los casos de uso son el hilo conductor entre las disciplinas y a lo largo de las iteraciones:

1. En **Inicio**, se identifican los actores y los casos de uso principales para delimitar alcance, estimar viabilidad y detectar riesgos.
2. En **Elaboración**, se detallan primero los casos de uso arquitectónicamente significativos o riesgosos; se valida que la arquitectura pueda soportarlos.
3. En **Construcción**, los casos de uso se implementan por incrementos y se integran con el resto del sistema.
4. En **Pruebas**, se verifica que cada flujo, alternativa y condición del caso de uso produzca el resultado esperado.

Por eso, no se trata de redactarlos una vez y archivarlos. Cada caso de uso importante se refina, se transforma en decisiones de análisis y diseño, orienta la implementación y luego da origen a pruebas de aceptación.

## Priorización y riesgo

No todos los casos de uso tienen la misma importancia. Conviene priorizar los que:

- aportan mayor valor al usuario o al negocio;
- atraviesan decisiones centrales de arquitectura;
- tienen reglas complejas o dependencias externas;
- concentran riesgos de seguridad, rendimiento o integración.

Un caso de uso como `Compartir historial médico con un profesional` puede ser crítico porque combina privacidad, autorización, interoperabilidad y facilidad de uso. Resolverlo temprano permite comprobar si la arquitectura y las decisiones de seguridad son viables antes de construir funcionalidades secundarias.

Esto conecta directamente con [[Riesgo y Entropía en Proyectos de Software]]: los casos de uso centrales ayudan a decidir qué incertidumbres se deben atacar primero.

## De los casos de uso al diseño orientado a objetos

Los casos de uso describen el sistema desde afuera; el [[Desarrollo Orientado a Objetos]] explica cómo organizar colaboraciones internas para cumplirlos.

Para realizar `Solicitar turno`, el análisis y diseño pueden identificar objetos como `Turno`, `Agenda`, `Profesional`, `Paciente` y `Notificación`. La transición no consiste en convertir cada sustantivo del texto en una clase. Consiste en asignar responsabilidades y colaboraciones que permitan cumplir el objetivo del actor con bajo acoplamiento y buena cohesión.

La cadena conceptual para explicar en el oral es:

```text
Actor y objetivo -> Caso de uso -> Requisito funcional ->
Análisis y diseño OO -> Implementación -> Pruebas
```

[[UML]] permite representar distintos puntos de esa cadena: el diagrama de casos de uso muestra la visión externa; los diagramas de secuencia, clases, estados o componentes sirven para profundizar la solución en análisis y diseño.

## Relaciones habituales en el diagrama

- **Asociación:** conecta un actor con el caso de uso en el que participa.
- **`<<include>>`:** un caso de uso incorpora obligatoriamente un comportamiento común. Sirve para no repetir una secuencia que varios casos necesitan.
- **`<<extend>>`:** agrega un comportamiento opcional o condicionado sobre un caso de uso base.
- **Generalización:** permite representar actores o casos de uso especializados que heredan comportamiento o relaciones más generales.

Estas relaciones deben usarse para aclarar el modelo, no para convertir el diagrama en una descripción técnica compleja. Cuando hay detalle de flujo, reglas y excepciones, corresponde a la especificación textual.

## Errores frecuentes

- Confundir el actor con una persona concreta en vez de un rol.
- Nombrar casos de uso con elementos de interfaz, por ejemplo `Pantalla de login`, en lugar de un objetivo como `Autenticarse`.
- Describir cómo se programa la solución en vez de qué valor obtiene el actor.
- Suponer que un diagrama sustituye la especificación de los flujos importantes.
- Ignorar escenarios alternativos y de excepción.
- Tratar todos los casos de uso como equivalentes, sin considerar valor, riesgo ni impacto arquitectónico.

## Cómo explicarlo oralmente

"Un caso de uso describe cómo un actor logra un objetivo de valor mediante el sistema. Es una forma de capturar requisitos funcionales desde una visión externa: todavía no define clases, pantallas ni tecnología. Se puede representar en un diagrama UML, pero los casos importantes también requieren una especificación con flujo principal, alternativas, precondiciones y postcondiciones. En el Proceso Unificado los casos de uso guían el proyecto: se identifican para delimitar alcance, se priorizan según valor y riesgo, orientan el análisis y diseño orientado a objetos, se implementan por iteraciones y se validan mediante pruebas."

## Preguntas probables de final

- ¿Qué es un caso de uso y qué problema resuelve?
- ¿Qué diferencia hay entre un actor y un usuario concreto?
- ¿Por qué un caso de uso no es una pantalla ni una clase?
- ¿Qué información debe contener la especificación de un caso de uso?
- ¿Qué diferencia hay entre requisito funcional y no funcional?
- ¿Cómo se relacionan los casos de uso con UML?
- ¿Qué significa que el Proceso Unificado sea guiado por casos de uso?
- ¿Por qué conviene implementar primero los casos de uso riesgosos o arquitectónicamente significativos?
- ¿Cómo se pasa de un caso de uso al análisis y diseño orientado a objetos?
- ¿Cuándo usaría `<<include>>` y cuándo `<<extend>>`?

## Respuesta corta para repasar

Un caso de uso es una descripción de cómo un actor obtiene un resultado de valor al interactuar con el sistema. Captura requisitos funcionales desde la perspectiva externa y se compone de actores, objetivo, flujo principal, alternativas, precondiciones y postcondiciones. En el Proceso Unificado guía las iteraciones: ayuda a definir alcance, priorizar riesgos, diseñar colaboraciones entre objetos, implementar incrementos y probar que el sistema cumpla lo esperado por el usuario.

## Conexiones importantes

- [[Proceso Unificado de Desarrollo]]
- [[Desarrollo Orientado a Objetos]]
- [[UML]]
- [[Arquitectura de Software]]
- [[Riesgo y Entropía en Proyectos de Software]]
- [[Ciclo de Vida Iterativo e Incremental]]

## Recursos

- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo_Introducción.pdf|Proceso Unificado de Desarrollo - Introducción]]
