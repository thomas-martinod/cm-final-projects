---
title: "Lagrangiano no relativista y relativista de una carga q inmersa en un campo electromagnético"
date: 2024-04-29
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "Ana Sofía Calle y Nancy Burgos Bedoya"
tags:
  - Entrega final
  - Grupo 4
  - Carga puntual en campo EM
  - Relativista
  - Fuerza electromagnética

image: /images/grupo4/videito.gif
description: "Trayectoria de dos partículas en un campo EM en el tiempo"
toc:
---

# Entrega final de proyecto

## Formulación lagrangiana no relativista y relativista de una carga q en un campo electromagnético.

### Grupo 4: Ana Sofía Calle y Nancy Burgos Bedoya


¡Hola! Esperamos que todo vaya bien :D esta será la última eentrada del blog, ya que por fin acabamos nuestro proyecto. Te contamos que en esta última actualización hallamos el lagrangiano de nuestra partícula, pero... ¡con correciones relativistas!

¿Por qué necesito corregir mis cálculos originales? ¿No pues que ya habíamos hallado el lagrangiano de la partícula en un campo electromagnético? Es totalmente correcto, ya lo habíamos hallado. Sin embargo, resulta que si usamos ese lagrangiano a velocidades muy altas (cercanas a la luz :o) ¡estaría completamente mal calculado jaja! Lo que habíamos hallado si funciona pero a velocidades clásicas, no te preocupes. Pero cuando entramos en el mundo relativista, tenemos que corregir nuestros cálculos. ¿Por qué? Pon mucha atencion:

Imagina que eres el capitán de una nave espacial futurista. Te empiezas a aburrir entonces aumentas la velocidad de la nave hasta el 99% de la velocidad de la luz. Resulta que empiezan a haber cambios en la nave que antes no ocurrían. 

Primero, la masa efectiva de la nave y todo lo que hay adentro empieza a aumentar significativamente. Claramente, si hay un aumento en masa debe de haber un cambio en el momentum del cuerpo. El momentum se acerca al infinito cuando llegamos a velocidades tan altas, lo que desemboca en cómo se mueve nuestra nave en el espacio.

Luego, resulta que alguien que está en la tierra con un telescopio capaz de ver al interior de la nave instantáneamente ve que todos empiezan a moverse extremadamente lento. ¡Como si el tiempo se dilatara! Dentro de la nave, no se notaría ningún cambio en el tiempo. Si tu vieras con el telescopio instantáneo de vuelta a la tierra verías que mucho tiempo ha pasado, incluso años.

<img src="/images/grupo4/abuela.png" alt="Tiempo" width="400"> 


Por último, las distancias parecen cambiar completamente. Este mismo observador nota que la nave se encogió notoriamente. Esto se llama contracción de longitud la cua ocurre en la dirección del movimiento a estas altas velocidades:

<img src="/images/grupo4/nave.png" alt="Nave" width="400"> 

Ahora, ¿cómo se supone que voy a calcular todos estos cambios extraños en mi sistema? Respira, es totalmente posible. Resulta que existe el factor relativista, también llamado gamma, que surgió en la teoría de relatividad de Einstein. Es literalmente un número que cambia dependiendo de la velocidad a la que esté yendo tu nave, así de simple. Con este numerito, podemos corregir cantidades como la longitud, tiempo, masa, momento y ecuaciones de movimiento del sistema que esté yendo a grandes velocidades.

En nuestro proyecto es fundamental, pues queremos acelerar a nuestra partícula a grandes velocidades donde estos efectos aparecen si o si. Las ecuaciones de movimiento se corrigen con el factor gamma, lo que nos entrega ecuaciones que describen con gran presición la trayectoria de la partícula.

Ahora que hemos repasado los conceptos básicos adentrémonos en los resultados. Para evaluar nuestros modelos realizamos una simulación en Pyhton que nos permitiera ver la evolución en el tiempo de nuestra partícula cargada en diferentes casos. ¡La simulación nos permite usar las condiciones que queramos! Pero para entender que está pasando enfoquémonos en un solo caso observemos qué pasa y por qué. 

En este caso particular el campo electromagnético que nuestra partícula atreviesa está compuesto por un campo magnético E uniforme en los ejes Y y Z y un campo magnético B con un único componente en x. Como vimos en la entrada anterior, cuando usamos un modelo obtenido a partir de un lagrangiano no relativista para la simulación de este caso obtenemos la imagen siguiente debido a que la velocidad inicial v_x0 coincide con la dirección del campo magnético en X por lo que la fuerza magnética es cero, permitiendo que la partícula mantenga una velocidad constante a lo largo del eje x.
Por otro lado, las componentes del campo eléctrico Ey y Ez desaceleran la partícula en las direcciones Y y Z, ya que ejercen fuerzas eléctricas opuestas a su velocidad. Además, la fuerza de Lorentz en estos planos perpendiculares al campo magnético causa una trayectoria helicoidal en esas direcciones.

<img src="/images/grupo4/holi1.png" alt="Imagen 1" width="400"> 

Ahora, ¿y si repetimos esta simulación para el lagrangiano relativista? Como ven en la siguiente imagen obtenemos, ¡exactamente lo mismo! Dado que las velocidades iniciales no son lo suficientemente bajas para ver efectos relativistas afectando la partícula esta se comporta como lo esperábamos, mostrando que nuestro modelo relativista funciona también para casos sin efectos relativistas.

<img src="/images/grupo4/holi2.png" alt="Imagen 2" width="400"> 

Bueno, ¿y si queremos ver efectos relativistas? Sencillo, establecemos una velocidad inicial vx0=0.99c, que corresponde a un 99% de la velocidad de la luz, ¡un montón! Veamos a continuación la diferencia que cambiar este parámetro produce en las simulaciones obtenidas con ambos modelos.

<img src="/images/grupo4/holi3.png" alt="Imagen 3" width="400"> 

<img src="/images/grupo4/holi4.png" alt="Imagen 4" width="400"> 

Es claro a simple vista que, ¡son diferentes!

Esto se debe a que en la primera imagen no se consideran los efectos relativistas. Aunque la velocidad inicial sea casi igual a la velocidad de la luz (0.99c), el modelo asume que la masa de la partícula y las leyes del electromagnetismo funcionan igual que a velocidades mucho más bajas. Sin embargo, a velocidades cercanas a la luz, es necesario tener en cuenta los efectos relativistas. Como se muestra en la segunda imagen, la masa de la partícula aumenta a medida que se acerca a la velocidad de la luz, lo que afecta su interacción con el campo electromagnético. Esto resulta en una trayectoria muy diferente, que el modelo relativista puede describir con mayor precisión. Así, la simulación computacional nos permite estudiar mejor la dinámica de partículas cargadas en campos electromagnéticos solo con langragianos y un computador.