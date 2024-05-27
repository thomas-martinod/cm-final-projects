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

image: /images/grupo5/robobaile.gif
description: "Describiendo el movimiento de un pendubot"
toc:
---
# Pendubot
## Un baile de física y robótica

¿Puedes imaginar a un robot que intenta imitar a un equilibrista? Eso es un pendubot, es un robot compuesto de dos barras acopladas entre sí que busca dominar el arte del equilibrio.  

A primera vista este dispositivo suena como un juguete, pero el pendubot es la base de los robots que vemos hoy en día, es un mecanismo avanzado con el que se estudia la física del movimiento proporcionando nuevos ángulos sobre la dinámica de los sistemas intrínsecamente inestables. 

### ¿Cómo danza un pendubot? 

Ya sabemos que el pendubot consta de dos barras, una de ellas acoplada a un motor y la otra libre, buscando moverse al ritmo de su compañera que lleva el compás de este baile. Este tipo de configuración es similar al de un péndulo doble, donde la primera barra impulsa a la segunda. Imagina a una persona buscando mantener parado un bastón en la palma de su mano; el control preciso de sus movimientos determina si el bastón se mantendrá elegantemente erguido o caerá al suelo. 

### Explorando la física de este sistema 

El pendubot es un gran ejemplo de cómo la correcta aplicación de los principios físicos pueden crear sistemas que se mantienen balanceándose al borde de la estabilidad. La base de su funcionamiento radica principalmente en dos conceptos claves: La energía cinética y la energía potencial, pero también entra en juego la rotación, el torque y el concepto de equilibrio inestable. 


### Energía cinética y potencial 

![DiagrmaPendubot](\images\grupo5\DiagramaPendubot.png)

Cuando hablamos de un pendubot, hablamos de que cada barra o segmento tiene su propia energía cinética, la cual deriva de su movimiento. La energía cinética de cada segmento depende de la velocidad angular que lleve, es decir que tan rápido está girando alrededor de su punto de acople. Este tipo de energía es crucial para el movimiento del sistema y la reacción del control de esta. 

Por otro lado, la energía potencial esta influenciada principalmente de la gravedad. Esta energía es máxima cuando la barra acoplada a la barra principal se encuentra en su punto de altura máxima. Aquí es donde el equilibrio entra en juego, nosotros queremos mantener esta barra en su punto de altura más alto, pero este punto también es el de mayor inestabilidad del sistema. 

### Rotación y equilibrio inestable. 

![estableeee](\images\grupo5\estableeee.png)

La dinámica de rotación del pendubot es compleja debido a que cara barra influye en movimiento de la otra, cuando la barra principal (la que está acoplada al motor) se mueve, transmite parte de su movimiento a la otra barra a través de la articulación que los une. Esta transmisión es crucial para realizar los movimientos controlados que se desea. 

Lo realmente llamativo de un pendubot es su capacidad de mantenerse en un estado de equilibrio inestable. En términos físicos, el equilibrio inestable es un estado cuando una pequeña fuerza o movimiento cualquiera que se le aplique mientras se encuentra en su punto de equilibrio puede alejarlo de ese punto. El pendubot utiliza un código de control que le permite mediante la implementación adecuada de sensores y actuadores, saber el estado del sistema y corregirlo para tratar de mantenerlo siempre en su punto de equilibrio inestable. Manteniendo así el equilibrio a pesar de su tendencia natural a caer. Un ejemplo de la vida cotidiana de esto es cuando una persona intenta mantenerse en un solo pie corrigiendo constantemente su postura para no caer. 

### Conclusión

En resumen, el pendubot puede ser un desafío de ingeniería, pero también es un sistema con el cual podemos explorar leyes fundamentales de la física en acción. Estudiar la controlabilidad de este robot y sus movimientos, ayuda a obtener una mejor comprensión de cómo aplicar principios físicos en nuevas tecnologías principalmente en la ingeniería de control y la robótica.