

## Estándar para la definición de un trámite y sus elementos

La Ley de Mejora Regulatoria establece la creación del Registro Nacional de Trámites (RNT). La ley establece que solamente los trámites y sus elementos inscritos y aprobados en este registro podrán ser requeridos a la ciudadanía. Corresponde al Organismo de Mejora Regulatoria su conformación y administración y a las instituciones de los tres órganos de estado inscribir y actualizar la información sobre los trámites.

A continuación se detalla la estructura definida en el RNT para los trámites y sus elementos.

### Trámite
#### Estructura
<table>
  <thead>
    <th></th>
    <th>Campo</th>
    <th>Tipo</th>
    <th>Descripción</th>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Nombre</td>
      <td>Alfanumérico</td>
      <td>Debe ser descriptivo para las personas.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Modalidades</td>
      <td>[Colección](#modalidad)</td>
      <td>Modalidades del trámite.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Institución</td>
      <td>Relación</td>
      <td>Institución a la que pertenece el trámite.</td>
    </tr>
  </tbody>
</table>

*El trámite puede tener una o muchas [modalidades](#modalidad)*.

### Modalidad
Cada trámite tiene las modalidades necesarias basadas en los requisitos solicitados para los diferentes procesos. Si cambia un solo requisito es necesario identificar ese proceso como otra modalidad.

#### Estructura
<table>
  <thead>
    <th></th>
    <th>Campo</th>
    <th>Tipo</th>
    <th>Descripción</th>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Trámite</td>
      <td>Relación</td>
      <td>Trámite al que pertenece.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Nombre</td>
      <td>Alfanumérico</td>
      <td>Debe ser descriptivo para las personas.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Descripción</td>
      <td>Alfanumérico</td>
      <td>Detalle del propósito del trámite y la modalidad en específico.</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Oficinas</td>
      <td>[Colección](#oficina)</td>
      <td>Oficinas de la institución donde se puede realizar.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Medios de presentación</td>
      <td>Alfanumérico</td>
      <td>Medios por los cuáles se puede presentar. Las opciones pueden ser: 'FA' (presencial), 'ON' (en línea), 'FO' (ambos).</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Periodicidad</td>
      <td>Alfanumérico</td>
      <td>Frecuencia con la que un usuario la debe gestionar. Las opciones pueden ser: 'DE' (a demanda), 'EX' (al vencimiento).</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Posee tiempo de respuesta legal</td>
      <td>Booleano</td>
      <td>Si la institución tiene normado el tiempo de respuesta.</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Tiempo de respuesta legal</td>
      <td>Tiempo</td>
      <td>El tiempo de respuesta normado. Su estructura se compone por 3 valores enteros: días, horas y minutos.</td>
    </tr>
    <tr>
      <td>9</td>
      <td>Vigencia</td>
      <td>[Relación](#vigencia)</td>
      <td>Vigencia de la modalidad.</td>
    </tr>
    <tr>
      <td>10</td>
      <td>Monto de pago</td>
      <td>[Relación](#monto-de-pago)</td>
      <td>Monto a pagar en concepto de tarifa.</td>
    </tr>
  </tbody>
</table>

### Vigencia
<table>
  <thead>
    <th></th>
    <th>Campo</th>
    <th>Tipo</th>
    <th>Descripción</th>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Posee vigencia</td>
      <td>Booleano</td>
      <td>Si la resolución tiene algún período de vigencia.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Tipo</td>
      <td>Alfanumérico</td>
      <td>Opciones: 'FX' (fija), 'VA' (variable).</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Detalle</td>
      <td>Alfanumérico</td>
      <td>Si la vigencia es variable se describe en este campo.</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Unidad</td>
      <td>Alfanumérico</td>
      <td>Para las vigencias fijas significa la unidad de tiempo en la que se establece la vigencia.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Monto</td>
      <td>Númerico</td>
      <td>Para las vigencias fijas significa el monto de tiempo en la unidad establecida.</td>
    </tr>
  </tbody>
</table>

### Oficina
<table>
  <thead>
    <th></th>
    <th>Campo</th>
    <th>Tipo</th>
    <th>Descripción</th>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Institución</td>
      <td>Relación</td>
      <td>Oficina de la institución.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Nombre</td>
      <td>Alfanumérico</td>
      <td>Identificador.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Dirección</td>
      <td>Alfanumérico</td>
      <td>Detalle de la ubicación.</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Municipio</td>
      <td>Relación</td>
      <td>Municipio donde está ubicada.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Horario</td>
      <td>Alfanumérico</td>
      <td>Horario de atención.</td>
    </tr>
  </tbody>
</table>

### Monto de pago
<table>
  <thead>
    <th></th>
    <th>Campo</th>
    <th>Tipo</th>
    <th>Descripción</th>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Posee monto de pago</td>
      <td>Booleano</td>
      <td>Si se debe pagar alguna tasa, tarifa o derechos.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Tipo</td>
      <td>Alfanumérico</td>
      <td>Opciones: 'FX' (fija), 'VA' (variable).</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Monto</td>
      <td>Númerico</td>
      <td>El valor en dólares de los montos de pago fijo.</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Detalle</td>
      <td>Alfanumérico</td>
      <td>Si el monto de pago es variable se describe en este campo.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Enlace</td>
      <td>Alfanumérico</td>
      <td>Enlace web directo al pliego tarifario.</td>
    </tr>
  </tbody>
</table>
  
## Licencia

Este trabajo esta cubierto dentro de la estrategia de desarrollo de servicios de Gobierno Electrónico del Gobierno de El Salvador y como tal es una obra de valor público sujeto a los lineamientos de la Política de Datos Abiertos y la licencia [CC-BY-SA](https://creativecommons.org/licenses/by-sa/3.0/deed.es).  
