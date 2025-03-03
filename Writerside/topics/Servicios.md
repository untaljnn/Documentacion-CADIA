# Servicios

Los servicios son la columna vertebral del sistema de CADIA. Pues son el mayor eje de operación y del cual se desprenden
los demás módulos, que si bien tienen su propia importancia y funciones particulares, dependen de los servicios para que
estos funcionen plenamente y de forma correcta. Es por ello que se le da especial atención a este módulo.

Los servicios por sí solos tienen una gran cantidad de funciones y operaciones que se realizan en el laboratorio. Desde
la recepción de muestras, hasta la entrega de resultados. Por lo que es necesario tener un control y seguimiento de cada
una de estas operaciones para garantizar la calidad y eficiencia del servicio.

Además de estos procesos, se derivan funcionalidades adicionales que dependen completamente de los mismos. Por ejemplo,
la generación de estadísticas, reportes, fichas técnicas, entre otros.

## Funcionamiento

Que los servicios sean la columna vertebral del sistema, no significa que sea un módulo independiente y monolítico. Por
el contrario, estos dependen de otro módulo, **[los clientes](Clientes.md)**, pues son los clientes quienes solicitan
los
servicios. Por
lo que es necesario tener un control de los clientes y de los servicios que solicitan.

Un cliente puede solicitar uno o varios servicios, y un servicio puede ser solicitado por un único cliente.
Esto quiere decir que un cliente puede solicitar varios servicios, pero este servicio en particular pertenecerá a un
cliente en específico. En otras palabras, el cliente **Juan Hernández López**(o su empresa) puede solicitar los
servicios de _Análisis Bromatológico_, _Vida de Anaquel_ y _Desarrollo de productos_, entre otros, pero cada uno de
estos servicios pertenecerán única y exclusivamente a **Juan Hérnandez López** y no a otro cliente.

Sin embargo, cada cliente puede tener su propio servicio de _Análisis Bromatológico_, _Vida de Anaquel_ y _Desarrollo de
productos_, o algún otro según sea requerido, pero este servicio será único del cliente que lo solicita.

Gracias a esto se puede tener una trazabilidad de los servicios que se solicitan y se realizan, así como de los
clientes, además de que se logra tener un registro particular y exacto de la información de cada uno de los servicios y
de los
clientes. Información que estará disponible para su consulta en cualquier momento, gracias a su persistencia en una base
de datos.

Esto se puede ver de forma gráfica en el siguiente diagrama de casos de uso.

<code-block lang="plantuml">
@startuml
left to right direction

actor Cliente

usecase "Desarrollo de productos" as UC1
usecase "Registro de marca" as UC2
usecase "Elaboración de manuales" as UC3
usecase "Mejora de procesos" as UC4

UC1 --> Cliente
UC2 --> Cliente
UC3 --> Cliente
UC4 --> Cliente

@enduml
</code-block>