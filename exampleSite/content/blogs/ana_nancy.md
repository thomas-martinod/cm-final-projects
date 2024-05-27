---
title: "Lagrangiano no relativista y relativista de una carga en un campo electromagnético"
date: 2024-03-04
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "Ana Sofía Calle y Nancy Burgos Bedoya"
tags:
  - Anteproyecto
  - Grupo 4
  - Carga puntual en campo EM
  - Relativista
  - Fuerza electromagnética

image: /images/grupo4/videito.gif
description: "Trayectoria de dos partículas en un campo EM en el tiempo"
toc:
---

# Anteproyecto

## Formulación lagrangiana no relativista y relativista de una carga q en un campo electromagnético.

### Grupo 4: Ana Sofía Calle y Nancy Burgos Bedoya


¿Has jugado alguna vez con los imanes de la nevera? ¿O visto un rayo en una tormenta? ¿O usado una brújula? ¿O se te ha parado el cabello jugando con globos? Seguro que sí, pero que tal si te dijera que todos estos fenómenos tan interesantes y diferentes entre sí son de hecho en el fondo, ¡uno solo! 

El universo en el que vivimos hay 4 fuerzas que gobiernan todos los fenómenos físicos que observamos a diario. Una de estas importantísimas interacciones se conoce como fuerza electromagnética, la cual describe todos los sucesos curiosos mencionados antes. Pero antes de explicar a profundidad qué es y por qué es tan importante, demos un repaso por algunos conceptos básicos para poder entenderla apropiadamente.

En primer lugar, el más conocido; el imán. ¿Quién no ha intentado unir dos imanes a la fuerza solo para encontrarse con una fuerza misteriosa repeliéndolos? Este fenómeno es propio de la naturaleza de los imanes, pero primero, ¿qué es un imán? Definimos como imán a todos aquellos materiales que poseen lo que llamamos magnetismo, que es la propiedad por la cual ciertos objetos se atraen o repelen. La principal característica de todos los imanes son sus 2 polos magnéticos inseparables, los cuales están ubicados en sus extremos y son denominados norte y sur. Cuando dos polos iguales de un imán se acercan se van a repeler entre sí, mientras que cuando dos polos opuestos se acercan se sienten atraídos. Esta fuerza de atracción o repulsión entre los polos dependerá de la distancia que los separa así como de la fuerza del imán. Este efecto fácilmente observable experimentalmente sucede debido a que las líneas de campo del imán, una herramienta gráfica que nos permite visualizar la distribución de su fuerza; siempre “salen” del polo norte y “entran” al polo sur. Estas líneas de campo conforman lo que se conoce como "campo magnético", un campo de fuerza que se extiende alrededor del imán y con el cual interactúa su región adyacente.

<img src="/images/grupo4/iman.jpeg" alt="iman" width="400">

Es posible crear un campo magnético no solo de un imán, sino que también a partir un campo eléctrico. Al igual que los polos norte y sur, existen las cargas eléctricas, que son o positivas o negativas y poseen las mismas propiedades; una carga positiva atraerá a una negativa, y ejercerá una fuerza de repulsión sobre otra carga positiva. La fuerza que actúa sobre estas cargas se denomina fuerza eléctrica. Cuando una carga eléctrica se encuentra en movimiento, ¡genera tanto un campo eléctrico como un campo magnético a su alrededor! En la historia se ha demostrado múltiples veces que la razón de esto es que la fuerza magnética y eléctrica están acopladas, lo que llamamos fuerza electromagnética. Algunos nombres famosos que realizaron experimentos sobre esto son Michael Faraday (planteó la inducción electromagnética), James Maxwell (cuyas famosas ecuaciones describen esta fuerza) y Nikola Tesla (famoso descubridor de la corriente alterna).

<img src="/images/grupo4/masters.png" alt="iman" width="500">

Al estudiar el comportamiento de una partícula al atravesar uno de estos campos, podemos describir adecuadamente la fuerza que este campo inevitablemente ejerce sobre ella. Existen muchas maneras de describir matemáticamente la fuerza electromagnética, cuyo estudio nos interesa. En nuestro proyecto nos centraremos en dos casos, su comportamiento general, ¡y su comportamiento relativista! Es decir, cuando las partículas tienen velociadades cercanas a la de la luz, ¡la velocidad máxima alcanzable en todo el universo! Este caso particular trae diferentes implicaciones físicas muy interesantes que se detallarán a medida que se desarrolla nuestro proyecto.

Ahora, para poder modelar el movimiento de una partícula contenida en un campo electromagnético, se necesita usar una herramienta muy poderosa: ¡La formulación lagrangiana! Recordemos que en física I nos enseñaban a armar un diagrama de fuerzas de un sistema simple para obtener sus ecuaciones de movimiento. Esto se conoce como la formulación newtoniana, y se enfoca más que todo en las fuerzas que actúan en un sistema. Ahora, la formulación lagrangiana se basa más que todo en las energías del sistema. Independientemente de qué formulación optes por usar, llegarás a las mismas ecuaciones de movimiento; el truco es que la formulación lagrangiana es mucho más sencilla y facilita el planteamiento para problemas de la física moderna y cuántica. 

Una vez encontremos el lagrangiano, se puede graficar fácilmente las trayectorias de nuestras partículas. Un ejemplo de una trayectoria que puede tomar una carga la puedes ver en el GIF de nuestro proyecto. Es un movimiento inquietante y un tanto elegante, el cual queremos estudiar. ¿No te preguntas, cómo cambiaría la trayectoria a la velocidad de la luz? 