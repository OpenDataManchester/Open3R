# RWS Services Offered

Services offered should be provided as a separate csv file, in tidy format. This means that each row of the csv file should be one service offered by one RWS. An example is provided.

The specification of this csv file is as follows:

[rws_services.csv](https://github.com/OpenDataManchester/Open3R/blob/V2/docs/8_Supporting_Files/8_1_3_RWS_Services_Template.csv){target=_blank}

|Column|Status|Format|Notes|
|:-|:-|:-|:-|
|identifier|`required`|String|A globally unique identifier. See identifiers section for information on how to construct this identifier|
|RWS|`required`|String|The unique identifier of the RWS that this row relates to. See the identifiers section for information about how to construct this identifier. There must be an equivalent record in the `RWS_Main` data|
|material|`required`|String|The identifier of the material or item that this row relates to. The entry here should be drawn from the materials controlled list|
|processing|`required`|String|What the RWS does to the material. Should be one of 're-use', 'recycle', or 'disposal'|
|charge|`required`|Boolean|Is there a cost for this service at this site?|
