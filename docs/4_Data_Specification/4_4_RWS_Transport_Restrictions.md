# HWRC Transport Restrictions

Transport Restrictions should be provided as a separate csv file, in tidy format. This means that each row of the csv file should be one service offered by one RWS. An example is provided.

The specification of this csv file is as follows:

RWS_transportRestrictions.csv 

|Column|Status|Format|Notes|
|:-|:-|:-|:-|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|RWS|`required`|String|The unique identifier of the RWS that this row relates to. See the identifiers section for information about how to construct this identifier. There must be an equivalent record in the `RWS_Main` data|
|transportType|`required`|String|The identifier of the transport type that this row relates to. The entry here should be drawn from the transport types controlled list|
|accessAllowed|`required`|Boolean|Does the RWS allow access to this type of transport?|
|openingHours|`recommended`|String|Specifies opening hours of the type of transport at this RWS. Opening hours should be specified as a weekly time range, starting with days, then times per day. Multiple days can be listed with commas ',' separating each day. Day or time ranges are specified using a hyphen '-'. Days are specified using the following two-letter combinations: Mo, Tu, We, Th, Fr, Sa, Su. Times are specified using 24:00 format. For example, 3pm is specified as 15:00, 10am as 10:00. An example of this would be `Tu,We,Th 08:00-17:00`. Months can be specified using three-letter combinations: Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec. Separate months before days with a ':'. An example of this would be `Apr: 08:00-17:00`. Multiple entries should be separated by semi-colons. Winter and Summer hours can be specified as `Apr-Sep: Mo-Fr 08:00-17:00; Oct-Mar: Mo-Fr 09:00-16:00`. Specific days can also be specified following the same format as days. An example of this would be `Dec 24 10:00-12:00`. See [Open Street Map](https://wiki.openstreetmap.org/wiki/Key:opening%20hours?uselang=en-GB) for more information about date formats. While all the documentation from Open Street Map is compatible, please avoid using phrases such as but not limited to: `dawn, sunrise, dusk, sunset`.|
|permitRequired|`recommended`|Boolean|Do users need to have a permit to access this RWS using this type of transport?|
|bookingRequired|`recommended`|Boolean|Do users need to book a slot prior to visiting the site for this type of transport?|
|bookingURL|`recommended`|String|The link for booking a slot to visit the site. Links can be provided if a booking system is in place but is not required.|
|maxHeight|`recommended`|String|The maximum height permissable to enter the RWS with this type of transport. Numbers should be entered with a decimal place and the unit should be specified using metres (m). For example: `2.0 m`.|
|maxLength|`recommended`|String|The maximum length permissable to enter the RWS with this type of transport. Numbers should be entered with a decimal place and the unit should be specified using metres (m). For example: `2.0 m`.|
|maxWidth|`recommended`|String|The maximum width permissable to enter the RWS with this type of transport. Numbers should be entered with a decimal place and the unit should be specified using metres (m). For example: `2.0 m`.|
|maxWeight|`recommended`|String|The maximum weight permissable to enter the RWS with this type of transport. Numbers should be entered with a decimal place and the unit should be specified using tonnes (t). For example: `3.0 t`.|
|trailerCombinedWith|`required`|String|The type of transport that can be used with the trailer. The entry here should be drawn from the transport types controlled list.|
|dateUpdated|`required`|String|The date that this record was last updated. Supply in format YYYY-MM-DD|