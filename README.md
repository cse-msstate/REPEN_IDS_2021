# REPEN_IDS_2021
Linux and Git 'diff' files for REPEN that allows for epoch-to-epoch testing

# Installation
This code was run using Python 3.6.9 on Ubuntu 18.04 'Bionic Beaver'. If you are having trouble with installation, try using these versions.

1. We are afraid to include python files that have no license, so use the diff files to re-create our code
2. Create 'results/', 'cachedir/', 'model/', 'data/', and 'survey_results/' directories
```
mkdir {results,cachedir,model,data,survey_results}
```
4. Install dependencies
```
pip3 install -r requirements.txt
```
   - add or remove the '3' as necessary
   - Use sudo if needed
   - Recommended to use a virtual environment


# Running the Script
Verify installation by placing a dataset csv in the 'data/' directory and running: 
```
python3 main.py <dataset-without-'.csv'> [0-3]

# example
python3 main.py nslkdd_100 0
```
- args[1] = name of dataset without '.csv'
- args[2] = fold number to be tested 0,1,2, or 3
Result csv should be in 'results/'
