# Spatial analytics final project - data

#### This repository consists of folders:
- **maps**: contains all the maps created in my script Special_schools.Rmd
- **raster_data**: isochrones converted into raster layers representing accessibility surfaces
- **results**: 
  - munic_walk: data frame with calculated area which does not fall within 5km distance from special school for each municipality
     - includes columns: `municipality`, `total area` (total area of the municipality), `out_reach` (area in m^2 not coevered by isochrones), `out_reach_perc` (percentage)
  - munic_drive: data frame with calculated area which does not fall within 30-minute driving time from special school for each municipality
     - includes columns: `municipality`, `total area` (total area of the municipality), `out_reach` (area in m^2 not coevered by isochrones), `out_reach_perc` (percentage)
- **w_data**: contains all isos files and pre-processed data: schools_new_cl.csv, student_count_cl.csv
- `schools_new.csv`: original file downloaded from [here](https://statistik.uni-c.dk/instregudtraek/) made by Uddannelssesstatistik, Børne– og Undervisningsministeriet.
- `student_count_FULL.xlsx`: original file downloaded [from here](https://uddannelsesstatistik.dk/Pages/Reports/1950.aspx) made by Uddannelssesstatistik, Børne– og Undervisningsministeriet.
- `student_count.csv`: one extracted sheet from student_count_FULL.xlsx, saved as a .csv

## How I accessed the school list data:
The data is available as a csv file of schools, their name with their respective address and latitude and longitude coordinates. Upon navigating to the [Udtræk fra Institutionsregisteret](https://statistik.uni-c.dk/instregudtraek/), a user can select different filters to extract lists of institutions.
Upon selecting the following criteria: 
“Institutionstype: Specialskoler for børn”; 
“Kommune/Region: Vælg alle”
you should be able to download the .csv file.

## How I accessed the student data:
On the front page of https://uddannelsesstatistik.dk I navigated to “Grundskole”, selected “Elevtal, inklusion og sprogprøver”
 in the new menu a scrolled down to the option [“Inklusion og specialundervisning”](https://uddannelsesstatistik.dk/Pages/Reports/1950.aspx).

Data is an excel table from the webpage Uddannelsesstatistik with a number of sheets providing different information regarding children with special needs in relation to schools. I opened the data using Microsoft Excel and extracted the sheet “Specialundervisning, kommuner” representing the total numbers of children visiting special schools in each municipality. 
Uddannelsesstatistik provides additional information about the dataset [here](https://uddannelsesstatistik.dk/Documents/Grundskole/datadokumentation/DVH_Grundskole_Elevtal.pdf)
