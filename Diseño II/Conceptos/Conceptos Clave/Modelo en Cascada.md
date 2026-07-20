---
title: Modelo en Cascada
tags:
  - uda/diseno-ii
  - unidad-i
  - repaso-oral
aliases:
  - Waterfall
  - Cascada
---

# Modelo en Cascada

El modelo en cascada es un ciclo de vida lineal y secuencial. Propone que el desarrollo avance por etapas ordenadas: requisitos, análisis, diseño, implementación, pruebas y entrega. ==Cada fase se apoya en la anterior y, en su versión más rígida, se pasa a la siguiente cuando la anterior está terminada.==

Su atractivo está en que da una sensación fuerte de control. Si cada etapa produce documentos o artefactos claros, el avance del proyecto parece visible y administrable.

## Idea central

La metáfora de cascada indica que el flujo va hacia abajo: una fase alimenta a la siguiente. Esto funciona razonablemente bien cuando:

- el problema es conocido;
- los requisitos son estables;
- la tecnología no introduce demasiada incertidumbre;
- el usuario puede definir con precisión lo que necesita desde el inicio;
- el costo de cambiar decisiones tarde es bajo o está muy controlado.

## Problema principal

El problema del modelo en cascada es que el sistema completo aparece muy tarde. ==Durante buena parte del proyecto, el usuario ve documentos, diagramas o especificaciones, pero no una solución ejecutable==.

Si hubo un malentendido en requisitos o diseño, puede descubrirse recién cuando ya se invirtió mucho trabajo. Por eso cascada ==se vuelve riesgoso en proyectos con incertidumbre, cambios frecuentes o usuarios que necesitan ver el producto para comprender mejor sus necesidades==.

## Relación con documentación

Cascada no es malo simplemente por documentar. La documentación puede ser necesaria. El riesgo aparece cuando la documentación reemplaza el aprendizaje con el sistema real.

En un oral conviene evitar una respuesta simplista como "cascada es malo". Es mejor decir: "cascada puede funcionar en contextos estables y bien conocidos, pero es débil frente al cambio y la incertidumbre".

## Comparación con iterativo

En cascada, se busca cerrar una etapa antes de avanzar. En un ciclo iterativo, se recorren varias actividades en ciclos más pequeños, produciendo prototipos o incrementos evaluables.

La diferencia fuerte es el momento del feedback:

- Cascada: feedback fuerte al final o cerca de la entrega.
- Iterativo: feedback temprano y repetido.

## Cómo explicarlo oralmente

"El modelo en cascada es un ciclo de vida lineal donde el proyecto avanza por fases sucesivas: primero requisitos, luego análisis, diseño, implementación, pruebas y entrega. Su ventaja es que ordena el trabajo y hace visible el avance mediante documentos y entregables. Su debilidad es que el sistema ejecutable aparece tarde; si los requisitos estaban mal entendidos o cambian, el costo de corregir puede ser alto. Por eso sirve mejor en proyectos estables y sencillos, pero es riesgoso cuando hay incertidumbre."

## Conexiones importantes

- [[Ciclos de Vida del Software]]
- [[Ciclo de Vida Iterativo e Incremental]]
- [[Ingeniería de Software y Metodologías]]
- [[Riesgo y Entropía en Proyectos de Software]]
- [[Proceso Unificado de Desarrollo]]

## Preguntas probables

- **¿Qué significa que cascada sea lineal?**
	- *Significa que antes de seguir con la siguiente fase, se asegura de que la anterior quede revisada y testeada, sobre esos artefactos producidos, es en lo que se va a basar la nueva fase.*
- **¿Cuál es su principal ventaja?**
	- *La principal ventaja es que si no hay mucha incertidumbre, esta metodología es muy útil y provee mucha seguridad y robustez a medida que va avanzando el proyecto.*
- **¿Cuál es su principal riesgo?**
	- *El principal riesgo es el de encontrar deficiencias o malentendidos tarde en el ciclo de vida de cascada. Al no contar con ningún prototipo o muestra tangible, es usual encontrar errores de concepto o de implementación tarde en el desarrollo del proyecto.*
- **¿En qué contexto podría funcionar?**
	- *Cascada funcionaría en un contexto en donde los requisitos sean fijos, claros y estables y no haya incertidumbre en cuanto al alcance del proyecto o su finalidad.*
- **¿Por qué los enfoques iterativos aparecen como respuesta a sus limitaciones?**
	- *Aparecen porque permiten ir generando pequeñas mejoras de manera continua para ir obteniendo feedback inmediato e ir ajustando el scope o finalidad del proyecto sobre la marcha, evitando así discrepancias tardías.*

## Recursos

- [[../../Recursos/Proceso Unificado/Proceso Unificado de Desarrollo_Introducción.pdf|Proceso Unificado de Desarrollo - Introducción]]
