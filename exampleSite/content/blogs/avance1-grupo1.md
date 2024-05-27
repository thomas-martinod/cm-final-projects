---
title: "El Principio de Fermat y los Caminos de la Luz"
date: 2024-04-19
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "Thomas Martinod y Juan Fernando Riascos"
tags:
  - Anteproyecto
  - Grupo 1
  - Principio de Fermat
  - Óptica
image: /images/grupo1/lights.gif
description: ""
toc:
mathjax: true
---

## Introducción

"¡Hola a todos! En este vlog les traemos el primer avance del proyecto para la asignatura de Mecánica Clásica en la Universidad EAFIT, titulado 'El Principio de Fermat y los Caminos de la Luz'.

En el proyecto, estamos investigando las trayectorias que la luz sigue en materiales que no son uniformes ni isotrópicos. Para esto, estamos utilizando principios variacionales y de la mecánica de Lagrange, lo cual nos permite entender mejor cómo se comporta la luz en diferentes medios.

En esta primera parte, estamos revisando la formulación del principio de Fermat en estos materiales no uniformes. Además, presentamos tres casos de aplicación donde determinamos las trayectorias que sigue la luz en estos medios.

## Variaciones del indice de refracción
Podemos comenzar observando cómo la trayectoria de la luz adopta una forma circular en un medio con un índice de refracción dado por $$ n(x,y) = \frac{k}{y} $$.
Esta expresión nos muestra cómo el índice de refracción varía con la coordenada \\(y\\), lo que resulta en un camino que se asemeja a una circunferencia.

<p align="center">
  <img src="/images/grupo1/ava1.jpeg" alt="iman" width="500">
</p>

Asi mismo podemos ver tambien como dicha trayecotria de la luz se veria afecta al tomar un indice de refracción de la forma $$ n(x,y)=\sqrt{1 + y} $$ asimilando dichas trayectorias a un camino parabolico

<p align="center">
  <img src="/images/grupo1/ava2.jpeg" alt="iman" width="500">
</p>

Por otro lado si se desea tomar una forma exponencial de dicho camino planteamos entonces como indice $$ n(x,y)=\sqrt{1 + y^2} $$ notando asi que los cambios en las trayectorias de la luz modifican su camino como se observa a continuación:

<p align="center">
  <img src="/images/grupo1/ava3.jpeg" alt="iman" width="500">
</p>

## Variaciones de los Campos Escalares de los Índices de Refracción en Medios Ópticos
El campo escalar \\( n(x, y) \\) representa el índice de refracción en un plano bidimensional, asignando un valor numérico a cada punto \\( (x, y) \\). Este campo describe cómo varía el índice de refracción en un medio, siendo útil en la modelización de sistemas ópticos complejos donde el índice de refracción puede cambiar de un punto a otro. Por ejemplo, se utiliza en lentes con aberraciones corregidas y guías de onda con características especiales de propagación de luz.

Este campo sigueindo los indices de refracción mencionados anteriormente serian respectivamente los siguientes: 


<p align="center">
  <img src="/images/grupo1/ava12.jpeg" alt="iman" width="500">
</p>


<p align="center">
  <img src="/images/grupo1/ava22.jpeg" alt="iman" width="500">
</p>


<p align="center">
  <img src="/images/grupo1/ava32.jpeg" alt="iman" width="500">
</p>


# Principio de Fermat para Medios Anisotrópicos y Ecuación Eiconal General

En este artículo, exploramos el avance en la modelación matemática del principio de Fermat para materiales anisotrópicos e inhomogéneos. Según Shen y colaboradores (1997), el principio de Fermat se formula tradicionalmente en un medio isotrópico estático como la minimización del camino óptico recorrido por la luz, representado matemáticamente por $\delta \int n \, dl = 0$, donde $n$ es el índice de refracción.
En medios anisotrópicos, la situación se complica debido a la dirección dependiente del índice de refracción. En estos medios, el tensor dieléctrico $\varepsilon$ y el tensor métrico $g_{ij}$ describen la variación espacial del medio, afectando tanto los valores de las constantes dieléctricas principales como las orientaciones de los ejes principales. Esto requiere una reescritura del principio de Fermat para adaptarse a condiciones anisotrópicas, resultando en $\delta \int ds = \delta \int \sqrt{n_1^2 dx^2 + n_2^2 dy^2 + n_3^2 dz^2} = 0$.
Sabemos que:
\[
\delta \int n \, dl = 0
\]

donde \( n \) es el índice de refracción escalar. Sin embargo, en medios anisotrópicos, la complejidad aumenta ya que el índice de refracción depende de la dirección. El tensor métrico asociado a estos medios, \( g_{ij} \), se define como:

\[
g_{ij} = n^2_i \delta_{ij}
\]

donde \( n_i \) son los índices de refracción principales. Esto lleva a una nueva formulación del principio de Fermat para adaptarse a condiciones anisotrópicas:

\[
\delta \int \sqrt{n_1^2 dx^2 + n_2^2 dy^2 + n_3^2 dz^2} = 0
\]


Además, se deriva la ecuación geodésica que obedecen los trayectos de la luz en medios anisotrópicos estáticos, describiendo cómo la conexión afín $\Gamma^i_{jk}$ del manifold tridimensional contribuye a la trayectoria de la luz, modificando el comportamiento típico observado en medios isotrópicos. Esta formulación amplía considerablemente nuestra comprensión de la óptica en medios anisotrópicos, proporcionando una base para futuras investigaciones y aplicaciones en diseño de materiales y óptica computacional.

Esta expresión refleja cómo la luz minimiza su trayectoria en un medio donde el índice de refracción varía con la dirección. Además, derivamos la ecuación geodésica para la trayectoria de la luz en estos medios, mostrando cómo la conexión afín \( \Gamma^i_{jk} \) influencia el camino óptico:

\[
\frac{d^2 x^i}{ds^2} + \Gamma^i_{jk} \frac{dx^j}{ds} \frac{dx^k}{ds} = 0
\]

Este trabajo profundiza en la óptica de medios anisotrópicos, ampliando la comprensión y abriendo nuevas vías para investigaciones futuras y aplicaciones en el diseño de materiales avanzados y óptica computacional.


## Conclusión

Hemos visto cómo la luz puede desviarse de su camino recto habitual y seguir trayectorias curvas y onduladas. Este comportamiento está regido por el principio de Fermat, que describe cómo la luz elige el camino más rápido entre dos puntos en medios con diferentes índices de refracción.

Durante este proyecto, hemos analizado detalladamente algunas de estas trayectorias en materiales inhomogéneos y anisotrópicos. A través de la mecánica de Lagrange y principios variacionales, hemos explorado cómo la luz interactúa con estos medios y cómo podemos predecir su comportamiento.

En futuras investigaciones, profundizaremos en la aplicación del principio de Fermat a materiales más complejos y en la interpretación física de estos fenómenos. ¡Gracias por acompañarnos en este viaje de descubrimiento y aprendizaje!



¡Esperamos que hayan comprendido un poco sobre lo que buscamos hacer este semestre!, o que se queden con uno de los enunciados más bonitos de la óptica, el principio de Fermat.
