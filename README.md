# ESTADÍSTICA-BAYESIANA-CON-PYTHON
Información con conceptos de estadística bayesiana
## DISTRIBUCIÓN CONJUNTA MARGINAL Y CONDICIONAL
Tenemos dos variables aleatorias A y B, entonces:

**Distribuciones Marginales:** p(A),p(B).  En la distribución marginal se obtiene alguna cuenta o un porcentaje tomando en cuenta un solo rango. Por ejemplo, en la imagen podemos observar que el porcentaje de alumnos que obtuvo entre 80 y 100% de aciertos fue solo el 20% de alumnos o 40 alumnos del TOTAL (que son 200).

![Imagen](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/Dis%20Marginal.PNG?raw=true)

**Distribución Conjunta:** p(A,B). Se puede leer como p de A **y** B. A partir de la distribución conjunta se pueden calcular las distribuciones Marginales y Condicionales.

**Distribución Condicional:** p(A|B),p(B|A). Se puede leer como **P de A**, dado **B**; y **P de B**, dado **A**. Por ejemplo, en la imagen podemos observar que una de las CONDICIONES es el tiempo, es decir, aquellos alumnos que estudiaron de 41-60 minutos, y usando esa condición podemos calcular el porcentaje de alumnos que sacaron cierta calificacion estudiando exclusivamente en este tiempo estimado.

![Imagen2](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/Dis%20Condicional.PNG?raw=true)

En la siguiente imagen se muestra un diagrama de Venn, en el que el rectángulo grande representa el espacio muestral y tenemos 4 subconjuntos de ese espacio muestral, los cuales representan eventos de interés. El área que abarca cada evento representa su probabilidad, por ejemplo, la probabilidad del evento A1 es más grande que la probabilidad del evento A3

![Imagen 3](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/diagrama%20venn.PNG?raw=true)

Posteriormente, si nos llega información de que el evento B ha ocurrido, entonces la incertidumbre se reduce a B, entonces B sería el nuevo espacio muestral. Por lo tanto, las probabilidades A1, A2 y A3 cambian de acuerdo a la nueva información. Como se muestra en la imagen la probabilidades de A3 dado que ya ocurrió B sería cero. En cambio, la probabilidad del evento A2 dado que B ocurrió, es mayor a la probabilidad del evento A1 dado que B ocurrió. Aquí como ya ocurrió el evento B no importa que el área de A1 sea mayor que el área A2, ya que A2 abarca mucho más área (más probabilidad) que A1 de acuerdo al evento B

![imagen 4](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/diagrama%20de%20venn%202.PNG?raw=true)

A continuación, se muestran algunas fórmulas para calcular la probabilidad condicional
![Imagen 5](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/formula.PNG?raw=true)

Y se lee como: la probabilidad de A dado B es igual a la probabilidad de la intersección de A con B, dividido entre la probabilidad de B. En cambio si queremos calcular la probabilidad de B dado A, lo único que cambia en la operación es el denominador, el cual es la probabilida de A. De la ecuación observamos que la probabilidad de A dado B es DIFERENTE a la probabilidad de B dado A.

![Imagen 6](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/formula%202.PNG?raw=true)
![Imagen 7](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/formula%203.PNG?raw=true)

La siguiente expresión es una primer forma de la REGLA DE BAYES

![Imagen 8](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/regla%20de%20bayes.PNG?raw=true)
![Imagen 9](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/GENERAL.PNG?raw=true)

![Imagen 10](https://github.com/Parkins555/OPTIMIZACION-BAYESIANA/blob/main/regla%20de%20bayes%202.PNG?raw=true)

EJEMPLO: Veamos el ejemplo de un "sidómetro", un aparato que al soplar determina si la persona tiene el virus de inmunodeficiencia humana. Donde: 

A= El aparato diagnostiva VIH
B= La persona efcetivamente tiene VIH

Se nos presenta además la siguiente informaciön:
P(A|B)=0.99=P(A <sup> c </sup> | B <sup> c </sup>)
