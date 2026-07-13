---
title: Unidad 4 - Simulación Estocástica
tags:
  - uda/investigacion-operativa
  - unidad-iv
  - repaso-practico
aliases:
  - Simulación
  - Simulación estocástica
---

# Unidad 4 - Simulación Estocástica

La simulación estocástica permite estudiar sistemas con incertidumbre cuando el comportamiento depende de variables aleatorias. En lugar de obtener una solución exacta por una fórmula cerrada, se imita el funcionamiento del sistema y se observan resultados bajo distintos escenarios.

## Idea central

Simular es experimentar con un modelo. Si el sistema real es costoso, riesgoso o difícil de modificar, se crea una representación y se prueban alternativas.

Es especialmente útil cuando:

- hay incertidumbre;
- el sistema tiene muchas interacciones;
- la solución analítica es muy difícil;
- se quieren comparar políticas antes de implementarlas.

## Elementos

- Sistema: realidad que se quiere estudiar.
- Modelo: representación simplificada.
- Variables aleatorias: entradas inciertas.
- Distribuciones de probabilidad: describen el comportamiento de esas variables.
- Corridas de simulación: repeticiones del experimento.
- Métricas: resultados a observar.

## Etapas

1. Definir el problema.
2. Formular el modelo.
3. Recolectar datos.
4. Elegir distribuciones.
5. Ejecutar simulaciones.
6. Analizar resultados.
7. Validar si el modelo representa razonablemente el sistema.
8. Comparar alternativas.

## Relación con probabilidad

La simulación usa conceptos como variables aleatorias, funciones de probabilidad, valor esperado y variabilidad. Por eso se conecta con colas, inventarios con demanda aleatoria y toma de decisiones bajo incertidumbre.

## Errores típicos

- Simular sin validar datos.
- Sacar conclusiones con pocas corridas.
- Confundir un resultado simulado con certeza.
- No definir métricas antes de simular.
- Usar una distribución sin justificarla.

## Conexiones

- [[Investigación Operativa - Índice]]
- [[Unidad 5 - Fenómenos de Espera]]
- [[Unidad 7 - Modelos de Inventario]]

