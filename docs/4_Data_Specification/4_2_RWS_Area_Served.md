# RWS Area Served

Each RWS has geographical limit. This may be the local authority area that the HWRC is owned by, a combination of local authorities, or some other boundary. Where the area served aligns to one or more local authority boundaries, then the identifiers of these local authorities can be provided as a semi-colon separated list of local authority identifiers in the `areaServed` field.

Where the area served is more complicated than this, a separate file should be provided. This can be published as a csv file, or as a spatial datafile. The important point is that the area should have a unique identifier that is referenced from within the main HWRC csv file. This way, anyone wanting to use the data can do so by joining the area served data to the HWRC data.

The specification for the csv format is as follows

[rws_area_served.csv](https://github.com/OpenDataManchester/Open3R/blob/V2/docs/8_Supporting_Files/8_1_2_RWS_Area_Served_Template.csv)

|Column|Status|Format|Notes|
|:-|:-|:-|:-|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|areaText|`optional`|String|A written description of the area served|
|areaWKT|`optional`|String|The area served described as a polygon in well known text format|

Shapefiles or geoJSON may also be provided, with each area served represented as a single or multipolygon. These polygons should be given identifiers as specified in the Identifiers section of this guidance.
