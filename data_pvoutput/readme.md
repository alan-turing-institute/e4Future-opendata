# Data Exploration PVOutput.org

This folder contains a Jupyter notebook which explores the openly accessible data from the PVOutput platform.
## Data Sources

### PVOutput.org

[PVOutput.org](pvoutput.org) is a free service for sharing and comparing PV output data. 


## Running the notebooks

The packages required to run the notebooks within this folder are listed in `requirements.txt`.
We recommend installing these packages into a virtual environment.

To install the packages for the notebook, run `pip install -r requirements.txt`

The notebooks use the [Python library](https://github.com/openclimatefix/pvoutput) to interact with the PVOutput API. The notebook assumes 
that the files and folders of the Python library are located in the folder `pvoutput`. Note that this directory was added to `.gitignore`. From the directory `pvoutput`, run `pip install -e git+https://github.com/openclimatefix/pvoutput#egg=pvoutput` (as described in the `README.md` of the client repo) to install the Python library.
After that, change to `data_pvoutput` and running `jupyter notebook` will open up the notebook interface in your web browser.
The API client needs an API key and a system ID to access the data. To obtain a key, [register on the webpage] (pvoutput.org). After login, navigate to `Settings` and then `API Settings`. Enable API access and click the `New key` button. To obtain the system ID, go to `Registered Systems` and click `Add System`.  Enter a name for the system, tick the `Energy consumption only` box and `Save`. The added system should now show up under `Registered Systems` where you can also find the assigned system ID. 

The API key is stored in the file `pvoutput_api_key.txt` and the system id in the file `pvoutput_system_id.txt`, which can be found in the `secrets` folder.

Please note that in order to access data of PV systems registered with PVOutput via the API, a donation (AUD 15) is required which grants access for one year. There are, however, limits on the number of requests per hour. 

In order to get the credentials of the VGI account, ask a project member. 