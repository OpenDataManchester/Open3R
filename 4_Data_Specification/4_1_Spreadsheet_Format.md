# Spreadsheet Format

The spreadsheet format is the simplest way to provide information about Household Waste Recycling Centres.

The following table lists the column headings that should be used. When providing this information, you can either build your spreadsheet from scratch, or use the template provided.



|Column|Status|Format|Notes|
|:-|:-|:-|:-|
||`required`|String|A type of place as defined by Schema.org|
||`required`|URI|A URI providing a unique identifier for the resource|
|Identifier|`required`|URI|A globally unique identifier obtained from the Public Registers service provided by Environment Agency|
|URL|`recommended`|URI|A URL that links to a web page that provides more information about this HWRC|
|Name|`required`|String|The name of this HWRC|
|Description|`recommended`|String|A description of this HWRC|
|Address|`required`|schema:PostalAddress|The street address of this HWRC|
|Latitude|`required`|number|Enter the latitude of a point close to the centre of the site. The value should be 6 or fewer decimal places, using the WGS84 or ETRS89 coordinate systems. See (this government guidance for more information about this standard)[https://www.gov.uk/government/publications/open-standards-for-government/exchange-of-location-point]|
|Longitude|`required`|number|Enter the longitude of a point close to the centre of the site. The value should be 6 or fewer decimal places, using the WGS84 or ETRS89 coordinate systems. See (this government guidance for more information about this standard)[https://www.gov.uk/government/publications/open-standards-for-government/exchange-of-location-point]|
|Telephone|`recommended`|String|Contact telephone number for this HWRC|
|Opening Hours|`recommended`|String|Specifies opening hours of this HWRC|
|operator|`required`|schema:Organization|The organisation responsible for operating the site|
|||||