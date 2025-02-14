# Juan Muñoz Tomas #

> BUEN TRABAJO, los recortes de pantalla se pueden mejorar para que los ejemplos sean más claros.

# Operaciones de Conjunto (union, except, intersect)

# union #

union 

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen en cualquiera de los operandos.

## EJEMPLO ##
$A union $B

![alt text](<imgJMT/image.png>)

> estas capturas son bastante aclaradoras

### EJEMPLO EN X QUERRY ###

Ejemplo para ver las los libros de programación y algoritmos

> en tu ejemplo se ve que has utilizado la expresión pero, como falta contexto, no se aprecia el resultado

![alt text](<imgJMT/image4.png>)

# intersect #

intersect

Toma dos secuencias de nodo y regresa una secuencia que contiene los nodos que aparecen ambos operandos.

## EJEMPLO ##
$A intersect $B

![alt text](<imgJMT/image2.png>)

### EJEMPLO EN X QUERRY ###

Ejemplo para ver las los libros con años menor al 2000 y mayor de 1900 pero solo los que sean menor de 2000 

![alt text](<imgJMT/image5.png>)

# except #

except

Toma dos secuencias de nodo como operandos y devuelve una secuencia que contiene todos los nodos que aparecen en el primer operando pero no en el segundo operando.

## EJEMPLO ##
$A except $B


![alt text](<imgJMT/image3.png>)

### EJEMPLO EN X QUERRY ###

Ejemplo para ver las los libros con años menor al 2000 y mayor de 1900 pero solo los que sean menor de 2000 

![alt text](<imgJMT/image6.png>)


## Aclaraciones para todos ##
> Todos estos operadores eliminan los nodos duplicados

Los operandos de (union, intersecto except) deben resolverse en secuencias que contengan sólo nodos. Si un operando contiene un elemento que no es un nodo, se devuelve un error.


<-- [Uso de Variables](./AbrahamLG.md) =======================  [Funciones Agregadas](./funciones-agregadas-IvanRodriguez.md) -->