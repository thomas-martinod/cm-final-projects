---
title: "Escuchando la forma de un tambor, o , ¿Qué #%$&$ es un autovalor?"
date: 2024-03-06
draft: false
github_link: "https://github.com/thomas-martinod/proyectos-finales-CM"
author: "José Ortiz-Ocampo"
tags:
  - Anteproyecto
  - Grupo 9
  - Análisis espectral
  - Propagación de ondas
  - Mecánica del medio continuo
image: /images/grupo9/circular_membrane_oscillation.png
description: "Como la matemática nos ayudar a escuchar formas, y una (de muchas) aplicaciones del análisis de autovalores y autofunciones de un operador (análisis espectral, para los jijijjujuju académicos)"
toc: false
mathjax: true
---
### Ojo: Lo que sigue es divulgación físico-matemática altamente adictiva! Siga con precaución ⚠️

# *¿Cómo así que escuchar una forma?*

Sí, así como lo ve. Consiste en determinar la **forma** de un tambor **sin verlo**, solamente escuchando los sonidos que genera. 

*¿Cómo es eso posible?* Ponga cuidado, aquí se lo explicamos sencillito:

- El sonido es una onda, y uno de los factores que la describen es su frecuencia. Esto es como decir que suena un **Do** o un **La** en música.
- El sonido del tambor se genera cuando uno le ✨ pega ✨. Eso lo pone a vibrar. Esa vibración genera la onda que uno escucha.
- Resulta que cualquier vibración que se logre sobre el tambor es, sí o sí, una combinación de vibraciones naturales que puede tener este por la forma de su membrana. A estas las llamamos **modos de oscilación** del tambor.
- Y resulta que esos modos de oscilación tienen asociadas **frecuencias naturales de oscilación**. Y como cualquier vibración es una combinación de los modos, así mismo cualquier sonido que emita el tambor es una combinación de esas frecuencias!

*¿O sea que qué?*

O sea que si uno coge el sonido del tambor, y les saca las frecuencias que tenga, que se conocen como el **espectro**, puede estimar la forma del tambor sin verlo. Like a pro 😎

*🤯 NO!, eso es posible enserio?*

Jajajaja, ... no 😢. Hay un pequeño problema en esta metodología, y es cómo calcular la forma a partir de las frecuencias que se hallen. 

Y, más grave todavía, es que asumimos que un único conjunto de frecuencias solo puede ser generado por una única forma, osea, que no hay dos formas que puedan sonar igual. Y resulta que sí, que **sí hay formas diferentes que generan las mismas frecuencias**, o sea, que pueden sonar potencialmente igual (dependiendo de cómo se les ✨ pegue ✨). Estas preguntas planteó muy famosamente en un artículo llamado [*¿Se puede oír la forma de un tambor?*](https://es.wikipedia.org/wiki/Escuchar_la_forma_de_un_tambor), escrito por Mark Kac en 1966. Y, en 1992, Carolyn gordon, David Webb y Scott Wolpert construyeron formas de superficies que compartían las mismas frecuencias, o sea, que son **isoespectrales**.

![Superficies isoespectrales](/images/grupo9/isospectral_surfaces.png)

# *¿Cómo se sabe eso? ¿Y qué tenía esto que ver con los tales auto-nosequé?*

Matemágicas! Resulta que hallar los posibles modos y frecuencias de oscilación consiste, después de bastante carreta, en solucionar una ecuación de la forma:

$$ A u_n = {\lambda}_n u_n $$

donde \\(u_n\\) es una función que describe el n-ésimo modo de oscilación y se llama **autofunción**, \\({\lambda}_n\\) es la frecuencia de oscilación asociada y se denomina **autovalor** y $A$ es un **operador**, que es un algo que opera sobre una función. Particularmente este operador es **diferencial** (o sea que las operaciones que hace incluyen derivadas), y es nada más y nada menos que el famosísimo **Laplaciano** (\\({\nabla}^2\\) para los de confianza). Entonces los modos y frecuencias de oscilación no son nada más y nada menos que los **autovalores y autofunciones del operador Laplaciano** (evaluado en el área con la forma del tambor). 

Este modelamiento matemático de la vibración de una membrana es lo que nos permite calcular las frecuencias y modos de oscilación. Y, aunque en efecto no nos dió para calcular la forma a partir de las frecuencias, el análisis de los autovalores sí nos dejó un regalito: Podemos calcular **el área** del tambor a partir de que tan rápido crecen las frecuencias de los modos de oscilación. Esta fórmula se conoce como **fórmula de Weyl** en honor a [don Hermann Weyl](https://es.wikipedia.org/wiki/Hermann_Weyl).

Pero bueno, hay una luz de esperanza. Y es que el modelo usado asume que el tambor es infinitamente delgado, hace caso omiso de las propiedades del material que lo compone, y en general idealiza el fenómeno. Se plantearon las mismas preguntas, esta vez usando la **Mecánica del Medio Continuo** para estudiar estas mismas propiedades pero para el **Operador de propagación de onda en mecánica clásica**. ¿Será que bajo ese nuevo modelo, las superficies isoespectrales lo siguen siendo? Será que cambia la forma de calcular el área? ¿Qué pasa si es un tambor más grueso, o una placa de metal? ...

# *¿Y qué hallaron? Cambiaron los resultados?*

🚧 No sabemos todavía! 🚧 

Sigue sintonizado a este blog para ver el desenlace de esta historia! 