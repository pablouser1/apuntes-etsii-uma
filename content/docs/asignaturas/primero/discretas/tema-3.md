---
weight: 3
---

# Grafos
Un grafo se define como: {{< katex >}}G = \{V, E\}{{</ katex >}}
$$V = \text{Vértices}$$
$$E = \text{Aristas}$$

## Grado
Se denota como {{< katex >}}\delta{{</ katex >}} y representa el número de aristas enlazadas a un vértice.

Si el grado es 0 decimos que es aislado, si es 1 decimos que es una hoja.

## Teorema de Euler
La suma de los grados de todos los vértices de un grafo simple es un número par

## Camino
* **Simple**, si cada arista se recorre una sola vez
* **Elemental**, si por cada vértice se pasa a lo sumo una vez
* **Cerrado**, si empieza y termina en el mismo vértice
* **Circuito**, si es un camino cerrado que no repite aristas
* **Ciclo**, si es un camino cerrado en el que todos los vértices son distintos
* **Conexo**, si cada par de vértices se puede conectar por un camino

## Grafos Eulerianos
### Camino de Euler
Camino simple que recorre todas las aristas

**Comprobación**: Un grafo simple tiene un camino de Euler entre los vértices u, v si y solo si es conexo y esos vértices son los únicos con grado impar.
### Circuito de Euler
Camino cerrado que recorre cada arista del grafo exactamente una vez

**Comprobación**: Un grafo simple tiene un circuito de Euler si y solo si es conexo y todos los vértices son de grado par

### Calcular
{{< youtube OwjcOPSWsyY >}}

## Grafos Hamiltonianos
### Camino de Hamilton
Es un camino elemental que recorre todos los vértices
### Ciclo de Hamilton
Un camino cerrado que recorre todas los vértices del grafo exactamente una vez

### Teorema Dirac
Si tiene un nº de vértices {{< katex >}}n \geq 3{{</ katex >}} y todos ellos tienen grado mayor o igual a
{{< katex >}}\dfrac{n}{2}{{</ katex >}}, entonces el grafo contiene un ciclo hamiltoniano

### Teorema Ore
Si {{< katex >}}n \geq 3{{</ katex >}} es el número de vértices de un grafo simple y para cada par de vértices NO adyacentes
u, v, se verifica que {{< katex >}}\delta(u)+\delta(v) \geq n{{</ katex >}}, entonces el grafo contiene un ciclo hamiltoniano.

## Planaridad
Un grafo es plano si puede dibujarse en el plano sin que se corten ningún par de aristas

Una representación plana de un grafo divide al plano en regiones, las partes del plano que quedan delimitadas por las aristas y los vértices, en donde la parte externa, no acotada, también se considera región

### Fórmula de Euler
$$v − e + r = 2$$

v = nº Vértices

e = nº Aristas

r = nº Regiones

### Homeomorfo
Decimos que el grafo G1 es homeomorfo a G2 si uno de ellos se puede obtener a partir de el otro insertando vértices en alguna de sus aristas.

### Teorema de Kuratowski
Un grafo es no plano si, y sólo si, contiene un subgrafo que es homeomorfo al grafo K5 ó al grafo K3,3.

## Grafos ponderados
La longitud de un camino en un grafo ponderado es la suma de los pesos de las aristas

### Algoritmo de Prim
Un árbol generador minimal de un grafo conexo ponderado es un árbol generador tal que la suma de los pesos de sus aristas es mínima, respecto de todos los árboles generadores.

{{< youtube KW5gvhOPdcA >}}

* Empezamos elegiendo un vértice cualquiera
* Miramos todas las aristas unidas al vértice y elegimos la que tenga menos peso
* Repetimos este proceso agregando el vértice al que une el paso anterior hasta quedarnos sin opciones
* Evitamos hacer un ciclo!!

### Algoritmo de Dijkstra
Sirve para encontrar el camino de longitud mínima entre dos vértices de un grafo ponderado
{{< youtube ZF0LbqZwoU4 >}}
