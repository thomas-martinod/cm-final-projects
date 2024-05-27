---
title: "Avance de Lagrangiano no relativista y relativista de una carga en un campo electromagnético"
date: 2024-04-29
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "Ana Sofía Calle y Nancy Burgos Bedoya"
tags:
  - Anteproyecto
  - Grupo 4
  - Carga puntual en campo EM
  -Relativista
  -Fuerza electromagnética

image: /images/grupo4/videito.gif
description: "Trayectoria de dos partículas en un campo EM en el tiempo"
toc:
---

# Avance de proyecto

## Formulación lagrangiana no relativista y relativista de una carga q en un campo electromagnético.

### Grupo 4: Ana Sofía Calle y Nancy Burgos Bedoya

¡Hola de nuevo!

Ahora que tuvimos un avance con este gran proyecto, queremos mostrartelo :D

Primeramente, realizamos el desarrollo matemático para hallar el famoso lagrangiano, del cual hablamos en el post anterior. Una vez se tiene el lagrangiano, es muy facil derivar las ecuaciones de movimiento del sistema. ¿Puedes creerlo? ¡tener una ecuación que me diga cómo se mueve una partícula en un campo electromagnético! 

Al inicio del proceso matemático, tuvimos que definir algo muy imortante. ¿El campo EM es conservativo o no? Realmente, no lo es ya que la fuerza magnética es perpendicular al desplazamiento de la partícula. Esto significa que no es posible describirla
a través de un potencial escalar (osea un número cualquiera). 

Y... ¿qué gano con que no sea conservativa? ¡Pues todo! El planteamiento matmático ahora estará igualado a una fuerza no conservativa, también conocida en la formulación lagrangiana como una "fuerza generalizada". ¿Por qué generalizada? debido a la adaptabilidad de la fuerza en distintos sistemas. Ahora, esta fuerza actua sobre nuestra partícula en presencia de campos eléctricos y magnéticos... ¿Te suena?

Hay que hacer memoria de cuando en física 2 nos ponían a hacer maromas extrañas con la mano, la verdad nunca lo entendi...
¡La fuerza de Lorentz!

<img src="/images/grupo4/mano.png" alt="Trayectorias" width="400">


Pudimos comprobar que la fuerza generalizada de nuestro sistema, era en realidad la mismisima fuerza de Lorentz :D lo que era de esperar ya que estamos en un campo electromagnético. Con nuestra demostración de fuerza y las ecuaciones de movimiento, ahora solo resta hacer una simulación computacional de nuestras ecuaciones para ver las trayectorias de la partícula. Mira una de las gráficas que realizamos:

<img src="/images/grupo4/holi.jpeg" alt="Trayectorias" width="400">

Y... ¿que está pasando?

Para entender cómo una partícula cargada se comporta en presencia de campos eléctricos y magnéticos realizamos una simulación computacional que nos permitiera visualizar los movimientos de esta partícula. En esta simulación, le asignamos una carga de 1 Coulomb y una masa de 1 kilogramo.

Primero, la colocamos en un espacio tridimensional con ciertas condiciones iniciales: la posición (en metros) y la velocidad inicial (en metros sobre segundos) con magnitud de 10 cada una. Además, le aplicamos un campo eléctrico en las direcciones y z, y un campo magnético en la dirección x.

Lo que vemos es que la partícula sigue una trayectoria recta en la dirección x, lo cual tiene sentido porque el campo magnético solo tiene un componente en esa dirección. Debido a que la velocidad inicial de la partícula en x es paralela al campo magnético, la fuerza magnética actuando sobre ella es cero, y por lo tanto, continúa moviéndose con la misma velocidad inicial que describimos anteriormente e en esa dirección.

Sin embargo, en las direcciones y z, el campo eléctrico causa una desaceleración. Esto sucede porque las fuerzas eléctricas actúan en sentido opuesto a la velocidad inicial de la partícula en esas direccionas. Además, debido a la fuerza de Lorentz, que es la fuerza resultante de la interacción entre el campo magnético y la carga eléctrica en movimiento, la trayectoria de la partícula se curva en esas direcciones, ¡creando una especie de espiral como la de la imagen! No solo hemos logrado estudiar este fenómeno desde un computador, pero gracias a nuestro programa podemos manipularlo como se nos antoje y observar cómo cambia la trayectoria de nuestra partícula.

En un segundo caso cambiamos nuestras condiciones iniciales; agregamos un parámetro extra al campo eléctrico en x y cambiamos el campo magnético para que actuara en z esta vez y no x. Para hacer las cosas más simples y para visualizar mejor su movimiento, al principio la partícula está a 1 metro de distancia y se mueve a 1 metro por segundo.
Lo que vemos en la simulación es que la partícula sigue una especie de espiral en el plano horizontal (xy). Esto se debe a que las fuerzas eléctricas la hacen girar mientras que su velocidad la mantiene en movimiento circular. Además, sigue moviéndose en la misma dirección que el campo magnético, pero no en línea recta hacia arriba o hacia abajo (z), sino que sigue una especie de forma de arco, ¡como una parábola!

Esto sucede porque la fuerza eléctrica en la dirección vertical (z) acelera la partícula uniformemente, similar al primer caso en la dirección x, mientras que la fuerza magnética en esa dirección evita que las fuerzas eléctricas la hagan girar en otros planos. Entonces, la combinación de estas fuerzas hace que la partícula siga una trayectoria curva parabólica en lugar de moverse en línea recta.



