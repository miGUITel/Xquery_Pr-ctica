# Juan Muñoz Tomas #
# Operaciones de Conjunto (union, except, intersect)

# union #

union 

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen en cualquiera de los operandos.



## EJEMPLO ##
$A union $B

![alt text](<imgJMT/image.png>)

![alt text](image4.png)

# intersect #

intersect

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen ambos operandos.

## EJEMPLO ##
$A intersect $B


![alt text](<imgJMT/image2.png>)

# except #

except

Toma dos secuencias de nodo como operandos y devuelve una secuencia que contiene todos los nodos que aparecen en el primer operando pero no en el segundo operando.

## EJEMPLO ##
$A except $B

![alt text](<imgJMT/image3.png>)


## Aclaraciones para todos ##
Todos estos operadores eliminan los nodos duplicados

Los operandos de (union, intersecto except) deben resolverse en secuencias que contengan sólo nodos. Si un operando contiene un elemento que no es un nodo, se devuelve un error.


[Uso de Variables](./AbrahamLG.md) ___________________ [Funciones Agregadas](./funciones-agregadas-IvanRodriguez.md)