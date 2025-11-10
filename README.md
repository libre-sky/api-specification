# api-specification
The API Specification for a LibreSky server

## Overview

The API is defined in segments. A segment is a grouping of similar measurements, with similarity being determined somewhat arbitrarily as parameters often captured using a single physical sensor



## Segments


### General Atmospheric

These measurements are typically the easiest to collect, as sensors that collect these readings are plentiful. The attributes provided in this section are:

<table><thead>
  <tr>
    <th>Name</th>
    <th>Units</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Temperature</td>
    <td>C,F,K</td>
    <td>The ambient temperature</td>
  </tr>
  <tr>
    <td>Pressure</td>
    <td><a href="https://en.wikipedia.org/wiki/Bar_(unit)">Bar</a>, mBar, <a href="https://en.wikipedia.org/wiki/Pascal_(unit)">Pa</a>, kPa, <a href="https://en.wikipedia.org/wiki/Inch_of_mercury">in Hg</a></td>
    <td>The altitude-adjusted pressure - <a href="https://en.wikipedia.org/wiki/Barometric_formula">adjusted to sea level</a></td>
  </tr>
  <tr>
    <td>Humidity</td>
    <td>%</td>
    <td>The relative humidity</td>
  </tr>
</tbody>
</table>


## Tools

### Autogen

```bash
./cmd/generate <language>
```