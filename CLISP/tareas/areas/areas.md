# Areas de figuras

## 1. Area de un cuadrado

La primera figura es un cuadrado para lo cual ocuparemos el siguiente codigo: 

~~~
(defun areaCuadrado()
    (princ "Dame la longitud de uno de sus lados: ")
    (setq num (read))
    (setq resultado (* num num))
)
~~~

1. Se define una funcion con el nombre ***areaCuadrado***.
2. Se usa la funcion ***princ*** para desplegar un mensaje.
3. Se usa la funcion ***setq*** para crear una variable y asignarle un valor, seguido de eso se usa la funcion ***read*** para realizar una lectura.
4. Se usa la funcion ***setq*** nuevamente para realizar una operacion con la variable antes guardada y guardar e imprimir este nuevo valor.
5. En el caso del cubo solo es necesario pedir la longitud de uno de sus lados ya que para encontrar el area de esta figura solo es necesario multiplicar por si mismo la longitud de uno de sus lados.
6. El *resultado* se despliega en la consola.
___

## 2. Area de un triangulo

Para realizar el calculo del area de un traingulo ocuparemos el siguiente codigo:

~~~
(defun areaTriangulo()
    (princ "Dame la longitud de la base: ")
    (setq base (read))
    (princ "Dame la longitud de la altura: ")
    (setq altura (read))
    (setq resultado (/ (* base altura) 2))
)
~~~

1. Se define una funcion con el nombre ***areaTriangulo***.
2. Desplegamos un mensaje con ***princ*** para que el usuario nos dé la longitud de la base del triangulo.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *base* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la altura del triangulo.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *altura* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Con la funcion ***setq*** inicializamos una nueva variable con el nombre *resultado* y realizamos la siguiente operacion de manera post-orden para obtener el area del triangulo: `(/ (* base altura) 2)` esto equivale a multiplicar la base por la altura y luego dividir el resultado entre 2.
7. El *resultado* se despliega en la consola.
___

## 3. Area de un rectangulo

Para realizar el calculo del area de un rectangulo ocuparemos el siguiente codigo:

~~~
(defun areaRectangulo()
    (princ "Dame la longitud de la base: ")
    (setq base (read))
    (princ "Dame la longitud de la altura: ")
    (setq altura (read))
    (setq resultado (* base altura))
)
~~~

1. Se define una funcion con el nombre ***areaRectangulo***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé la longitud de la base del rectangulo.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *base* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la altura del rectangulo.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *altura* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Con la funcion ***setq*** incializaremos una nueva variable con el nombre *resultado* y realizaremos la operacion `(* base altura)` que no es otra cosa mas que multiplicar la base por la altura del rectangulo y asi obtendremos el area del rectangulo.
7. El *resultado* se despliega en la consola.
___

## 4. Area de un rombo

Para realizar el calculo del area de un rombo ocuparemos el siguiente codigo:

~~~
(defun areaRombo()
    (princ "Dame la longitud de la diagonal mayor: ")
    (setq dMayor (read))
    (princ "Dame la longitud de la diagonal menor: ")
    (setq dMenor (read))
    (setq resultado (/ (* dMayor dMenor) 2))
)
~~~

1. Se define una funcion con el nombre ***areaRombo***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé la longitud de la diagonal mayor del rombo.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *dMayor* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la diagonal menor del rombo.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *dMenor* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Con la funcion ***setq*** inicializamos una variable con el nombre *resultado* y realizamos la operacion `(/ (* dMayor dMenor) 2)` la cual se realizara de manera post-orden donde primero multiplicara la diagonal mayor por la diagonal menor y el resultado lo dividira entre 2.
7. El *resultado* se despliega en la consola.
___

## 5. Area de un trapecio

Para realizar el calculo del area de un trapecio ocuparemos el siguiente codigo:

~~~
(defun areaTrapecio()
    (princ "Dame la longitud de la base mayor: ")
    (setq bMayor (read))
    (princ "Dame la longitud de la base menor: ")
    (setq bMenor (read))
    (princ "Dale la longitud de la altura: ")
    (setq altura (read))
    (setq resultado (/ (* (+ bMayor bMenor) altura) 2))
)
~~~

1. Se define una funcion con el nombre ***areaTrapecio***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé la longitud de la base mayor del trapecio.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *bMayor* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la base menor del trapecio.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *bMenor* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la altura del trapecio.
7. Con la funcion ***setq*** inicializamos una variable con el nombre *altura* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
8. Con la funcion ***setq*** inicializamos una variable con el nombre *resultado* y realizamos la operacion `(/ (* (+ bMayor bMenor) altura) 2)` que recordemos hara en post-orden, iniciando primero por realizar la suma de las bases, despues multiplicara el resultado por la altura del trapecio y finalmente el resultado lo dividira entre 2.
9. El *resultado* se despliega en la consola.
___

## 6. Area de un circulo

Para realizar el calculo del area de un circulo ocuparemos el siguiente codigo:

~~~
(defun areaCirculo() 
    (princ "Dame el radio del circulo: ")
    (setq radio (read))
    (setq resultado (* 3.14 (* radio radio)))
)
~~~

1. Se define una funcion con el nombre ***areaCirculo***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé el radio del circulo.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *radio* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Con la funcion ***setq*** inicializamos una variable con el nombre *resultado* y realizamos la operacion `(* 3.14 (* radio radio))` que estará elevando al cuadro el radio y luego multiplicandolo por Pi.
5. El *resultado* se despliega en la consola.
___

## 7. Area de un poligono regular

Para realizar el calculo del area de un poligono regular ocuparemos el siguiente codigo:

~~~
(defun areaPoligonoReg()
    (princ "Dame el numero de lados que tiene el poligono: ")
    (setq lados (read))
    (princ "Dame la longitud de la base de uno de los lados: ")
    (setq base (read))
    (princ "Dame la longitud del apotema: ")
    (setq apotema (read))
    (setq resultado (/ (* (* lados base) apotema) 2))
)
~~~

1. Se define una funcion con el nombre ***areaPoligonoReg***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé el numero de lados que tiene el poligono regular.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *lados* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la base de uno de los lados del poligono regular.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *base* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud del apotema del poligono regular.
7. Con la funcion ***setq*** inicializamos una variable con el nombre *apotema* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
8. Con la funcion ***setq*** inicializamos una variable con el nombre *resultado* y realizamos la operacion `(/ (* (* lados base) apotema) 2)` que en un inicio obtendremos el perimetro del poligono ya que multiplicaremos el numero de lados que tiene por la longitud de la base de uno de los lados, el resultado lo multiplicaremos por el apotema y finalmente lo dividiremos entre 2 para asi obtener el area del poligono regular.
9. El *resultado* se despliega en la consola.
___

## 8. Area de un paralelogramo

Para realizar el calculo del area de un paralelogramo ocuparemos el siguiente codigo:

~~~
(defun areaParalelogramo()
    (princ "Dame la longitud de la base: ")
    (setq base (read))
    (princ "Dame la longitud de la altura: ")
    (setq altura (read))
    (setq resultado (* base altura))
)
~~~

1. Se define una funcion con el nombre ***areaParalelogramo***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé la longitud de la base del paralelogramo.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *base* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la altura del paralelogramo.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *altura* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Con la funcion ***setq*** inicializamos una variable con el nombre *resultado* y realizamos la operacion `(* base altura)` la cual multiplicara la base por la altura y asi obtendremos el area del paralelogramo.
7. El *resultado* se despliega en la consola.
___

## 9. Area de un ovalo

Para realizar el calculo del area de un ovalo ocuparemos el siguiente codigo:

~~~
(defun areaOvalo()
    (princ "Dame la longitud del primero radio: ")
    (setq r1 (read))
    (princ "Dame la longitud del segundo radio: ")
    (setq r2 (read))
    (setq resultado (* r1 r2 3.14))
)
~~~

1. Se define una funcion con el nombre ***areaOvalo***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé la longitud del primero radio.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *r1* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud del segundo radio.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *r2* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Con la funcion ***setq*** inicializamos una variable con el nombre *resultado* y realizamos la operacion `(* r1 r2 3.14)` que es multiplicar los dos radios y el resultado por Pi.
7. El *resultado* se despliega en la consola.

## 10. Area de un cometa

Para realizar el calculo del area de un cometa ocuparemos el siguiente codigo:

~~~
(defun areaCometa()
    (princ "Dame la longitud de la diagonal mayor: ")
    (setq diagMayor (read))
    (princ "Dame la longitud de la diagonal menor: ")
    (setq diagMenor (read))
    (setq resultado (/ (* diagMayor diagMenor) 2))
)
~~~

1. Se define una funcion con el nombre ***areaCometa***.
2. Se despliega un mensaje con ***princ*** para que el usuario nos dé la longitud de la diagonal mayor del cometa.
3. Con la funcion ***setq*** inicializamos una variable con el nombre *diagMayor* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
4. Desplegamos un nuevo mensaje con ***princ*** para que el usuario nos dé la longitud de la diagonal menor del cometa.
5. Con la funcion ***setq*** inicializamos una variable con el nombre *diagMenor* y realizamos una lectura con ***read*** para guardar en la variable lo que el usuario a digitado.
6. Con la funcion ***setq*** inicializamos una variable con el nombre *resultado* y realizamos la operacion `(/ (* diagMayor diagMenor) 2)` esto hará que primero se multipliquen las diagonales y luego se divida entre 2 y esto se almacene en la variable *resultado*.
7. El *resultado* se despliega en la consola.