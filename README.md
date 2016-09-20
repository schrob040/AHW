# AHW
The scripts and raw data used to compare atmospheric and marine heat waves and cold-spells along the coast of South Africa.

## File description
* The text of the paper may be found in "..."
* The code used to prepare the raw data for use in the analysis may be found in "load/load.SACTN.R" and "load/load.SAWS.R"
* The code used to create the site list/ meta-data for the two datasets may be found in "load/load.SACTN.R" and "prep/SACTN.sitelist.R"
* The code used to calculate indices of comparison between the datasets may be found in "SAWS.SACTN.compare.R"
* The code used to perform the extreme event analyses may be found in "proc/SACTN.RMarineHeatweaves.R" and "proc/SAWS.RMarineHeatweaves.R"
* The code used to calculate the rates of co-occurrence may be found in "proc/cooccurrence.R"
* The code used to create the figures seen in the paper may be found in "graph/..."
* The code used to create the tables seen in the paper may be found in "..."
* The "/data" folder contains the raw data used in the analyses as well as the output from the "prep/..." and "proc/..." scripts
* The "/func" folder contains custom made functions used in the analyses
* The "/graph" folder contains the files necessary to create maps, as well as the output of the "graph/..." scripts
* The "/setupParams" folder contains the site lists, comparison indices and a custom ggplot2 theme
* The "/LaTeX" folder contains the files used to compile "/LaTeX/...", the body of the text
* The python folder contains everything required to run the "ehfheatwaves.py" script
* All folders labeled "/old/" contain scripts and data from previous versions of the analysis/ methodology

## 2016/09/18
* All for loops removed from extreme event calculation work flow
* A for loop is still used to "grow" the SAWS data, allowing for it to be compared against each SACTN time series
* All possible extreme events combinations etc. have been calculated as per current agreement on methodology

## 2016/09/19
* All for loops removed from the co-occurrence calculations
* Co-occurrence calculated for all combinations of SACTN and SAWS sites inlcuding tmean, tmin and tmax

## 2016/09/20
* Corrected error in calculation of co-occurrence proportions