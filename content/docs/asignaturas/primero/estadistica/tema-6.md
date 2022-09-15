---
weight: 6
---

# Tema 6 (Inferencia Estadística)
## Recursos
{{< tabs "videos" >}}
{{< tab "Video 3.12" >}}
{{< youtube MDSsanlk5YE >}}
{{< /tab >}}
{{< tab "Video 3.13" >}}
{{< youtube QihrZkortOw >}}
{{< /tab >}}
{{< /tabs >}}

## Introducción
### Ventajas e inconvenientes del muestro
Ventajas:
- Menor conste
- Más rapidez
- Mayor facilidad

Desventajas:
- Necesidad de tener una muestra representativa
- Posibilidad de cometer errores (sesgos)

### Variable aleatoria muestral
Una variable aleatoria muestral de una población X es una colección de n variables aleatorias tales que:
- Cada variable Xi sigue la misma distribución de probabilidad que la X de partida
- Todas las variables son mutuamente independientes

### Estimación de parametros
Las tres cuestiones fundamentales respecto a la VAM son:
- Homogeneidad: Las n variables que componen la variable aleatoria muestral siguen la misma distribución
- Independencia: Las variables son independientes entre sí
- Modelo de distribución: El modelo de distribución que siguen las n variables

Una vez elegido el modelo de distribución adecuado para nuestro conjunto de datos tenemos que averiguar que estadístico del modelo nos interesa y
cómo sacar su valor

## Distribución variable aleatoria muestral
Depende de la distribución de probabilidad de los valores de la población

Ejemplo: Sea una población en la que la cuarta parte de la familia no tiene hijos, la mitad de la familia tiene 1 hijo y el resto tiene 2 hijos:

Distribución poblacional:
| X | P(x) |
| :---: | :---: |
| 0 | 0.25 |
| 1 | 0.5 |
| 2 | 0.25 |

Si elegimos muestras de tamaño 2 nos quedaría una distribución muestral:
| (X1, X2) | P(x1, x2) |
| :---: | :---: |
| (0, 0) | 0.0625 (X0 * X0) |
| (0, 1) | 0.125 (X0 * X1) |
| (0, 2) | 0.0625 |
| (1, 0) | 0.125 |
| (1, 1) | 0.25 |
| (1, 2) | 0.125 |
| (2, 0) | 0.0625 |
| (2, 1) | 0.125 |
| (2, 2) | 0.0625 |

### Teorema central del límite
Este teorema se utiliza para aproximar la distribución de algunos estadísticos de muestras grandes

...
TODO
