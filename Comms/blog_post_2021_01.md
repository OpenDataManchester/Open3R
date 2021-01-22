
![](https://github.com/northernjamie/hwrc_data_standard/blob/main/Comms/images/scrapyard.jpg)

Image by [vkingxl](https://pixabay.com/users/vkingxl-4313077/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2441432) from [Pixabay](https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2441432)

# Household waste recycling centre data standard

I've ben working with waste-related data and organisations on and off for over 10 years now, and the people in this ecosystem are amongst the most knowledgable and passionate people I've ever worked with. Waste and recycling is a hugely important area of work, and has many facets, from waste crime, to environmental impact. These two factors mean that when I was given the chance to work on a data standard with [Open Data Manchester](https://www.opendatamanchester.org.uk/) and Dsposal for household waste recycling centres (HWRCs), I jumped at it. I've worked with [Dsposal](https://dsposal.uk/) previously, on the Defra-funded [KnoWaste data standard](https://github.com/OpenDataManchester/KnoWaste), so this was a great opportunity to get the band back together.

## What's the current situation?

Household waste recycling centres have lots of different names. HWRCs, household waste sorting sites, re-use and recycling centres, the dump, the tip, etc. Local authorities publish details about these HWRCs, usually on their websites, but there is no standard for publishing this information, leading to potential inequalities in access to information, and therefore access to waste and recycling services for people living in different parts of the UK.  

HWRCs are typically 'owned' by a local authority - the organisation with legal responsibility for providing waste services to its residents. Local authorities will often have multiple HWRCs in the local authority area, each providing different services. HWRCs also have an operator - this could be the local authority, or it could be another local authority, a collection of local authorities, or a private company.

In most cases, residents are only permitted to dispose of waste at HWRCs in the local authority in which they live. There are, however, some exceptions to this.

## What's the problem we're trying to solve?

The main problems that we are trying to solve with this data standard is one of information inequality. By developing a standard for publishing this data, we are providing local authorities with a prescriptive set of data to publish about their HWRCs. If the standard is adopted by local authorities, then residents across the UK will have access to the same information about HWRCs in their area.

Another problem that would be solved by this approach is that it will be possible to aggregate data from different local authorities. This would provide different views for the data, allowing exploration of  HWRC data on a regional level, for example, or by services offered. This would support streategic planning, and the potential for cross-referenign provision data with recycling rates, for example.

Having the data in this format would also make it easier to be consumed by other infomediaries - such as Google, or OpenStreetMap. This has the potential to make the information even more widely available.

## How are we trying to solve it?

Our approach to this has been to develop a data standard, aiming to strike a balance between ease of use for publishers, and usefulness for users. To do this, we've carried out some desktop research based on other standards in place, and held a series of six workshops with professionals from across the sector. This has allowed us to design a proposed workflow, a set of fields to be collected, structure of the data, and controlled lists, and the format of the data to be published.

We will be holding another set of workshops week beginning the 25th January 2021 to proesent the progress, and check that the things we've put in place so far make sense.

We are also developing this standard in the open - the details of the standard are being made available in this Github repo.

## What have been the challenges so far?

One of the potential problems with developing a standard like this is the potential lack of engagement from the community that we'd hope would use the standard, but this hasn't been the case here - people have been very generous with their time and expertise. 

Of the challenges we've faced, the main ones have been around technical decisions around the best way to model certain elements of the standard. Particularly challenging are the topics of how to capture the materials that are handled by each HWRC, as there are so many (one professional said "it is impossible to state everything that could be accepted"). The other challenge has been around the best way to capture the area served by a particular HWRC - by not making the publishing process too onerous for those HWRCs with simple boundaries (eg a single local authority), but able to capture those cases where boundaries are more complex.

## How can you get involved?

THe more eyes on a data standard the better. There are three workshops next week, and if you are reading this on the day it was published, then it's not too late to register. ALternatively, keep an eye on the [Github repo](https://github.com/northernjamie/hwrc_data_standard), and also the [YourDsposal website](https://dsposal.uk/) for information on the standard as it develops further. 



