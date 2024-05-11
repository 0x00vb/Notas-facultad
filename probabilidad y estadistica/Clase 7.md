
## Variable aleatoria discreta

## Variable aleatoria continua



# Distribuciones de probabilidad
Variable aleatoria que describe como se distribuyen las probabilidades entre los valores de la misma.



Metodos para asignar probabilidades a las variables aleatorias:

(x, f(x)) -> Funcion de densidad/dist de prob

Condiciones:
1) f(x) >0
2) Ef(x) =1
3) P(X = x) = f(x)

Discreta
F(x) = P(X <= x) = Ef(t)


Dist prop continuas
1) f(x) >= 0
2) integral(f(x)dx) = 1
3) P(a <= x <= b) = integral[a,b]f(x)dx = F(b) - F(a)

F(x) != f(x)
F(x) -> funcion distribucion acumulada -> Acumulacion de probabilidades hasta x.
f -> funcion de desidad -> brinda un valor de la densidad en determinado punto.

f(x) = derivada(F(X))

Distribucuiones continuas -> No tiene probabilidad puntual.


Esperanza/valor esperado -> Promedio
variable discreta = E(xf(x))
var. continua = Integral(xf(x)) 

e = esperanza
1) e(k) = k
2) e(k.x) = k.e(x)
3) e(x +- y) = e(x) +- e(y)
4) e(ax +- bx) 0 a.e(x) +- b-e(y)
5) .

Varianza -> e(x²) - e²(x)
- discreta = E(x² . f(x))
- continua = Integral(x² . f(x) dx)

condiciones
- Discretas.
	- f(x) >= 0
	- E(f(x)) = 1
	- P(X = x) = f(x)
	- F(x) = P(X>=x) = E(f(t))
	- M = e(x) = E(x . f(x))
	- 
- Continuas
	- f(x) >= 0
	- Integral(f(x) dx) = 1
	- P(a<= 0 <= b) = Integral(f(x)dx) = F(b) - F(a)
	- P(X = a) = 0
	- F(x) = P(x<=x) = Integral(f(x)dx)[0, x]
	- M = e(x) = Integral(x.f(x)dx)
	- 

Varianza -> 
1) V(k) = 0
2) V(kx) = k² V(x)
3) V(ax + b) = a²V(x)
4) V(x+-y) = V(x) +- V(y) -> Solo si x e y son var. independientes.

Dist de prop discret as especificadas por formulas:
 - uniforme:
		 f(x) = 1/n, siendo n los valores que puede tomar una variable aleatoria.
 - binomial ->
		n ensayos identicos.
		2 posibles resultados: exito / fracaso.
		p = probabilidad de exito.
		Ensayos independientes.
		f(x) = (n)  . p^x . q^(n-x)
		     (x)
		M = n . p 
		Var = n . p . q
		Desvio = Raiz(n . p . q)
	 - binomial negativa ->
			
		 - Geometrica
 - Poisson
 - Hipergeometrica