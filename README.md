# Supporting data and analysis code for the manuscript:

> Evaluation of modified autocidal gravid ovitraps for the control of container-breeding mosquitoes in Saint Augustine, FL

[Rendered R makrdown document of statistical analysis is here](https://usda-ars-gbru.github.io/dixon_etal_2021/glm-tests.html)

[![DOI](https://zenodo.org/badge/322486553.svg)](https://zenodo.org/badge/latestdoi/322486553)

## Authors

Author | Affiliation
---|---
Daniel Dixon | United States Department of Agriculture, ARS, CMAVE, Gainesville, FL USA
Christopher S. Bibbs | Central Life Sciences, Dallas, TX, USA
Dena L. Autry | Anastasia Mosquito Control District of Saint Johns County, Saint Augustine, FL, USA
Michael Banfield | BanfieldBio Inc., Woodinville, WA, USA
Rui-De Xue | Central Life Sciences, Dallas, TX, USA
Adam Rivers | United States Department of Agriculture, ARS, GBRU, Gainesville, FL USA

## Experimental overview

The goal of the study was to evaluate the effectiveness of modified autocidal gravid ovitraps on mosquito populations in one city.  Three sections of the city of Saint Augustine Florida were chosen and termed North, Downtown and South. each section was divided into treatment and control groups.

Three types of traps were used in the study:

* AGO - Autocidal Gravid Traps, the traps being tested
* SAGO - Sentinal Autocidal Gravid Traps, The same as the AGO traps but placed in the treatment and control sites for monitoring
* BG traps - A different type of traps placed in the treatment and control location for monitoring


Monitoring traps were placed for 4 weeks prior to the start of the study then the AGO traps were placed and monitored for 20 weeks. animals in traps were collected, identified and counted weekly.

## Repository files

* README.md - this file
* all_data_long.csv.gz - a gzipped csv file containing the count and metadata from the experiment.
* glm-tests.Rmd - an R markdown document with the statistical analysis and
  figure creation code for figures 3 and 4
* docs/ a file containing rendered R markdown

## Data description

Field | Data type | Description
---|---|---
trap_id | int | ID number of specific trap
location_id | int | ID number of specific site
trap_type | factor | the type of monitoring trap
site_pair | factor | site [ north, south, downtown]
treatment_type | factor | control or treatment
trap.density | float | traps per unit area
address | chr | Street address
city | chr | city
state | chr | State
lat | float | latitude in decimal degrees
lon | float |  longitude in decimal degrees
sample_id | int | the specific sample id for contents removed from a trap at a specific time
datetime | datetime | date time of collection (accurate to the day)
organism | factor | The organism/sex category
count | int | the count of organisms

Total records: 37,152
Complete records (No NA's): 36,542
