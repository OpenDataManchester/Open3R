# HWRC Services Offered

Services offered should be provided as a separate csv file, in tidy format. This means that each row of the csv file should be one service offered by one HWRC. An example is provided.

The specification of this csv file is as follows:

hwrc_services.csv 

|Column|Status|Format|Notes|
|:-|:-|:-|:-|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|HWRC|`required`|String|The unique identifier of the HWRC that this row relates to. See the identifiers section for information about how to construct this identifier. There must be an equivalent record in the `HWRC_Main` data|
|material|`required`|String|The identifier of the material or item that this row relates to. The entry here should be drawn from the materials controlled list|
|processing|`required`|String|What the HWRC does to the material. Should be one of 're-use', 'recycle', or 'disposal'|
|charge|`required`|Boolean|Is there a cast for this service at this site?|
