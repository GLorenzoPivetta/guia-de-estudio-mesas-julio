---
title: Unidad 6 - Logística Transporte y Asignación
tags:
  - uda/investigacion-operativa
  - unidad-vi
  - repaso-practico
aliases:
  - Transporte
  - Asignación
  - Logística y transporte
---

# Unidad 6 - Logística Transporte y Asignación

La unidad estudia problemas donde se deben distribuir recursos desde orígenes hacia destinos minimizando costos o maximizando beneficios. Transporte y asignación son casos especiales de [[Unidad 2 - Programación Lineal]].

## Problema de transporte

Tiene:

- orígenes con oferta;
- destinos con demanda;
- costos de transportar de cada origen a cada destino;
- objetivo de minimizar costo total.

Si oferta total y demanda total no coinciden, se agrega un origen o destino artificial.

## Primera solución

Métodos habituales:

- Regla del Noroeste.
- Costos mínimos.
- Costos mínimos progresivos.

La primera solución debe ser factible, pero no necesariamente óptima.

## Optimización

Después de obtener una solución inicial, se verifica si puede mejorarse. La idea es detectar rutas que reduzcan el costo total y ajustar asignaciones sin violar oferta ni demanda.

## Problema de asignación

Es un caso particular donde se asignan recursos a tareas uno a uno. Puede plantearse para minimización o maximización.

Ejemplos:

- trabajadores a tareas;
- máquinas a trabajos;
- personas a turnos;
- proyectos a equipos.

## Logística

La logística analiza el flujo de bienes, información y recursos. Incluye transporte, inventario, almacenamiento, distribución y servicio.

Un punto importante es que hay costos contrapuestos: mejorar el servicio de transporte puede aumentar costos, pero reducir inventario o tiempos de entrega.

## Errores típicos

- No balancear oferta y demanda.
- Creer que la primera solución es óptima.
- Confundir transporte con asignación.
- No interpretar qué representa una celda artificial.
- Resolver la tabla sin explicar el costo total.

## Conexiones

- [[Investigación Operativa - Índice]]
- [[Unidad 2 - Programación Lineal]]
- [[Unidad 7 - Modelos de Inventario]]

