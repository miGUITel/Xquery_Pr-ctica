# Ordenación en XQuery (order by)

## Explicación Teórica
El operador order by en XQuery permite ordenar los resultados de una consulta basándose en uno o más criterios. Se usa dentro de una expresión 
FLWOR(for, let, where, order by, return). 
Ascending (ascendente) es el orden predeterminado y descending (descendente) se usa para invertir el orden.

## Sintaxis Básica

for $var in collection('ejemplo')/elemento
order by $var/campo ascending
return $var

## Ejemplo practico
Supongamos que tenemos una base de datos XML con una lista de libros y queremos ordenarlos por precio de menor a mayor.

<libros>
    <libro>
        <titulo>Libro A</titulo>
        <precio>25</precio>
    </libro>
    <libro>
        <titulo>Libro B</titulo>
        <precio>18</precio>
    </libro>
    <libro>
        <titulo>Libro C</titulo>
        <precio>30</precio>
    </libro>
</libros>

## Ejemplo de consulta

for $libro in doc('libros.xml')/libros/libro
order by $libro/precio ascending
return $libro

## Salida esperada por el programa

<libro>
    <titulo>Libro B</titulo>
    <precio>18</precio>
</libro>
<libro>
    <titulo>Libro A</titulo>
    <precio>25</precio>
</libro>
<libro>
    <titulo>Libro C</titulo>
    <precio>30</precio>
</libro>

