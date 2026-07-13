---
title: Unidad 5 - Fenómenos de Espera
tags:
  - uda/investigacion-operativa
  - unidad-v
  - repaso-practico
aliases:
  - Colas
  - Teoría de colas
  - Fenómenos de espera
---

# Unidad 5 - Fenómenos de Espera

Los fenómenos de espera estudian sistemas donde clientes, trabajos, pedidos o procesos llegan a recibir un servicio y pueden formar cola. El objetivo es analizar el equilibrio entre costo de espera y costo de capacidad de servicio.

## Estructura básica

Un sistema de espera tiene:

- población fuente;
- patrón de llegadas;
- cola;
- servidores;
- patrón de servicio;
- disciplina de atención;
- salida del sistema.

## Llegadas y servicio

En muchos modelos se asume:

- Llegadas con distribución de Poisson.
- Tiempos de servicio con distribución exponencial.

La tasa de llegada suele representarse con $\lambda$ y la tasa de servicio con $\mu$.

## Estados

- Estado transitorio: el sistema todavía no estabilizó su comportamiento.
- Estado estacionario: las medidas promedio se estabilizan en el tiempo.

## Medidas de desempeño

Según el modelo, se analizan:

- cantidad promedio en el sistema;
- cantidad promedio en cola;
- tiempo promedio en el sistema;
- tiempo promedio en cola;
- utilización del servidor;
- probabilidad de que el sistema esté vacío u ocupado.

## Interpretación

La teoría de colas no busca eliminar toda espera. Busca encontrar una relación razonable entre nivel de servicio y costo. Aumentar servidores reduce esperas, pero aumenta costo.

## Errores típicos

- Confundir $\lambda$ con $\mu$.
- No verificar condición de estabilidad.
- Interpretar utilización alta como siempre positiva.
- Olvidar distinguir tiempo en cola y tiempo total en sistema.
- Aplicar fórmulas sin identificar el modelo.

## Conexiones

- [[Investigación Operativa - Índice]]
- [[Unidad 4 - Simulación Estocástica]]
- [[Unidad 7 - Modelos de Inventario]]

