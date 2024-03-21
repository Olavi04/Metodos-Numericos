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

En el método de Gauss-Seidel se propone ir sustituyendo los nuevos valores de la aproximación siguiente conforme se vayan obteniendo sin esperar a tener un vector completo. De esta forma se acelera la convergencia.

Para resolverlo podemos seguir los siguientes pasos:
+ Asignar valores iniciales a las incógnitas, pudiendo ser hipotéticos o arbitrarios.
+ Empezar con la primera ecuación y calcular el valor de la incógnita con el coeficiente más grande, usando los valores asignados en el paso 1 para las otras incógnitas.
+ Proceder a la siguiente ecuación y calcular el valor de la incógnita con el coeficiente más grande, usando el valor calculado en el paso anterior y los valores iniciales para las otras incógnitas.
+ Repetir este proceso para las ecuaciones restantes, calculando siempre el valor de la incógnita con el coeficiente más grande en cada ecuación y usando los últimos valores calculados para las otras incógnitas.
+ Continuar iterando hasta que los valores de las incógnitas no cambien significativamente entre iteraciones.

Matriz a resolver

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/23561183-a5ab-4579-b9a4-f7589fb0054a)

## SOLUCION O DEDSARROLLO

Primero ordenamos las ecuaciones, de modo que en la diagonal principal esten los coeficientes mayores para asegurar la convergencia.

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/b61d977d-dd5e-4edb-8270-107f1e0a6e28)

Despejamos cada una de las variables sobre la diagonal:

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/ca6743a0-9c53-454f-8b82-b737fcdaad0c)

Suponemos los valores iniciales X2 = 0 y X3 = 0 y calculamos X1

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/646d73c4-9007-416e-973c-79bd1703ed1e)

La primera iteración se completa sustituyendo los valores de X1 y X2 calculados obteniendo:

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/afbf3a25-48b4-41cd-83df-d8ad07e2ea6b)

En la segunda iteración, se repite el mismo procedimiento:

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/7453b4c6-7010-4961-8385-2207c5b41983)

Comparando los valores calculados entre la primera y la segunda iteración

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/daf0178f-43bf-4cb6-ab1e-2493a8776869)

Entonces tomamos los valores calculados en la última iteración y se toman como supuestos para la siguiente iteración. Se repite entonces el proceso:

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/3dca4bdb-4b59-4b66-be3e-2548760dae33)

Comparando los valores obtenidos

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/74631221-10a0-48ab-8bfb-2cd8b725a108)


![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/656f91e7-1f88-461c-82a6-2b1ebdee9811)


## Jacobi

> Ejemplo base

Método Jacobi para resolver ecuaciones.</p>
método iterativo (llamado así por Carl Gustav Jacob Jacobi):


![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/d11cba64-1f83-4d91-8322-9e16e2e04238)

Aquí hay un esquema básico del algoritmo del método Jacobi:

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/c56cfb83-d06a-4ee1-977f-b4cec6910e8f)


![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/4dbc3d79-a82a-43cb-bff9-57b9b8a08953)

Ejemplo

![image](https://github.com/Olavi04/Metodos-Numericos/assets/160789479/b5d5db9d-93ec-4e73-ab99-4c7262ef1314)




