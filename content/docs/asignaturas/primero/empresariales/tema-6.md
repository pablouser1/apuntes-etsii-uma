---
weight: 6
---

# Tema 6 (El subsistema de inversiones)
## Valor del dinero en tiempo
Misma cantidad de dinero, tiene diferente valor a lo largo del tiempo.

{{< columns >}}
## Futuro
{{< katex display >}}
V_{Fn} = K_o \cdot (1 + r)^n
{{< /katex >}}

n = años

Ko = inversión inicial

r = tasa de interés

<--->

## Actual
{{< katex display >}}
V_A = \frac{K_n}{(1+r)^n}
{{< /katex >}}

{{< /columns >}}

## Inversiones, rentabilidad y riesgo
La inversión se puede definir por flujos de cobros y pagos que origina. Se evalúa analizando estos
parámetros: Desembolso inicial o tamaño de inversión, Pagos o salidas de dinero, cobros o entradas
de dinero y horizonte temporal o vida útil.

Parámetros a tener en cuenta al invertir:
- Rentabilidad: Relación entre la cantidad de flujos de caja que recibirá el inversor en un tiempo y la
cantidad de inversión al momento inicial.
- Riesgo: Incertidumbre del proyecto y probabilidad de que se produzcan los flujos de caja.
A más riesgo, más rentabilidad mínima deseada.

## Análisis y selección de inversiones
Limitaciones técnicas y Restricciones financieras => Analizar y seleccionar los proyectos más
rentables.
- Métodos Estáticos: Pay Back o plazo de recuperación (PB) y Rendimiento de inversión (RI).
- Métodos Dinámicos: Valor Actual Neto (VAN), Pay Back descontado (PBD) y Tasa Interna de
Rentabilidad (TIR)

### Pay back
Es el periodo de tiempo que pasa desde inversión inicial hasta que los cash flow(CF), permiten
recuperar el coste de inversión

Es el tiempo {{< katex >}}t_{PB}{{< /katex >}} tal que:
- D0: Montante
- CFN: Cash flow (después de impuestos)

{{< katex display >}}
D_0 = \sum_{n=1}^{t}CFN_t
{{< /katex >}}

+: Simple y rápido /-:No considera el CF tras recuperarse e Ignora valor del dinero en el tiempo

### Rendimiento de la inversión
Es la media de los cocientes entre los CFN de los periodos y el desembolso inicial (en forma de
porcentaje).

{{< katex display >}}
RI = \sum_{1}^n \frac{\frac{CFN_t}{D_0} \cdot 100}{n}
{{< /katex >}}

+: Simple y rápido /-:Es poco preciso en CF variables en el tiempo

### Actualizar vs Capitalizar
Actualizar es calcular el valor que tendrían hoy cantidad que tendremos en el futuro y Capitalizar es
calcular el valor que tendrán en fecha futura cantidades recibidas de forma previa

### Valor actual neto (VAN)
Es la diferencia entre flujos actualizados de cobros y los flujos actualizados de pagos de una
inversión a determinada tasa de descuento

{{< katex display >}}
VAN = -D_0 + \sum_{i=0}^{n} \frac{CFN_i}{(1 + r)^i} + \frac{V_t}{(1 + r)^n}
{{< /katex >}}

Vt: Valor residual

Criterio de aceptación de esta: VAN >0

Criterio de elección entre diferentes proyectos: VAN + alto

### Pay back descontado (PBD)
Usa los flujos de caja descontados para calcular el tiempo necesario de recuperación de inversión
inicial (tPDB)

{{< katex display >}}
D_0 = \sum_{t=1}^{t_{PBD}} \frac{CFN_t}{(1 + r)^t}
{{< /katex >}}

### Tasa interna de rentabilidad (TIR)
Tasa que hace que el valor actual de la inversión sea cero:

{{< katex display >}}
-D_0 + \sum_{i=0}^{n} \frac{CFN_i}{(1 + TIR)^i} + \frac{V_t}{(1 + TIR)^n} = 0
{{< /katex >}}
