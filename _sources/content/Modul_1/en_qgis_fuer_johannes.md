## Non-Spatial Analyses in QGIS 

### Geoprocessing Tools - Overview and Selection

![Geoprocessing icons](/fig/en_geoprocessing_icons.png)

![Geoprocessing tools](/fig/en_geoprocessing_tools.png)

```{Tip}
Example for a clip:
```
Creates a __selection__ based on the spatial relationship between each feature in the input layer and the features in an additional layer.

Step by step:
- __Input Layer__: Layer from which the selection is clipped 
- __Overlay Layer__: Area of interest that the input layer will be clipped to 

 <tagName>  <tagName>

![Clip](/fig/en_clip.png)

```{Tip}
Example for a buffer:
```
- __Computes (a) buffer area(s)__ for all the features in an input layer, using a specified distance

Step by step:
- __Input Layer__: Layer around which features the buffer(s) are to be created
- __Distance__: Choose a value and unit (make sure that your input data is projected)
- __Segments__: Add value
- Mark __„Dissolve result“__ to automatically dissolve the buffer outputs 
- If individual buffers are needed, leave __blank__

 <tagName>  <tagName>

![Buffer](/fig/en_buffer.png)

```{Tip}
Examples for buffer usage: 
```
Philippines: Taal Volcano, Base surge hazard map
[https://www.phivolcs.dost.gov.ph/vault/1BaseSurge_Layout-Jan2020_A0_v5.jpg](https://www.phivolcs.dost.gov.ph/vault/1BaseSurge_Layout-Jan2020_A0_v5.jpg)

![Taal Volcano](/fig/en_Taal_Volcano.png)

Nepal: Earthquake, april 2015
[https://reliefweb.int/sites/reliefweb.int/files/resources/reach_npl_map_earthquakeaffected_27apr2015_a3.pdf](https://reliefweb.int/sites/reliefweb.int/files/resources/reach_npl_map_earthquakeaffected_27apr2015_a3.pdf)

![Nepal Earthquake](/fig/en_Nepal_earthquake.png)

Fukushima: may 2011, Integrated doce results<br>
[https://www.emsics.com/five-years-fukushima-incident-management-considerations/](https://www.emsics.com/five-years-fukushima-incident-management-considerations/)

![Aerial measuring results](/fig/en_Aerial_measuring_results.jpg)

### Buffer: with and without “Dissolve”

With dissolve results:

![With dissolve results](/fig/en_dissolve_results.png)

Without dissolve results:

![Without dissolve results](/fig/en_without_dissolve_results.png) 

## Non-Spatial Joins in QGIS

- Choose __“Join Attributes by Field Value”__ Tool (use search tool):

- __Adds attributes__ of a non-spatial table to the layer

- Enables join using a __field/column__ that is present in both data sets

Step by step:
- Input layer: __Vector layer__ 
- Table field: Field/ column that exists in __both data sets__ (name of column in vector layer)
- Input layer 2: __Text/csv/xls data__ 
- Table field 2: Field/ column that exists in __both data sets__ (name of column in text/csv/xls)
- Join type: Select __„Take attributes of the first matching feature only (one-to-one)“__.
- Define __output layer name and destination__ or leave at temporary layer


 <tagName>  <tagName>

![Join attributes by field value](/fig/en_join_attributes_by_field_value.png)

```{Tip} 
Hint
```
If a table join does not work via the “Join Attributes by Field Value” tool, a join can also be performed via the __layer properties__ (right-click, Properties) under the Join tab.

 <tagName>  <tagName>

![Add vector join](/fig/en_add_vector_join.png)

## Spatial Joins in QGIS

Choose __“Join Attributes by Location”__ Tool:
- Adds __additional attributes__ of the join layer to the input layer based on the spatial relationship
- __Input Layer__: Dataset you want to enrich
- __Join layer__: Dataset with additional information/attributes
(you can specify which fields of the join layer should be added)

 <tagName>  <tagName>

![Spatial joins](/fig/en_spatial_joins.png)