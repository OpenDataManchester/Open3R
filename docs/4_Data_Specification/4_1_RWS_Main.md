# Open3R Standard Spreadsheet Format

The spreadsheet format is the simplest way to provide information about recycling and waste sites (RWS).

The following table lists the column headings that should be used. When providing this information, you can either build your spreadsheet from scratch, or use the template provided.

[open3R_main.csv](https://github.com/OpenDataManchester/Open3R/blob/V2/docs/8_Supporting_Files/8_1_1_RWS_Main_Template.csv){target=_blank}


|Column|Status|Format|Notes|
|:-|:-|:-|:-|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|govIdentifier|`recommended`|String|An identifier that is used by Government environmental departments|
|RWStype|`required`|String|The identifier of the RWS Type controlled list that this row relates to.|
|URL|`recommended`|URI|A URL that links to a web page that provides more information about this site|
|name|`required`|String|The name of this RWS service. Could be site name, store, or some other useful name|
|description|`recommended`|String|A description of this RWS|
|siteAddressName|`recommended`|String|The name of the building/location of the RWS. For example: Car Park indicates the bring bank is located in a car park; Tesco indicates the bring bank is located either inside or outside a Tesco.|
|siteAddressStreet|`required`|String|The street address of this RWS|
|siteAddressCity|`required`|String|The street address of this RWS|
|siteAddressCounty|`required`|String|The street address of this RWS|
|siteAddressCountry|`required`|String|The street address of this RWS|
|siteAddressPostcode|`required`|String|The postcode of this RWS |
|latitude|`required`|number|The latitude of a point close to the centre of the site. The value should be 6 or fewer decimal places, using the WGS84 or ETRS89 coordinate systems. See [this government guidance for more information about this standard](https://www.gov.uk/government/publications/open-standards-for-government/exchange-of-location-point){target=_blank}|
|longitude|`required`|number|The longitude of a point close to the centre of the site. The value should be 6 or fewer decimal places, using the WGS84 or ETRS89 coordinate systems. See [this government guidance for more information about this standard](https://www.gov.uk/government/publications/open-standards-for-government/exchange-of-location-point){target=_blank}|
|telephone|`optional`|String|Contact telephone number for this RWS, or the operator / owner's call centre. Please enter numbers using the format: +<country_code> <area_code> <local_number>. For example: `+44 123 456789`. For more information, please see [Open Street Map](https://wiki.openstreetmap.org/wiki/Key:phone){target=_blank}.|
|openingHours|`recommended`|String|Specifies opening hours of this RWS. Opening hours should be specified as a weekly time range, starting with days, then times per day. Multiple days can be listed with commas ',' separating each day. Day or time ranges are specified using a hyphen '-'. Days are specified using the following two-letter combinations: Mo, Tu, We, Th, Fr, Sa, Su. Times are specified using 24:00 format. For example, 3pm is specified as 15:00, 10am as 10:00. An example of this would be `Tu,We,Th 08:00-17:00`. Months can be specified using three-letter combinations: Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec. Separate months before days with a ':'. An example of this would be `Apr: 08:00-17:00`. Multiple entries should be separated by semi-colons. Winter and Summer hours can be specified as `Apr-Sep: Mo-Fr 08:00-17:00; Oct-Mar: Mo-Fr 09:00-16:00`. Specific days can also be specified following the same format as days. An example of this would be `Dec 24 10:00-12:00`. See [Open Street Map](https://wiki.openstreetmap.org/wiki/Key:opening%20hours?uselang=en-GB){target=_blank} for more information about date formats. While all the documentation from Open Street Map is compatible, please avoid using phrases such as but not limited to: `dawn, sunrise, dusk, sunset`.|
|openingHoursNotes|`recommended`|String|Can make notes about openingHours like: `Site may close at dusk if earlier`.|
|openingHoursTransportRestrictions|`required`|Boolean|Do openingHours differ based on transport type (e.g., pedestrian access, small or large vehicles)?|
|ownerID|`required`|String|An identifier from the local authorities controlled list|
|ownerName|`required`|String|The name of the owner of the RWS|
|operatorID|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier |
|operatorCompanyID|`recommended`|String|The UK Companies House identifier for this RWS's operator|
|operatorName|`required`|String|The name of the organisation responsible for operating the site|
|operatorAddressStreet|`recommended`|String|The street address of this RWS's operator|
|operatorAddressCity|`recommended`|String|The street address of this RWS's operator|
|operatorAddressCounty|`recommended`|String|The street address of this RWS's operator|
|operatorAddressCountry|`recommended`|String|The street address of this RWS's operator|
|operatorAddressPostcode|`recommended`|String|The postcode of this RWS's operator|
|dateOpened|`optional`|String|The date that this RWS opened. Supply in format YYYY-MM-DD. If day and month are not known, then just supplying the year will suffice|
|dateClosed|`optional`|String|The date that this RWS closed. Supply in format YYYY-MM-DD. If day and month are not known, then just supplying the year will suffice|
|areaServed|`recommended`|String|Either a semi-colon-separated list of local authorities identifiers, or a unique identifier of an area served provided in a separate csv, geoJSON or Shape file| 
|proofOfResidency|`recommended`|Boolean|Do household users of this site need to provide proof of residency to access the site?|
|accessibilityNotes|`recommended`|String|Details of any accessibility issues at the site - eg split-level access with stairs only|
|trade|`optional`|Boolean|Is this RWS accessible by tradespeople?|
|ANPR|`recommended`|Boolean|Is automatic number plate recognition in use at the site?|
|reuseShop|`recommended`|Boolean|Is there a reuse shop at this site?|
|dateUpdated|`required`|String|The date that this record was last updated. Supply in format YYYY-MM-DD|
|dateValidFrom|`required`|String|The date that this record is valid from. Supply in format YYYY-MM-DD|
|dateValidTo|`required`|String|The date that this record is valid to. Supply in format YYYY-MM-DD|

