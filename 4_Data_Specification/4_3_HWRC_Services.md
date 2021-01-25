# HWRC Services Offered

Services offered should be provided as a separate csv file, in tidy format. This means that each row of the csv file should be one service offered by one HWRC. 

The specification of this csv file isas follows:

hwrc_services.csv 

|Column|Status|Format|Notes|
|:-|:-|:-|:-|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|HWRC|`required`|String|The unique identifier of the HWRC that this row relates to|
|material|`required`|String|The material or item that this row relates to. The entry here should be drawn from the materials controlled list|
|treatment|`required`|String|What the HWRC does to the material. Should be one of 're-use', 'recycle', or 'disposal'|