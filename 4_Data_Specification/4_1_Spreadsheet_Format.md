# Spreadsheet Format

All Household Waste recycling Centres are considered to be a site. This information uses `schema:Place` to describe the location.

The following table lists the properties that can be used in this specification to describe a Household Waste Recycling Centre.

|Property|Status|Format|Notes|
|:-|:-|:-|:-|
|@type|`required`|String|A type of place as defined by Schema.org|
|@id|`required`|URI|A URI providing a unique identifier for the resource|
|schema:identifier|`optional`|String|Local identifier(s) for this resource|
|schema:url|`recommended`|URI|A URL that links to a web page that provides more information about this HWRC|
|schema:name|`required`|String|The name of this HWRC|
|schema:description|`recommended`|String|A description of this HWRC|
|schema:image|`optional`|Array of schema:ImageObject|One or more images or photographs of this HWRC|
|schema:address|`required`|schema:PostalAddress|The street address of this HWRC|
|schema:geo|`required`|schema:GeoCoordinates|Latitude and longitude of thie HWRC|
|schema:telephone|`recommended`|String|Contact telephone number for this HWRC|
|schema:openingHoursSpecification|`recommended`|Array of schema:OpeningHoursSpecification|Specifies opening hours of this HWRC|
|operator|`required`|schema:Organization|The organisation responsible for operating the site|
|||||