---
weight: 5
---

# Tema 5 (Variables aleatorias)
## Recursos
{{< tabs "videos" >}}
{{< tab "Video 3.8" >}}
{{< youtube VofLkVdpKas >}}
{{< /tab >}}
{{< tab "Video 3.9" >}}
{{< youtube huA6HA9RMko >}}
{{< /tab >}}
{{< tab "Video 3.10" >}}
{{< youtube ZJT63lU6BoI >}}
{{< /tab >}}
{{< tab "Video 3.11" >}}
{{< youtube Z_AmMo50U4Q >}}
{{< /tab >}}
{{< /tabs >}}

## Introducción
Una variable aleatoria (X) es una función que asocia cada elemento del espacio muestral un número real

Se pueden clasificar en dos tipos:
- Discretas
    - Toman valores aislados (recorrido finito/infinito numerable)
    - Ejemplo: Nº hijos, nº accidentes, nº cigarrillos...
- Continuas
    - Valores en un intervalo real
    - Ejemplo: Peso, estatura, nivel de colesterol...

### Ejemplo básico
Experimento: Lanzar 2 monedas

X: Sacar cara

Posibilidades (E): { (C, C), (x, x), (C, x), (x, C) }

X(C, C) = 2

X(x, x) = 0

X(C, x) = 1

## Discretas
### Función de probabilidad
La función de probabilidad de una variable discreta (X) es una función f(x) que asocia a cada valor su probabilidad
$$p_i = f(x_i) = P(X = x_i)$$

#### Ejemplos
##### Ejemplo 1
Tenemos una variable discreta que mide el número de caras en el lanzamiento de una moneda

E = { (C, C), (x, x), (C, x), (x, C) }

X: E --> R
- (c, c) = 2
- (c, x) = 1
- (x, c) = 1
- (x, x) = 0

Los valores que puede tomar
X = 0, 1, 2

Usando la regla de Laplace:
| X | 0 | 1 | 2 |
| :---: | :---: | :---: | :---: |
| $$f(x) = P(X = x_i)$$ | $$P(X = 0) = 1/4$$ | $$P(X = 1) = 1/2$$ | $$P(X = 2) = 1/4$$ |

##### Ejemplo 2
Experimento: Lanzo un dado

X = Sacar un resultado

E = {1, 2, 3, 4, 5, 6}

X = E --> R
- 1 = 1
- 2 = 1
- 3 = 1
- 4 = 1
- 5 = 1
- 6 = 1

Usando la regla de Laplace:

| X | 1 | 2 | 3 | 4 | 5 | 6 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| $$f(x) = P(X = x_i)$$ | 1/6 | 1/6 | 1/6 | 1/6 | 1/6 | 1/6 |

### Función de distribución
La función de distribución de una variable discreta X es una función F(x) que asocia a cada valor xi la probabilidad de que la variable
tome un valor menor o igual que el dicho valor.

$$F(-\infty) = 0$$
$$F(+\infty) = 1$$

#### Ejemplos
##### Ejemplo 1
| X | 0 | 1 | 2 |
| :---: | :---: | :---: | :---: |
| f(x) | 1/4 | 1/2 | 1/4 |
| F(x) | 1/4 | 1/2 + 1/4 | 1/4 + 1/2 + 1/4 (Siempre tiene que ser uno) |

F(x) también se puede escribir como una función a trozos

{{< katex display>}}
F(x) = \begin{cases}
0 \hspace{1cm} (x < 0) \\
0.25 \hspace{1cm} (0 \leq x < 1) \\
0.75 \hspace{1cm} (1 \leq x < 2) \\
1 \hspace{1cm} (x \geq 2)
\end{cases}
{{</ katex >}}

$$P(X = 0) = 0.25$$
$$P(X = 1) = 0.5$$
$$P(X = 2) = 0.25$$

##### Ejemplo 2
| X | 1 | 2 | 3 | 4 | 5 | 6 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| f(x) | 1/6 | 1/6 | 1/6 | 1/6 | 1/6 | 1/6 |
| F(x) | 1/6 | 2/3 | 3/6 | 4/6 | 5/6 | 6/6 |

{{< katex display>}}
F(x) = \begin{cases}
0 \hspace{1cm} (x < 1) \\
1/6 \hspace{1cm} (1 \leq x < 2) \\
2/6 \hspace{1cm} (2 \leq x < 3) \\
3/6 \hspace{1cm} (3 \leq x < 4) \\
4/6 \hspace{1cm} (4 \leq x < 5) \\
5/6 \hspace{1cm} (5 \leq x < 6) \\
1 \hspace{1cm} (x \geq 6)
\end{cases}
{{</ katex >}}

##### Ejemplo 3
Una variable aleatoria X tiene la siguiente función de distribución:

{{< katex display>}}
F(x) = \begin{cases}
0 \hspace{1cm} (x < 0) \\
1/9 \hspace{1cm} (0 \leq x < 2) \\
4/9 \hspace{1cm} (2 \leq x < 3) \\
1 \hspace{1cm} (x \geq 3)
\end{cases}
{{</ katex >}}

Calcule P[(0, 2)], P[[0, 2)], P[[0, 2]]

$$P[(0, 2)] = F(2^{-}) - F(0) = 1/9 - 1/9 = 0$$

$$P[[0, 2)] = F(2^{-}) - F(0^{-}) = 1/9 - 0 = 1/9$$

$$P[[0, 2]] = F(2) - F(0^-) = 4/9 - 0 = 4/9$$

Para encontrar estos valores nos tenemos que fijar en la función F(x), en este caso nos piden (0, 2) ambos intervalos abiertos.

### Distribución uniforme
Características:
- Partimos de un experimento aleatorio
- Tenemos dos posibles resultados (éxito o fracaso)
Este caso se aplica en casos en la que cada elemento del conjunto tiene la misma probabilidades de aparecer

Por ejemplo, el experimento de tirar un dado sería uniforme, ya que todos los elementos (1, 2, 3, 4, 5, 6) tienen la misma probabilidad de aparecer

### Distribución binomial
Antes de empezar, hablaremos del modelo de Bernoulli

Digamos que lanzamos una moneda:
- 1 éxíto (Cara)
- 0 fracaso (Cruz)

Por lo que, P(éxito) = 1/2

Esto se denota: X --> B(p)

El modelo de Bernoulli es un caso particular de la distribución binomial.

La distribución binomial es un experimento aleatorio con las características:
- Consiste en una secuencia con n repeticiones
- Los ensayos se hacen bajo idénticas condiciones
- Los ensayos son independientes entre si
- La probabilidad de éxito es idéntica para todos los ensayos

Una variable aleatoria sigue este modelo si su recorrido es Re(X) = {0, 1, \cdots, n} y su función de probabilidad es:
{{< katex display>}}
f(x) = \binom{n}{x} p^{x}(1 - p)^{n - x}
{{</ katex >}}

Esta información también se puede sacar de la tabla, no hace falta aplicar la fórmula

#### Ejemplo
Experimento: Lanzar una moneda 4 veces

n = 4 veces

p = 0.5

X --> B(n, p) = X --> B(4, 0.5)

a) P[X = Salir dos caras]

$$f(x) = 0.375$$

b) P[X <= 2 caras]

$$F(2) = P[X = 0] + P[X = 1] + P[X = 2] = 0.0625 + 0.25 + 0.375 = 0.6875$$

c) P[X > 2]

$$1 - P[X <= 2] = 1 - 0.6875 = 0.3125$$

### Distribución Poisson
Es un experimento aleatorio con las características:
- Consiste en observar la aparición de los fenómenos puntuales (Ej: Llamadas recibidas a una centralita)
- Este experimento produce a largo plazo un número medio de fenómenos puntuales por unidad de soporte continuo ({{< katex >}}\lambda{{</ katex >}})

La variable aleatoria X mide el número de ocurrencias del fenómeno por unidad de soporte continuo sigue un modelo de distribución de Poisson

Su función de probabilidad es:
{{< katex display>}}
f(x) = e^{-\lambda} \cdot \frac{\lambda^x}{x!}
{{</ katex >}}

#### Ejemplo
La llegada de vehículos a una gasolinera es de {{< katex >}}P(\lambda = 1.6){{</ katex >}}

Calcula la probabilidad de que el número de vehículos que lleguen a la gasolinera sea mayor que tres

X ~ P(1.6)

{{< katex display>}}
P[X > 3] = 0.0551 + 0.0176 + 0.0047 + 0.0011 + 0.0002 = 0.0789
{{</ katex >}}

## Continuas
Se caracterizan por tomar cualquier valor en un intervalo real, por lo tanto, son infinitas y no numerables.

Esto hace imposible el cálculo de posibilidades, por lo que no podremos usar la función de probabilidad para definir los modelos de distribución.

### Función de densidad
Es una función que:
- Siempre es positiva
- El área encerrada entre f(x) y el eje de absicas es 1

{{< katex display>}}
\int_{-\infty}^{\infty} f(x) dx = 1
{{</ katex >}}

y tal que la probabilidad de que la variable tome un valor dentro de un intervalo cualquiera [a, b] es de:

{{< katex display>}}
P(a \leq X \leq b) = \int_{a}^{b} f(x) dx
{{</ katex >}}

### Función de distribución
Es uan función F(x) que asocia cada valor la posibilidad de que la variable tome un valor
menor o igual que dicho valor

{{< katex display>}}
F(x_i) = P(X \leq x_i) = \int_{-\infty}^{x_i} f(x) dx
{{</ katex >}}

IMPORTANTE:
{{< katex display>}}
f(x) = F'(x)
{{</ katex >}}

Lo que quiere decir que la función densidad es la derivada de la función de distribución
