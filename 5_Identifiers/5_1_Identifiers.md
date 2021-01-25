# Identifiers

Identifiers are the way that humans and machines can know that a particular thing is definitely that thing. In the context of HWRCs, there are difference ways of talking about various things. A member of the public may refer to a particular HWRC as 'Carrington tip', but a local authority waste officer may know it as 'Woodhouse Lane Recycling Centre'. In a database it may be recorded as 'Woodhouse Ln Rec Ctre'. While these all talk about the same thing, it could be hard for a human to know that they are the same, and pretty much impossible for a computer. 

To help get around this, we use identifiers. These are codes that we use to unambiguously reference a particular thing in our database. These identifiers must be unique, and to make sure of this, there are a few tricks we can use when deciding on an identifier. The main one is, wherever possible, to use an identifier from another source. An example of this would be for operators of HWRCs, who are companies, and therefore have entries in the Companies House database. By using the Companies House identifier for these operators, we can be certain the code is unique, and we know that we can join together different local authorities datasets to analyse which companies operate sites across the country. A bonus here is that usine the Companies House ID means an analyst can access additional information about the operator using the Companies House API, such as the date that the company was incorporated, or its filing history.

Some identifiers are linked to the controlled lists, and again these can used to look up additional information about a thing - Local Authorities being one example.

These are the identifiers that are proposed for this standard

## HWRC Identifier

Each HWRC needs a unique identifier, and this should be created by the publishing organisation. Usually, publishing organisations will already have identifiers for the HWRCs for which it is responsible. These are likely to be in use in CRM systems, waste management systems, or other databases. Although these identifiers are likely to be unique within the publishing organisation, there is a risk that two publishing organisations may use the same identifier for two different HWRCs. To avoid this issue, the identifier is prefixed with the publishing organisation's unique identifier. To construct the HWRC identifier follow these steps:

1. Start with the text `hwrc-`. This means the identifier relates to HWRCs

2. Add the three letter code of the country that the owner is in:
	* England: `eng-`
	* Scotland: `sct-`
	* Wales: `pla-`
	* Northern Ireland: `nir-`

3. Add the three letter code for the owner from one of the registers listed below (with a hyphen):

	* [England](https://local-authority-eng.register.gov.uk/records?page-index=1&page-size=5000)
	* [Scotland](https://local-authority-sct.register.gov.uk/records?page-index=1&page-size=5000)
	* [Wales](https://principal-local-authority.register.gov.uk/records)
	* [Northern Ireland](https://www.registers.service.gov.uk/registers/local-authority-nir)

4. Add your organisation's unique identifier for the HWRC

As an example, if Trafford local authority has the unique identifier `1234` for Woodhouse Lane Recycling Centre, then the unique identifier for that site in this standard would be `hwrc-eng-trf-1234`

## Local Authority Identifiers

Use the following sites to obtain your three-letter local authority identifier:

	* [England](https://local-authority-eng.register.gov.uk/records?page-index=1&page-size=5000)
	* [Scotland](https://local-authority-sct.register.gov.uk/records?page-index=1&page-size=5000)
	* [Wales](https://principal-local-authority.register.gov.uk/records)
	* [Northern Ireland](https://www.registers.service.gov.uk/registers/local-authority-nir)

To avoid duplicates, prefix your local authority identifier with the three letter country code:

	* England: `eng-`
	* Scotland: `sct-`
	* Wales: `pla-`
	* Northern Ireland: `nir-`

For example, the code for Trafford would be `eng-trf`

## Area Served

When providing separate information about the area served by a HWRC, the identifier should be constructed in the following way:

1. Start with the prefix `hwrc-area`
 
2. Add the three letter code of the country that the owner is in:
	* England: `eng-`
	* Scotland: `sct-`
	* Wales: `pla-`
	* Northern Ireland: `nir-`

3. Add the three letter code for the owner from one of the registers listed below (with a hyphen):

	* [England](https://local-authority-eng.register.gov.uk/records?page-index=1&page-size=5000)
	* [Scotland](https://local-authority-sct.register.gov.uk/records?page-index=1&page-size=5000)
	* [Wales](https://principal-local-authority.register.gov.uk/records)
	* [Northern Ireland](https://www.registers.service.gov.uk/registers/local-authority-nir)

4. Add a unique code to differentiate this area from others that your organisation might publish

As an example, if Trafford published data about the area served by Woodhouse Lane Recycling Centre, they would use the identifier `hwrc-area-eng-trf-a001`

## Operator identifiers

Using commom identifiers for HWRC operators will enable analysis of aggregated data, such counting sites by operator across the country. Where the operator is a limited company, then the Companies House identifier should be used.

[Should we have Dsposal create a curated list of operators - eg Greater Manchester Combined Authority]










