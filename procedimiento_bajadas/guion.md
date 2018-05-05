## GUION

--------------
Hola, en este video probaremos que "si P es un prcedimiento efectivo cuyo
conjunto de datos de entrada es [omega por (sigma estrella)], entonces
el conjunto formado por los pares (x, alfa) pertenecientes a
[omega por (sigma estrella)] tal que P termina partiendo de (x, alfa) es
Sigma-efectivamente enumerable".

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
- El conjunto de salida de (P sub ese) es S

--------------
Bueno, daremos entonces, de manera explicita el procedimiento (P sub
ese).

Como el conjunto S no es vacío, entonces sabemos que existe, al menos,
un elemento en S. Sea (x uno, alfa uno) un elemento de S.

---------------
Supongamos (menor) un orden sobre [sigma estrella].

Veamos, entonces, la definición dicho procedimiento.
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
  termina, devolver el elemento desde el cual corrimos P y deterse.
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
[FILMINA en la que empiezan los subitems!!!]
