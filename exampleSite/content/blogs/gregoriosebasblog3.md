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
image: /images/grupo1/lights.gif
description: ""
toc:
mathjax: true
---

## Se baja el telon: la conclusion de la danza celestial de los tres cuerpos

Es con gran lastima que escribimos este ultimo blog; ha sido un interesante viaje de conocimiento el estudiar movimientos celestes. Hoy les traemos la conclusion del proyecto, asi como mas imagenes y datos interesantes que hemos encontrado y desarrollado durante los ultimos meses. Para empezar, la matematica se volvio mas aburrida; quien lo diria. Logramos desarrollar algo llamado el Lagrangiano, una ecuacion que como por arte de magia nos puede dar mucha informacion sobre como algo se comporta. En este caso, el Lagrangiano es para los tres cuerpos, cuando estos estan posicionados en un triangulo equilatero (de tres lados iguales). Se necesito mucha trigonometria. Mucha. Vamos a comparar la informacion que nos da este Lagrangiano con la informacion que teniamos anteriormente, que habiamos encontrado usando la matematica usada por Isaac Newton, para poder ver cual de las dos formas puede darnos informacion mas precisa sobre el sistema. 

#### Dato curioso: ¿Sabias que la estrella mas cercana al sol, Proxima Centauri o Alfa Centauri C, es parte de un sistema de tres cuerpos? Junto con Alfa Centauri A y Alfa Centauri B, conforman el sistema estelar Alfa Centauri.

En primer lugar, usamos el modelo que desarrollo Newton para intentar estudiar un sistema de tres cuerpos en forma de triangulo, utilizando la ley que el descubrio, la ley de gravitacion universal, para ver que tan fuertemente se atraen los cuerpos. 

$$\frac{d^2 \vec{r_i}}{dt^2} = \sum_{j \neq i} \frac{G m_j}{r^3_{ij}} \vec{r_{ij}}$$

¿Pero que es eso? Que espeluznante. Pero no se preocupen, solo es notacion complicada; lo unico que nos quiere decir, es que el cambio en el tiempo del cambio en el tiempo(la aceleracion) de la distancia entre los cuerpos, que es la letra r; depende de m, que es la masa de los cuerpos; de r, que otra vez, es la distancia entre ellos; y G, que es un numero muy pequeño (¡la gravedad es muy debil!) que se llama la constante de gravedad. Esta es la famosa ley de gravitacion universal de Newton. Utilizando esta formula para relacionar las distintas cantidades del sistema, nos dio el siguiente comportamiento:

<p align="center">
  <img src="/exampleSite/static/images/grupo 2/mecanicalagr.png" alt="Lag4" width="300" class="center">
</p>

Tristemente, este metodo nos dio una respuesta bastante poco satisfactoria: los cuerpos no son suficientemente masivos para quedar enlazados en las orbitas de los otros, es decir, no son los suficientemente pesados. Estos cuerpos pesan $1*10^{10}$ kilogramos, es decir, ¡un uno seguido por diez ceros! Les dije, la gravedad es bastante debil. 

Pero ahora, si utilizamos el Lagrangiano... 

$$L = \frac{3}{2} m (\dot r^2 + r^2 \dot \theta^2) + \sqrt{3} G (\frac{Gm^2}{r})$$

<p align="center">
  <img src="/exampleSite/static/images/grupo 2/tres_cuerpos.gif" alt="Lag5" width="300">
</p>

¡Ta-da! Increible, ¿no? Asi se ve un sistema de orbita de tres masas, cuando se cumplen ciertas condiciones, por supuesto; en este caso, los tres cuerpos pesan lo mismo, estan a las mismas distancia entre ellos, e inician con las mismas velocidades. De no ser el caso, es dificil saber con certeza que puede pasar; puede que el sistema nisiquiera sea estable, es decir, que despues de cierto tiempo choquen entre si, o que pase lo que paso anteriormente, la gravedad no es lo suficientemente fuerte para mantenerlos ligados.

La pregunta ahora es, porque son comportamientos tan distintos, si ambos escenarios tienen las mismas masas, distancias y velocidades? Pues eso tiene que ver con el hecho de que todo lo que hemos visto hasta ahora son aproximaciones, a las cuales les llamamos metodos numericos. Estos metodos numericos aproximan como puede pasar, y no siempre son exactos; el hecho de que ambos casos fueran ligeramente distintos nos arroja soluciones que pueden ser muy diferentes.

Asi que, lo logramos, y esperamos hayan entendido y disfrutado este pequeño vistazo de la mecanica clasica y del problema de los tres cuerpos, dos areas de estudio sumamente fascinantes de la fisica. 



