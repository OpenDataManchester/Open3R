# Introduction

## What is an open data standard?

An open data standard is a set of rules that describe the structure and components of an open dataset. Putting rules in place means people and organisations that publish data about the same thing can use the same language to talk about it. Having a standard makes it a lot easier to understand and reuse data that has been published. It is especially useful if data is being published by lots of different people to make an even bigger dataset. Anyone can then read about the standard, contribute data, or use the data knowing everyone is talking about the same thing.

## What is the Open3R open data standard?

The Open3R open data standard describes information about the UK’s Household Waste Recycling Centres, and other places people can take waste from their home for recycling or reuse. It has been designed to provide guidance to local authorities (like local councils) for publishing data about these places. It includes data such as opening times, services offered and location of ‘bring-banks’. A data standard will make the available data better for users, because it means that different publishers, with different data capture or publishing systems, can publish data in the same format. If every local authority publishes its data in this way, then it is theoretically possible to have a dataset that covers the whole of the UK. This could then be used to power a ‘Where’s My Nearest Recycling Centre’ app, or support ‘time-to-travel’ analyses of local recycling centres.

The standard is being developed according to the [OpenStand](https://open-stand.org/){target=_blank} principles of:

* Due process
* Broad consensus
* Transparency
* Balance
* Openness

## How is the standard being developed?

The initial standard development was funded by the [Open Data Institute](https://www.opendatamanchester.org.uk/odistimulus-environment/){target=_blank}, with the later stages supported by [Innovate UK](https://www.opendatamanchester.org.uk/plastics-packaging-portal/){target=_blank}, and is being developed through workshops with industry experts over a number of iterations.

## How to use the standard

The documentation here details how to *publish* data to the standard, and how to use data that has been published to the standard. At a high level, the publishing flow is as follows:

1. Someone at a local authority decides they want to publish HWRC data to the standard
2. They populate the csv [template](https://github.com/OpenDataManchester/Open3R/blob/V2/docs/8_Supporting_Files/8_1_1_RWS_Main_Template.csv){target=_blank} (or prepare one from scratch using the specified column names)
3. They create a csv file or spatial file of local areas served by each HWRC, then:
    1. They publish the csv file(s) and/or spatial files on their website OR
    2. They send the data to the custodian of the standard for publishing
4. Let the custodian of the standard know that there is new data

These steps must be repeated whenever there is a change to the data.
