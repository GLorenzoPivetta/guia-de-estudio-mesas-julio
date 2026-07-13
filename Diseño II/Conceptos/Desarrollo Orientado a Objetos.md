---
title: Desarrollo Orientado a Objetos
tags:
  - uda/diseno-ii
  - unidad-i
  - repaso-oral
aliases:
  - Desarrollo OO
  - Orientación a objetos
  - Analisis y diseño orientado a objetos
---

# Desarrollo Orientado a Objetos

El desarrollo orientado a objetos es una forma de analizar, diseñar y construir software modelando el sistema como una colaboración entre objetos. Cada objeto representa una entidad, concepto o responsabilidad relevante del dominio o de la solución.

La idea fuerte para Diseño II es que la orientación a objetos no es solo una técnica de programación. También es una forma de pensar el análisis y el diseño.

## Objeto

Un objeto combina estado y comportamiento.

El estado representa los datos que el objeto conoce. El comportamiento representa lo que el objeto puede hacer. En diseño, lo importante no es listar atributos mecánicamente, sino entender qué responsabilidad tiene cada objeto dentro del sistema.

Ejemplo: en un sistema de turnos médicos, un objeto `Turno` podría conocer fecha, hora, paciente y profesional, pero su responsabilidad conceptual puede ser reservar, cancelar, reprogramar o validar disponibilidad.

## Clase

Una clase describe una familia de objetos con la misma estructura y comportamiento. Es una abstracción: no representa un caso individual, sino el molde conceptual de muchos objetos posibles.

En análisis se identifican clases del dominio. En diseño se refinan clases para que puedan colaborar y sostener la solución técnica.

## Abstracción

Abstraer significa quedarse con lo importante para el problema y dejar afuera detalles innecesarios.

En un oral, conviene explicar que una buena abstracción depende del contexto. Una persona puede ser `Paciente` en un sistema de salud, `Alumno` en un sistema académico o `Cliente` en un sistema comercial.

## Encapsulamiento

El encapsulamiento busca proteger el estado interno de un objeto y exponer operaciones claras para usarlo. Esto reduce acoplamiento, porque otros objetos no necesitan conocer todos sus detalles internos.

La idea no es ocultar por ocultar, sino controlar cómo se modifica y consulta la información.

## Responsabilidades y colaboración

Diseñar orientado a objetos implica repartir responsabilidades. Cada objeto debe tener una razón clara para existir y debe colaborar con otros mediante mensajes u operaciones.

Esta mirada conecta con patrones y principios de diseño, porque muchos patrones intentan resolver problemas de asignación de responsabilidades, acoplamiento, cohesión y flexibilidad.

## Relación con UML

[[UML]] se usa para representar modelos orientados a objetos: clases, relaciones, interacciones, estados, componentes y despliegue, entre otros.

Para el examen, no alcanza con decir "UML dibuja diagramas". Hay que poder explicar que UML ayuda a comunicar decisiones de análisis y diseño entre miembros del equipo.

## Relación con Proceso Unificado

El [[Proceso Unificado de Desarrollo]] se apoya fuertemente en análisis y diseño orientado a objetos. Los casos de uso ayudan a capturar comportamiento desde la perspectiva del usuario, y los modelos de análisis y diseño transforman esos requisitos en objetos, responsabilidades, clases, colaboraciones y arquitectura.

## Cómo explicarlo oralmente

"El desarrollo orientado a objetos modela el sistema como objetos que combinan estado y comportamiento. No es solamente programar con clases, sino analizar el dominio, identificar abstracciones relevantes y asignar responsabilidades. Un buen diseño orientado a objetos busca objetos cohesivos, con bajo acoplamiento y colaboraciones claras. UML ayuda a representar esos modelos, y el Proceso Unificado los usa dentro de sus actividades de análisis y diseño."

## Conexiones importantes

- [[Ciclos de Vida del Software]]
- [[Proceso Unificado de Desarrollo]]
- [[UML]]
- [[Casos de Uso]]
- [[Arquitectura de Software]]
- [[Riesgo y Entropía en Proyectos de Software]]

## Preguntas probables

- ¿Qué es un objeto?
- ¿Qué diferencia hay entre objeto y clase?
- ¿Qué significa abstracción en OO?
- ¿Por qué el encapsulamiento reduce acoplamiento?
- ¿Qué quiere decir asignar responsabilidades?
- ¿Cómo se conecta OO con UML y Proceso Unificado?

## Recursos

- [[../Recursos/CV Introduccion/Schach_Ing de Software Clásica y OO_Cap 2.pdf|Schach - Ingeniería de Software Clásica y OO, Cap. 2]]

