---
title: Unidad 7 - Modelos de Inventario
tags:
  - uda/investigacion-operativa
  - unidad-vii
  - repaso-practico
aliases:
  - Inventarios
  - Modelos de inventario
---

# Unidad 7 - Modelos de Inventario

Los modelos de inventario ayudan a decidir cuánto pedir, cuándo pedir y qué costo tiene mantener stock. Buscan equilibrar costos de compra, pedido, almacenamiento, faltantes y nivel de servicio.

## Conceptos base

- Stock: cantidad disponible.
- Demanda: consumo o requerimiento.
- Reaprovisionamiento: reposición del inventario.
- Costo de pedido: costo de emitir una orden.
- Costo de almacenamiento: costo de mantener unidades en stock.
- Costo de ruptura: costo de no poder satisfacer demanda.
- Stock de seguridad: inventario adicional para cubrir incertidumbre.

## Modelos determinísticos

Asumen demanda conocida o constante. Permiten calcular políticas de reposición cuando el comportamiento es estable.

Casos del programa:

- demanda constante;
- demanda constante con stock de seguridad;
- ruptura permitida;
- modelo generalizado;
- precio de adquisición variable según tamaño del lote.

## Modelos aleatorios

Incorporan incertidumbre en la demanda. Se usan cuando no se conoce exactamente cuánto se va a necesitar.

Casos del programa:

- demanda aleatoria con costo por sobrante y ruptura;
- demanda aleatoria con costo de almacenamiento y ruptura.

## Interpretación

Inventario no es solo "tener productos". Es una decisión económica: demasiado stock inmoviliza capital y genera costos; poco stock aumenta rupturas, demoras y pérdida de servicio.

## Errores típicos

- Mezclar demanda determinística y aleatoria.
- No distinguir costo de pedido y costo de almacenamiento.
- Olvidar el costo de ruptura.
- Calcular una cantidad óptima sin interpretar la política.
- No explicar qué representa el stock de seguridad.

## Conexiones

- [[Investigación Operativa - Índice]]
- [[Unidad 5 - Fenómenos de Espera]]
- [[Unidad 6 - Logística Transporte y Asignación]]

