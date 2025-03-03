# Colaboradores

Este módulo es ajeno a los demás, pero que también tiene un funcionamiento importante en el sistema. Pues es el
encargado de llevar un control de las personas que colaboran con el laboratorio.

El laboratorio puede tener colaboradores que son tesistas, residentes profesionales, prestadores de servicio social,
entre otros, por lo que es necesario llevar un control de estos colaboradores y de la información que se tiene de ellos.
CADIA puede tener múltiples colaboradores al mismo tiempo y de diferente carácter.

El siguiente diagrama muestra la relación entre los colaboradores y el laboratorio

<code-block lang="PlantUML">
@startuml
left to right direction

entity Laboratorio
actor Colaborador1
actor Colaborador2
actor Colaborador3
actor Colaborador4

Colaborador1 --> Laboratorio
Colaborador2 --> Laboratorio
Colaborador3 --> Laboratorio
Colaborador4 --> Laboratorio
@enduml
</code-block>

## Información de un colaborador

<table>
<tr>
<td>Nombre</td>
<td>Tipo</td>
<td>Ejemplo / Uso</td>
</tr>
<tr>
<td>Nombre</td>
<td><code>Texto</code></td>
<td>Nombre completo del colaborador</td>
</tr>

<tr>
<td>Relación</td>
<td><code>Texto</code></td>
<td>La relación que tiene con el laboratorio, es decir, si es algún tesista, residente profesional o 
prestante de servicio social</td>
</tr>

<tr>
<td>Acuerdo de confidencialidad</td>
<td><code>Archivo</code></td>
<td>Una copia del acuerdo de confidencialidad firmado por ambas partes</td>
</tr>

<tr>
<td>Documentos</td>
<td><code>Archivo</code></td>
<td>Los documentos pertinentes por cada caso, para dar un seguimiento y tener un registro de uno</td>
</tr>
</table>

<warning>
Se debe de definir todos los casos de colaboración que puede llegar a tener el laboratorio y ver la mejor forma
de abordarlo, pues puede ser de manera general o tomar un registro diferente por cada caso.
</warning>