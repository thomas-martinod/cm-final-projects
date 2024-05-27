---
title: "Escuchando la forma de un tambor, o , ¿Qué #%$&$ es un autovalor?"
date: 2024-04-15
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "José Ortiz-Ocampo"
tags:
  - Primera entrega
  - Grupo 9
  - Análisis espectral
  - Propagación de ondas
  - Mecánica del medio continuo
image: /images/grupo9/circular_membrane_oscillation.png
description: "Como la matemática nos ayudar a escuchar formas, y una (de muchas) aplicaciones del análisis de autovalores y autofunciones de un operador (análisis espectral, para los jijijjujuju académicos) - parte 2"
toc: false
mathjax: true
---
### Ojo: Lo que sigue es divulgación físico-matemática altamente adictiva! Siga con precaución ⚠️

# *¿Entonces que, si siguen siendo isoespectrales?*

Pues veamos. Tomamos varios pares de geometrías que eran isoespectrales para el Laplaciano, y verificamos si los autovalores siguen siendo iguales entre sí para el caso del operador presentado en la entrada anterior. Hallamos los autovalores usando un método numérico para solucionar el problema de autovalores y autovectores aproximadamente. El método se llama [*Método de Elementos Finitos*](https://es.wikipedia.org/wiki/M%C3%A9todo_de_los_elementos_finitos).

Y bueno, las parejas de geometrías las sacamos de [este trabajote](https://academic.oup.com/imrn/article-abstract/1994/9/391/767759?redirectedFrom=fulltext&login=false), por Peter Buser y sus amigos. 

La siguiente imagen muestra como no nos dieron iguales 😆:

![Superficies no isoespectrales](/images/grupo9/non_isospectral_example.png)

Pues nada... En otros escenarios las frecuencias sí se mantienen iguales entre sí, pero en este por ejemplo no, lo que indica que sí hay superficies isospectrales, pero que no son necesariamente las mismas que para el operador Laplaciano...

*¿De qué depende eso? ¿O qué?*

No, ni idea. Un ejercicio como estos pertenece a la matemática ✨experimental✨, osea que miramos más o menos cómo se están comportando estructuras matemáticas diversas y con eso damos pistas para que llegue un matemático teórico más teso y obtenga resultados que expliquen esos comportamientos partiendo de las teorías puras y duras. Lápiz y papel y a darle 🔥

*🫤 ª*

Jajajaj, sí, pero fresc@, que vamos a mitad de camino! Todavía nos queda otra cosa por hacer: Les dije que con el análisis de autovalores también habían logrado estimar el **área** de las geometrías evaluadas, con la **fórmula de Weyl**. Veamos qué tanto se sostiene eso para nuestro caso de oscilación de mecánica del medio continuo 2D.

Checa el blog final para ver el descenlace de esta historia!


*¿Pero si viste? Mero mero poder saber qué son los autovalores, mira que cosa tan llamativamente útil e interesante 💡*