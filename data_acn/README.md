# Data Exploration ACN dataset

This folder contains Jupyter notebooks which explore the openly accessible EV charging data.

## Data Sources

### ACN Dataset Caltech
The [Adaptive Charging Network dataset](https://ev.caltech.edu/dataset) is used to collect charging profiles.

## Running the notebooks

- The packages required to run the notebooks within this folder are listed in `requirements.txt`.
We recommend installing these packages into a virtual environment.

- To install the packages for the notebook, activate your virtual environment and run `pip install -r requirements.txt`. If there is any issues, try runnin `pip install --upgrade pip` before installing the requirements. 

- The notebooks use the [API client](https://github.com/zach401/acnportal). Follow these steps to install it:
  - `git clone https://github.com/zach401/acnportal`
  - `pip install .`
  
- After that, running `jupyter notebook` will open up the notebook interface in your web browser.
- The API client also needs an API token to access the data. To obtain a token, [register on the webpage](https://ev.caltech.edu/dataset). The token should be stored in the file `acn_api_token.txt`, which should be added to the `secrets` folder.
)
