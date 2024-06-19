# New Hampshire Election Shapefile

This shapefile was processed by Professor Ellen Veomett and her student Ananya Agarwal.

# **Sources**
@author: eveomett AI for Redistricting, USF All data retrieved 06/09/24:

Obtain the following data from Restricting Data Hub

[Population data](https://redistrictingdatahub.org/dataset/new-hampshire-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2022-new-hampshire-congressional-districts-plan-approved/): 2021 New Hampshire Congressional Districts plan enacted on 1/13/22

[State House District data](https://redistrictingdatahub.org/dataset/2022-new-hampshire-state-house-of-representatives-approved-plan/): 2022 State House Approved Plan

[State Senate District data](https://redistrictingdatahub.org/dataset/2022-new-hampshire-state-senate-approved-plan/): 2022 State Senate Approved Plan

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-new-hampshire-precinct-and-election-results/)**:**  VEST 2020 New Hampshire precinct and election results

[2018 election data](https://redistrictingdatahub.org/dataset/vest-2018-new-hampshire-precinct-and-election-results/)**:**  VEST 2018 New Hampshire precinct and election results

[2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-new-hampshire-precinct-and-election-results/)**:**  VEST 2016 New Hampshire precinct and election results

# **Processing**

Demographic data were aggregated from the census block level and precincts were assigned to districts using [MGGG's proration software](https://github.com/mggg/maup). Election data were also prorated onto VTDs from the original precinct shapefile using the `maup` package.

## Metadata
* `STATE`: State
* `STATEFP`: State FIPS code
* `COUNTY`: County name
* `COUNTYFP`: County FIPS code
* `Precinct`: Precinct name
* `PRES12D`: Number of votes for 2012 Democratic presidential candidate
* `PRES12R`: Number of votes for 2012 Republican presidential candidate
* `GOV12D`: Number of votes for 2012 Democratic gubernatorial candidate
* `GOV12R`: Number of votes for 2012 Republican gubernatorial candidate
*	`USH12D`: Number of votes for 2012 Democratic US House candidate
*	`USH12R`: Number of votes for 2012 Republican US House candidate
* `EC12D`: Number of votes for 2012 Democratic executive council candidate
* `EC12R`: Number of votes for 2012 Republican executive council candidate
* `GOV14D`: Number of votes for 2014 Democratic gubernatorial candidate
* `GOV14R`: Number of votes for 2014 Republican gubernatorial candidate
* `SSEN14D`: Number of votes for 2014 Democratic state senate candidate
*	`SSEN14R`: Number of votes for 2014 Republican state senate candidate
* `EC14D`: Number of votes for 2014 Democratic executive council candidate
* `EC14R`: Number of votes for 2014 Republican executive council candidate
*	`PRES16D`: Number of votes for 2016 Democratic presidential candidate
*	`PRES16R`: Number of votes for 2016 Republican presidential candidate
* `GOV16D`: Number of votes for 2016 Democratic gubernatorial candidate
* `GOV16R`: Number of votes for 2016 Republican gubernatorial candidate
*	`SEN16D`: Number of votes for 2016 Democratic senate candidate
*	`SEN16R`: Number of votes for 2016 Republican senate candidate
*	`USH16D`: Number of votes for 2016 Democratic US House candidate
*	`USH16R`: Number of votes for 2016 Republican US House candidate
* `SSEN16D`: Number of votes for 2016 Democratic state senate candidate
*	`SSEN16R`: Number of votes for 2016 Republican state senate candidate
* `GOV18D`: Number of votes for 2018 Democratic gubernatorial candidate
* `GOV18R`: Number of votes for 2018 Republican gubernatorial candidate
* `EC20D`: Number of votes for 2020 Democratic executive council candidate
* `EC20R`: Number of votes for 2020 Republican executive council candidate
* `GOV20D`: Number of votes for 2020 Democratic gubernatorial candidate
* `GOV20R`: Number of votes for 2020 Republican gubernatorial candidate
* `PRES20D`: Number of votes for 2020 Democratic presidential candidate
*	`PRES20R`: Number of votes for 2020 Republican presidential candidate
*	`SEN20D`: Number of votes for 2020 Democratic senate candidate
*	`SEN20R`: Number of votes for 2020 Republican senate candidate
*	`USH20D`: Number of votes for 2020 Democratic US House candidate
*	`USH20R`: Number of votes for 2020 Republican US House candidate
* `SSEN20D`: Number of votes for 2020 Democratic state senate candidate
*	`SSEN20R`: Number of votes for 2020 Republican state senate candidate
* `TOTPOP`: Total population from 2010 Decennial Census
* `NH_WHITE`: White, non-hispanic, population from 2010 Decennial Census
* `NH_BLACK`: Black, non-hispanic, population from 2010 Decennial Census
* `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population from 2010 Decennial Census
* `NH_ASIAN`: Asian, non-hispanic, population from 2010 Decennial Census
* `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population from 2010 Decennial Census
* `NH_OTHER`: Other race, non-hispanic, population from 2010 Decennial Census
* `NH_2MORE`: Two or more races, non-hispanic, population from 2010 Decennial Census
* `HISP`: Hispanic population from 2010 Decennial Census
* `H_WHITE`: White, hispanic, population from 2010 Decennial Census
* `H_BLACK`: Black, hispanic, population from 2010 Decennial Census
* `H_AMIN`: American Indian and Alaska Native, hispanic, population from 2010 Decennial Census
* `H_ASIAN`: Asian, hispanic, population from 2010 Decennial Census
* `H_NHPI`: Native Hawaiian and Pacific Islander, hispanic, population from 2010 Decennial Census
* `H_OTHER`: Other race, hispanic, population from 2010 Decennial Census
* `H_2MORE`: Two or more races, hispanic, population from 2010 Decennial Census
* `VAP`: Total voting age population from 2010 Decennial Census
* `HVAP`: Hispanic voting age population from 2010 Decennial Census
* `WVAP`: White, non-hispanic, voting age population from 2010 Decennial Census
* `BVAP`: Black, non-hispanic, voting age population from 2010 Decennial Census
* `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population from 2010 Decennial Census
* `ASIANVAP`: Asian, non-hispanic, voting age population from 2010 Decennial Census
* `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population from 2010 Decennial Census
* `OTHERVAP`: Other race, non-hispanic, voting age population from 2010 Decennial Census
* `2MOREVAP`: Two or more races, non-hispanic, voting age population from 2010 Decennial Census
* `CD`: Congressional district
* `HDIST`: State House district
* `SEND`: State Senate district

## Projection
This shapefile uses a UTM projection centered on New Hampshire (ESPG: 3437).