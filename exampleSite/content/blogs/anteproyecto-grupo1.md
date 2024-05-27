---
title: "El Principio de Fermat y los Caminos de la Luz"
date: 2024-03-09
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

Hoy nos adentraremos en el emocionante mundo de la **óptica** 👁️ (la ciencia que estudia la luz) y descubriremos un principio intrigante llamado el "Principio de Fermat", nombrado en honor al brillante matemático y físico Pierre de Fermat.

La idea de esta pequeña entrada de blog es describir brevemente el proyecto que se llevará a cabo para la asignatura de Mecánica Clásica en la Universidad EAFIT, que consiste en hallar los caminos de la luz cuando esta se desplaza entre dos puntos.

## Caminos e índice de refracción \\(n\\)

Todo parte de el principio de Fermat ¿Qué es exactamente el Principio de Fermat? Bueno, es una idea simple pero poderosa que nos ayuda a entender cómo la luz viaja y se comporta. Imagina que estás en un parque y quieres ir de un punto \\( A\\) a un punto \\( B \\).

<p align="center">
  <img src="/images/grupo1/multi.jpeg" alt="iman" width="500">
</p>

¿Cuál es el camino más rápido para llegar allí? Probablemente dirías que el camino más corto es \\(\Gamma_3\\) ¿verdad?, por eso de que es una línea recta ¡Y estarías en lo correcto!

Ahora, digamos que el camino recto, \\(\Gamma_3\\), es una piscina, ¿seguiría siendo el camino más rápido? Sin duda sigue siendo el camino más corto en cuanto a distacia, como bien podrías verificar con un flexómetro, pero en la piscina, **nadas** (pero eres más lento nadando 💀) por lo que podrías correr más rápido por uno de los otros caminos antes que nadar por el recto. Es decir, en ambos medios tienes velocidades diferentes y el parámetro que afecta esto en un material se llama el **índice de refracción** \\( n\\).

Para entenderlo, imagina que estás caminando por un campo abierto y llegas a un bosque. Cuando entras en el bosque, la cantidad de árboles aumenta. Esto te obliga a cambiar un poco tu dirección y a moverte más despacio para evitar chocar con los árboles.

Ahora, piensa en el índice de refracción como la densidad del bosque para la luz. Cuando la luz viaja a través de diferentes materiales, como del aire al agua o al vidrio, se encuentra con átomos y moléculas que están más "apretados" en algunos materiales que en otros. Esto se traduce en un cambio en la velocidad y dirección de la luz, similar a cómo tienes que cambiar tu dirección y velocidad al caminar a través de un bosque denso.

En la imagen a continuación, a la izquierda te presento un material con un índice de refracción más alto que el de la derecha:

<p align="center">
  <img src="/images/grupo1/indices.jpeg" alt="iman" width="500">
</p>


Puedes pensar esto del índice de refracción como una medida de la probabilidad de que la luz se choque con algún átomo, si hay más átomos, o los átomos están más pegados entre sí en el material, ¡es mucho más fácil que la luz se choque!

## El principio de Fermat

Ahora bien, el **Principio de Fermat** es la idea básica que venimos desarrollando que soluciona la pregunta ¿qué camino sigue la luz? Este principio nos dice que la luz viaja desde un punto a otro **siguiendo el camino más rápido posible, no el más corto**. Esto puede sonar un poco extraño al principio, pero aquí está la clave: la luz no siempre viaja en línea recta. De hecho, puede doblarse o refractarse cuando pasa de un medio a otro, como del aire al agua o al vidrio.

Entonces, ¿cómo podemos aplicar este principio en la vida real? Imagina que tienes una linterna y quieres iluminar un objeto en el fondo de una piscina. La luz no viajará en línea recta a través del agua, ¿verdad? Seguirá un camino que minimice el tiempo que tarda en llegar al objeto, teniendo en cuenta la refracción en el agua.

Este principio es fundamental en el diseño de lentes, prismas y otros dispositivos ópticos que utilizamos en nuestra vida diaria. Nos ayuda a comprender cómo se forma una imagen en una cámara, cómo funciona un microscopio y muchas otras aplicaciones importantes en la tecnología moderna.

## Un breve ejemplo

Para ejemplificar, el primer caso que se evaluó en el proyecto es el caso de un material en el que la velocidad de propagación $v$ de la luz es proporcional a la altura del material, es decir \\( v(y) \propto y\\). or lo que considerando que \\(n=c/v\\) donde \\(c\\) es la velocidad de la luz en le vacío, estamos enfrentandonos a un material con un índice de refracción que disminuye con la altura, es decir \\(n=k/y\\) para alguna constante \\(k\\).

Por poco intuitivo que parezca, para que la luz vaya de un punto \\( (x_0, y_0)\\) a un punto  \\( (x_1, y_1)\\), la ecuación que sigue la trayectoria de la luz es un círculo, es decir:

$$ (x+A)^2 + y^2 = B $$

Una visualización gráfica de una de estas trayectorias, se enseña a continuación:

<p align="center">
  <img src="/images/grupo1/circulo.jpeg" alt="iman" width="700">
</p>


(observa que el índice de refracción \\(n\\) disminuye con la altura).

## Conclusión

Si te perdiste en esta última parte, quedate con lo más importante: **La luz no siempre se mueve en línea recta, sino que puede curvarse o doblarse**. La ley que describe estas trayectorias es el **principio de Fermat**, y lo que vamos a hacer en este proyecto es analizar algunas de las trayctorias de la luz en distintos materiales con distintos índices de refracción.

Como conclusión, la próxima vez que uses unas gafas, tomes una foto con tu teléfono o simplemente disfrutes de un día soleado, recuerda el Principio de Fermat y cómo nos ayuda a entender el maravilloso mundo de la luz, diciendonos que la luz es la mejor atleta, **no le importa que el camino que recorra no sea el más corto, sino que le importa llegar lo más rápido posible**.

¡Esperamos que hayan comprendido un poco sobre lo que buscamos hacer este semestre!, o que se queden con uno de los enunciados más bonitos de la óptica, el principio de Fermat.
