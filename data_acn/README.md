# Data Exploration ACN dataset

This folder contains Jupyter notebooks which explore the openly accessible EV charging data.

## Data Sources

### ACN Dataset Caltech
The [Adaptive Charging Network dataset](https://ev.caltech.edu/dataset) is used to collect charging profiles.

## Running the notebooks

The packages required to run the notebooks within this folder are listed in `requirements.txt`.
We recommend installing these packages into a virtual environment.

To install the packages for the notebook, run `pip install -r requirements.txt`

The notebooks use the [API client](https://github.com/zach401/acnportal). The notebooks assume 
that the required parts of the API client repository (the folder `acnportal`) are copied into the folder `acn_client`. Note that this directory was added to `.gitignore`. From the directory `acn_client`, run `pip install .` (as described in the README.md of the client repo) to install the required modules for the API client. 

After that, running `jupyter notebook` will open up the notebook interface in your web browser.
The API client also needs an API token to access the data. To obtain a token, [register on the webpage] (https://ev.caltech.edu/dataset). The token is stored in the file `acn_api_token.txt`, which can be found in the `secrets` folder.

(Note that the list in `requirements.txt` does not include the `notebook` package in case you already have it set up.
If you need to install it here, run `pip install notebook`.)
