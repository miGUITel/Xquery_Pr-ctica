### Funciones Agregadas en XQuery
Las funciones agregadas en XQuery permiten realizar cálculos sobre una secuencia de valores dentro de un documento XML. Son útiles para procesar grandes volúmenes de datos estructurados y obtener resultados como suma, promedio, máximo, mínimo y conteo de elementos.

### Características de las funciones agregadas en XQuery
- Operan sobre una secuencia de valores (puede ser vacía, contener un solo valor o múltiples valores).
- Son parte del espacio de nombres fn (funciones estándar de XQuery).
- Se utilizan comúnmente para análisis y reportes de datos XML.
- Pueden aplicarse sobre números, fechas y cadenas de texto, dependiendo de la función.
dsfdsfds

### Ejemplos Prácticos
- Ejemplo 1: Suma de valores

let $precios := (10, 20, 30, 40)
return fn:sum($precios)
![alt text](<capturas Ivan/1.png>)

- Ejemplo 2: Promedio de valores

let $precios := (10, 20, 30, 40)
return fn:avg($precios)

- Ejemplo 3: Valor máximo

let $edades := (25, 30, 18, 40, 22)
return fn:max($edades)

- Ejemplo 4: Valor mínimo

let $edades := (25, 30, 18, 40, 22)
return fn:min($edades)

- Ejemplo 5: Conteo de elementos en un XML

let $productos := doc("productos.xml")
return fn:count($productos)



