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

#### Ejemplo
Hallar la función de distribución F(x) a partir de la función densidad
{{< katex display>}}
f(x) = \begin{cases}
x/2 \hspace{1cm} (0 \leq x \leq 2) \\
0 \hspace{1cm} (resto)
\end{cases}
{{</ katex >}}

Tenemos que definir la función a trozos:
{{< katex display>}}
f(x) = \begin{cases}
0 \hspace{1cm} (-\infty \leq x \leq 0) \\
x/2 \hspace{1cm} (0 \leq x \leq 2) \\
0 \hspace{1cm} (x > 2) \\
\end{cases}
{{</ katex >}}

Si {{< katex >}}-\infty < x < 0{{</ katex >}}
{{< katex display>}}
F(x) = \int_{-\infty}^{x} f(t) dt = \int_{-\infty}^{x} 0 dt = 0
{{</ katex >}}

Si {{< katex >}}0 \leq x \leq 2{{</ katex >}}
{{< katex display>}}
F(x) = F(0) + \int_{0}^{x} f(t) dt = \int_{0}^{x} \frac{t}{2} dt = \frac{x^2}{4}
{{</ katex >}}

Si {{< katex >}}x > 2 {{</ katex >}}
{{< katex display>}}
F(x) = F(2) + \int_{2}^{x} f(t) dt = \frac{2^2}{4} + \int_{2}^{x} 0 dt = 1
{{</ katex >}}


### Estadísticos poblacionales
{{< columns >}}
#### Media o esperanza matemática
{{< katex display>}}
\mu = E(X) = \int_{-\infty}^{\infty} x \cdot f(x) dx
{{</ katex >}}

<--->
#### Varianza
{{< katex display>}}
\sigma^2 = Var(X) = \int_{-\infty}^{\infty} x^2 \cdot f(x) - \mu^2 dx
{{</ katex >}}
{{< /columns >}}

#### Ejemplo
Sea la función de densidad:
{{< katex display>}}
f(x) = \begin{cases}
0 \hspace{1cm} (x < 0) \\
e^{-x} \hspace{0.6cm} (x \geq x 0)
\end{cases}
{{</ katex >}}

Su media es:
{{< katex display>}}
\mu = \int_{-\infty}^{\infty} x f(x) dx = \int_{-\infty}^{0} x f(x) dx + \int_{0}^{\infty} x f(x) dx = \cdots
{{</ katex >}}

### Distribución uniforme contínua
Una variable aleatoria continua X, cuyo recorrido es el intervalo [a, b] sigue un modelo de distribución uniforme
si todos los valores de la variable son equiprobables

{{< katex display>}}
f(x) = \frac{1}{b - a}
{{</ katex >}}

Su media y varianza valen:
{{< columns >}}
#### Media o esperanza matemática
{{< katex display>}}
\mu = \frac{a + b}{2}
{{</ katex >}}

<--->
#### Varianza
{{< katex display>}}
\sigma^2 = \frac{(b - a)^2}{12}
{{</ katex >}}
{{< /columns >}}

### Distribución normal
Este modelo es el modelo de distribución contínuo más importante, ya que se suele presentar en la naturaleza

Una variable continua X sigue un modelo de distribución normal {{< katex >}}N(\mu, \sigma){{</ katex >}} si su recorrido es R y su
función de densidad vale:
{{< katex display>}}
f(x) = \frac{1}{\sigma \sqrt{2\pi}}e^{-\frac{(x - \mu)^2}{2\sigma^2}}
{{</ katex >}}

La gráfica de la función de densidad se conoce como campana de Gauss. Esta gráfica depende de dos parámetros (media y desviación típica)

#### Propiedades
- La función de densidad es simétrica respecto a la media, por lo tanto su coeficiente de asimetría es 0
- También es mescúrtica, por lo tanto su coeficiente de apuntamiento vale 0
- La media, la mediana y la moda coinciden
- Tiende asintóticamente a 0 cuando x tiende a +- infinito
- Se cumple que:
    - {{< katex >}}P(\mu - \sigma < X \leq \mu + \sigma) = 0.68{{</ katex >}}
    - {{< katex >}}P(\mu - 2\sigma < X \leq \mu + 2\sigma) = 0.95{{</ katex >}}
    - {{< katex >}}P(\mu - 3\sigma < X \leq \mu + 3\sigma) = 0.99{{</ katex >}}

#### Estándar o tipificada
{{< katex display>}}
N(0, 1)
{{</ katex >}}

Para calcularla podemos mirar la tabla tabulada

#### Tipificación
{{< katex display>}}
X ~ N(\mu, \sigma) \rightarrow Z = \frac{X - \mu}{\sigma} ~ N(0, 1)
{{</ katex >}}

{{< hint warning >}}
Para poder mirar en la tabla el valor tiene que ser un número positivo,
si no es el caso tenemos que invertir la condición

**Ejemplo**: P[z <= -3] = P[z >= 3]
{{< /hint >}}

##### Ejemplo
Sea X una variable aleatoria continua con distribución normal N(60, 10) hallar:

{{< katex display>}}
\mu = 60; \sigma = 10
{{</ katex >}}

a) {{< katex >}}P[X \geq 70]{{</ katex >}}
{{< katex display>}}
P[Z \geq \frac{70 - 60}{10}] = P[Z \geq 1] = 0.1587
{{</ katex >}}

b) {{< katex >}}P[X \leq 80{{</ katex >}}
{{< katex display>}}
P[Z \leq \frac{80 - 60}{10}] = P[Z \leq 2] = 1 - P[Z > 2] = 1 - 0.0288 = 0.9772
{{</ katex >}}

c) {{< katex >}}P[X \leq 30{{</ katex >}}
{{< katex display>}}
P[z \leq -3] = P[z \geq 3] = 1.35 \cdot 10^{-3}
{{</ katex >}}

d) {{< katex >}}P[39 \leq X \leq 80]{{</ katex >}}
{{< katex display>}}
P[-2.1 \leq Z \leq 2] = P[Z \geq -2.1] - P[Z > 2] = P[Z \leq 2.1] - P[Z > 2] =
{{</ katex >}}

{{< katex display>}}
1 - P[Z > 2.1] - P[Z > 2] = 1 - 0.0179 - 0.0228 = 0.9593
{{</ katex >}}

#### Correción de continuidad o de Yates
Utilizamos esta corrección cuando aproximamos una distribución binomial o de poisson a una normal

Esto es debido a que con distribuciones binomiales o de poisson estamos trabajando con variables aleatorias discretas y al pasar a una distribución normal estaremos trabajando con variables aleatorias continuas.

**Recordatorio**: La probabilidad para valores fijos de una Variable Aleatoria Continua es cero

| Binomial/Poisson | Normal |
| :---: | :---: |
| $$P[X \leq a]$$ | $$P[X \leq a + 0.5]$$ |
| $$P[X < a]$$ | $$P[X \leq a - 0.5]$$ |
| $$P[X \geq a]$$ | $$P[X \leq a - 0.5]$$ |
| $$P[X > a]$$ | $$P[X \leq a + 0.5]$$ |
| $$P[X = a]$$ | $$P[a - 0.5 \leq X \leq a + 0.5]$$ |
| $$P[a \leq X \leq b]$$ | $$P[a - 0.5 \leq Y \leq a + 0.5]$$ |
| $$P[a < X < b]$$ | $$P[a + 0.5 \leq Y \leq b - 0.5]$$ |

##### Ejemplo (Aproximación de la binomial)
Para acceder a un puesto ejecutivo, los aspirantes deben realizar un test de 100 preguntas con 5 posibles respuestas.
Si uno de ellos contesta al azar, ¿cuál es la probabilidad de que acierte más de 25 preguntas? ¿Y menos de 30?

X = Acertar

n = 100 preguntas

p = 1/5 = 0.2

X ~ B(100, 0.2)

Vamos a comprobar si reune las condiciones para poder pasarla de binomial a normal:
- {{< katex >}}np > 5 \rightarrow 100 \cdot 0.2 = 20 > 5{{</ katex >}}
- {{< katex >}}n(1 - p) > 5 \rightarrow 100(1 - 0.2) = 80 > 5{{</ katex >}}

**Reune las condiciones**
{{< katex display>}}
X ~ B(100, 0.2) = N(np, \sqrt{np(1 - p)})
{{</ katex >}}

{{< katex display>}}
X ~ B(100, 0.2) \approx N(20, 4)
{{</ katex >}}

Calculamos la prob. de acertar más de 25 preguntas:

Tenemos que aplicar la corrección de continuidad y después tipificar
{{< katex display>}}
P[X > 25] = P[Y \geq 25 + 0.5] = P[Y \geq 25.5] = P[Z \geq \frac{25.5 - 20}{4}] = P[Z \geq 1.38] = 0.0838
{{</ katex >}}

**Un 8.38% acertaría más de 25 preguntas**

Calculamos la probabilidad de acertar menos de 30 preguntas:

Aplicamos el mismo procedimiento que en el apartado anterior
{{< katex display>}}
P[X < 30] = P[Y \leq 30 - 0.5] = P[Y \leq 29.5] = P[Z \leq \frac{29.5 - 20}{4}] = P[Z \leq 2.38] = 1 - P[Z > 2.38] = 1 - 0.0087 = 0.9913
{{</ katex >}}

**Un 99.13% acertaría menos de 30 preguntas**
