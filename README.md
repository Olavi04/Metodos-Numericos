# Metodos Numericos

  + Eliminacion Gaussiana
  + Gauss-Jordan
  + Gauss-Seidel
  + Jacobi
  

##EJEMPLOS##

## Eliminacion Gaussiana

> Ejemplo


  


## Método de Gauss-Jordan

> Ejemplo

+ Método de Gauss-Jordan
+Solución a Sistemas de Ecuaciones de la forma A.X=B

***### INGRESO ###***

A = np.array([[4,2,5],
              [2,5,8],
              [5,4,3]])

B = np.array([[60.70],
              [92.90],
              [56.30]])
              
***### Salida ###***

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

## Gauss-Seidel

> Ejemplo

respuesta X: 
[[ 3. ]
 [-2.5]
 [ 7. ]]
verificar A.X=B: 
[[  7.84999999]
 [-19.3       ]
 [ 71.4       ]]
>>> 



## Jacobi

> Ejemplo
