# Sceloporus_2021_acute_changes

This repository houses all data and code associated with the publication "Cutaneous evaporative water loss in lizards changes immediately with temperature", published in _ by Calvin Davis, Savannah Weaver, and Emily Taylor. The study investigates the instantaneous change in cutaneous evaporative water loss (CEWL) in response to temperature changes in Western Fence Lizards (*Sceloporus occidentalis*).


## Data

The **"Data" folder** includes the following:

- "AquaFlux data" subfolder = includes one file of time series CEWL data for each lizard.
- "AquaFlux start times.csv" = when each Aquaflux data collection period began for each lizard.
- "CEWL_time_series.RDS" = formatted CEWL time series data, created in "data_wrangling.Rmd".
- "Collection Data.csv" = basic lizard capture and measurement information (date, time of capture, transport sock ID, assigned individual lizard ID, assigned temperature treatment, mass (g), SVL (mm), incubation times, thermocouple assignment, additional notes), explained in "data_wrangling.Rmd".
- "collection_dat_formatted.csv" = a formatted version of "Collection Data.csv", created in "data_wrangling.Rmd".
- "dead lizards" subfolder = 
  - "R format" subfolder = includes one file of time series CEWL data for each dead lizard doing each temperature treatment.
  - "TC" subfolder = thermocouple recordings and calibration data for the dead lizards.
- "exp design.csv" = artificial values used to show the desired effect of experimental treatment steps, not data from a scientific study.
- "HOBO data" subfolder = data collected by each HOBO External Temperature/RH Sensor Data Loggers for all five capture days: two HOBOs per cold chamber, two per hot chamber, and one for the control area.
- "HOBO_assignments.csv" = notes on which HOBOs were recording which treatment on a given date.
- "TC calibration" subfolder = temperature recordings used to calibrate thermocouples against a reference thermometer.
- "temp_time_series.RDS" = formatted temperature time series data, created in "data_wrangling.Rmd".
- "Thermocouple Data" subfolder = lizard body temperature recordings for each date.
- "Weather Data" subfolder = contains weather data corresponding to each of the five different capture and measurement days of the study (California Polytechnic State University Irrigation Training and Research Center).


## Code

See .Rmd files for source code, and .html files for a step-by-step explanation in a cleaner format.

**"data_analysis"** includes model building/selection and figure creation. 

**"data_wrangling"** loads in all the data, removes errors, properly formats everything, exports cleaner dataframes for use in "data_analysis", and calculates some summary statistics. 

**"dead_lizards"** has all summary statistics and figures for the dead lizards opportunistically studied.

**"HOBO_stats"** loads in all the HOBO logger data, selects the data collected during the study, and calculates summary statistics.


## Results

All figures created for publication can be found in the "Results_Figures" subfolder and all the model results presented can be found in the "Results_Statistics" subfolder.
