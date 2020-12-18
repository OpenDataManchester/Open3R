# Identifiers

Identifiers are the way that humans and machines can know that a particular thing is definitely that thing. In the context of HWRCs, there are difference ways of talking about various things. A member of the public may refer to a particular HWRC as 'Carrington tip', but a local authority waste officer may know it as 'Woodhouse Lane Recycling Centre'. In a database it may be recorded as 'Woodhouse Ln Rec Ctre'. While these all talk about the same thing, it could be hard for a human to know that they are the same, and pretty much impossible for a computer. 

To help get around this, we use identifiers. These are codes that we use to unambiguously reference a particular thing in our database. These identifiers must be unique, and to make sure of this, there are a few tricks we can use when deciding on an identifier. The main one is, wherever possible, to use an identifier from another source. An example of this would be for operators of HWRCs, who are companies, and therefore have entries in the Companies House database. By using the Companies House identifier for these operators, we can be certain the code is unique, and we know that we can join together different local authorities datasets to analyse which companies operate sites across the country. A bonus here is that usine the Companies House ID means an analyst can access additional information about the operator using the Companies House API, such as the date that the company was incorporated, or its filing history.

Some identifiers are linked to the controlled lists, and again these can used to look up additional information about a thing - Local Authorities being one example.

These are the identifiers that are proposed for this standard

## HWRC Identifier

Each HWRC needs a unique identifier, and this should be created by the publishing organisation. Usually, publishing organisations will already have identifiers for the HWRCs for which it is responsible. These are likely to be in use in CRm systems, waste management systems, or other databases. Although these identifiers are likely to be unique within the publishing organisation, there is a risk that two publishing organisations may use the same identifier for two different HWRCs. To avoid this issue, the identifier is prefixed with the publishing organisation's unique identifier. 

1. Each identifier should be prfixe