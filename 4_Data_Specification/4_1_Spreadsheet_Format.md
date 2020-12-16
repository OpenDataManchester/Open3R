# Spreadsheet Format

The spreadsheet format is the simplest way to provide information about Household Waste Recycling Centres.

The following table lists the column headings that should be used. When providing this information, you can either build your spreadsheet from scratch, or use the template provided.



|Column|Status|Format|Notes|
|:-|:-|:-|:-|
||`required`|URI|A URI providing a unique identifier for the resource|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|govIdentifier|`recommended`|String|An identifier that is used by Government environmental departments|
|URL|`recommended`|URI|A URL that links to a web page that provides more information about this HWRC|
|name|`required`|String|The name of this HWRC|
|description|`recommended`|String|A description of this HWRC|
|siteAddressStreet|`required`|String|The street address of this HWRC|
|siteAddressCity|`required`|String|The street address of this HWRC|
|siteAddressCounty|`required`|String|The street address of this HWRC|
|siteAddressCountry|`required`|String|The street address of this HWRC|
|siteAddressPostcode|`required`|String|The postcode of this HWRC|
|latitude|`required`|number|The latitude of a point close to the centre of the site. The value should be 6 or fewer decimal places, using the WGS84 or ETRS89 coordinate systems. See [this government guidance for more information about this standard](https://www.gov.uk/government/publications/open-standards-for-government/exchange-of-location-point)|
|longitude|`required`|number|The longitude of a point close to the centre of the site. The value should be 6 or fewer decimal places, using the WGS84 or ETRS89 coordinate systems. See [this government guidance for more information about this standard](https://www.gov.uk/government/publications/open-standards-for-government/exchange-of-location-point)|
|telephone|`recommended`|String|Contact telephone number for this HWRC|
|openingHours|`recommended`|String|Specifies opening hours of this HWRC|
|parentID|`required`|String|An identifier from|
|operatorID|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier |
|operatorCompanyID|`recommended`|String|The UK Companies House identifier for this HWRC's operator|
|operatorName|`required`|String|The name of the organisation responsible for operating the site|
|operatorAddressStreet|`recommended`|String|The street address of this HWRC's operator|
|operatorAddressCity|`recommended`|String|The street address of this HWRC's operator|
|operatorAddressCounty|`recommended`|String|The street address of this HWRC's operator|
|operatorAddressCountry|`recommended`|String|The street address of this HWRC's operator|
|operatorAddressPostcode|`recommended`|String|The postcode of this HWRC's operator|
|dateOpened|`optional`|String|The date that this HWRC opened. Supply in format YYYY-MM-DD. If day and month are not known, then just supplying the year will suffice|
|dateClosed|`optional`|String|The date that this HWRC closed. Supply in format YYYY-MM-DD. If day and month are not known, then just supplying the year will suffice|
|servicesAvailable|`recommended`|String|A semi-colon separated list of identifiers from the `Services` reference dataset|
|areaServed|`recommended`|String|The identifier of the area served. Details to be provided in the HWRC Reach Areas reference dataset| 

