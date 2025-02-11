# Juan Muñoz Tomas #
# Operaciones de Conjunto (union, except, intersect)

# union #

union o |

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen en cualquiera de los operandos.
La palabra clave union y el carácter | son equivalentes.

## EJEMPLO ##


# intersect #

intersect

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen ambos operandos.

## EJEMPLO ##


# except #

except

Toma dos secuencias de nodo como operandos y devuelve una secuencia que contiene todos los nodos que aparecen en el primer operando pero no en el segundo operando.

## EJEMPLO ##


## Aclaraciones para todos ##
Todos estos operadores eliminan los nodos duplicados

Los operandos de (union, intersecto except) deben resolverse en secuencias que contengan sólo nodos. Si un operando contiene un elemento que no es un nodo, se devuelve un error.

## Pagina anterior ##
[Pagina anterior](./AbrahamLG.md)


## Pagina siguiente ##
[Pagina anterior](./AbrahamLG.md)




Las expresiones siguientes son todos ejemplos válidos que utilizan operadores para combinar secuencias de nodos:
$managers union $students devuelve el conjunto de nodos que representan a los empleados que son gestores o estudiantes.
$managers intersect $students devuelve el conjunto de nodos que representan a los empleados que son gestores y estudiantes.
$managers except $students devuelve el conjunto de nodos que representan a los empleados que son gestores pero no estudiantes.


braham	        Uso de Variables (let)
Juan	        Operaciones de Conjunto (union, except, intersect)
Iván	        Funciones Agregadas (count(), sum(), etc.)
