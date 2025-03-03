# Trámites

Un servicio de realización de trámites legales en el sector alimentario y empresarial facilita la gestión y cumplimiento
de los requisitos legales para la operación y realización exitosa de un negocio.

## Pasos

<procedure>
<step>
<b>Requisitos del trámite</b>
<table>
<tr>
<td>Nombre</td>
<td>Tipo</td>
<td>Ejemplo / Uso</td>
</tr>
<tr>
<td>Tipo de Tramite</td>
<td><code>Texto</code></td>
<td>COFEPRIS, Registro de marca, código de barras</td>
</tr>
<tr>
<td>Acuerdo de confidencialiad</td>
<td><code>Archivo</code></td>
<td>Se carga una copia del acuerdo de confidencialidad</td>
</tr>
</table>
</step>

<step>
<b>Documentación</b>
Se lleva un seguimiento del trámite y se recopila la documentación necesaria para la realización del mismo.
<table>
<tr>
<td>Nombre</td>
<td>Tipo</td>
<td>Ejemplo / Uso</td>
</tr>
<tr>
<td>Fecha del proceso</td>
<td><code>Fecha</code></td>
<td>Se documenta la fecha en que el proceso tuvo alguna actualización</td>
</tr>
<tr>
<td>Descripción de la etapa</td>
<td><code>Texto</code></td>
<td>Se describe la etapa en la que se encuentra el proceso</td>
</tr>
<tr>
<td>Observaciones de la etapa</td>
<td><code>Texto</code></td>
<td>
Se hacen observaciones de la etapa en la que se encuentra, es decir, si existe algún problema, se describe
</td>
</tr>
<tr>
<td>Estado</td>
<td><code>Texto</code></td>
<td>El estado de la etapa en la que se encuentra, es decir, en proceso, denegado, completado entre otros</td>
</tr>
<tr>
<td>Evidencia</td>
<td><code>Archivo</code></td>
<td>Se cargan documento que sirvan como evidencia o respaldo del proceso que se está llevando</td>
</tr>
</table>
</step>
</procedure>

## Consideraciones de funcionalidad

- Si se maneja información sensible, se debe contar con un acuerdo de confidencialidad firmado por ambas partes.
- Se debería de poder borrar la información o censurar la información sensible en caso de que se requiera.