# Sistemas de primer orden
## Introduccion
Los sistemas de primer orden se modelan por medio de ecuaciones diferenciales de primer orden y son esenciales en el análisis de sistemas de control. Nos permiten estudiar la respuesta ante diferentes tipos de entradas, como escalón, rampa e impulso. Este informe aborda temas como la transformada de Laplace, la función de transferencia y las respuestas temporales de estos sistemas.
## Transformada de Laplace
La transformada de Laplace es una herramienta matemática que convierte ecuaciones diferenciales del dominio del tiempo a ecuaciones algebraicas en el dominio de la frecuencia compleja esto nos facilita el análisis de sistemas dinámicos. La transformada de Laplace de una función f(t) se define como:
\[
\mathcal{L}\{f(t)\} = F(s)
\]

## Entradas de prueba a un sistema
### Entrada escalon


![](500px-Escalon_mod.png)


Representa un cambio de nivel de forma repentina. representada por la siguiente ecuacion:

$$L(u[t])=\frac{A}{s}$$

### Entrada rampa


![](450px-Rampa_mod.png)


Esta señal varia en el tiempo de forma lineal, representada por la siguiente ecuacion:

$$L(x[t])=\frac{A}{s^{2}}$$

### Entrada parabola
![](capitulo60x.png)

Esta entrada  considera una variacion no lineal en el tiempo lo cual permitira evaluar las condiciones de inicio y final, normalmente se representa como la siguiente expresion:

$$L(r[t])=\frac{A}{s^{3}}$$

## Ecuaciones de primer orden
