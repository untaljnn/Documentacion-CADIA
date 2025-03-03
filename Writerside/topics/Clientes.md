# Clientes

Los clientes son el elemento más importante y a su vez  el más simple. Pues son los que solicitan los servicios que se
ofrecen en el laboratorio. Por lo que es necesario tener un control de los clientes y de los servicios que solicitan.

Un cliente puede solicitar uno o varios servicios, y un servicio puede ser solicitado por un cliente. A su vez, un 
cliente puede pedir más de una vez el mismo servicio pero estos serán distintos entre sí.

<code-block lang="PlantUML">
@startuml
left to right direction

actor Cliente

usecase "Desarrollo de productos" as UC1
usecase "Registro de marca" as UC2
usecase "Elaboración de manuales" as UC3
usecase "Mejora de procesos" as UC4

Cliente --> UC1
Cliente --> UC2
Cliente --> UC3
Cliente --> UC4

@enduml
</code-block>

## Información de un cliente

<table>
<tr>
<td>Nombre</td>
<td>Tipo</td>
<td>Ejemplo / Uso</td>
</tr>

<tr>
<td>Nombre Completo</td>
<td><code>Texto</code></td>
<td>Se registra el nombre completo del cliente</td>
</tr>

<tr>
<td>Número de teléfono</td>
<td><code>Numérico</code></td>
<td>Número de contacto del cliente</td>
</tr>

<tr>
<td>Correo electrónico</td>
<td><code>Texto</code></td>
<td>Se registra el correo electrónico de contacto del cliente</td>
</tr>

<tr>
<td>Dirección</td>
<td><code>Texto</code></td>
<td>Se registra la dirección del clente</td>
</tr>

<tr>
<td>Nombre de la empresa</td>
<td><code>Texto</code></td>
<td>Nombre de la empresa a la que pertenece o representa el cliente</td>
</tr>

<tr>
<td>Descripción empresa</td>
<td><code>Texto</code></td>
<td>Descripción o giro de la empresa con la que se está trabajando</td>
</tr>

<tr>
<td>Fecha de registro</td>
<td><code>Fecha</code></td>
<td>La fecha en la que se registro el cliente en el sistema</td>
</tr>
</table>