# Re-evaluation of Bitcoin’s Potential as an Inflation Hedge

By Meng Wu (m59wu) & Sijie Xu (s362xu). Link

### Introduction

In this research, we use the most current data available to re-evaluate the existing
evidence surrounding Bitcoin’s potential to be used as a hedge against inflation.
Using vector autoregressive (VAR) models and GARCH-VAR models to assess
correlation and causal relationships, we find evidence that refutes the findings of
previous studies that Bitcoin can be used to hedge against inflation [Inflation and Bitcoin: A descriptive time-series analysis ], 
[Bitcoin: An inflation hedge but not a safe haven], [Bitcoin, gold and the dollar – A GARCH volatility analysis]. Using
a bootstrapping algorithm combined with the GARCH-VAR models, we also es-
tablish the presence of a paradigm shift occurring around the start of the COVID
pandemic that serves as evidence supporting a pandemic impact on the behaviour
of both Bitcoin returns and expected inflation rates. The multi-series VAR models
also identify the oil and real estate index to be more strongly correlated with ex-
pected inflation rates than Bitcoin returns, suggesting the presence of confounding
variables that may be behind any apparent correlation between Bitcoin returns and
expected inflation. Based on the results of our study, the existing claims on the
relationship between Bitcoin returns and inflation no longer appear to hold true
based on more current post-pandemic data

### Environment

Install R and R Studio for virtual python environments. 
Run following command in console to ensure same working configuration.
```bash
list.of.packages <- c("rugarch", "dplyr", "tidyverse", "quantmod", 
    "FinTS", "tseries", "PerformanceAnalytics", "vars", "zoo", "rmgarch")

# Check if packages installed 
new.packages <- list.of.packages[!(list.of.packages %in% installed.packages()[,"Package"])]

# Install missing packages 
if(length(new.packages)) install.packages(new.packages)
```

### Methodology

#### Data Cleaning / Acquiring
Please refer to the [Data_Preprocessing.Rmd](Data_Preprocessing.Rmd) for the data cleaning and initial testing procedure. 

#### Model Fitting
The VAR model mentioned in phase 1 of the study can be found via [Model_VAR_Fitting.Rmd](Model_VAR_Fitting.Rmd).
The GARCH-VAR model mentioned in phase 2 and 3 of the study can be found via [Model_VAR_GARCH_Fitting.Rmd](Model_VAR_GARCH_Fitting.Rmd).
The model reguliaized VAR model mentioned in phase 4 of the study can be found via [Model_Regularized_VAR.rmd](Model_Regularized_VAR.rmd).


> *Re-evaluation of Bitcoin’s Potential as an Inflation Hedge (2022) (c) by Meng Wu & Sijie Xu* *Re-evaluation of Bitcoin’s Potential as an Inflation Hedge
> (2022) is licensed under a Creative Commons Attribution
> 4.0 International License.* *You should have received a copy of the
> license along with this work. If not, see
> <http://creativecommons.org/licenses/by/4.0/>.*
