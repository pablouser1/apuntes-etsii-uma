---
weight: 3
---

# Tema 3 (Subsistema de producción)

## Concepto y objetivos del sistema de producción
### Producción
Todo proceso que genere valor o utilizadad.
Siendo utilidad la capacidad de satisfacer una necesidad

Este proceso implica transformación de bienes y servicios en otros con mayor valor. La
producción se expresa en función de la utilización que se hace de los recursos productivos (trabajo y capital)
### Objetivos
- Costes y producción
    - Minimizar los costes
    - Maximizar la producción
- Calidad
- Fiabilidad
- Capacidad de adaptación

## Gestión de inventarios
### Inventarios
Conjunto de artículos acumulado su almacenados en espera de una posterior utilización

El principal objetivo de los inventarios es actuar como reguladores entre los ritmos de
salida de una fase y los de entrada.

Más concretamente, pueden señalarse los siguientes objetivos:
- Reducción del riesgo
    - Stock de seguridad de productos terminados —> demanda
    - Stock de materias primas —> proceso de producción
- Abaratar las adquisiciones y la producción: costes
- Anticipar las variaciones previstas de la oferta y la demanda
- Facilitar el transporte y la distribución del producto: se almacena para ser transportado en lotes

### Gestión
Para que el proceso de producción no sufra ningún retraso, será necesario que los
materiales precisos estén siempre disponibles para evitar roturas de stock (interrupción
en el proceso de producción de la empresa debido a la falta de materiales)

Los objetivos de una adecuada gestión de inventarios son:
- Mantener una seguridad máxima frente a posibles roturas de stock.
- Minimizar los costes de mantenimiento de los inventarios.

{{< hint danger >}}
Se debería almacenar la cantidad justa: ni tanto que se almacenen productos
que no se van a llegar a vender ni tan pocos que puede que la empresa se quede sin stock
{{< /hint >}}

Para realizar una correcta gestión de los inventarios que permita fijar los niveles de stock
óptimos es necesario identificar:
- Stock máximo: cantidad máxima almacanable.
- Stock mínimo o de seguridad: cantidad mínima que hay que mantener para evitar la
ruptura de stocks.
- Punto de pedido: nivel de existencias en el cual se ha de realizar el pedido para
reaprovisionar el almacén.

### Costes
- Costes de adquisición: Coste de adquirir artículos al proveedor o de fabricarlos.
- Coste de emisión o renovación: necesaria para realizar cada pedido o emitir orden de fabricación.
- Costes de posición almacenamiento: coste del almacenamiento físico en almacén.
- Coste de ruptura: coste de inactividad, pérdida de ventas, pérdida de imagen, etc.

## Tipos básicos de procesos de producción
| Destino del producto | Razón de producir | Tipificación | Dimensión temporal |
| :---: | :---: | :---: | :---: |
| Por encargo: pedido | Por órdenes: de frabricación | Individualizada: producto características específicas | Intermitente: con tramos discontínuos |
| Para el mercado: consumidores en general | Para almacén | En serie: todas unidades iguales | Continua: sin interrupción |

## Costes y tipos de costes
### Costes
- Costes: Expresión monetaria de los consumos de factores aplicados a la actividad productiva
- Gasto: Expresión monetaria de las adquisiciones de factores que realiza la empresa.
El coste recoge el precio pagado por los factores y todos los gastos organizados por su
adquisición, conservación y consumo.
### Tipos de costes
#### Según la producción
- Costes fijos (CV): Son independientes de la cantidad producida
- Costes variables (CV): Crecen proporcionalmente con el volumen de producción
- Costes totales (CT): la suma de los costes fijos (CF) y los costes variables (CV) da lugar al coste total de producción (CT)
##### Fórmulas
Q = Unidades producidas

| Coste Total Medio | Coste Variable Medio | Coste Fijo Medio | Coste Marginal |
| :---: | :---: | :---: | :---: |
| {{< katex >}}CTM_{e} = \frac{CF+CV}{Q}{{</ katex >}} | {{< katex >}}CVM_{e} = \frac{CV}{Q}{{</ katex >}} | {{< katex >}}CFM_{e} = \frac{CF}{Q}{{</ katex >}} | {{< katex >}}CM_{g} = \frac{\delta CV}{\delta Q}{{</ katex >}} |
#### Según la vinculación al producto
- Costes directos: Se pueden imputar a un producto terminado de forma clara
- Costes indirectos: Pueden imputtar de forma directa. Para ello se necesita de criterios de imputación

## Análisis del punto muerto
{{< hint info >}}
Punto Muerto (p.m.) o umbral de rentabilidad: nivel de ventas a partir del cual se
empiezan a obtener beneficios, o nivel de ventas con el que se cubren los gastos y el
beneficio de cero (ingreso total = a coste total)
{{< /hint >}}

{{< katex display >}}
Q* = \frac{CF}{p - CVM_e}
{{</ katex >}}

Donde {{< katex >}}(p - CVM_e){{</ katex >}} es conocido como el Margen de Cobertura.
Expresa la contribución de cada unidad producida y vendida al beneficio.

## Productividad
{{< hint info >}}
La productividad es el índice, relación o cociente entre la producción que se
obtiene y la cuantía de los recursos empleados en su consecución para un periodo
concreto
{{</ hint >}}
### Propiedad parcial o técnica
Relaciona la producción de un periodo dado con un único
factor, por lo general, los trabajadores (número de horas trabajadas o número de
trabajadores utilizado).

{{< katex display >}}
\text{Pdad del factor A} = \frac{\text{Producción obtenida}}{\text{Cantidad empleada del factor A}}
{{</ katex >}}
#### Ejemplos
- Propiedad de la superficie: producción obtenida/superficie ocupada.
- Propiedad de la maquinaria: producción obtenida/maquinarias utilizadas.
- Propiedad de materia primas: producción obtenida/materias primas empleadas.
- Propiedad operarios: producción obtenida/número de trabajadores empleados.
- Propiedad del servicio: número de cliente satisfecho/hora de servicio al cliente.
- Propiedad del corte: número de piezas cortadas/horas de trabajo empleada.
### Propiedad total o global
Relaciona la producción de un periodo dado con el
conjunto de factores que le han hecho posible y no con uno o un grupo de ellos.

{{< katex display >}}
\text{Pdad global (PG)} = \frac{\text{Valor de la producción botenida}}{\text{Valor de los factores empleados}}
{{</ katex >}}

{{< hint warning >}}
- La Pdad parcial o técnica se mide en unidades físicas
- La Pdad total o global se mide en unidades monetarias
{{</ hint >}}
### Errores en Interpretaciones
- La productividad no es solo la productividad del trabajo. Aunque tradicionalmente si
lo ha sido, hay que tener en cuenta en un contexto creciente de tecnología y
reducción de mano de obra hay que buscar otras medidas productivas.
- Confundir productividad con eficiencia.
### Índice de productividad global
{{< hint info >}}
Mide la relación entre productividades globales de dos pedidos diferentes
{{</ hint >}}

{{< katex display >}}
IPG = \frac{PG_1}{PG_0}
{{</ katex >}}
### Tasa de productividad global
{{< hint info >}}
Representa el crecimiento de la productividad
{{</ hint >}}

{{< katex display >}}
TPG = \frac{PG_1 - PG_0}{PG_0} = IPG - 1
{{</ katex >}}

### Mejora de productividad
#### A corto plazo
- Suponemos que los factores externos como precios de materias primas, etc.
Permanecen constantes.
- Solo se puede aprovechar mejor los recursos disponibles pero no podemos hacer
Las actuaciones posibles a corto plazo son:
1. Estudio y mejora de métodos de trabajo.
2. Estudio y reducción de los tiempos de trabajo.
3. Mejora de la organización interna.
4. Motivación de los trabajadores.
#### A largo plazo
Las posibles actuaciones a largo plazo van destinadas a modificar la estructura
productiva de la empresa, esto es, incrementar el inmovilizado mediante aumento de la
dimensión, tecnificación de las instalaciones, introducción de tecnologías más
avanzadas.
### Empeoramiento de productividad
Factores que disminuyen la productividad:
- Despilfarro de energía
- Sobreproducción
- Existencias
- Manipulaciones excesiva de los materiales
- Esperas
- Pérdida del tiempo
- Movimiento excesivo
- Piezas defectuosas
- Equipamiento defectuoso
- Desequilibrios en la carga de trabajo
- Utilización incongruente de los recursos
- Diseño deficiente
- Exceso de supervisión
- Falta de mantenimiento

## Dimensión y localización de las instalaciones
### Dimensión
La dimensión empresarial no se refiere al tamaño físico o al espacio ocupado por las
explotaciones, sino la capacidad de producción de la misma, entendida como la tasa
máxima de producción.
- Existen numerosos métodos de medición del tamaño de la empresa.
- Los criterios son relativos (depende del sector, sistema técnico, campo de actividad
característica de la propia realización), y en algunos casos, incluso son subjetivos
(Depende de la persona que toma la decisión).
- Una clasificación que se parece mucho es la siguiente:
    - Activo total.
    - Importe neto cifra negocio.
    - Número de empleados.

Las ventajas y los inconvemientes de la empresa según su tamaño son:
| Grandes | Pequeñas |
| :---: | :---: |
| Consecución de economías de escala | Dificultades para alcanzar economías de escala
| Mejor acceso a fuentes de financiación ajenas y mayor poder de negociación | Dificultades para acceder a la financiación ajena |
| Mayor poder de mercado | Menor cuota de mercado |
| Mayor burocracia y rigidez en su organización. Lentitud en toma de decisiones | Mayor flexibilidad en su organización. Favorece la rapidez en toma de decisiones e innovación |
| Mayores costes de coordinación y de control interno de sus objetivos y actividades | Menores costes de coordinación y control interno |
### Localización
- Es una decisión estratégica muy importante, por su enorme trascendencia para la
empresa. Consiste en la elección del lugar para la implantación o instalación de la
misma o parte de ella.
- Afecta muy directamente a los costes y a los ingresos y, por tanto puede tener un gran
impacto en el beneficio de la empresa.

Factores que influyen en la localización:
- Materias primas: Precio y lugar de adquisición
- Energía: Precio y facilidades de acceso
- Mano de obra: Especialización, dinamismo
- Mercado de consumo: Stock necesario, posventa
- Terreno: Precio, polígono industrial, comunicaciones
- Obtención de capital: Primera inversión
- Ventajas fiscales
- Ambiente social
- Suministro de componentes y existencia de servicios
- Eliminación de residuos: Infraestructura, vertederos industriales
- Dinamismo empresarial

Los principales factores a considerar derivados de la localización son los siguientes:
- La localización de su domicilio social y/o fiscal
- La localización de los servicios centrales: sede central
- La localización de sus fábricas, de sus instalaciones industriales o de producción,
influye los costes de transporte y mano de obra
- La localización de sus almacenes o centros de distribución
- La localización de sus puntos de venta (tiendas, establecimientos comerciales)

Una idea de negocio puede ser genial, pero una buena parte de su éxito o fracaso se
fundamentará en donde decidas ubicarla físicamente. La elección del lugar idóneo
dependerá de las características de la actividad empresarial en cuestión.

A este respecto, podemos distinguir entre cinco categorías de negocios:
- Negocios de proximidad: restaurantes, bancos o comercio minoristas
- Despachos profesionales: actividad profesional requiere visitas frecuentes, será
necesario un despacho o consulta
- Trabajo desde casa
- Centros de negocio: opinión muy interesante es la de alquilar un local en un centro
de negocios, edificios que ofrecen servicios comunes a las empresas que allí se
instalan como puede ser seguridad, aparcamiento o secretaría
- Empresas industriales: Las ubicaciones más típicas de este tipo de empresa suelen
ser dos: los polígonos y y lugares próximos a la materia prima
