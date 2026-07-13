---
title: Ciclos de Vida del Software
tags:
  - uda/diseno-ii
  - unidad-i
  - repaso-oral
aliases:
  - Ciclo de vida del software
  - CV del software
---

# Ciclos de Vida del Software

Un ciclo de vida del software describe cómo evoluciona un proyecto desde la identificación de una necesidad hasta la entrega, operación y mantenimiento del sistema. Sirve para ordenar el avance del trabajo y definir cuándo se hacen actividades como requisitos, análisis, diseño, implementación, integración y pruebas.

La discusión central de la unidad es la diferencia entre ciclos lineales y ciclos iterativos.

## Ciclos lineales

Los ciclos lineales organizan el proyecto como una secuencia de etapas. Primero se definen requisitos, después se analiza, luego se diseña, se implementa, se prueba y finalmente se entrega.

La ventaja principal es la claridad: cada etapa tiene una salida esperada y el avance parece fácil de controlar.

El problema aparece cuando los requisitos cambian o cuando el usuario recién entiende lo que necesita al ver el sistema funcionando. Si el producto ejecutable aparece muy tarde, los errores de interpretación también aparecen tarde.

El ejemplo clásico es [[Modelo en Cascada]].

## Ciclos iterativos

Los ciclos iterativos se basan en repetir ciclos de trabajo. Cada iteración puede incluir requisitos, análisis, diseño, implementación, integración y pruebas, pero sobre una parte acotada del sistema.

Cada iteración produce aprendizaje. El equipo puede evaluar lo construido, corregir decisiones y ajustar el rumbo.

En los materiales de la cátedra aparece una idea clave: cada iteración puede entenderse como una "minicascada", pero con un alcance menor y con evaluación más temprana.

## Ciclos incrementales

Un ciclo incremental produce avances concretos del producto. No solo repite trabajo: agrega funcionalidad, conocimiento validado o una versión más completa del sistema.

Iterativo e incremental suelen ir juntos, pero no significan exactamente lo mismo:

- Iterativo: repite ciclos de trabajo para aprender y corregir.
- Incremental: agrega partes o mejoras al producto.

[[Proceso Unificado de Desarrollo]] es iterativo e incremental porque organiza el proyecto en fases, pero dentro de cada fase realiza iteraciones que producen avances.

## Prototipos ejecutables

En un enfoque iterativo, el avance se mide mejor con software demostrable que con documentos aislados. Un prototipo ejecutable permite que el usuario se coloque en una situación concreta de uso y dé feedback más preciso.

Esto reduce el riesgo de construir correctamente algo que no era lo que el usuario necesitaba.

## Comparación para oral

| Enfoque | Idea principal | Ventaja | Riesgo |
|---|---|---|---|
| Lineal | Etapas sucesivas | Orden y visibilidad documental | El sistema aparece tarde |
| Cascada | Una fase termina antes de iniciar la siguiente | Control formal | Reacciona mal al cambio |
| Iterativo | Repetir ciclos de trabajo | Aprendizaje temprano | Requiere planificación continua |
| Incremental | Agregar valor por partes | Avance demostrable | Necesita controlar integración y alcance |

## Cómo explicarlo oralmente

"Un ciclo de vida define cómo avanza un proyecto de software. En los ciclos lineales, las etapas se suceden una detrás de otra, lo que da orden pero puede ser riesgoso si el usuario cambia requisitos o si los errores se descubren tarde. En los ciclos iterativos, el proyecto avanza por ciclos cortos que permiten revisar y corregir. En los incrementales, cada ciclo agrega una parte del producto o del conocimiento validado. Por eso los enfoques iterativos e incrementales son más adecuados cuando hay incertidumbre."

## Conexiones importantes

- [[Modelo en Cascada]]
- [[Ciclo de Vida Iterativo e Incremental]]
- [[Ingeniería de Software y Metodologías]]
- [[Proceso Unificado de Desarrollo]]
- [[Riesgo y Entropía en Proyectos de Software]]

## Preguntas probables

- ¿Qué es un ciclo de vida?
- ¿Qué diferencia hay entre lineal, iterativo e incremental?
- ¿Por qué el sistema completo aparece tarde en cascada?
- ¿Qué ventaja tiene un prototipo ejecutable?
- ¿Por qué un ciclo iterativo no significa falta de planificación?

## Recursos

- [[../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo_Introducción.pdf|Proceso Unificado de Desarrollo - Introducción]]

