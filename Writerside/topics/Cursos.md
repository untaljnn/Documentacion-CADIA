# Cursos

Los cursos son otro tipo de servicio, pero que se separa de estos por sus particularidades en funcionalidad.
Se espera tener un registro de los cursos que se ofrecen, así como de los participantes que se inscriben en ellos.

El laboratorio puede tener varios cursos y estos a su vez pueden tener varios participantes. Por lo que es necesario
llevar un control de los cursos y de los participantes que se inscriben en ellos, así como la trazabilidad de los mismos.
Registrando los participantes, su asistencia, certificado o constancia, entre otros.
El siguiente diagrama muestra la relación entre los cursos y los participantes.

<code-block lang="PlantUML">
@startuml
left to right direction

entity Laboratorio
entity Curso1
entity Curso2
actor Participante11
actor Participante21
actor Participante31
actor Participante12
actor Participante22
actor Participante32

Participante11 --> Curso1
Participante21 --> Curso1
Participante31 --> Curso1
Curso1 --> Laboratorio

Participante12 --> Curso2
Participante22 --> Curso2
Participante32 --> Curso2
Curso2 --> Laboratorio
@enduml
</code-block>

## Información de un curso

<table>
<tr>
<td>Nombre</td>
<td>Tipo</td>
<td>Ejemplo / Uso</td>
</tr>

<tr>
<td>Nombre del curso</td>
<td><code>Texto</code></td>
<td>Nombre del curso que se realiza</td>
</tr>

<tr>
<td>Descripción</td>
<td><code>Texto</code></td>
<td>Descripción del curso que se realiza</td>
</tr>

<tr>
<td>Duración en minutos</td>
<td><code>Numérico</code></td>
<td>La duración estimada del curso</td>
</tr>

<tr>
<td>Fecha de realización</td>
<td><code>Fecha</code></td>
<td>La fecha en la que imparte el curso</td>
</tr>
</table>


## Información de un participante

<table>
<tr>
<td>Nombre</td>
<td>Tipo</td>
<td>Ejemplo / Uso</td>
</tr>

<tr>
<td>Nombre Completo</td>
<td><code>Texto</code></td>
<td>Nombre del participante</td>
</tr>

<tr>
<td>Asistencia</td>
<td><code>Binario</code></td>
<td>Se registra si el participante asistió al curso o no</td>
</tr>

<tr>
<td>Constancia</td>
<td><code>Archivo</code></td>
<td>La constancia de termino del curso</td>
</tr>
</table>