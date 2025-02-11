# Juan Muñoz Tomas #
# Operaciones de Conjunto (union, except, intersect)

# union #

union o |

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen en cualquiera de los operandos.
La palabra clave union y el carácter | son equivalentes.

# intersect #

intersect

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen ambos operandos.

# except #

except

Toma dos secuencias de nodo como operandos y devuelve una secuencia que contiene todos los nodos que aparecen en el primer operando pero no en el segundo operando.


####
Todos estos operadores eliminan los nodos duplicados




Los operandos de union, intersecto except deben resolverse en secuencias que contengan sólo nodos. Si un operando contiene un elemento que no es un nodo, se devuelve un error.

Además de los operadores que se describen en este tema, Db2 XQuery proporciona funciones para el acceso indexado a elementos o subsecuencias de una secuencia (fn:index-of), para la inserción o eliminación indexada de elementos en una secuencia (fn:insert-before y fn:remove) y para eliminar elementos duplicados de una secuencia (fn:distt-values).

ejemplos
En estos ejemplos, supongamos que la variable $managers está enlazada a un conjunto de nodos de empleado que representan a los empleados que son gestores, y que la variable $students está enlazada a un conjunto de nodos de empleado que representan a los empleados que son estudiantes.

Las expresiones siguientes son todos ejemplos válidos que utilizan operadores para combinar secuencias de nodos:
$managers union $students devuelve el conjunto de nodos que representan a los empleados que son gestores o estudiantes.
$managers intersect $students devuelve el conjunto de nodos que representan a los empleados que son gestores y estudiantes.
$managers except $students devuelve el conjunto de nodos que representan a los empleados que son gestores pero no estudiantes.



### Primera captura

![alt](./capturasIllia/Captura%20de%20pantalla%20de%202025-02-07%2012-58-33.png)