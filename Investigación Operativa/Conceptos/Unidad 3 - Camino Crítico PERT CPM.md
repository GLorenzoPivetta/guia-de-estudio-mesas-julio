---
title: Unidad 3 - Camino Crítico PERT CPM
tags:
  - uda/investigacion-operativa
  - unidad-iii
  - repaso-practico
aliases:
  - Camino crítico
  - PERT
  - CPM
---

# Unidad 3 - Camino Crítico PERT CPM

PERT y CPM son técnicas para planificar y controlar proyectos mediante redes de actividades. Permiten estimar duración total, detectar actividades críticas y analizar el efecto de retrasos o aceleraciones.

## Conceptos base

- Proyecto: conjunto de actividades orientadas a un objetivo.
- Actividad: tarea con duración y precedencias.
- Precedencia: relación que indica qué debe terminar antes de iniciar otra actividad.
- Red: representación gráfica o matricial del proyecto.
- Camino: secuencia de actividades conectadas.
- Camino crítico: camino de mayor duración; determina la duración mínima del proyecto.

## Fechas y holguras

En un ejercicio típico se calculan:

- Inicio temprano.
- Fin temprano.
- Inicio tardío.
- Fin tardío.
- Holgura o margen.

Una actividad crítica tiene holgura cero. Si se retrasa, retrasa el proyecto completo.

## PERT

PERT usa estimaciones probabilísticas de duración. Suele trabajar con tres tiempos:

- Optimista.
- Más probable.
- Pesimista.

La duración esperada se calcula como una ponderación. Se usa cuando hay incertidumbre en las duraciones.

## CPM

CPM suele trabajar con duraciones conocidas o estimadas de forma determinística. Se enfoca en identificar el camino crítico, controlar tiempos y analizar aceleración de actividades.

## Procedimiento de resolución

1. Listar actividades.
2. Identificar precedencias.
3. Dibujar la red.
4. Calcular fechas tempranas hacia adelante.
5. Calcular fechas tardías hacia atrás.
6. Calcular holguras.
7. Identificar camino crítico.
8. Interpretar duración del proyecto y actividades sensibles.

## Errores típicos

- Dibujar mal las precedencias.
- Confundir actividad con nodo.
- Calcular hacia atrás usando un valor incorrecto de fin del proyecto.
- Decir que una actividad es crítica sin justificar holgura cero.
- Olvidar interpretar qué pasa si se retrasa una actividad no crítica.

## Conexiones

- [[Investigación Operativa - Índice]]
- [[Unidad 1 - Introducción a la Investigación Operativa]]
- [[Unidad 4 - Simulación Estocástica]]

