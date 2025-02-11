# Uso de variables(let) #
## Abraham Lozano ##
## Explicación teórica ##
### Expresión FLWOR ###
La expresión XQuery más importante es la llamada expresión FLWOR. FLWOR es el acrónimo inglés de **For-Let-Where-Order-Return** y suele pronunciarse como la palabra inglesa "flower" (flor). Funciona de manera parecida a la instrucción SQL SELECT, que tiene cláusulas similares, como FROM, WHERE, ORDER BY, etc. La expresión FLWOR permite consultar datos XML y de BD con mayor eficacia que con expresiones XPath.

En XQuery, la cláusula **let** se utiliza para incializar una varible intermedia cuando ya hemos usado la claúsula **for**.
Por ejemplo, si queremos una variable que llamada "nombre" cuyo contenido sea una cadena con valor "Abraham", podemos expresarlo de así:

    let $nombre := "Abraham"

    return $nombre

Le hemos asignado el valor "Abraham" al atributo nombre.

Si combinamos **for** con **let**, podríamos estructurar la consulta de esta manera:


    for $persona in ("Abraham")
    let $apellido := "Lozano"
    return concat($persona, " ", $apellido)
En este caso:

**for $persona** recorre una secuencia (en este ejemplo, solo contiene "Abraham").

**let $apellido** almacena el valor "Lozano", sin iterar.

**return concat($persona, " ", $apellido)** genera "Abraham Lozano".

De esta manera, **let** permite definir variables auxiliares dentro de una consulta sin afectar la iteración de **for**



## Ejemplos ##
Para los siguientes ejemplos, utilizaremos una base de datos XML de una librería, proporcionada en una tarea anterior.

### Ejemplo 1 ###
Queremos sacar todos los libros cuya fecha sea de antes del 2000.

![alt text](<capturasAbraham/XQueryAño.png>)

### Ejemplo 2 ###
Queremos sacar todos los libros cuyo precio sea menor de 50 y su fecha sea de antes del 2000, ordenados de forma descendente

![alt text](<capturasAbraham/XQueryAñoPrecio.png>)

<-- [Creacion de nuevos elementos XML](./asdrian.md) ======================= [Operaciones de Conjunto (union, except, intersect)](./JuanMt.md)-->
