---
title: "Modelo Matemático de un Pendubot Mediante Mecánica Lagrangiana"
date: 2024-04-19
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "Dayana Estefanía Carmona Gamarra y Santiago Moncayo Sarria"
tags:
  - Anteproyecto
  - Grupo 5
  - Pendubot

image: /images/grupo5/simulacion.gif
description: "Y ¿Cómo controlo el pendubot?"
toc:
---
# Pendubot
## Vamos a dominar el mundo

Imagina que eres una IA que quiere dominar el mundo, para ello fabricas una cantidad absurda de robots bípedos que serán tu punta de lanza para conquistar a los humanos, pero ¡Oh sorpresa!, ellos no pueden caminar por si solos, aunque hayas hecho con precisión milimétrica todo su cuerpo mecánico y sus conexiones eléctricas, ¿Por qué será? Te podrías preguntar, y en tu búsqueda por todo el internet encuentras este blog que te dará la respuesta, ¡Te falta control! Y no me refiero control en tus acciones, sino implementar la teoría del control, así tu robot caminará, acompáñame a ver como el control de un pendubot puede hacer mover a tus robots e incluso que puedan mover libremente sus brazos.

### Lo básico, ¿Qué es la teoría del control?

La teoría de control es un campo que une la ingeniería y la matemática de una manera bella y hermosa par sistemas dinámicos, es decir que se mueven, en ella se busca que un sistema se mantenga en un estado que buscamos, ya sea una posición, un voltaje constante, una señal que sea periódica, etc. Para ello existen diversos métodos, entre ellos el PID el cuál se centra en buscar unas constantes que afecten la amplitud, la estabilidad y el tiempo de estabilización de un sistema, en el caso del pendubot esta será el método que usaremos para lograr nuestro cometido.

### Explorando la física de este sistema 

El pendubot es un gran ejemplo de cómo la correcta aplicación de los principios físicos pueden crear sistemas que se mantienen balanceándose al borde de la estabilidad. La base de su funcionamiento radica principalmente en dos conceptos claves: La energía cinética y la energía potencial, pero también entra en juego la rotación, el torque y el concepto de equilibrio inestable. 


### PID con pendubot

![DiagrmaPendubot](\images\grupo5\DiagramaPendubot.png)

Imagina que estas agarrando un café con tu brazo, tu vas a intentar que tu brazo se mantenga en un estado específico para que no se riegue, para ello tu antebrazo intentará moverse para mantener la estabilidad de este, de igual manera el pendubot intenta mover el primer brazo para que el segundo se mantenga siempre hacia arriba, esto es lo que busca el PID, mantener el según brazo apuntando al cielo, pero el primer paso para aplicar el PID es encontrar el modelo del sistema representado por una función de transferencia.

### Pendubot en el dominio de la frecuencia

![estableeee](\images\grupo5\estableeee.png)

En la entrada anterior vimos como funcionaba el modelo matemático del pendubot, ahora vamos a tomar dicho modelo y gracias a un amigable señor con apellido Laplace, podemos mover nuestro modelo a un dominio extraño, pero efectivo, es como si el tiempo ya no fuera tiempo y ahora son oscilaciones de una cuerda, gracias a la transformada de Laplace podemos obtener nuestra función de transferencia a la cuál podemos aplicar calcular el con métodos como el Tunning o dejando que nuestro programa de confianza Matlab lo haga por nosotros, ahora que tenemos nuestro PID, podrás mantener en pie a tu ejercito de robots para dominar el mundo.

### Conclusión

En resumen, ahora ya conoces las bases de funcionamiento de un pendubot, e incluso ¡cómo controlarlo!, además pudimos observar como podemos modelar este sistema tan complejo usando la mecánica lagrangiana, algo imposible en métodos Newtonianos, toda una ganga, y aprendimos la importancia del control en este tipo de sistemas que, cuando miras un poco más allá, es la base para poder modelar y adentrarte en este tipo de sistemas, esperamos que te hayas divertido y sobre todo aprendido. ¡Gracias!
