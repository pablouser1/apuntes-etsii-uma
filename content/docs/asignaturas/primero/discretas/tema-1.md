---
weight: 1
---
{{< katex >}}{{</ katex >}}
# Aritmética
## División Euclídea
$$n = m \cdot q + r$$

* n = Dividendo
* m = Divisor
* q = Cociente
* r = Resto

## Algoritmo de euclides
{{< youtube rG9nQe-7is8 >}}

Para calcular el mcd(a, b) aplicamos la división euclídea hasta que el resto sea 0.

El resto anterior será el mcd de a y b

## Identidad de Bezout
{{< youtube EUqkQB2YdKE >}}

## Ecuaciones diofánticas
{{< youtube DuNQIsTQu9o >}}

$$150x + 39y = 228$$

* Aplicamos el [alg. de euclides](#algoritmo-de-euclides) para conseguir el mcd(150, 39)
    * {{< katex >}} mcd(150, 39) = 3 {{</ katex >}}
* Comprobamos si tiene solución viendo si el término independiente (228) es múltiplo del resultado del mcd
* Aplicamos la identidad de Bezout
    * {{< katex >}} 150 \cdot 6 + 39 \cdot (-23) {{</ katex >}}
* Escribimos el término independiente como múltiplo del resultado del mcd
    * {{< katex >}} 228 = 3 \cdot 76{{</ katex >}}
* Sobre la Identidad de Bezout multiplicamos por el resultado del paso anterior (76)
    * {{< katex >}} 150 \cdot 6 \cdot 76 + 39 \cdot (-23) \cdot 76 = 228{{</ katex >}}
* El primer resultado sería {{< katex >}} 6 \cdot 76 {{</ katex >}} y {{< katex >}} (-23) \cdot 76 {{</ katex >}}

## Congruencia
$$a \equiv b \pmod{m}$$
$$a \cdot x + m \cdot y = b$$

### Inverso
$$[a]_{m}^{-1} = a^{\phi m}$$

### Teorema de Brahmagupta
$$a \equiv b \pmod{m}$$

* Tiene solución si y sólo si mcd(a, m) divide a b

## Euler-Fermat
### Función de Euler
* Si p es primo: {{< katex >}} \phi(p) = p - 1{{</ katex >}}
* Si p no es primo: {{< katex >}} \phi(p) = p^e - p^{e - 1}{{</ katex >}}
* Si m y n son coprimos: {{< katex >}} \phi(m, n) = \phi(m) \cdot \phi(n){{</ katex >}}

Caso general:

Número de enteros positivos menores que n y coprimos con n.

#### Ejemplo
$$\phi(180) = \phi(2^2 \cdot 3^2 \cdot 5^1) = (2^2 - 2) (3^2 - 3) (5^1 - 5^0) = 48$$

### Teorema
Sirve para resolver ecuaciones diofánticas no muy grandes cuando mcd(a, m) = 1

$$a^{\phi(m)} \equiv 1 \pmod{m}$$

#### Ejemplo
$$2x \equiv 8 \pmod{9}$$

mcd(2, 9) = 1, así que podemos continuar

$$x \equiv 2^{\phi(9) - 1} \cdot 8 \pmod{9}$$
$$x \equiv 2^5 \cdot 8 \pmod{9}$$
$$x \equiv 4 \pmod{9}$$

## Sistema de congruencias lineales
{{< youtube xAQiFowBJ3Q >}}
