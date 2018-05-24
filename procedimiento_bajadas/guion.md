## GUION

--------------


si P es un procedimiento efectivo cuyo conjunto de datos de entrada es
[omega por (sigma estrella)], entonces el conjunto de datos de entrada
para los cuales P termina es Sigma-efectivamente enumerable.


---------------
Veamos esto.
Primero, Supongamos que P es un procedimiento efectivo cuyo conjunto de
datos de entrada es [omega por (sigma estrella)].

-----------------

Probaremos entonces, que el conjunto (S igual a los pares (x, alfa)
pertenecientes a [omega por (sigma estrella)] tal que P termina partiendo
de (x, alfa) es Sigma-efectivamente enumerable).

----------------

Veamos los dos casos posibles.

Si (S es el conjunto vacío), entonces S es Sigma-efectivamente enumerable por definición.

----------------

Ahora bien, si (S no es vacío) daremos un procedimiento efectivo
(P sub ese) que enumere al conjunto S.

Veamos.

---------------
Por definición, como (P sub ese) debe enumerar a S, entonces debe
cumplir que:
- El conjunto de entrada de (P sub ese) es omega.

---------------
- (P sub ese) siempre termina

---------------
- El conjunto de salida de (P sub ese) es S. Es decir, (P sub ese) devuelve SOLO
elementos que estan en S, y eventualmente devuelve TODOS los elementos de S

--------------
Bueno, daremos entonces, de manera explicita el procedimiento (P sub
ese).

Como el conjunto S no es vacío, entonces sabemos que existe, al menos,
un elemento en S.
Sea (x uno, alfa uno) un elemento de S.

---------------
Supongamos (menor) un orden sobre [sigma estrella].

---------------
Recordemos una función que será de vital importancia en nuestra definición del
procedimiento. Esta será la (bajada i de x).

Por definición, la bajada i de x es el máximo t tal que el i-ésimo primo elevado
a la t divide a x.

En otras palabras, si factorizamos a x en números primos, la bajada i de x
nos dirá el exponente con el que aparece, en dicha factorización, el i-ésimo
número primo.

También recordemos que el orden i-ésimo es el absoluto y
no el que aparece en la factorización de x. Es decir, que, por ejemplo, el 3er
número primo es SIEMPRE el número 5.


Ahora si, veamos entonces, la definición dicho procedimiento.

---------------

(P sub ese) toma como entrada un valor (x en omega).

Lo que hará en la Etapa 1 es:
- Si el valor de entrada, x, es igual a cero, devolver el elemento
  (x uno, alfa uno) y detenerse.
- Si no, correr el procedimiento P una cantidad [bajada 1 de x] pasos
  con entrada el elemento cuya primer coordenada es (bajada 2 de x) y
  la segunda es (la palabra en la posición [bajada 3 de x] según el
  orden determinado anteriormente).
  Y, si luego de una cantidad [bajada 1 de x] pasos, el procedimiento P
  termina, devolver el elemento desde el cual corrimos P y detenerse.
  Si no termina, devolver (x uno, alfa 1) y detenerse.

-----------------
Ahora veamos que (P sub ese) cumple con las propiedades necesarias para
que enumere a S, mencionadas anteriormente.

Resulta evidente, por la naturaleza de las instrucciones llevadas a cabo
por (P sub ese) y dado que el P es efectivo, que el procedimiento
(P sub ese) es efectivo.
Veamos ahora que cumple con las propiedades 1, 2 y 3.

Las propiedades 1 y 2, se cumplen trivialmente. Veamos entonces que se
cumple la propiedad 3.

------------------
Sabemos que si (x, alpha) es un elemento cualquiera de S, por definición, P
terminará partiendo de (x, alfa)

------------------
Por otra parte. Sea 'p' la cantidad de pasos que necesita el procedimiento P
para terminar partiendo de (x, alfa).

------------------
Entonces, si tenemos en cuenta las 'bajadas de x' usadas, podemos ver
que para el valor de entrada [z igual a (2^(p+1) * 3^x * 5^(número correspondiente a alfa))],
el procedimiento (P sub ese) termina y da como salida (x, alfa).

Cabe aclarar que dicho valor de zeta queda en evidencia siguiendo la definición
de la función 'bajada de un número' y prestando atención a cómo usamos dicha
función en el procedimiento. Más aún, en el procedimiento, podríamos haber
usado cualesquiera otras bajadas de x, que también hubieran funcionado (sólo
que claramente, el valor de entrada necesario para dar como salida el elemento
[x, alfa] también cambiaría)


------------------
Y de esta manera hemos probado que el procedimiento que dimos cumple con
las propiedades 1, 2 y 3

------------------
Finalmente, como dimos un procedimiento efectivo [P sub ese] que cumple con
1, 2 y 3, dicho procedimiento enumera a S.

Por lo tanto, el conjunto S es efectivamente enumerable
