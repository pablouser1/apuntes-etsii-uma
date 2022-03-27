---
weight: 2
---

# Tema 2 (Modelización estadística. Regresión y correlación)
## Recursos
https://aprendeconalf.es/docencia/estadistica/manual/regresion/

{{< tabs "videos" >}}
{{< tab "Video 3.3" >}}
{{< youtube Ne59233X_dc >}}
{{< /tab >}}
{{< tab "Video 3.4" >}}
- A partir de relación entre atributos no os entra, de página 14 en adelante
{{< youtube PVRIOQX3-ME >}}
{{< /tab >}}
{{< /tabs >}}

Pasamos de tratar una sola variable a tratar dos (bidimensional)

- Peso (variable dependiente) {{< katex >}}y{{</ katex >}}
	- Deporte ({{< katex >}}x_{1}{{</ katex >}}) (variables independientes)
	- Alimentación ({{< katex >}}x_{2}{{</ katex >}}) ''
	- Edad ({{< katex >}}x_{3}{{</ katex >}}) ''
	...

Tabla contenidos:
- Correlación
- Rectas de regresión (Modelo predictivo)

Los gráficos que nos interesa son los _diagramas de dispersión_

Condicion variables:
- Hay relación (dependientes)
- Independientes (tabla frecuencias bidimensional en términos relativos)
- Un poco de relación

## Correlación
### Tabla absoluta
Tabla de frecuencias absolutas (variable bidimensional)
| x/y | 0 | 1 | $$n_{x} (n_{i}.)$$ |
| :---: | :---: | :---: | :---: |
| 0 | 2 | 4 | 2 + 4 = 6 |
| 1 | 4 | 8 | 4 + 8 = 12 |
| 2 | 2 | 0 | 2 + 0 = 2 |
| $$n_{y} (n_{.j})$$ | 2 + 4 + 2 = 8 | 4 + 8 + 0 = 12 | 6 + 12 + 2 = 20 |

{{< katex >}}n_{ij}{{</ katex >}} (i = filas, j = columnas)

{{< katex >}}n_{21} = 4{{</ katex >}}

### Tabla relativa
Tabla de frecuencias relativas (var bidimensional)
| x/y | 0 | 1 | $$f_{x} (f_{i}.)$$ |
| :---: | :---: | :---: | :---: |
| 0 | $$\frac{2}{20}$$ | $$\frac{4}{20}$$ | $$\frac{6}{20}$$ |
| 1 | $$\frac{4}{20}$$ | $$\frac{8}{20}$$ | $$\frac{12}{20}$$ |
| 2 | $$\frac{2}{20}$$ | 0 | $$\frac{2}{20}$$ |
| $$f_{y} (f_{.j})$$ | $$\frac{8}{20}$$ | $$\frac{12}{20}$$ | 1 |

Vamos a ver si {{< katex >}}x{{</ katex >}} e {{< katex >}}y{{</ katex >}} son independientes
(arriba derecha * abajo derecha = arriba izquierda)
$$\frac{6}{20} \cdot \frac{8}{20} \neq \frac{2}{20}$$
No se cumple la igualdad, las variables son dependientes

| x/y | $$y_{1}$$ | $$y_{2}$$ | $$y_{3}$$ | $$y_{4}$$ | $$f_{x} (f_{i.})$$ |
| :---: | :---: | :---: | :---: | :---: | :---: |
| $$x_{1}$$ | $$\frac{1}{60}$$ | $$\frac{3}{60}$$ | $$\frac{2}{60}$$ | $$\frac{4}{60}$$ | $$\frac{10}{60}$$ |
| $$x_{2}$$ | $$\frac{3}{60}$$ | $$\frac{9}{60}$$ | $$\frac{6}{60}$$ | $$\frac{12}{60}$$ | $$\frac{30}{60}$$ |
| $$x_{3}$$ | $$\frac{2}{60}$$ | $$\frac{6}{60}$$ | $$\frac{4}{60}$$ | $$\frac{8}{60}$$ | $$\frac{20}{60}$$ |
| $$f_{y} (f_{.j})$$ | $$\frac{6}{60}$$ | $$\frac{18}{60}$$ | $$\frac{12}{60}$$ | $$\frac{24}{60}$$ | 1 |

{{< katex >}}\frac{20}{60} \cdot \frac{24}{60} = \frac{P}{60} {{</ katex >}} (Las variables son independientes)
{{< katex >}}f_{3.} \cdot f_{.4} = f_{3,4}{{</ katex >}}

### Covarianza
$$s_{xy}=\frac{\sum x_iy_j}{n}-\bar{x}\bar{y}$$

## Regresión
### Ajuste de mínimos cuadrados
$$\sum (y_j - a - bx_i)^2$$
### Lineal
#### Recta de regresión
##### y/x
$$y=\bar{y}+\frac{s_{xy}}{s_x^2}(x-\bar{x})$$
##### x/y
$$x=\bar{x}+\frac{s_{xy}}{s_y^2}(y-\bar{y})$$

#### Coeficiente de determinación lineal
$$r^2=\frac{s_{xy}^2}{s_x^2s_y^2}$$

#### Coeficiente de correlación lineal
$$r=\frac{s_{xy}}{s_xs_y}$$

### No lineal
{{< youtube Jx8R4fTFjoE >}}
