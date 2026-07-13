---
title: Unidad 2 - Programación Lineal
tags:
  - uda/investigacion-operativa
  - unidad-ii
  - repaso-practico
aliases:
  - PL
  - Programación Lineal
---

# Unidad 2 - Programación Lineal

La programación lineal busca optimizar una función objetivo lineal sujeta a restricciones lineales. Es uno de los temas centrales de Investigación Operativa porque permite modelar decisiones de producción, mezcla, asignación de recursos y planificación.

## Componentes de un modelo

- Variables de decisión: lo que el modelo debe decidir.
- Función objetivo: lo que se maximiza o minimiza.
- Restricciones: límites de recursos, demanda, capacidad, proporciones o condiciones.
- Condiciones de no negatividad: normalmente las variables no pueden ser negativas.

## Forma general

Un problema típico de maximización:

$$
\max Z = c_1x_1 + c_2x_2 + ... + c_nx_n
$$

sujeto a:

$$
a_{11}x_1 + a_{12}x_2 + ... + a_{1n}x_n \leq b_1
$$

con:

$$
x_i \geq 0
$$

## Resolución gráfica

Se usa cuando hay dos variables. Los pasos son:

1. Graficar cada restricción.
2. Identificar la región factible.
3. Hallar los vértices.
4. Evaluar la función objetivo en cada vértice.
5. Elegir el valor óptimo.
6. Interpretar el resultado.

## Simplex

El método simplex resuelve problemas de mayor dimensión recorriendo soluciones básicas factibles. En cada iteración mejora el valor de la función objetivo hasta llegar a una solución óptima o detectar un caso especial.

Conceptos clave:

- Variables de holgura: convierten restricciones `<=` en igualdades.
- Variables de exceso: aparecen en restricciones `>=`.
- Base: conjunto de variables activas en una solución básica.
- Solución básica factible: solución que cumple restricciones y no negatividad.
- Variable entrante y saliente: definen el cambio de base.

## Tipos de solución

- Única: hay un solo óptimo.
- Alternativa: existen múltiples soluciones óptimas.
- Infactible: no hay región factible.
- No acotada: la función objetivo puede crecer o decrecer sin límite.
- Degenerada: alguna variable básica vale cero.

## Dualidad y sensibilidad

El dual permite interpretar el valor de los recursos. En problemas de maximización con restricciones de recursos, las variables duales suelen representar precios sombra: cuánto mejora el objetivo si aumenta una unidad de recurso.

El análisis de sensibilidad estudia qué pasa si cambian coeficientes de la función objetivo o disponibilidad de recursos.

## Procedimiento mínimo de práctica

Para cada ejercicio:

1. Definir variables con unidades.
2. Escribir función objetivo.
3. Escribir restricciones.
4. Resolver por gráfico, simplex o Solver.
5. Identificar tipo de solución.
6. Interpretar resultado y recursos agotados.

## Errores típicos

- Definir variables ambiguas.
- Cambiar unidades entre restricciones.
- Olvidar no negatividad.
- Confundir `<=` con `>=`.
- No interpretar holguras.
- Presentar el óptimo sin explicar qué significa.

## Conexiones

- [[Investigación Operativa - Índice]]
- [[Unidad 6 - Logística Transporte y Asignación]]
- [[Unidad 8 - Teoría de Juegos]]

