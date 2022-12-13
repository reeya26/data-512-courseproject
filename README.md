# Part 4: Final Project

During the last three years we all have been experiencing a global pandemic. This has been tragic and disruptive to many countries and has taken a deep personal toll on many individuals and their families. 
One aspect that has been hard to miss in the last three years is the datafication of the pandemic. That is, many aspects of the individual toll of the pandemic have been collected, aggregated and re-represented as data. This datafication gives us the privilege to examine the pandemic from potentially many different perspectives to understand how it has changed lives and how it has changed society

Through this analysis, we learn how the population of a specific region was impacted by the pandemic, not only in quantitative terms like number of cases, but also in qualitative terms like life standards. For the purpose of this analysis, we have chosen Jackson county from the state of Missouri, in the United States of America. Jackson county is the second most populated county in Missouri with a significantly urban population.


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
- [OpenDataKC](https://data.kcmo.org/browse?q=death&sortBy=last_modified&utf8=✓) This is the open data portal of Kansas city, Missouri. It contains the Covid-19 Case & Death trends by date and was last updated on 10th November, 2022. It was created to support city operations and provide access to Kansas
city data for the community
- [Legal Dissolutions from Missouri Department of Health & Senior Services](https://health.mo.gov/data/vitalstatistics/data.php) This is the official Department of Health website of the State of Missouri. It contains annual and monthly reports of marriages and divorces in the State.



Intermediary Files:

- jackson_confirmed_cases: Cleaned dataset containing the confirmed cases in Jackson Missouri from Feb 2020 to Oct 2021
- jackson_cdc_mandates: Cleaned dataset containing the Face Mask requirement guidelines in Jackson county
- jackson_mask_compliance_survey: Responses from residents of Jackson county for the NY Times survey
- missouri_divorces_cleaned: Collated set of monthly legal dissolutions from 2018 to 2021


## Methodology 
In a two-pronged approach, we will first analyze the quantitative impact in the county, using a national level dataset from John Hopkins University and the Center for Disease Control. A strict mask mandate was implemented at varying points of the pandemic, which also resulted in wide-spread uproar during the later stages of the pandemic, with a certain section of people in the USA claiming that it infringed upon their freedom. The policy-makers stated that using masks will prevent the spread of Covid-19, with other factors kept constant. Through this approach, we will analyze whether this is any truth to this statement, and if the confirmed Covid-19 did slow-down every time a mask mandate was implemented. 

In the second approach, we view the qualitative impact of the pandemic by understanding how it affected family health in Jackson county. The long months of isolation resulted in increased levels of depression and anxiety as stated by medical professionals across the world. When the pandemic began everyone had to strictly remain indoors, and in the first year itself, the global prevalence of depression and anxiety increased by a staggering 25%[1]. Another impact of remaining indoors was a strain in relationships between partners, which led to break-ups and dissolution of marriages. This analysis will help us understand whether we should lend credence to these claims, and specifically, whether they apply to Missouri state.


## Project Organization

This package has the following structure.

```
data-512-courseproject/
  |- license
  |- readme.md
  |- rawdata/
    |- RAW_us_confirmed_cases.csv
    |- mask_use_by_county.csv
    |- cdc_mo.csv
    |- kansascity.csv
    |- dissolutions_excel
  |- cleaned_intermediary_files/
    |- jackson_confirmed_cases.csv
    |- jackson_cdc_mandates.csv
    |- jackson_mask_compliance_survey.csv
    |- missouri_divorces_cleaned
  |- Part 1 Common Analysis.ipynb
  |- Part 4 Analysis.ipynb
  |- part1_a4_visualization.png
    
```
    
    
## Results

Change Point Detection of COVID-19 Cases in Jackson county, Missouri

![Change Point Detection of COVID-19 Cases in Jackson county, Missouri](https://github.com/reeya26/data-512-courseproject/blob/main/part1_a4_visualization.png)

We can note the following points from the visualization:

1. During the first part of no mask guidelines, the cases were at a minimal, as Covid-19 had not spread to all parts of US.

2. During the 1st change-point, around July 2020 we can observe that even though the mask guidelines required compulsory masks, there was a slight rise in cases. This could be as Jackson county did not have any strict mask mandates as this was also a few month into the pandemic when people were more aware about COVID-19.

3. A similar pattern is observed in the 2nd change-point, around November 2020, where the cases continue to rise.

4. During the 3rd change-point, February 2021, we can see that the even though mask guidelines were relaxed, there was still a decline in the cases. This could be due to the fact that vaccines had started rolling out.

5. Between the 4th and 5th change-point, from July to September 2021, with the relaxed mask guidelines the cases increased again but decreased soon.

In conclusion, there isn't a very direct relation between mask guidelines and the Covid-19 cases. This makes sense since Jackson county did not have a strict mask mandate so people would not be following CDC guidelines strictly, but rather use caution when they deem fit. We also observe a clear decrease once the vaccines started being provided



## Disclaimer

Missouri Department of Health & Senior Services Disclaimer:
“The data made available here has been modified for use from its original source, which is
the State of Missouri. THE STATE OF MISSOURI MAKES NO REPRESENTATIONS OR
WARRANTY AS TO THE COMPLETENESS, ACCURACY, TIMELINESS, OR CONTENT OF ANY
DATA MADE AVAILABLE THROUGH THIS SITE. THE STATE OF MISSOURI EXPRESSLY
DISCLAIMS ALL WARRANTIES, WHETHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED
WARRANTIES OF MERCHANTABILITY, OR FITNESS FOR A PARTICULAR PURPOSE. The data
is subject to change as modifications and updates are complete. It is understood that the
information contained in the Web feed is being used at one’s own risk.”

