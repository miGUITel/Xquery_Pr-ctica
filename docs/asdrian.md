# Creación de Nuevos Elementos XML #

Ejemplo 1: Crear un nuevo elemento XML sin atributos

xquery
Copiar
Editar
let $nuevoElemento := <persona>
                        <nombre>Juan</nombre>
                        <edad>30</edad>
                      </persona>
return $nuevoElemento
Este código crea un nuevo elemento XML llamado <persona>, con dos subelementos <nombre> y <edad>, con valores específicos.

Ejemplo 2: Crear un nuevo elemento XML con atributos

xquery
Copiar
Editar
let $nuevoElemento := <producto id="123" categoria="Electrónica">
                        <nombre>Smartphone</nombre>
                        <precio>599.99</precio>
                      </producto>
return $nuevoElemento