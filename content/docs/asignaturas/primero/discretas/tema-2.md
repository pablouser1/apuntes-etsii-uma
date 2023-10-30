---
weight: 2
---

# Conjuntos y recuentos
{{< katex >}}
r = |A|
{{</ katex >}}
<br/>
{{< katex >}}
n = |B|
{{</ katex >}}

### Tabla resumen
| Objeto | Recipiente | ¿Pueden haber vacíos? | Solución |
| :--: | :--: | :--: | :--: |
| Indistinguible | Distinguible | Sí | [$$CR(n, r)$$](#con-repetición) |
| Distinguible | Distinguible | No | [$$n! \cdot S(r, n)$$](#aplicaciones-sobreyectivas-de-a-en-b) |
| Distinguible | Indistinguible | No | [$$S(r, n)$$](#particiones) |

## Números de Stirling
$$S(r. n) = S(r - 1, n - 1) + n \cdot S(r - 1, n)$$

{{< katex >}}
S(r, 1) = 1
;
S(r, r) = 1
{{</ katex >}}

## No importa el orden
### Combinaciones
$$C(n,r) = \frac{n!}{r!(n-r)!} = \binom{n}{r}$$
Los elementos no pueden repetirse y, porque no importa el orden
en el que dispongamos los elementos de la combinación, de n
objetos escogemos r.

#### Con repetición
De cada tipo tengo varios objetos y existe la posibilidad de repetir en la combinación resultante.

$$CR(n, r) = \binom{n+r+1}{n-1}$$

### Particiones
$$S(r, n)$$

Se divide un conjunto en lotes, r > n o tendremos querevisar junto al teorema del palomar.

## Importa el orden
### Todas las aplicaciones de A en B
$$n^r$$

Tienes (suficientes) para todo de cada tipo o cada uno se puede llevar más de uno

### Aplicaciones inyectivas de A en B
No podemos repetir elementos y el orden en que disponemos los
elementos determina permutaciones distintas

$$P(n, r) = \frac{n!}{(n - r)!}$$

De n posibilidades tenemos disponibles (n-r)

### Permutaciones
Las aplicaciones inyectivas en el mismo conjunto se llaman permutaciones y consisten en la
alteración de la posición u orden de los elementos

$$P(n, n) = n!$$

#### Generalizadas
Permutaciones con objetos de cada tipo son indistinguibles

$$P(x; y_1, y_2 ... y_k) = \frac{x!}{y_1! \cdot ... \cdot y_k!}$$

Permutaciones con limitaciones en cajas o posibilidades, y puede repetirse. Objetos indistinguibles.

### Aplicaciones sobreyectivas de A en B
A todo elemento de B le corresponde uno de A

$$n! \cdot S(r, n)$$

A objetos distintos se le asignan recipientes distinguibles, los cuales tendrán asignados como mínimo un objeto.
