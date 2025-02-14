# Ordenación en XQuery (order by)

## Explicación Teórica
En XQuery, el operador order by permite ordenar los resultados de una consulta basándose en uno o más criterios. Se utiliza dentro de una expresión FLWOR (acrónimo de for, let, where, order by, return).

Tipos de ordenación disponibles:

ascending → Orden ascendente (menor a mayor) (por defecto)

descending → Orden descendente (mayor a menor)

También es posible ordenar por múltiples criterios, combinando diferentes órdenes.

## Su Sintaxis Básica

```
for $var in ejemplo/elemento
order by $var/campo ascending
return $var
```

## Ejemplo practico
Supongamos que tenemos una base de datos XML con una lista de libros y queremos ordenarlos por precio de menor a mayor.

```
<?xml version="1.0" encoding="UTF-8"?>
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
```

## Ejemplo de consulta

```
for $libro in libros/libro
order by $libro/precio ascending
return $libro
```

## Salida esperada por el programa

```
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
```

### Captura probando el ejemplo ###

![alt](docs\capturasSamuel\image.png)


<-- [Uso de Variables (let)](./docs/AbrahamLG.md) ============= [Manipulación de Cadenas](./gabriel.md) -->