# Processing the EV data from the Electric Nation project

This folder contains a Jupyter notebook which explores the openly accessible data from the WPD Electric Nation project.

 ## Data Sources

### Electric Nation
The [WPD Electric Nation project](https://www.westernpower.co.uk/electric-nation-data) was a large home smart charging trial over 18 months with almost 700 EV owner taking part. There were two providers which managed the chargers: CrowdCharge and Greenflux. The data of the two providers slightly differ from each other. Hence, there are separate notebooks for each providers. 

For CrowdCharge, there are two notebooks: 

-  `EV_crowdCharge_separate_data_by_charger.ipynb` separates the data in the file _CrowdChargeMeterValues.csv_ according to the charger type (3.6 or 7 kW)
-  `create_crowdCharge_profiles.ipynb` resamples the charging current timeseries and converts it into power (kW). 
  
For Greenflux, there are also two notebooks:

- `EV_GreenFlux_separate_data_by_charger.ipynb` separates the data in the file _GreenFlux3Minute.csv_ into a separate file for each charger type.
- `create_greenflux_profiles.ipynb` resamples the charging current timeseries and converts it into power (kW). 
- 
## Running the notebooks

The packages required to run the notebooks within this folder are listed in `requirements.txt`.
We recommend installing these packages into a virtual environment.

To install the packages for the notebook, run `pip install -r requirements.txt`

The notebook assumes that the raw data files for each provider (can be found on the WPD Electric Nation webpage mentioned above) are located in the folder `raw_data`. Note that this directory was added to `.gitignore`. 
From the directory `data_electric_nation`, running `jupyter notebook` will open up the notebook interface in your web browser.


