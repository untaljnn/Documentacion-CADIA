# Inventario

El inventario es una lista de bienes y productos que se encuentran en el laboratorio. En este caso,
el inventario es una lista de los productos, reactivos, materiales y equipos que se encuentran en el laboratorio.
Su principal función es llevar un control sobre los reactivos y materiales que se tienen en el laboratorio mejorando
la trazabilidad de los mismos.

## Información de un producto

<table>
<tr>
<td>Nombre</td>
<td>Tipo</td>
<td>Ejemplo / Uso</td>
</tr>

<tr>
<td>Foto del reactivo</td>
<td><code>Imagen</code></td>
<td>Imagen de como se presenta el reactivo</td>
</tr>

<tr>
<td>Nombre</td>
<td><code>Texto</code></td>
<td>Nombre del reactivo</td>
</tr>

<tr>
<td>Descripción</td>
<td><code>Texto</code></td>
<td>Descripción general del reactivo, producto o equipo, principalmente de su funcionalidad</td>
</tr>

<tr>
<td>Unidad de medida</td>
<td><code>Numérico</code></td>
<td>Unidad de medida del reactivo (gramos, mililitros, etc.)</td>
</tr>

<tr>
<td>Cantidad</td>
<td><code>Numérico</code></td>
<td>La cantidad actual con la que se cuenta de reactivo</td>
</tr>

<tr>
<td>Cantidad mínima</td>
<td><code>Numérico</code></td>
<td>La cantidad mínima con la que se espera contar, de rebasar esta marca el sistema avisará que está por agotarse</td>
</tr>

<tr>
<td>Fecha de entrega</td>
<td><code>Fecha</code></td>
<td>Fecha que indique la llegada de un equipo, bien o reactivo al laboratorio</td>
</tr>
</table>

## Condiciones de funcionamiento
- Se espera tener una alerta que indique cuando un reactivo está por agotarse.