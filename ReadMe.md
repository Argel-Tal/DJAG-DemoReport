# AO7 Principal Data Analyst Interview Practical 

## Purpose: Demonstrate the ability to produce data visualisations and commentary around a selected crime trend, based on QPS data
Selected analysis is the impact of the Queensland COVID-19 travel restrictions on "Other Theft", aka Theft without threat or use of violence.

Connects directly to data downloaded from QPS's [interactive data visualisation tool](https://mypolice.qld.gov.au/queensland-crime-statistics), as [data.qld.gov](https://www.data.qld.gov.au/dataset?q=crime%20statistics&sort=score%20desc%2C%20metadata_modified%20desc) does not have corresponding regional crime data 2024. 

## Datasets
### Queensland Police Service (QPS)
1. Queensland Crime Statistics - Advanced
    Link: https://mypolice.qld.gov.au/queensland-crime-statistics/
    Filters:
    - Offence type: `Other Theft (excl. Unlawful Entry)`
    - Date range: `[2019-11-01, 2024-09-30]`
2. QPS Regions: Geographic data
    Link: https://www.data.qld.gov.au/dataset/qps-regions
    Filters: None
### PowerBI
- Calendar

## Measures and Calculations
Measure   | Defintion
----------|---------------
Change    | Post COVID volume - Pre-COVID restriction volume <br> `Offences(Aug24) - Offences(Jan2020)`
Offences  | Sum of offence count, by region by month
Last refreshed  | Last time PowerBI checked for new data
Latest data | Date of most recent data point

<div style="page-break-after: always;"></div>

## Pages
Index | Display | Configuration
-------|--------|--------------
Interface | <img src="./ReadMeImgs/Landing.png" width="350" title = "Landing Page"> | <img src="./ReadMeImgs/QueryWeb.png" width="350" title = "Web Interface">
Data Model | <img src="./ReadMeImgs/QueryStructure.png" width="350" title = "PBI Queries"> | <img src="./ReadMeImgs/Schema.png" width="350" title = "Schema">

## Tools:
- [Filled Shape tutorial PowerBI](https://servian.dev/power-bi-custom-maps-part-ii-shape-map-939873da3f66)
- [GeoJSON tool](https://mapshaper.org/)