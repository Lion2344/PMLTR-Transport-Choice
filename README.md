# PMLTR-Transport-Choice

This repository contains a computational study comparing the **PMLTR model**, **RumBoost**, and manually specified **MNL models**.  

## Repository structure
- **Conclusion/**
  - has all results regarding the comparison of the performance of the algorithms at each dataset  
- **Datasets/**  
  - `Raw/`: input files required to run the code.  
  - `Input/`: automatically filled with preprocessed data after running `main.py`.  
  - `Logfiles/`: Created automatically during the lambda search if the respective lambda value is missing.
  - `Output/`: Contains the test results of all algorithms for the respected dataset.
- **Metafiles/**  
  - Contains configuration files to adjust the lambda search parameters, to apply different lambda values for testing or to set the parameters for plotting. 

## Notes
- **Do not delete logfiles.** For some datasets (especially *Swissmetro* and *SchoolTripsDresden*), the lambda search can take several days and may require a large amount of RAM.  
- Plotting is currently limited to the calculation of the **value of time (VoT)**, and only for the synthetic datasets.  

## Installation
We recommend using Python ≥ 3.11.  
Install all required dependencies via:

```bash
pip install -r requirements.txt
