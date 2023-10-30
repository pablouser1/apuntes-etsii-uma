---
weight: 1
---

# Tema 1
## Coste temporal
{{< youtube 9TlHvipP5yA >}}

## Teorema Maestro
$$t(n) = a \cdot t(\frac{n}{b}) + f(n)$$

* **n** es el tamaño original del problema
* **a** es el número de llamadas recursivas (a ≥ 1).
* **n/b** es el tamaño de cada subproblema (b > 1).
* **f(n)** es el coste del trabajo restante.

{{< katex >}}
T(n) =
\begin{cases}
\theta(n^{\log_b{a}}) & \text{if} & a > b^c \\
\theta(n^{c} \cdot \log{n}) & \text{if} & a = b^c \\
\theta(n^{c}) & \text{if} & a < b^c \\
\end{cases}
{{</ katex >}}
<br />
{{< youtube T68vN1FNY4o >}}

## Ecuaciones de recurrencia
{{< button href="/files/asignaturas/segundo/ada/erl.pdf" >}}Guía{{< /button >}}
