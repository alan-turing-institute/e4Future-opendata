# e4Future-opendata

This repository contains Jupyter notebooks to process three open source datasets for either electric vehicle (EV) charging data or photovoltaic (PV) data:
1. [Caltech ACN](https://ev.caltech.edu/dataset): EV data 
2. [WPD Electric Nation](https://www.westernpower.co.uk/electric-nation-data): EV data
3. [PVOutput](https://pvoutput.org): PV data

There is a separate folder for each of these datasets with the relevant Jupyter notebooks and more details about the data and how to run the notebooks.
The Jupyter notebooks process the data (charging power for EV data and power output of the PV system for PVOutput) and resample it by averaging the data over the resampling interval. 
The notebooks have a parameter to control the time resolution for the resampling.

The output files all follow the same format: 

- The first column contains the timestamps over a 24h period. 
- Each of the following column contains an individual profile (charging or PV output) for one day.
- The profiles are for all datasets are power in kW.

