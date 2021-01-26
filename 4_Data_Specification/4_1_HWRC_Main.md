# HWRC Standard Spreadsheet Format

The spreadsheet format is the simplest way to provide information about Household Waste Recycling Centres.

The following table lists the column headings that should be used. When providing this information, you can either build your spreadsheet from scratch, or use the template provided.

hwrc_main.csv


|Column|Status|Format|Notes|
|:-|:-|:-|:-|
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
|openingHours|`recommended`|String|Specifies opening hours of this HWRC. Opening hours should be specified as a weekly time range, starting with days, then times per day. Multiple days can be listed with commas ',' separating each day. Day or time ranges are specified using a hyphen '-'. Days are specified using the following two-letter combinations: Mo, Tu, We, Th, Fr, Sa, Su. Times are specified using 24:00 format. For example, 3pm is specified as 15:00, 10am as 10:00. An example of this would be `Tu,We,Th 08:00-17:00`. Multiple entries should be separated by semi-colons.|
|ownerID|`required`|String|An identifier from the local authorities controlled list|
|ownerName|`required`|String|The name of the owner of the HWRC|
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
|areaServed|`recommended`|String|Either a semi-colon-separated list of local authorities identifiers, or a unique identifier of an area served provided in a separate csv, geoJSON or Shape file| 
|charge|`recommended`|Boolean|Is there a cost associated with using this HWRC?|
|permitRequired|`recommended`|Boolean|Is a permit required to use this site?|
|trade|`recommended`|Boolean|Is this HWRC accessible by tradespeople|
|ANPR|`recommended`|Boolean|Is automatic number plate recognition in use at the site?|
|reuseShop|`recommended`|Boolean|Is there a reuse shop at this site?|

