# A Markov Chain Model for Identifying Changes in Daily Activity Patterns of People Living with Dementia

This repository contains the code for the statistical tests and algorithm described in the paper "[A Markov Chain Model for Identifying Changes in Daily Activity Patterns of People Living with Dementia](https://ieeexplore.ieee.org/document/10171194)". We have also included anonymized data.

## Dependencies

In order to generate the datasets and run the statistical experiments and algorithm, your environment will need to contains the following main packages:

- `pandas 2.0.1`
- `numpy 1.24.4`
- `scipy 1.8.0`

## Code 

### Statistics

Statistical Analyses.ipynb provides the pipeline for generating the datasets needed for the statistical analyses presented in the paper. To derive these datasets locally, download the 'COVID_kitchen' dataset in the 'Core Data Zip Files' folder and run Statistical Analyses.ipynb. 

Alternatively, you can downloaded the datasets needed for the statistical analyses from the 'Datasets for Statistical Analyses' folder.

To conduct the statistical experiments locally, you will need to install and download R and RStudio. See https://posit.co/download/rstudio-desktop/ for more information on dowloading and installing R and RStudio for desktop. 

You will then need to load the datasets needed for the statistical analyses into RStudio. Following the instructions in this 'Statistical Analyses' section of the Statistical Analyses.ipynb, you can then access the liner mixed-effects regression (LMER) modelling packages in R and model the effects of the pandemic, pandemic periods, household occupancy, and time of day on kitchen activity. 

Alternatively, you can download Statistical Analyses.RData and load this straight into RStudio. In this case, the effects have already been modelled as detailed in the paper. You can then just print the summary or anova results of each model using the code 'print(summary(model))' or 'print(anova(model))', respectively.

### Algorithm

Algorithm.ipynb provides the pipeline for extracting and comparing transition matrices using a sliding window function, as referred to in the paper entitled "A Markov Chain Model for Identifying Changes in Daily Activity Patterns of People Living with Dementia". This pipeline can be applied to the COVID_kitchen_ or kitchen_ datasets in the core data folder.

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

### Contact

Nan Fletcher-Lloyd 

## Citation

If you use this code in any way, please refer to it by citing my paper "[A Markov Chain Model for Identifying Changes in Daily Activity Pattern of People Living with Dementia](https://ieeexplore.ieee.org/document/10171194)":

- Bibtex:
```
@article{fletcher-lloyd2023markov,
	author={Nan Fletcher-Lloyd and Alina-Irina Serban and Magdalena Kolanko and David Wingfield and Danielle Wilson and Ramin Nilforooshan and Payam Barnaghi and Eyal Soreq},
	year={2023},
	title={A Markov Chain Model for Identifying Changes in Daily Activity Patterns of People Living with Dementia},
	journal={IEEE internet of things journal},
	isbn={2327-4662},
	doi={10.1109/JIOT.2023.3291652}
}
```

