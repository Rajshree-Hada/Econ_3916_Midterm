# Econ_3916_Midterm

# County Poverty and Life Expectancy in the United States

## Question

How is county-level poverty associated with life expectancy in the United States, after accounting for adult educational attainment and metropolitan status?

## Data

The analysis uses four datasets:

1. **USALEEP Life Expectancy by Census Tract (US_A.CSV)**  
   Source: [CDC National Center for Health Statistics – USALEEP](https://www.cdc.gov/nchs/nvss/usaleep/usaleep.html)  
   File: `US_A.CSV`  
   Download date: 10/29/2026

2. **2010 Census Tract Population**  
   Source: [U.S. Census Bureau – 2010 Decennial Census API, Summary File 1](https://api.census.gov/data/2010/dec/sf1)  
   Table: P1 (Total Population)  
   Download date: 10/29/2026

3. **2015 County Poverty Estimates (SAIPE)**  
   Source: (https://www.census.gov/data/datasets/2015/demo/saipe/2015-state-and-county.html)  
   Download date: 10/29/2026

4. **County Educational Attainment and Urban Influence Codes**  
   Sources:
   - USDA Economic Research Service (ERS), County-Level Educational Attainment, 2008–2012: [INSERT EXACT ERS SOURCE PAGE]
   - USDA ERS, 2013 Urban Influence Codes: (https://www.ers.usda.gov/data-products/county-level-data-sets/county-level-data-sets-download-data)  
   Download date(s): 10/29/2026

## How to run

To reproduce the analysis:

1. Open the code in a Google Colab notebook.
2. Select **Runtime → Restart session and run all**.
3. No file uploads are required. All four data files are stored in this GitHub repository, and the notebook gets them from GitHub.

The repository also includes `get_data.py`, a script for rebuilding the Census tract population file and the USALEEP `US_A.CSV` file. Running this script requires a Census API key, which users can obtain from the U.S. Census Bureau. The API key must be set as a variable on the user's own machine. But the notebook can also be run without uploading files or providing an API key because the prepared data files are already included in the repository.

## Repository contents

- Google Colab/Jupyter notebook
- Analysis report
- USALEEP life expectancy data: `US_A.CSV`
- 2010 Census tract population data
- 2015 SAIPE county poverty data
- USDA ERS education and Urban Influence Codes data

## Headline finding

Across 3,108 counties, a one-percentage-point higher poverty rate is associated with approximately 0.17 fewer years of life expectancy, holding adult educational attainment and metropolitan status constant (95% confidence interval: −0.189 to −0.150).

This represents a **conditional association, not a causal effect**. The results indicate a relationship between county poverty and life expectancy after accounting for the other variables in the model; they do not establish that higher poverty causes lower life expectancy.
