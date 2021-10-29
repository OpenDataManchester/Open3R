# Controlled Lists

Controlled lists are possible options in certain fields of the dataset. These are items that are maintained by a custodian of the data, and may be a list of local authorities, the services that are offered by HWRCs, or even days of the week.

It is important that these controlled lists are adhered to. Software developers building applications or services around this standard, will rely on these options. Some software developers at the publishing end may introduce validation of the data to ensure compliance with these controlled lists. 

The controlled lists in use in the standard are:

* Local Authorities
* HWRC Area Served
* Services
* Processing
* Countries
* Transport Types

## 1. Local Authorities

Each HWRC is effectively owned by a local authority. The local authority list should be drawn from the list of Local Authorites in the UK, provided in the controlled lists section of this documentation.


## 2. HWRC Area Served

Each HWRC has an area that it serves. This means that only people who live in the specified area can use the HWRC. Many of these areas are aligned with Local Authority boundaries, but some are more complex than that. Information about areas served will need to be published as a separate file. This can be either as a CSV file, or a spatial file, such as geojson.

## 3. Services

This list is a list of materials accepted by the HWRC. This list is quite high-level, to accommodate the nuances of waste management. This will allow residents to make informaed choices about where they take their waste.

## 4. Processing

This list provides the different treatment options for materials.

## 5. Countries

This open data standard currently covers the 4 nations of the United Kingdom - England, Scotland, Northern Ireland, and Wales. See the identifiers section for guidance.

## 6. Transport Types

This list provides 4 different transport types: small vehicle, large vehicle, small trailer, large trailer, pedestrian.


