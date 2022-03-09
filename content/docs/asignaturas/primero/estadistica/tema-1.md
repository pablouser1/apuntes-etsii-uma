---
weight: 1
---

# Tema 1 (Estadística Descriptiva)
{{< tabs "videos" >}}
{{< tab "Video 3.1" >}}
{{< youtube CuTQu3iDjVE >}}
{{< /tab >}}
{{< tab "Video 3.2" >}}
{{< youtube iyrvsqlrvWE >}}
{{< /tab >}}
{{< /tabs >}}

## Ordenar datos
- Menor a mayor
- Agrupados o no ({{< katex >}}\sqrt{n}{{</ katex >}} = nº de intervalos)
- Tabla de frecuencia de
    - Datos agrupados
    - Datos no agrupados
- Tipo de variable
    - Cualitativa
        - Nominales
            - País={Francia, España,...}
            - Color={Rojo, Verde, Amarillo...}
        - Ordinal (Común en escalas jerárcicas)
            - {Todo, Mucho, Regular, Poco, Nada}
            - {Muy alto, Alto, Regular, Bajo, Muy Bajo}
    - Cuantitativa
        - Discreta
            - Número de hijos={0, 1, 2...}
            - Número de símbolos en un mensaje={2, 3, 4...}
        - Continua:
            - Altura en cm
            - Peso en kg
            - Ruido en decibelios

## Tratamiento de datos
- Agrupar de mayor a menor
- Agrupados en términos
    - {{< katex >}}(l_{i} - 1, l_{i}]{{</ katex >}}
    - {{< katex >}}(-\infty, l_{i}){{</ katex >}}
    - {{< katex >}}(l_{i}-1, \infty){{</ katex >}}
- Marca de clase y amplitud
    - {{< katex >}}(160, 170]{{</ katex >}} = Despejar usando lo anterior

## Tabla de frencuencias
| x | Freq. Absoluta<br>$$n_{i}$$ | Frecuencia relativa<br>$$f_{i}=\frac{n_{i}}{n}$$ | Frecuencia absoluta acomulada<br>$$N_{i}$$ | Frecuencia relativa acomulada<br>$$F_{i}=\frac{N_{i}}{n}$$ |
| :---: | :---: | :---: | :---: | :---: |
| Falda | 2 | {{< katex >}}\frac{2}{10}{{</ katex >}} | 2 | {{< katex>}}\frac{2}{10}{{</ katex >}} |
| Chaqueta | 3 | {{< katex >}}\frac{3}{10}{{</ katex >}} | 2 + 3 | {{< katex>}}\frac{2}{10} + \frac{3}{10}{{</ katex >}} |
| Periódico | 3 | {{< katex >}}\frac{3}{10}{{</ katex >}} | 2 + 3 + 3 | {{< katex>}}\frac{2}{10} + \frac{3}{10} + \frac{3}{10}{{</ katex >}} |
| Maletín | 2 | {{< katex >}}\frac{2}{10}{{</ katex >}} | 2 + 3 + 3 + 2 = **10** | {{< katex>}}\frac{2}{10} + \frac{3}{10} + \frac{3}{10} + \frac{2}{10} = {{</ katex >}} **1** |
| {{< katex >}}\sum{{</ katex >}} | n = **10** | **1** | - | - |

### Ejemplo transparencias
| x | Freq. Absoluta<br>$$n_{i}$$ | Frecuencia relativa<br>$$f_{i}=\frac{n_{i}}{n}$$ | Frecuencia absoluta acomulada<br>$$N_{i}$$ | Frecuencia relativa acomulada<br>$$F_{i}=\frac{N_{i}}{n}$$ |
| :---: | :---: | :---: | :---: | :---: |
| 0 | 2 | {{< katex >}}\frac{2}{25}{{</ katex >}} | 2 | {{< katex >}}\frac{2}{25}{{</ katex >}} |
| 1 | 6 | {{< katex >}}\frac{10}{25}{{</ katex >}} | 8 | {{< katex >}}\frac{8}{25}{{</ katex >}} |
| 2 | 14 | {{< katex >}}\frac{14}{25}{{</ katex >}} | 22 | {{< katex >}}\frac{22}{25}{{</ katex >}} |
| 3 | 2 | {{< katex >}}\frac{2}{25}{{</ katex >}} | 24 | {{< katex >}}\frac{24}{25}{{</ katex >}} |
| 4 | 1 | {{< katex >}}\frac{1}{25}{{</ katex >}} | **25** | **1** |
| {{< katex >}}\sum{{</ katex >}} | **25** | **1** | - | - |

## Diagramas
Eje x: Variable
Eje y: Frecuencia absoluta/relativa

- Dispersión y barra
    - Cuantitativa y discreta
- Histograma
    - Igual que la de barra pero con las barras juntas
    - Cuantitativa y continua
- Sector (pie chart)
    - Cualitativa/Atributo

### Densidad
- Absoluta: {{< katex >}}d_{n_{i}}=\frac{n_{i}}{a_{i}}{{</ katex >}}
- Relativa: {{< katex >}}d_{f_{i}}=\frac{f_{i}}{a_{i}}{{</ katex >}}

## Medidas de posición
En torno a qué valores se agrupan los datos

### Tendencia central
Datos agrupados o no agrupados

#### Media ({{< katex >}}\bar{x}{{</ katex >}})
{{< katex display>}}
\frac{\sum \bar{x}_{i} \cdot n_{i}}{n} = \sum x_{i} \cdot f_{i}
{{</ katex >}}

| Población | Muestra |
| :---: | :---: |
| N | n |
| {{< katex >}}\mu{{</ katex >}} | {{< katex >}}\bar{x}, \bar{y}{{</ katex >}} (media) |

#### Mediana (Me) (0.5 Ni)
{{< katex display >}}
M_{e}=(l_{i}-1)+\frac{\frac{n}{2}-N_{i}-1}{N_{i}{N_{i} - 1}} \cdot (l_{i}-l_{i}-1)=
(l_{i}-1)+\frac{\frac{n}{2}-N_{i}-1}{n_{i}}\cdot a_{i}
{{</ katex >}}

{{< katex >}}\frac{n+1}{2} = 26 / 2 = 13{{</ katex >}} (posición 13)

{{< katex >}}\frac{n+1}{2} = 51 / 2 = 25.5{{</ katex >}} (posición 25 y 26)

Me voy a Ni el que se acerque más por _exceso_

#### Moda (Mo) (Max ni)

### Tendencia no central
- Cuantíles
    - Cuartiles (C Q) 4 partes
		- C1: 25%
		- C2: 50% (Mediana)
		- C3: 75%
		- C4: 100%
    - Deciles (D) 10 partes
		- D1: 10%
		- D2: 20%
		...
    - Percentiles (P) 100 partes
        - P1: 1%
        - P2: 2%
        ...

### Ejemplos
{{< tabs "medidas-posicion-ejemplos" >}}
{{< tab "Ejercicio 1" >}}
{{< columns >}}

| $$X_{i}$$ | $$n_{i}$$ | $$N_{i}$$ |
| :---: | :---: | :---: |
| 4 | 20 | 20 |
| 7 | 120 | 140 |
| 8 | 60 | 200 |
| $$\sum$$ | 200 | - |

<--->

$$\bar x: \frac{x_{i} \cdot n_{i}}{\sum} = 7$$
$$M_{e}: \frac{n+1}{2} = 7$$
$$M_{o} (n_{i}): 7$$
$$C_{1}: x_{50} (x_{200 \cdot 0.75}) = 7$$
$$C_{2}: x_{100} = 7$$
$$D_{1}: x_{200 \cdot 0.1} = 4$$
$$P_{20}: x_{200 * 0.2} = 7$$

{{< /columns >}}
{{< /tab >}}
{{< tab "Ejercicio 2" >}}
{{< columns >}}
| Inter | $$x_{i}$$ | $$n_{i}$$ | $$N_{i}$$ |
| :---: | :---: | :---: | :---: |
| (150, 160] | 155 | 2 | 2 |
| (160, 170] | 165 | 8 | 10 |
| (170, 180] | 175 | 11 | 21 |
| (180, 190] | 185 | 7 | 28 |
| (190, 200] | 195 | 2 | **30** |
| $$\sum$$ | - | n = **30** | - |

<--->

$$\frac{n}{4} = 7.5 \text{(posición 7 y 8)}$$
$$C_{i} = 166.875$$
$$M_{e} = (l_{i}-1)+\frac{\frac{n}{2}-N_{i}-1}{n_{i}}\cdot a_{i}$$
$$l_{i} = 160, a_{i} = 10 \text{(diferencia intervalo)}$$

{{< /columns >}}
{{< /tab >}}
{{< /tabs >}}

## Medidas de dispersión

### Recorrido
{{< katex display >}}
R_{e} = X_{n} \text{Max} - X_{n} \text{Min}
{{</ katex >}}

{**120**, 130, 140, 165, **200**}

{{< katex >}}R_{e}: 200 - 120 = 80{{</ katex >}}

### Rango intercuartílico
{{< katex display >}}
R_{Q} = Q_{3} - Q_{1}
{{</ katex >}}

### Rango intercentílico
{{< katex display >}}
R_{P} = R_{99} - R_{1}
{{</ katex >}}

### Desviación
Desviación a la media respecto de un parámetro DM(P)

Suelen ser medidas de tendencia central

{{< katex display >}}
\sum \frac{|x_{i} - p| \cdot n_{i}}{n} = \sum |x_{i} - p| \cdot f_{i}
{{</ katex >}}

#### Media DM
{{< katex display >}}
\sum \frac{|x_{i} - \bar x| \cdot n_{i}}{n} = \sum |x_{i} - \bar x| \cdot f_{i}
{{</ katex >}}

### Error cuadrático
Igual que [Desviación]({{< relref "#desviación" >}} "Desviación") pero elevando al cuadrado {{< katex >}}x_{i} - p{{</ katex >}}

#### ECM
Igual que [MediaDM]({{< relref "#media-dm" >}} "Media DM") pero elevando al cuadrado {{< katex >}}x_{i} - \bar x{{</ katex >}}

### Varianza / Desviación
{{< katex >}}S^2 o VAR(x){{</ katex >}}
$$VAR(x), S^2 = \sum \frac{(x_{i}-\bar x)^2 \cdot n_{i}}{n}$$
$$\sum(x_{i}-\bar x)^2 \cdot f_{i}$$
$$\sum \frac{x_{i}^2 \cdot n_{i}}{n} - x^{-2} \text{(Top pick)}$$
$$\sum x_{i}^2 \cdot f_{i} - x^{-2} \text{(Top pick)}$$

| Población | Muestra |
| :---: | :---: |
| N   | n   |
| $$\mu$$ | $$\bar{x}, \bar{y}, \bar{t}$$ (media) |
| O^2 | S^2 (TEMA 6) |
| $$\sigma$$ | S |

{{< hint warning >}}
Si la varianza y la dispersión son altos {{< katex >}}\bar x{{</ katex >}} no es suficientemente representativa

Si son bajas {{< katex >}}\bar x{{</ katex >}} si es representativa
{{< /hint >}}

### Coeficiente
{{< katex display >}}
CV = \frac{S}{|\bar X|} \cdot 100
{{</ katex >}}

#### Momento ordinario de orden r respecto de 1 punto C

$$M_{r}(c) = \frac{\sum(x_{i}-c)^r \cdot r_{i}}{n} = \sum (x_{i}-c)^r \cdot f_{i}$$

#### Momento ordinario de orden r respecto al origen
$$M_{i} = \frac{\sum x^r \cdot n_{i}}{n} = \sum x^r \cdot f_{i}$$
$$M_{1} = 1$$
$$M_{2}=\bar x$$

#### Momento central de orden r
$$u_{r}=\frac{\sum(x_{i} - \bar x)^r \cdot n_{i}}{n} = \sum(x - \bar x)^r \cdot f_{i}$$

$$u_{0} = 1$$
$$u_{1} = 0$$
$$u_{2} = \frac{(x_{i} - \bar x)^2 \cdot n_{i}}{n}$$

##### Ejemplo
{0, 0, 2, 2, 2, 2, 3, 3, 4, 4, 7, 7}

- Halla el momento ordinario de orden 1 respecto de la Mediana
- Halla el momento ordinario de orden 2 respecto de la mediana

| $$X_{i}$$ | $$n_{i}$$ | $$N_{i}$$ | $$X_{i} - M_{e}$$ |
| :---: | :---: | :---: | :---: |
| 0 | 2 | 2 | -2.5 |
| 2 | 4 | 6 | -0.5 |
| 3 | 2 | 8 | 0.5 |
| 4 | 2 | 10 | 1.5 |
| 7 | 2 | 12 | 4.5 |
| $$\sum$$ | 12 | - | - |

## Diagramas. Medidas de forma
Determinar la forma de cómo se distribuye la variable

### Pirson
$$A_{p} = \frac{\bar x - M_{o}}{S}; A_{p} = \frac{3(\bar x - M_{e})}{S}$$

### Fisher
$$g_{1} = \frac{\sum (x_{i} - \bar x)^3 \cdot f_{i}}{S^3}$$

### Coeficiente de aplastamiento...
$$g_{2} = \frac{\sum(x_{i} - \bar x)^4 \cdot f_{i}}{S^4} - 3$$

### Interpretaciones (Simetría)
{{< katex >}}A_{p} > 0{{</ katex >}} o {{< katex >}}g_{1} > 0{{</ katex >}}
La distribución es asimétrica hacia la derecha (tiene una mayor concentración a la derecha)

{{< katex >}}A_{p} = 0{{</ katex >}} o {{< katex >}}g_{1} = 0{{</ katex >}}
La distribución es perfectamente simétrica (Media, Mediana y Moda coinciden)

{{< katex >}}A_{p} < 0{{</ katex >}} o {{< katex >}}g_{1} < 0{{</ katex >}}
La distribución es asimétrica hacia la izquierda (tiene una mayor concentración a la izquierda)

#### Curtosis
Mesocúrtica: {{< katex >}}g_{2} = 0{{</ katex >}}

Platicúrtica: {{< katex >}}g_{2} < 0{{</ katex >}}

Leptocúrtica: {{< katex >}}g_{2} > 0{{</ katex >}}
