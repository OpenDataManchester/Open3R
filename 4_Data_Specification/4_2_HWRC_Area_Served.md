# HWRC Area Served

Each HWRC has geographical limit. This may be the local authority area that the HWRC is owned by, a combination of local authorities, or some other boundary. This information should be published as a separate dataset. This can be published as a csv file, or as a spatial datafile. The important point is that the area should have a unique identifier that is referenced from within the main HWRC csv file. This way, anyone wanting to use the data can do so by joining the area served data to the HWRC data.

The specification for the csv format is as follows

|Column|Status|Format|Notes|
|:-|:-|:-|:-|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|areaText|`optional`|String|A written description of the area served|
|areaWKT|`optional`|String|The area served described as a polygon in well known text format|
