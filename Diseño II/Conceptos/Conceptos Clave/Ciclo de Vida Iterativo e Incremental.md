---
title: Ciclo de Vida Iterativo e Incremental
tags:
  - uda/diseno-ii
  - unidad-i
  - repaso-oral
aliases:
  - Iterativo e incremental
  - Ciclo iterativo
  - Ciclo incremental
---

# Ciclo de Vida Iterativo e Incremental

Un ciclo de vida iterativo e incremental organiza el desarrollo en ciclos repetidos que producen avances evaluables. En lugar de esperar hasta el final para ver el sistema funcionando, el equipo construye partes, prototipos o incrementos que permiten aprender, validar y corregir.

Es una respuesta directa a los límites de [[Modelo en Cascada]] cuando hay incertidumbre.

## Iterativo

Iterativo significa que el trabajo se repite en ciclos. En cada iteración se pueden realizar actividades de requisitos, análisis, diseño, implementación, integración y pruebas.

La repetición no implica volver siempre al punto cero. Implica revisar decisiones, mejorar el entendimiento del problema y ajustar la solución.

Una iteración sirve para responder preguntas como:

- ¿entendimos bien el requisito?
- ¿la arquitectura soporta este caso de uso?
- ¿el usuario valida este flujo?
- ¿el riesgo técnico era real?
- ¿hay que corregir el diseño?

## Incremental

Incremental significa que cada ciclo agrega algo: funcionalidad, conocimiento validado, una parte integrada del sistema, un prototipo o una versión más completa.

El incremento permite medir avance con evidencia concreta. No se avanza solo porque se escribieron documentos, sino porque hay algo que puede demostrarse, probarse o validarse.

## Prototipado y feedback

El prototipo ejecutable coloca al usuario en una situación de uso concreta. Eso mejora la comunicación, porque el usuario no responde sobre abstracciones sino sobre algo que puede ver, tocar o recorrer.

Las ventajas principales son:

- feedback temprano;
- mejor comprensión de necesidades reales;
- mayor compromiso del usuario;
- integración progresiva;
- reducción del efecto "big bang";
- avance medido por software demostrable.

## Mitos comunes

Un ciclo iterativo no significa improvisar.

La cátedra remarca tres mitos:

- Mito: el ciclo iterativo genera problemas. Realidad: revela problemas antes.
- Mito: es una excusa para no planificar. Realidad: exige planificación continua.
- Mito: agrega necesidades sin fin. Realidad: permite priorizar primero lo principal y después lo secundario.

## Relación con Proceso Unificado

[[Proceso Unificado de Desarrollo]] usa este enfoque. El proyecto se divide en fases, pero dentro de cada fase hay iteraciones. Cada iteración produce un avance y ayuda a reducir riesgos.

La diferencia con un enfoque ágil liviano es que el Proceso Unificado mantiene una estructura más formal: fases, hitos, arquitectura, casos de uso y artefactos.

## Cómo explicarlo oralmente

"Un ciclo iterativo e incremental divide el desarrollo en ciclos. Es iterativo porque repite actividades como análisis, diseño, implementación y pruebas para aprender y corregir. Es incremental porque cada ciclo agrega una parte validable del sistema o del conocimiento del proyecto. Su ventaja frente a cascada es que permite obtener feedback temprano, integrar progresivamente y detectar riesgos antes. No elimina la planificación: la vuelve continua."

## Conexiones importantes

- [[Ciclos de Vida del Software]]
- [[Modelo en Cascada]]
- [[Proceso Unificado de Desarrollo]]
- [[Riesgo y Entropía en Proyectos de Software]]
- [[Desarrollo Orientado a Objetos]]

## Preguntas probables

- ¿Qué diferencia hay entre iterativo e incremental?
- ¿Por qué cada iteración puede verse como una minicascada?
- ¿Qué ventaja tiene el prototipado?
- ¿Por qué iterar no significa falta de planificación?
- ¿Cómo se relaciona con el Proceso Unificado?

## Recursos

- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo_Introducción.pdf|Proceso Unificado de Desarrollo - Introducción]]
- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo. La Iteración Genérica.pdf|Proceso Unificado de Desarrollo - Iteración genérica]]
