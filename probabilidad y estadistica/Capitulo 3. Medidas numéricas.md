## Medidas de Posición
Nos ayuadan a indicar/buscar la posicion media, o como estan distribuidos los datos.

- Media -> Promedio de mediciones. ==NO SE REDONDEA==
	media muestral -> x =  $S(x)/n$
	media poblacional -> $S(x)/N$

	Media aritmetica: x = S(xi.fi)/n

- Media ponderada -> Calcula la media dando una importancia relativa.
	x = $s(w,x)/E(w)$
		w = peso
		
- Mediana -> Valor del medio con datos ascendentes, se usa cuando un conjunto de datos posee valores extremos

	x = $n/2$
	Si es impar redondeo hacia arriba,
	Sino, se saca un promedio entre los valores del medio.

- Mediana recortada ->se calcula eliminando una cierta cantidad de valores más pequeños y más grandes de un conjunto de datos ordenados, y luego encontrando la mediana del conjunto de datos recortado.

- Mediana Geometrica -> Cantidad arbitraria de  

x = $a$

- Moda -> Dato que mas se repite.

- Percentiles -> valor por debajo del cual cae un porcentaje específico de los datos en un conjunto ordenado

- Cuartiles -> ...

## Medidas de Variabilidad
	Nos dicen que tan dispersos estan los datos entre si.

- **Rango**
Conjunto de datos, que es la diferencia entre el mayor valor y el menor.
Es una de las medidas mas sencillas, pero es muy sencible, ya que solo esta basada en 2 valores extremos.

- **Rango intercuatilico**
	Agrega la consecuencia de tener intercuatiles. -> LA diferencia entre en 3er cuartil y el 1ero.
	Es decir, es el rango de la media de 50% de los datos.

- **Varianza**
Medida de variabilidad que utiliza toda las variables.
Diferencia entre el valor de cada observacion y la media.
Es util para comparar la variabilidad de 2 o mas variables.

muestra -> $s²= \sum{(xi-x)}²/(n-1)$  

- **Desviacion estandar** 
Raiz cuadrada positiva de la varianza.
Es mas facil de interpretar que la varianza ya que se mide en las mismas medias que los datos
muestra -> x = $\sqrt{x}$


- **Coeficiente de Variación**
Indica que tan grade es la desviación estandar con respecto a la media.
x = $((s/n) . 100)$ %

# Datos agrupados
Media de clase -> xi = $(Li - Ls) / 2$
Media -> x = $Sum(xi . frecuencia)/n$

- Mediana
	1.  Definir la posicion.
		- Si n es par -> Posición = $n/2$
		- Si n es impar -> Posición = $(n+1)/2$
	2. Consignar la media.
		- Si existe una frec. acumulada = posición -> El L sup de la clase =~ Media
		- Sino -> 
			- Se toma la posición mas cercana siguiente a FA = Pos.
			- Me = $Li + ((pos - F(i - 1))/fi) . (Ls-Li)$

- Moda
	- Se busca en mayor frecuencia.
	- Si hay varias frecuencias con el valor maximo -> Hay mas de 1 moda.

- Percentiles
Posicion percentil k = $(k.n)/100$

- Cuartiles
Posicion cuartil k = $(k.n)/25$

- Varianza
	Var(x) = $\sum{(xi² . fr)/n} - x²$

 - Desvio
 Desvio(x) = $\sqrt{Var(x)}$

## Medidas numericas
### Formas de distribucion
- Sesgo -> $n/((n-1)(n-2)) . \sum{}$
	- Simetrico -> sesgo = 0.
		- Media y mediana son iguales.
	- Moderadamente sesgado a la izq. -> sesgo = negativo.
		- La media es menor que la mediana.
	- Moderadamente sesgado a la derecha. -> Sesgo = positivo
		- La media es mayor a la mediana.
	- Muy sesgado a la derecha -> Sesgo = positivo (mayor a 1)
	- Muy sesgado a la izq.
- Valor z -> numero de desviaciones estandar que xi, se encuentra de la media
	- Traslada la curva a la media central, que es igual a 0.
		zi = $(xi-x)/s$
		El valor z para cualquier observacion puede interpretarse como una medida de la posicion relativa de la observacion en un conjunto de datos 
	- z < 0 -> observaciones con valor menor a la media
	- z > 0 -> observaciones con valor mayor a la media
	- z = 0 -> el valor de laobservacion es igual a la media
	Es utilizado para el teorema de Chebyshez -> 
		Por lo menos (1 - 1/z²) de los valores de datos debe estar dentro de z desviaciones estandar de la media, donde z es culquier valor mayor a 1.
		- Por lo menos 0.75 datos debe estar dentro de z = 2 desviaciones estadar de la media.
		- 0.89 dentro de z = 3.
		- 0.94 dentro de z = 4.
- Regla empirica
		Se usa para determinar el porcentaje de valores de datos que deben estar dentro de un numero especifico de desviaciones estandar de la media.

- Deteccion de observaciones atipicas
	Un conjunto de datos puede tener una o mas observaciones con valores inusualmente grandes o pequeños.
	Se los consideran atipicos cuando los valores tiene una puntuacion de z menores a -3 o mayores a 3. 
- Resumenes de 5 numeros y diagramas de cajas

- Herramientas para resuimir grandes cantidades de datos
	- Resumen de 5 num
		1. Menor valor
		2. Primer cuartil
		3. Mediana
		4. Tercer cuartil
		5. Mayor valor
	
	- Diagrama de caja
		- Se traza una caja con sus extremos ubicados en el 1er y 3er cuartil.
		- Se traza una linea vertical en donde se ubica la mediana.
		- Se localizan los limites con el rango inteercuartilico. (Q3 - Q1)
			- Datos fuera de los limites se consideran atipicos.

Medidas de asociasion entre 2 variables
- Covarianza -> Medida descriptiva de la asociasion lineal entre 2 variables

- Coeficiente de correlación -> La correlacion nos proporciona una medida de asociasion lineal.
	- Rxy = $Sxy/(Sx.Sy)$
	- Los valores cercanos a -1 indican una relacion negativa solida
	- LOs cercanos a 1 inversamente proporcional a lo anterior.
