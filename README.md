# Paleo sea level utilities
This repository contains a variety of sea level calculation utilities related to paleo sea level changes, used in different papers published or in preparation.

## Folder "VLM Simple"
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Alerovere/Paleo-SL-utilities.git/master?filepath=VLM_Simple%2FSea%20level%20calculations.ipynb)

This folder contains a simple Jupyter notebook that calculates long-term vertical land motion (VLM) rates from four inputs:

1. An eustatic sea level (ESL) estimate for a given time period (interval, with max-min)
2. The time interval (Time) (interval, max-min)
3. GIA corrections for the same time period (mean and standard deviation)
4. Observed Relative sea level (RSL) for the same period (mean and standard deviation)

With these inputs, the script calculates long-term uplift rates with the following rationale:

1. The ESL estimate and Time are sampled randomly, with no assumptions on their probability distribution
2. GIA and RSL are sampled as normally distributed
3. The calculation of the rate is iterated 1.000.000 times with the formula (RSL − GIA − ESL)/Time

A histogram plot is then drawn, together with percentile bounds.

## Folder "ESL Calculations"
This folder contains a Jupyter notebook that calculates global mean sea level from paleo RSL data and estimates of GIA and vertical land motions for two sea level indicators, and compares the results to a set of reference values.  

1. Paleo Relative Sea Level (RSL) and associated uncertainty.
2. Glacial Isostatic Adjustment (GIA) prediction and associated standard deviation
3. Vertical land motion (VLM) rate and associated uncertainty
4. Age and associated uncertainty

## Folder "Sea Level Curves"
This script compares published sea-level curves with sea-level observations organised into a pandas dataframe.

## Papers using the scripts contained in these folders.
Version 1.3 of this repository was used to calculate values for the discussion of some sea level data vs VLM in Hearty et al. (2020), https://doi.org/10.1029/2019PA003835

Version 1.4 of this repository was used to calculate values for the discussion in Rovere et al (2020), https://eartharxiv.org/ycp6t/
