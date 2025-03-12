# Sistemas de primer orden
## Introduccion
Los sistemas de primer orden se modelan por medio de ecuaciones diferenciales de primer orden y son esenciales en el análisis de sistemas de control. Nos permiten estudiar la respuesta ante diferentes tipos de entradas, como escalón, rampa e impulso. Este informe aborda temas como la transformada de Laplace, la función de transferencia y las respuestas temporales de estos sistemas.
## Transformada de Laplace
La transformada de Laplace es una herramienta matemática que convierte ecuaciones diferenciales del dominio del tiempo a ecuaciones algebraicas en el dominio de la frecuencia compleja esto nos facilita el análisis de sistemas dinámicos. La transformada de Laplace de una función f(t) se define como:

$$L\[f(t)]=F(s) $$

## 2. Respuesta Temporal de Sistemas de Primer Orden

### 2.1. Respuesta al Escalón

La respuesta de un sistema de primer orden ante una entrada escalón $$u\(t) = \frac{A}{s}$$ se puede obtener aplicando la transformada de Laplace. La salida en el dominio de Laplace es:

$$Y(s) = \frac{AK}{s(\tau s + 1)}$$


Aplicando fracciones parciales y la transformada inversa de Laplace, se obtiene la respuesta en el tiempo:

$$y(t) = AK(1 - e^{-\frac{t}{\tau}})$$

Esta ecuación muestra que la respuesta al escalón tiene un comportamiento exponencial, donde el sistema alcanza el estado estacionario después de un tiempo determinado por la constante de tiempo $$\( \tau \)$$.

![](500px-Escalon_mod.png)

### 2.2. Respuesta a la Rampa

Para una entrada rampa $$\( u(t) = At \)$$, la salida en el dominio de Laplace es:

$$Y(s) = \frac{AK}{s^2 (\tau s + 1)}$$

Desarrollando las fracciones parciales y aplicando la transformada inversa de Laplace, se obtiene:


$$y(t) = AK \left( t - \tau + \tau e^{-\frac{t}{\tau}} \right)$$


La respuesta a la rampa también tiene un comportamiento exponencial, pero en este caso, la salida no está acotada por un valor constante, sino que crece linealmente con el tiempo.

![](450px-Rampa_mod.png)

### 2.3. Respuesta al Impulso

La respuesta de un sistema de primer orden ante una entrada impulso $$\( \delta(t) \)$$ se obtiene aplicando la transformada de Laplace. La salida en el dominio de Laplace es:

$$Y(s) = \frac{AK}{\tau s + 1}$$

Aplicando la transformada inversa de Laplace, se obtiene la respuesta en el tiempo:

$$y(t) = \frac{AK}{\tau} e^{-\frac{t}{\tau}}$$

Esta respuesta muestra que el sistema tiene un decaimiento exponencial después de un impulso, lo que indica que el sistema disipa la energía rápidamente.

### Entrada parabola

![](capitulo60x.png)

Esta entrada  considera una variacion no lineal en el tiempo lo cual permitira evaluar las condiciones de inicio y final, normalmente se representa como la siguiente expresion:

$$L(r[t])=\frac{A}{s^{3}}$$

