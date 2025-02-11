# Uso de variables(let) #
## Abraham Lozano ##
## Explicación teórica ##
### Expresión FLWOR ###
La expresión XQuery más importante es la llamada expresión FLWOR. FLWOR es el acrónimo inglés de **For-Let-Where-Order-Return** y suele pronunciarse como la palabra inglesa "flower" (flor). Funciona de manera parecida a la instrucción SQL SELECT, que tiene cláusulas similares, como FROM, WHERE, ORDER BY, etc. La expresión FLWOR permite consultar datos XML y de BD con mayor eficacia que con expresiones XPath.

En XQuery, la cláusula **let** se utiliza para incializar una varible intermedia cuando ya hemos usado la claúsula **for**.
Por ejemplo, si queremos una variable que llamada "nombre" cuyo contenido sea una cadena con valor "Abraham", podemos expresarlo de así:

    let $nombre := "Abraham"

    Le hemos asignado el valor "Abraham al atributo nombre.

Si ya hemos declarado una variable con **for** tendriamos una estructura como la siguiente:

    for $nombre := "Abraham"

    let  $apellido:= "Lozano"




## Ejemplos ##
Para los siguientes ejemplos usaremos una bse de datos XML dada en una tarea anterior. Esta base de datos gestiona una librería



[Página Anterior---Creacion de nuevos elementos XML](./AGP.MD)

[Página Siguiente---Operaciones de Conjunto (union, except, intersect)](./JuanMt.md)
