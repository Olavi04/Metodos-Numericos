# Metodos Numericos

  + Eliminacion Gaussiana
  + Gauss-Jordan
  + Gauss-Seidel
  + Jacobi
  

##EJEMPLOS##

## Eliminacion Gaussiana

> Ejemplo

Resolver el sistema de ecuaciones lineales

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/eaaced2b-a676-45c5-be23-1139ce505e1a)

  ![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/da744597-d160-43f0-9cab-afe2ed201b0f)

Utilizando Eliminación Gaussiana obtenemos lo siguiente:

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/9c749304-daee-4c01-a08b-dbffc8f1977b)

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/6d1e570c-1b72-4f92-ae8d-d663f84123fa)

Concluimos que la solución del sistema de ecuaciones es:

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/4153b975-aa6e-41b5-80c2-b60cfa39d4c4)




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
