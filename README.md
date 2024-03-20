# Metodos Numericos

  + Biseccion
  + Gauss
  + Lagrange
  + Newton
  + Secante
  + Euler

##EJEMPLOS##

## Metodo por Biseccion
  + Entrada
La ecuación mostrada tiene una raiz en [1,2], ya que f(1)=-5 y f(2)=14 y existe cambio de signo. Muestre los resultados parciales del algoritmo de la bisección con una tolerancia de 0.0001
f(x)=x^3+4x^2−10=0
+ INGRESO
fx = lambda x: x^3+4x^2−10 
a = 1
b = 2
tolera = 0.001

+ Salida
  
***[   i   , a    , c    , b   , f(a)   , f(c)   , f(b)   ,  tramo]***
<p>1 - 1.000 1.500 2.000 -5.000 2.375 14.000 1.000</p>
<p>2 - 1.000 1.250 1.500 -5.000 -1.797 2.375 0.500 </p>
<p>3 - 1.250 1.375 1.500 -1.797 0.162 2.375 0.250 </p>
<p>4 - 1.250 1.312 1.375 -1.797 -0.848 0.162 0.125 </p>
<p>5 - 1.312 1.344 1.375 -0.848 -0.351 0.162 0.062 </p>
<p>6 - 1.344 1.359 1.375 -0.351 -0.096 0.162 0.031 </p>
<p>7 - 1.359 1.367 1.375 -0.096 0.032 0.162 0.016 </p>
<p>8 - 1.359 1.363 1.367 -0.096 -0.032 0.032 0.008 </p>
<p>9 - 1.363 1.365 1.367 -0.032 0.000 0.032 0.004 </p>
<p>10 - 1.363 1.364 1.365 -0.032 -0.016 0.000 0.002 </p>
<p>11 - 1.364 1.365 1.365 -0.016 -0.008 0.000 0.001 </p>
raiz: - 1.36474609375

## Método de Gauss-Jordan

+ Método de Gauss-Jordan
+Solución a Sistemas de Ecuaciones de la forma A.X=B

+ INGRESO
A = np.array([[4,2,5],
              [2,5,8],
              [5,4,3]])

B = np.array([[60.70],
              [92.90],
              [56.30]])
+ Salida

Matriz aumentada:
<p>[[ 4.   2.   5.  60.7]</p>
 <p>[ 2.   5.   8.  92.9]</p>
<p> [ 5.   4.   3.  56.3]]</p>
<p>Pivoteo parcial por filas</p>
<p>[[ 5.   4.   3.  56.3]</p>
<p> [ 2.   5.   8.  92.9]</p>
<p> [ 4.   2.   5.  60.7]]</p>
<p>eliminacion hacia adelante</p>
<p>[[ 5.    4.    3.   56.3 ]</p>
<p> [ 0.    3.4   6.8  70.38]</p>
<p> [ 0.    0.    5.   40.5 ]]</p>
<p>eliminación hacia atrás</p>
<p>[[ 1.00000000e+00  0.00000000e+00 -2.08983158e-16  2.80000000e+00]</p>
<p> [ 0.00000000e+00  1.00000000e+00  2.61228947e-16  4.50000000e+00]</p>
<p> [ 0.00000000e+00  0.00000000e+00  1.00000000e+00  8.10000000e+00]]</p>
<p>solución de X: </p>
<p>[[2.8]</p>
<p>[4.5]</p>
<p>[8.1]]</p>

## Metodo de Lagrange


