---
title: "Modelación de la dinámica de reentrada de un satélite LEO"
date: 2024-05-26
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "Camila Posada y Alejandra Ocampo"
tags:
  - Proyecto
  - Grupo 7
  - Dinámica satelital

image: /images/grupo7/satelite_LEO
description: "Modelando la reentrada de satélites LEO"
toc:
---
# Modelando la reentrada de satélites LEO 

![Satelite_LEO](/images/grupo7/satelite_LEO.jpg)

En la era moderna, los satélites en órbitas bajas terrestres (LEO, por sus siglas en inglés) son esenciales para una variedad de actividades, como la observación terrestre, las telecomunicaciones y la navegación satelital. Estos satélites operan en una región del espacio densamente poblada, donde el control de sus trayectorias es crucial para evitar colisiones y garantizar su correcto funcionamiento. El proyecto que abordamos aquí se centra en un aspecto fundamental de la ingeniería orbital: la dinámica de reentrada de estos satélites.

**Dato curioso:** ¿Quieres enterarte sobre las diferentes órbitas de los satélites? Mira este video: **[Órbitas de satélites](https://www.youtube.com/watch?v=NFc3oU_wq7I&ab_channel=GlobalInvacomGroup)**. 

# Enfoque Lagrangiano en la modelización

Para abordar este desafío, nuestro proyecto emplea principios de la mecánica lagrangiana, un enfoque que utiliza coordenadas generalizadas y se centra en la conservación de la energía. Este método es particularmente adecuado para modelar las fuerzas no conservativas, como la resistencia atmosférica, que juegan un papel crucial en la dinámica de reentrada. La mecánica lagrangiana nos permite desarrollar un marco matemático robusto para simular las interacciones complejas que un satélite experimenta durante su descenso.

# Simulaciones del modelo

Utilizamos Python para realizar simulaciones que visualizaran la dinámica de los satélites con respecto a su altitud, tiempo de reingreso y coordenada angular.

La primera figura muestra el descenso de un satélite en órbita baja terrestre (LEO) con el tiempo. En el eje horizontal vemos los días, y en el vertical, la altitud del satélite. Al principio, la altitud disminuye lentamente porque la atmósfera es tenue. Con el paso del tiempo, la caída se acelera debido al aumento de la densidad atmosférica, lo que incrementa la fricción. Después de unos 80 días, el descenso se vuelve muy rápido, indicando que el satélite ha encontrado una atmósfera más densa, lo que provoca su desintegración o impacto con la Tierra. Esta gráfica destaca la importancia de entender y controlar la reentrada de satélites para la seguridad de las misiones espaciales.

![Altitud vs. Tiempo](/images/grupo7/Altitud_tiempo.jpg)

La siguiente gráfica muestra cómo cambia la coordenada angular del satélite con el tiempo durante su reentrada. Al principio, la línea es casi plana, lo que significa que el satélite cambia muy poco su posición angular porque está en una órbita estable y moviéndose a velocidad constante. Con el tiempo, la curva se vuelve más empinada, indicando que el satélite está acelerando su movimiento angular alrededor de la Tierra. Esto sucede porque, a medida que el satélite desciende y baja su altitud, su velocidad angular aumenta. Si el satélite estuviera en una órbita perfecta y sin arrastre, veríamos una línea recta constante. Pero el aumento de la pendiente sugiere que la fricción atmosférica está afectando al satélite. Este aumento en la velocidad angular nos dice que el satélite se está acercando a su reentrada en la atmósfera, donde la fricción es más fuerte y cambia su velocidad más rápidamente.

![Coordenada Angular vs. Tiempo](/images/grupo7/Coord_angular.jpg)

Para finalizar, graficamos el tiempo de reingreso según su radio inicial. En el eje horizontal, vemos el radio inicial desde el centro de la Tierra en kilómetros, que incluye el radio de la Tierra (aproximadamente 6371 km) más la altitud del satélite. En el eje vertical, se representa el tiempo de reingreso en días. A medida que el radio inicial aumenta, el tiempo de reingreso también aumenta. Esto significa que los satélites en órbitas más altas tardan más en reingresar. En altitudes bajas (6600-6800 km), la mayor densidad atmosférica provoca más fricción, acelerando el reingreso. En altitudes altas (6800-7400 km), la menor densidad atmosférica reduce la fricción, permitiendo que los satélites permanezcan en órbita por más tiempo. En resumen, a mayor altitud, menor densidad del aire y menor fricción, lo que prolonga la permanencia en órbita. A menor altitud, mayor densidad del aire y mayor fricción, acelerando el reingreso.

![Tiempo de reingreso vs. Radio inicial](/images/grupo7/treingreso_radio.jpg)

# ¿Qué se puede concluir?

Al considerar todas las fuerzas relevantes, incluidos los efectos no conservativos como la resistencia atmosférica, hemos mejorado nuestra comprensión teórica de la dinámica orbital. Esto no solo tiene implicaciones prácticas significativas en la optimización de recursos y la mitigación de riesgos, sino que también impulsa el desarrollo de tecnologías espaciales avanzadas. La capacidad de predecir y controlar con precisión la reentrada de satélites es crucial para garantizar la seguridad y sostenibilidad de las operaciones espaciales.

Además, hemos observado que los satélites en órbitas más bajas tienen tiempos de reingreso más cortos debido a la mayor densidad atmosférica que encuentran, mientras que los satélites en órbitas más altas experimentan tiempos de reingreso más largos debido a la menor densidad atmosférica.

