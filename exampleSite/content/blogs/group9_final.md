---
title: "Escuchando la forma de un tambor, o , ¿Qué #%$&$ es un autovalor?"
date: 2024-05-23
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "José Ortiz-Ocampo"
tags:
  - Entrega final
  - Grupo 9
  - Análisis espectral
  - Propagación de ondas
  - Mecánica del medio continuo
image: /images/grupo9/circular_membrane_oscillation.png
description: "Como la matemática nos ayudar a escuchar formas, y una (de muchas) aplicaciones del análisis de autovalores y autofunciones de un operador (análisis espectral, para los jijijjujuju académicos) - parte 3, final"
toc: false
mathjax: true
---
### Ojo: Lo que sigue es divulgación físico-matemática altamente adictiva! Siga con precaución ⚠️

Parte final del blog, mira las entradas previas para enterarte de toda la historia!

Aquí vamos! Cogimos dos formas, cuadrados y triángulos, de diferentes áreas, y les calculamos los autovalores respectivos con el [*Método de Elementos Finitos*](https://es.wikipedia.org/wiki/M%C3%A9todo_de_los_elementos_finitos) montado. 

Con esos autovalores calculamos una variable que llamaremos \\(N\\), que se relaciona con **que tan rápido crecen esos autovalores**. Y se supone que debemos encontrar una relación lineal entre esta variable y el área, osea \\(A = C * N\\), según la [**Fórmula de Weyl**](https://en.wikipedia.org/wiki/Weyl_law) para el Laplaciano.

veamos lo que nos dio en el siguiente gráfico:

![Relación Área-Evolución](/images/grupo9/weyls_law_analog_more_areas.png)


*¿Qué significa??? ¿qué significa???? ¿sí nos dio? o qué?*

Cómo diría el poeta: pues ahí maso. Porque en efecto vemos que hay una relación lineal entre área y \\(N\\), pero esa relación parece depender levemente de la geometría misma. Y si tengo que conocer la geometría para poder indicar la constante de la relación, pues sería mucho más fácil estimar el área por otros métodos... toda la idea aquí era hacerlo sin tener que conocer la geometría.

Pero no todo es malo! Igual la dependencia parece leve, entonces la expresión sí podría dar una primera estimación del área, que puede ser suficientemente buena al menos como orden de magnitud. Y de nuevo el comentario de la entrada anterior, esto es matemática experimental ✨, por lo que más que los resultados o las aplicaciones, nos interesa que sirva de insumo y pista para investigadores teóricos que quieran trabajar sobre esto

## ¿Qué aprendimos?

Querido lector, vamos llegando al final de esta pequeña aventura. Espero te haya gustado, haya sido fácil de leer, y hayas aprendido algo nuevo. Si me lo preguntas, quisiera que te fueras con las siguientes ideas en la cabeza:

- Los autovalores son importantes. Nos dicen mucho sobre los operadores a los que pertenecen, y tienen muchas más aplicaciones prácticas e interpretaciones interesantes de las que suelen contarnos en los cursos elementales de Álgebra Lineal.
- Existen algunos trabajos en la matemática que se denominan **matemática experimental**, que son trabajos que buscan simular el comportamiento de sistemas o estructuras matemáticas, y que, más que extraer conclusiones o demostrar poderosos teoremas, sientan las bases y dan pistas para que otros puedan hacerlo. La ciencia es una construcción de todos!
- La matemática está en todas partes! Incluso en el sonido que hacen las cosas cuando son golpeadas. Tener un pensamiento matemático y abstracto sobre las cosas en general te permitirá verlas desde nuevas y disruptivas perspectivas!


Hasta la próxima! 👋


### Bonus track: errata

*PD: sobre los resultados obtenidos. En la retroalimentación del trabajo nos dimos cuenta que a esta historia le falta un pedazo. Y es que en la implementación del método de elementos finitos hace falta verificar que el mallado realizado de la geometría es suficientemente pequeño para indicar que ya hubo un proceso de convergencia. En español, hay que hacer varias pruebas para ver que los resultados son congruentes y aproximan bien las soluciones exactas. Esto no se incluyó en el alcance del trabajo. Y todo esto para decir que, tal vez, si a la aproximación numérica se le exige un poquito más, es posible que esas ligeras desviaciones que llevan a las conclusiones presentadas desaparezcan, y las conclusiones obtenidas cambien. Te invito, querido lector, a indagar más alrededor de esto 🔍*