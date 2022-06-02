---
weight: 4
---

# Tema 4 (Probabilidad)
## Recursos
{{< tabs "videos" >}}
{{< tab "Video 3.6" >}}
{{< youtube yIL9lzL7QdM >}}
{{< /tab >}}
{{< tab "Video 3.7" >}}
{{< youtube WPbIGxmHoqg >}}
{{< /tab >}}
{{< /tabs >}}

## Experimentos y sucesos aleatorios
{{< hint info >}}
Un experimento aleatorio es aquel en el que se conocen los posibles resultados pero no se conoce cuál será el resultado contreto
de este experimento
{{< /hint >}}

Por ejemplo, un lanzamiento de dado es un experimento aleatorio ya que:
- Se conocen los posibles resultados (1, 2, 3, 4, 5, 6)
- Antes de lanzar el dado no se puede predecir con certeza el valor que saldrá

### Espacio muestral
{{< hint info >}}
Es el conjunto de todos los posibles resultados de un experimento aleatorio. Se suele denotar con E
{{< /hint >}}

Ejemplo:
- Lanzar una moneda: E = {c, x}
- Lanzar un dado: E = {1, 2, 3, 4, 5, 6}
- Grupo sanguíneo de un individuo seleccionado al azar: E = {A, B, AB, 0}

### Suceso aleatorio
{{< hint info >}}
Es cualquier subconjunto del espacio muestral E
{{< /hint >}}

Existen varios tipos:
- Suceso imposible: Es el subconjunto vacío {{< katex >}}\emptyset{{</ katex >}}. Este suceso _nunca_ ocurre
- Sucesos elementales: Subconjuntos formados por un solo elemento
- Sucesos compuestos: Subconjuntos formados por dos o más elementos
- Suceso seguro: Es el propio espacio muestral. Este suceso _siempre_ ocurre

### Espacio de sucesos
{{< hint info >}}
Dado un espacio muestral E de un experimento aleatorio, el conjunto formado por todos los
posibles sucesos de E se llama espacio de sucesos de E se llama espacio de sucesos de E y se denota P(E)
{{< /hint >}}

#### Ejemplo
Dado el espacio muestral E = {a, b, c}:

P(E) = {{< katex >}}[\emptyset, (a), (b), (c), (a, b), (a, c), (b, c), E]{{</ katex >}}

## Teoría de conjuntos
- Unión {{< katex >}}\cup{{</ katex >}}
- Intersección {{< katex >}}\cap{{</ katex >}}
- Diferencia simétrica {{< katex >}}\triangle{{</ katex >}}
- Complementario: A ~ {{< katex >}}\bar{A}{{</ katex >}}

### Unión
El suceso {{< katex >}}A \cup B{{</ katex >}} ocurre siempre que ocurre A **o** B

Ejemplo: Tiramos un dado

E = (1, 2, 3, 4, 5, 6)

A = (2, 4, 6) y B (1, 2, 3, 4)

{{< katex >}}A \cup B = (1, 2, 3, 4, 6){{</ katex >}}

### Intersección
El suceso {{< katex >}}A \cap B{{</ katex >}} ocurre siempre que ocurre A **y** B

Ejemplo: Tiramos un dado

E = (1, 2, 3, 4, 5, 6)

A = (2, 4, 6) y B = (1, 2, 3, 4)

{{< katex >}}A \cap B = (2, 4){{</ katex >}}

### Diferencia
El suceso diferencia A - B es todos los elementos de A que no pertenezca en B

Ejemplo: Tiramos un dado

E = (1, 2, 3, 4, 5, 6)

A = (2, 4, 6) y B (1, 2, 3, 4)

A - B = Todo lo que está en A que no está en B = (6)

### Diferencia simétrica
{{< katex display >}}
A \triangle B = (A - B) \cup (B - A)
{{</ katex >}}

El suceso diferencia simétrico es el suceso formado por todos los sucesos que están en A o en B pero **no** en ambos

### Contrario
El suceso contrario {{< katex >}}\bar{A}{{</ katex >}} ocurre siempre que no ocurre A

### Álgebra de sucesos
Dado los sucesos A, B, C perteneciente a P(E) se cumplen las siguientes propiedades:
- {{< katex >}}A \cup A = A; A \cap A = A{{</ katex >}} (idempotencia)
- {{< katex >}}A \cup B = B \cup A; A \cap B = B \cap A{{</ katex >}} (conmutativa)
- {{< katex >}}(A \cup B) \cup C = A \cup (B \cup C); (A \cap B) \cap C = A \cap (B \cap C){{</ katex >}} (asociativa)
- {{< katex >}}(A \cup B) \cap C = (A \cap C) \cup (B \cap C); (A \cap B) \cup C = (A \cup C) \cap (B \cup C){{</ katex >}} (distributiva)
- {{< katex >}}A \cup \emptyset = A; A \cap E = A{{</ katex >}} (elemento neutro)
- {{< katex >}}A \cup E = E; A \cap \emptyset = \emptyset{{</ katex >}} (elemento absorvente)
- {{< katex >}}A \cup \bar{A} = E; A \cap \bar{A} = \emptyset{{</ katex >}} (elemento simétrico complementario)
- {{< katex >}}\bar{\bar{A}} = A{{</ katex >}} (doble contrario)
- {{< katex >}}\bar{A \cup B} = \bar{A} \cap \bar{B}; \bar{A \cap B} = \bar{A} \cup \bar{B}{{</ katex >}} (leyes de Morgan)
- {{< katex >}}A \cap B \subseteq A \cup B{{</ katex >}}

## Definición de probabilidad
### Probabilidad clásica de Laplace
Para hallar la probabilidad de un suceso usando el método de probabilidad clásica de Lapllace tenemos que usar la siguiente fórmula:
{{< katex display >}}
P(A) = \frac{|A|}{|E|}
{{</ katex >}}

Siendo:
- |A|: Número de casos favorables a A
- |E|: Número de casos posibles

Esta definición es ampliamente utilizada, pero tiene las siguientes restricciones:
{{< hint danger >}}
- No puede utilizarse con espacios muestrales infinitos, o de los que no conocemos el número de casos
- Todos los elementos del espacio muestral deben tener la misma probabilidad de ocurrir
- No se cumple en muchos experimentos aleatorios reales
{{< /hint >}}
#### Ejemplo
Tenemos un dado E = {1, 2, 3, 4, 5, 6}

A = Par

Nº de casos favorables: 3 (2, 4, 6),
Nº de casos posibles: 6

{{< katex display >}}
P(A) = \frac{3}{6} = 0.5
{{</ katex >}}

### Probabilidad frecuentista
Esta definición se apoye en la ley de los grandes números, su definición es la siguiente:
{{< hint info >}}
Cuando repetimos un experimento muchas veces, la frecuencia relativa tiende a estabilizarse en torno a un número, el cuál sería
su probabilidad
{{< /hint >}}

Con este teorema, podemos suponer que:
{{< katex display >}}
P(A) = \lim_{n\to\infty} \frac{n_{A}}{n}
{{</ katex >}}

Esta definición es muy útil en experimentos reproducibles pero tiene los siguientes inconvemientes:
{{< hint danger >}}
- Sólo se calcula una aproximación de la probabilidad real
- La repetición del experimento tiene que ser en las mismas condiciones
{{< /hint >}}

### Probabilidad axiomática
{{< hint info >}}
- La probabilidad de un suceso cualquiera es positiva o nula
- La posibilidad de la unión de dos sucesos incompatibles es igual a la suma de las probabilidades de cada uno de ellos
- La probabilidad de un suceso cierto siempre es igual a 1
{{< /hint >}}
#### Consecuencias de los axiomas de probabilidad
- {{< katex >}}P(\bar{A}) = 1 - P(A){{</ katex >}}
- {{< katex >}}P(\emptyset) = 0{{</ katex >}}
- Si {{< katex >}}A \subseteq B{{</ katex >}} entonces {{< katex >}}P(A) \leq P(B){{</ katex >}}
- {{< katex >}}P(A) \leq 1{{</ katex >}}
- Si A y B son sucesos compatibles, entonces
{{< katex display >}}
P(A \cup B) = P(A) + P(B) - P(A \cap B)
{{</ katex >}}
- Si el suceso A está compuesto por los sucesos elementeales e1, e2, e3, ..., en, entonces
{{< katex display >}}
P(A) = \sum_{i = 1}^{n} P(e_i)
{{</ katex >}}

## Probabilidad condicionada
Dado dos sucesos A y B de un mismo espacio de sucesos de un experimento aleatorio, la probabilidad condicionada de A por B es:
{{< katex display >}}
P(A/B) = \frac{P(A \cap B)}{P(B)}
{{</ katex >}}

De esta definición se deduce que la posibilidad de intersección es:
{{< katex display >}}
P(A \cap B) = P(A) \cdot P(B/A) = P(B) \cdot P(A/B)
{{</ katex >}}

### Ejemplo
Hemos observado la siguiente frecuencia de aprobados:

| - | Aprobados | Suspensos | Total |
| :---: | :---: | :---: | :---: |
| Mujeres | 80 | 20 | 100 |
| Hombres | 60 | 40 | 100 |
| - | 140 | 60 | 200 |

¿Cuál es la probabilidad de que una persona al azar haya aprobado?
{{< katex display >}}
P(A) = \frac{140}{200} = 0.7
{{</ katex >}}

¿Cuál es la probabilidad de que una mujer al azar haya aprobado?
{{< katex display >}}
P(A/M) = \frac{80}{100} = 0.8
{{</ katex >}}

Ahora vamos a hacer este mismo apartado usando la fórmula de la probabilidad condicionada

¿Cuál es la probabilidad de que una persona al azar haya aprobado?
{{< katex display >}}
P(A/M) = \frac{P(A \cap M)}{P(M)} = \frac{80/200}{100/200} = 0.8
{{</ katex >}}

## Dependencia/Independencia de sucesos
Dos sucesos son independientes cuando:
{{< katex display >}}
P(A/B) = P(A)
{{</ katex >}}

También se cumple que si A y B son independientes, entonces:
{{< katex display >}}
P(A \cap B) = P(A) \cdot P(B)
{{</ katex >}}

## Árbol de probabilidad
Sea una población en la que el 30% de personas fuman y que la incidencia del cáncer de pulmón en fumadores el del 40%
mientras que en los no fumadores el del 10%.

El árbol de probabilidad en este experimento es:
{{< mermaid >}}
flowchart LR
    P[Probabilidad] --> F["F (0.3)"] & NF["NF (0.7)"]
    F --> C["Cáncer (0.4)"] & NC["NC (0.6)"]
    NF --> C2["Cáncer (0.1)"] & NC2["NC (0.9)"]
{{< /mermaid >}}

Vamos a calcular la probabilidad de que la persona fume y tenga cáncer
{{< katex display >}}
P(F \cap C) = P(F) \cdot P(C/F) = 0.3 \cdot 0.4
{{</ katex >}}

Vamos a calcular la posibilidad de que no fume y no tenga cáncer
{{< katex display >}}
P(\bar{F} \cap \bar{C}) = P(\bar{F}) \cdot P(\bar{C}/\bar{F}) = 0.7 \cdot 0.9
{{</ katex >}}

## Teorema de la probabilidad total
Antes de definir la probabilidad total, tenemos que entender cómo funciuona el sistema completo de sucesos:

Una colección de sucesos: A1, A2, ..., An de un mismo espacio de sucesos es un sistema completo si cumple lo siguiente:
- La unión de todos es el espacio muestral: {{< katex >}}A_i \cup \cdots \cup A_n = E{{</ katex >}}
- Son incompatibles dos a dos: {{< katex >}}A_i \cap A_j = \emptyset{{</ katex >}}

Con esto, ya podemos definir la probabilidad total:

Dado un sistema completo de sucesos A1, ..., An y un suceso B de un mismo espacio de sucesos, se cumple:
{{< katex display >}}
P(B) = \sum_{i = 1}^{n} P(A_i) \cdot P(B/A_i)
{{</ katex >}}

### Ejemplo
Un determinado síntoma B puede ser originado por una enfermedad A pero también lo pueden tener personas sin enfermedad.
Sabemos que en la población la tasa de personas con la enfermedad A es 0.2. Además, de las personas que presentan la enfermedad el 90% tiene síntomas, mientras que los no tienen la enfermedad presentan el 40%

Si tomamos una persona al azar, ¿qué posibilidad hay que tenga el síntoma?
{{< mermaid >}}
flowchart LR
    P[P] --> E["E(0.2)"] & NE["NE (0.8)"]
    E --> S["Síntoma (0.9)"] & NS["NS (0.1)"]
    NE --> S2["Síntoma (0.4)"] & NCS["NS (0.6)"]
{{< /mermaid >}}

En este caso podemos aplicar el teorema de la probabilidad total, ya que:
- E y NE son incompatibles entre si (no puedes estar enfermo y no enfermo al mismo tiempo)
- La unión entre enfermo y no enfermo es el total de la población (son los dos únicos casos posibles)

{{< katex display >}}
P(S) = P(E) \cdot P(S/E) + P(\bar{E}) \cdot P(S/E) = 0.2 \cdot 0.9 + 0.8 \cdot 0.4 = 0.5
{{</ katex >}}

Es decir, si elegimos a una persona aleatoria tenemos un 50% de probabilidades de que tenga el síntoma

## Teorema de Bayes
Dado un sistema completo de sucesos y un suceso B de un mismo espacio de sucesos, se cumple:

{{< katex display >}}
P(A_i/B) = \frac{P(A_i) \cdot P(B/A_i)}{\sum_{i = 1}^{n} P(A_i) \cdot P(B/A_i)}
{{</ katex >}}

### Ejemplo
En una empresa de auditorias se han contratado a tres personas para inspeccionar a las empresas bancarias realizando auditorias. La primera efectua el 30%, la segunda el 45% y la tercera el 25%. Se ha comprobado que de las inspecciones realizadas por la primera persona, el 1% es erroneo, del segundo el 3% y del tercero el 2%.

Al elegir una inspección correcta. ¿Cuál es la probabilidad de que la haya realizado la segunda persona?
{{< mermaid >}}
flowchart LR
    P[P] --> 1["1 (0.3)"] & 2["2 (0.45)"] & 3["3 (0.25)"]
    1 --> E["E (0.01)"] & NE["NE (0.99)"]
    2 --> E2["E (0.03)"] & NE2["NE (0.97)"]
    3 --> E3["E (0.02)"] & NE3["NE (0.98)"]
{{< /mermaid >}}

{{< katex display >}}
P(2/E) = \frac{P(2) \cdot P(E/2)}{P(1) \cdot P(E/1) + P(2) \cdot P(E/2) + P(3) \cdot P(E/3)}
{{</ katex >}}

{{< katex display >}}
P(2/E) = \frac{0.45 \cdot 0.03}{0.3 \cdot 0.01 + 0.45 \cdot 0.03 + 0.25 \cdot 0.02} = 0.554
{{</ katex >}}
