# A Markov Chain Model for Identifying Changes in Daily Activity Patterns of People Living With Dementia

## Code 

Statistical Analyses.ipynb provides the pipeline for generating datasets for the statistical analyses using the COVID_kitchen dataset in the core data folder. Alternatively, using the datasets in the Datasets for Statistical Analyses folder, you can use the instructions in this Statistical Analyses section of this code to access the liner mixed-effects regression (LMER) modelling packages in R.

Algorithm.ipynb provides the pipeline for extracting and comparing transition matrices using a sliding window function, as referred to in the paper entitled "A Markov Chain Model for Identifying Changes in Daily Activity Patterns of People Living With Dementia". This pipeline can be applied to the COVID_kitchen_ or kitchen_ datasets in the core data folder.

## Datasets

### Core Data Zip Files 

COVID_kitchen.csv is the raw activity data for the 21-household subset of our study cohort on which statistical analyses were conducted to investigate the effect of the COVID-19 pandemic on kitchen activity.

COVID_kitchen_.csv is the unprocessed transition data for the 21-household subset of our study cohort.

kitchen_.csv is the unprocessed transition data for the study cohort (n = 73).

### Datasets for Statistical Analyses

All datasets in this folder are from the 21-household subset of our study cohort.

COVID_wo.csv is the aggregated activity data for investigating the effect of the COVID-19 pandemic on kitchen activity.

Period_wo.csv is the aggregated activity data for investigating the effect of the individual COVID-19 pandemic periods on kitchen activity.

COVID_occupancy.csv is the aggregated activity data for investigating the interaction between the COVID-19 pandemic and occupancy on kitchen activity.

Period_occupancy.csv is the aggregated activity data for investigating the interaction between the individual COVID-19 pandemic periods and occupancy on kitchen activity.

COVID_tod.csv is the aggregated activity data for investigating the interaction between the COVID-19 pandemic and time of day on kitchen activity.

Period_tod.csv is the aggregated activity data for investigating the interaction between the individual COVID-19 pandemic periods and time of day on kitchen activity.
