# Metodos Numericos

  + Biseccion
  + Gauss
  + Lagrange
  + Newton
  + Secante
  + Euler

##EJEMPLOS##

## Biseccion
  + Entrada
La ecuación mostrada tiene una raiz en [1,2], ya que f(1)=-5 y f(2)=14 y existe cambio de signo. Muestre los resultados parciales del algoritmo de la bisección con una tolerancia de 0.0001
f(x)=x^3+4x^2−10=0
+ INGRESO
fx = lambda x: x**3 + 4*x**2 - 10 
a = 1
b = 2
tolera = 0.001

+ Salida
  [?2004l
[ i, a, c, b, f(a), f(c), f(b), tramo]
1 1.000 1.500 2.000 -5.000 2.375 14.000 1.000 
2 1.000 1.250 1.500 -5.000 -1.797 2.375 0.500 
3 1.250 1.375 1.500 -1.797 0.162 2.375 0.250 
4 1.250 1.312 1.375 -1.797 -0.848 0.162 0.125 
5 1.312 1.344 1.375 -0.848 -0.351 0.162 0.062 
6 1.344 1.359 1.375 -0.351 -0.096 0.162 0.031 
7 1.359 1.367 1.375 -0.096 0.032 0.162 0.016 
8 1.359 1.363 1.367 -0.096 -0.032 0.032 0.008 
9 1.363 1.365 1.367 -0.032 0.000 0.032 0.004 
10 1.363 1.364 1.365 -0.032 -0.016 0.000 0.002 
11 1.364 1.365 1.365 -0.016 -0.008 0.000 0.001 
raiz:  1.36474609375

### Gaus
