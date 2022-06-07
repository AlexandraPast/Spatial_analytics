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
