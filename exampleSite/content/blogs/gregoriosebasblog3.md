---
title: "El problema de los tres cuerpos en arreglo triangular equilatero"
date: 2024-05-27
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "Gregorio Lince y Sebastian Betancur"
tags:
  - Avance de proyecto
  - Grupo 2
  - Problema de los tres cuerpos
  - Mecánica clásica
image: /images/grupo 2/Three-body_Problem_Animation_with_COM.gif
description: ""
toc:
mathjax: true
---

## Se baja el telon: la conclusión de la danza celestial de los tres cuerpos

Es con gran lástima que escribimos este último blog; ha sido un interesante viaje de conocimiento el estudiar movimientos celestes. Hoy les traemos la conclusión del proyecto, así como más imágenes y datos interesantes que hemos encontrado y desarrollado durante los últimos meses. Para empezar, las matemáticas se volvieron más aburridas; quién lo diría. Logramos desarrollar algo llamado el Lagrangiano, una ecuación que como por arte de magia nos puede dar mucha información sobre cómo algo se comporta. En este caso, el Lagrangiano es para los tres cuerpos, cuando estos están posicionados en un triángulo equilátero (de tres lados iguales). Se necesitó mucha trigonometría. Mucha. Vamos a comparar la información que nos da este Lagrangiano con la información que teníamos anteriormente, que habíamos encontrado usando la matemática usada por Isaac Newton, para poder ver cuál de las dos formas puede darnos información más precisa sobre el sistema. 

#### Dato curioso: ¿Sabías que la estrella más cercana al sol, Próxima Centauri o Alfa Centauri C, es parte de un sistema de tres cuerpos? Junto con Alfa Centauri A y Alfa Centauri B, conforman el sistema estelar Alfa Centauri.

En primer lugar, usamos el modelo que desarrolló Newton para intentar estudiar un sistema de tres cuerpos en forma de triángulo, utilizando la ley que él descubrió, la ley de gravitación universal, para ver qué tan fuertemente se atraen los cuerpos.

$$\frac{d^2 \vec{r_i}}{dt^2} = \sum_{j \neq i} \frac{G m_j}{r^3_{ij}} \vec{r_{ij}}$$

¿Pero qué es eso? Qué espeluznante. Pero no se preocupen, solo es notación complicada; lo único que nos quiere decir, es que el cambio en el tiempo del cambio en el tiempo (la aceleración) de la distancia entre los cuerpos, que es la letra r; depende de m, que es la masa de los cuerpos; de r, que otra vez, es la distancia entre ellos; y G, que es un número muy pequeño (¡la gravedad es muy débil!) que se llama la constante de gravedad. Esta es la famosa ley de gravitación universal de Newton. Utilizando esta fórmula para relacionar las distintas cantidades del sistema, nos dio el siguiente comportamiento:

<p align="center">
  <img src="/exampleSite/static/images/grupo 2/mecanicalagr.png" alt="Lag4" width="300" class="center">
</p>

Tristemente, este método nos dio una respuesta bastante poco satisfactoria: los cuerpos no son suficientemente masivos para quedar enlazados en las órbitas de los otros, es decir, no son los suficientemente pesados. Estos cuerpos pesan $1*10^{10}$ kilogramos, es decir, ¡un uno seguido por diez ceros! Les dije, la gravedad es bastante débil.

Pero ahora, si utilizamos el Lagrangiano... 

$$L = \frac{3}{2} m (\dot r^2 + r^2 \dot \theta^2) + \sqrt{3} G (\frac{Gm^2}{r})$$

<p align="center">
  <img src="/exampleSite/static/images/grupo 2/tres_cuerpos.gif" alt="Lag5" width="300">
</p>

¡Ta-da! Increíble, ¿no? Así se ve un sistema de órbita de tres masas, cuando se cumplen ciertas condiciones, por supuesto; en este caso, los tres cuerpos pesan lo mismo, están a las mismas distancia entre ellos, e inician con las mismas velocidades. De no ser el caso, es difícil saber con certeza qué puede pasar; puede que el sistema ni siquiera sea estable, es decir, que después de cierto tiempo choquen entre sí, o que pase lo que pasó anteriormente, la gravedad no es lo suficientemente fuerte para mantenerlos ligados.

La pregunta ahora es, ¿por qué son comportamientos tan distintos, si ambos escenarios tienen las mismas masas, distancias y velocidades? Pues eso tiene que ver con el hecho de que todo lo que hemos visto hasta ahora son aproximaciones, a las cuales les llamamos métodos numéricos. Estos métodos numéricos aproximan cómo puede pasar, y no siempre son exactos; el hecho de que ambos casos fueran ligeramente distintos nos arroja soluciones que pueden ser muy diferentes.

Así que, lo logramos, y esperamos hayan entendido y disfrutado este pequeño vistazo de la mecánica clásica y del problema de los tres cuerpos, dos áreas de estudio sumamente fascinantes de la física. A través de este blog, así como este proyecto, esperamos hayas aprendido y disfrutado algo de nuestros últimos meses de trabajo. ¡Adiós!


