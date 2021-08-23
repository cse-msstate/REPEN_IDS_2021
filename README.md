# REPEN_IDS_2021
Linux and Git 'diff' files for REPEN that allows for epoch-to-epoch testing

# Installation
1. Use the diff files to make your own???
2. Create 'results/', 'cachedir/', 'model/', 'data/', and 'survey_results/' directories
3. Install dependencies [TODO - add requirements.txt]
```
pip3 install -r requirements.txt
```
   - Python 3.6 works for this code. This was run on Ubuntu 18.04. You may have trouble otherwise
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
