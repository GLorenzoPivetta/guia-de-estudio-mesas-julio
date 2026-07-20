---
title: Proceso Unificado de Desarrollo
tags:
  - uda/diseno-ii
  - unidad-i
  - unidad-ii
  - repaso-oral
aliases:
  - PUD
  - Proceso Unificado
---

# Proceso Unificado de Desarrollo

El Proceso Unificado de Desarrollo ==es una metodologia de desarrollo de software iterativa e incremental==. Su objetivo es ordenar el trabajo para transformar una idea inicial en un sistema operativo, reduciendo riesgos, validando decisiones importantes y produciendo avances concretos en cada iteracion.

No se trabaja como en un ciclo lineal donde primero se termina todo el análisis, después todo el diseño y después toda la implementación. En cambio, en cada iteracion se recorren las actividades principales del desarrollo y se obtiene un incremento del producto o del conocimiento del proyecto.

## Idea central

==La idea mas importante es que el proyecto avanza por fases, pero dentro de cada fase hay iteraciones.== Cada iteracion combina actividades como modelado del negocio, requerimientos, análisis, diseño, implementación y pruebas, aunque ==el peso de cada actividad cambia según la fase.==

Esto permite revisar, corregir y mejorar decisiones anteriores. Por eso se dice que es:

- Iterativo: repite ciclos de trabajo.
- Incremental: cada ciclo agrega avance o conocimiento.
- ==Dirigido por riesgos: prioriza resolver primero lo mas incierto o peligroso.==
- ==Centrado en la arquitectura: busca estabilizar una base tecnica antes de construir todo el sistema.==
- Guiado por casos de uso: los requisitos funcionales se organizan desde la interacción entre actores y sistema.

## Por que hace falta una metodologia

Una metodologia busca que el desarrollo sea mas fiable y reproducible. En software aparecen problemas como requisitos complejos, tecnologia heterogenea, costos altos de mantenimiento y dependencia de desarrolladores "heroicos" que concentran demasiado conocimiento.

El Proceso Unificado intenta combatir esa entropia organizando el trabajo, propagando conocimiento dentro del equipo y obligando a tomar decisiones explicitas sobre alcance, arquitectura, riesgos y calidad.

## Actividades principales

Las actividades fundamentales son:

- Modelado de negocios: entender el contexto, procesos, objetivos y actores del dominio.
- Requerimientos: identificar que necesita el usuario y que debe hacer el sistema.
- Analisis y diseno: transformar requisitos en una solucion conceptual y tecnica.
- Implementacion: construir componentes ejecutables.
- Pruebas: verificar que lo construido cumple los requisitos y tiene la calidad esperada.

Estas actividades no desaparecen en ninguna fase. Lo que cambia es la intensidad. En Inicio pesan mas la viabilidad y el alcance; en Elaboracion pesan la arquitectura y los riesgos; en Construccion pesa la implementacion; en Transicion pesan despliegue, validacion, correccion y capacitacion.

## Fases e hitos

### Inicio

La fase de Inicio pone en marcha el proyecto. ==Busca responder si el proyecto es factible, cuales son sus limites, cual es su alcance y cuales son los riesgos críticos.==

Su objetivo no es tener todo el sistema definido en detalle, sino justificar que vale la pena realizarlo y comenzar a transformar una idea en un sistema tangible.

==En esta fase se identifican actores, interacciones actor-sistema, casos de uso principales, requisitos funcionales y no funcionales iniciales, una arquitectura candidata y los riesgos mas importantes.==

==El hito de Inicio es lograr una vision suficientemente clara del proyecto para decidir si conviene avanzar.== En términos de examen, se puede expresar como alcanzar una base de especificaciones funcionales y viabilidad que permita estimar contrato, costo y tiempo con mas seriedad.

### Elaboración

La fase de Elaboración ==tiene como objetivo principal formular la linea base de la arquitectura.== Esto significa estabilizar las decisiones estructurales del sistema para que Construcción no avance sobre una base débil.

En esta fase ==se recopilan requisitos pendientes, se afianza la arquitectura, se hace seguimiento de riesgos críticos y se detalla el plan del proyecto.==

==Una pregunta clave de Elaboración es si la arquitectura va a soportar la Construcción y futuras versiones==. También se evalúa si los riesgos críticos fueron mitigados o si existe un plan creíble para tratarlos.

El hito de Elaboración es la arquitectura validada. ==Si este hito esta bien logrado, el equipo puede comprometerse con mayor confianza a construir el sistema.==

### Construcción

==La fase de Construcción busca obtener una version operativa inicial, muchas veces llamada version beta.==

==Aquí se implementa la mayor parte de los casos de uso==, se completan modelos de análisis, diseño e implementación, se ajusta la arquitectura cuando haga falta, se integran componentes y se prueba el sistema completo.

Tambien se actualiza la lista de riesgos. Al final de esta fase, los riesgos importantes deberían estar mitigados, salvo los vinculados con operación real.

==El hito de Construcción es una version beta integrada y suficientemente completa como para ser probada en condiciones cercanas a la realidad.==

### Transición

==La fase de Transición gestiona la puesta en producción en el entorno del usuario.==

Incluye despliegue, corrección de defectos encontrados en la beta, migración de datos, validación con usuarios, documentación, capacitación y soporte.

Tambien gestiona cambios menores solicitados por el usuario, mientras que cambios mayores suelen reservarse para versiones futuras para no romper el plan del proyecto.

==El hito de Transición es dejar el sistema operacional. No se trata solo de que el código compile, sino de que el usuario pueda usarlo en su contexto real.==

## Iteracion generica

==Una iteracion tiene planificación, ejecución de flujos de trabajo y evaluación. Segun la fase, esa iteracion se orienta a objetivos distintos.==

==En Inicio, la iteracion apunta a analizar el negocio==, evaluar viabilidad, delimitar el sistema, esbozar arquitectura, identificar riesgos críticos y crear prototipos exploratorios.

==En Elaboración, la iteracion apunta a estabilizar arquitectura==, planificar Construcción, estimar costos con mas precision, mitigar riesgos, definir niveles de calidad, recopilar una parte importante de los casos de uso e identificar recursos necesarios.

==En Construcción, la iteracion apunta a implementar casos de uso==, finalizar análisis y diseño, monitorear riesgos, crear la version beta y cuidar la integridad de la arquitectura.

==En Transición, la iteracion apunta a preparar el entorno==, cerrar documentación, ajustar parámetros de producción, corregir errores finales y registrar lecciones aprendidas.

## Controlado (o guiado) por Casos de Uso

En el PUD, los [[Casos de Uso]] (CU) no son solo una lista de requisitos que se lee y se guarda; son el **hilo conductor de todo el ciclo de vida**.

- **Definición:** ==Los CU dictan la funcionalidad del sistema desde la perspectiva del usuario y guían todas las disciplinas==: el análisis, el diseño, la implementación y las pruebas giran en torno a cumplir esos casos de uso.
- **Priorización:** No todos los CU valen lo mismo. En el PUD, los CU se clasifican meticulosamente para decidir en qué orden se abordarán. Se dividen en **Críticos** (fundamentales para el usuario o con altos requisitos de rendimiento), **Secundarios** (apoyo a los críticos), **Auxiliares** y **Opcionales**
## Como explicarlo oralmente

Una forma solida de explicarlo en el final:

"El Proceso Unificado organiza el desarrollo en fases e iteraciones. Las fases marcan grandes objetivos del proyecto: Inicio define viabilidad y alcance, Elaboracion estabiliza la arquitectura, Construccion produce una version beta y Transicion lleva el sistema a produccion. Dentro de cada fase hay iteraciones que recorren requerimientos, analisis, diseno, implementacion y pruebas, pero con distinto peso segun el momento del proyecto. La ventaja es que permite reducir riesgos temprano, validar la arquitectura y avanzar por incrementos en lugar de apostar todo a una entrega final."

## Conexiones importantes

- [[Unidad I - Desarrollo OO y Ciclos de Vida]]: aporta la base para entender por que el Proceso Unificado prefiere iteraciones, incrementos, arquitectura y gestion temprana de riesgos.
- [[Ingeniería de Software y Metodologías]]: explica por que hace falta formalizar actividades de desarrollo.
- [[Ciclos de Vida del Software]]: ubica al Proceso Unificado dentro de los enfoques iterativos e incrementales.
- [[Ciclo de Vida Iterativo e Incremental]]: desarrolla la diferencia entre repetir ciclos y agregar avances.
- [[RUP]]: RUP es una version o marco mas concreto basado en el Proceso Unificado, con roles, artefactos, actividades y disciplinas mas definidos.
- [[UML]]: UML sirve para representar visualmente distintos aspectos del sistema durante las actividades de analisis y diseno.
- [[Casos de Uso]]: guian los requisitos y ayudan a organizar las funcionalidades desde el punto de vista de los actores.
- [[Arquitectura de Software]]: es central en Elaboracion, porque condiciona el resto del desarrollo.
- [[Riesgo y Entropía en Proyectos de Software]]: el proceso prioriza identificar y mitigar riesgos temprano.
- [[Metodologias Agiles]]: comparten la idea de iterar, pero suelen ser mas livianas y adaptativas que un proceso unificado formal.
- [[Design Thinking]]: puede usarse antes o durante el proceso cuando el problema es ambiguo y requiere entender mejor a las personas.

## Preguntas probables de final

- **Que significa que el Proceso Unificado sea iterativo e incremental.**
- **Que diferencia hay entre fase e iteracion.**
- **Cuales son las cuatro fases y cual es el hito de cada una.**
- **Por que la arquitectura es tan importante en Elaboracion.**
- **Que relacion hay entre casos de uso, UML y Proceso Unificado.**
- **Que riesgos se buscan reducir en Inicio y Elaboracion.**
- **Que diferencia hay entre Construccion y Transicion.**
- **En que se parece y en que se diferencia de una metodologia agil.**

## Respuesta corta para repasar

El Proceso Unificado es una metodologia iterativa e incremental que organiza el desarrollo en cuatro fases: Inicio, Elaboracion, Construccion y Transicion. Cada fase tiene un hito: viabilidad y alcance, arquitectura estable, version beta y sistema operacional. En cada iteracion se recorren actividades como requerimientos, analisis, diseno, implementacion y pruebas, pero con distinto peso segun la fase. Sirve para controlar la complejidad, reducir riesgos, validar la arquitectura y construir el sistema por incrementos.

## Recursos

- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo_Introducción.pdf|Proceso Unificado de Desarrollo - Introduccion]]
- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo. Inicio.pdf|Proceso Unificado de Desarrollo - Inicio]]
- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo. Elaboración.pdf|Proceso Unificado de Desarrollo - Elaboracion]]
- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo. Construcción.pdf|Proceso Unificado de Desarrollo - Construccion]]
- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo. Transición.pdf|Proceso Unificado de Desarrollo - Transicion]]
- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo. La Iteración Genérica.pdf|Proceso Unificado de Desarrollo - Iteracion generica]]
