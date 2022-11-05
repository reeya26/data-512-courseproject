# Part 1: Common Analysis

During the last three years we all have been experiencing a global pandemic. This has been tragic and disruptive to many countries and has taken a deep personal toll on many individuals and their families. 
One aspect that has been hard to miss in the last three years is the datafication of the pandemic. That is, many aspects of the individual toll of the pandemic have been collected, aggregated and re-represented as data. This datafication gives us the privilege to examine the pandemic from potentially many different perspectives to understand how it has changed lives and how it has changed society

Through this analysis, we understand how masking policies change the progression of confirmed COVID-19 in Jackson county, Missouri, and how the CDC guidelines affected this change, from February 1, 2020 through October 1, 2021.

This repository contains the data files, code and results of Part 1, for the course Data 512: Human Centered Data Science.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/reeya26/data-512-homework_1/blob/main/LICENSE) ![Language](https://img.shields.io/badge/language-python-blue.svg)

## Resources Used
- Editor used: Jupyter Notebook
- Python version: 3.9.4
- Packages used: pandas, numpy, seaborn, matplotlib, ruptures

## Data 

Source Files:

- [Confirmed cases in USA](https://www.kaggle.com/datasets/antgoldbloom/covid19-data-from-john-hopkins-university) This file is from the Kaggle repository of John Hopkins University COVID-19 data. This data is updated daily. 
- [CDC Dataset](https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i) The CDC dataset of masking mandates by county.
- [NY Times Survey](https://github.com/nytimes/covid-19-data/tree/master/mask-use) The mask compliance survey by county conducted by NY Times.


Intermediary Files:

- jackson_confirmed_cases: Cleaned dataset containing the confirmed cases in Jackson Missouri from Feb 2020 to Oct 2021
- jackson_cdc_mandates: Cleaned dataset containing the Face Mask requirement guidelines in Jackson county
- jackson_mask_compliance_survey: Responses from residents of Jackson county for the NY Times survey


## Project Organization

This package has the following structure.

```
data-512-courseproject/
  |- license
  |- readme.md
  |- rawdata/
    |- dinosaur.genera.cleaned
  |- cleaneddata/
    |- jackson_confirmed_cases.csv
    |- jackson_cdc_mandates.csv
    |- jackson_mask_compliance_survey.csv
  |- results/
    |- 
    |- 
    |- 
  |- Part 1 Common Analysis
    
```
    
    
## Results



