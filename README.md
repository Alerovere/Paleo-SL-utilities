# Paleo sea level utilities
This repository contains a variety of sea level calculation utilities related to paleo sea level changes, used in different papaers published or in preparation.

## Folder "VLM Simple"
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Alerovere/Paleo-SL-utilities.git/master?filepath=VLM_Simple%2FSea%20level%20calculations.ipynb)

This folder contains a simple Jupyter notebook that calculates long-term vertical land motion (VLM) rates from three inputs:

1. An eustatic sea level (ESL) estimate for a given time period (interval, with max-min)
2. The time interval (Time) (interval, max-min)
3. GIA corrections for the same time period (mean and standard deviation)
4. Observed Relative sea level (RSL) for the same period (mean and standard deviation)

With these three inputs, the script calculates long-term uplift rates with the following rationale:

1. The ESL estimate and Time are sampled randomly, with no assumptions on their probability distribution
2. GIA and RSL are sampled as normally distributed
3. The calculation of the rate is iterated 1.000.000 times with the formula (RSL − GIA − ESL)/Time

A histogram plot is then drawn, together with percentile bounds
This script was used to calculate values for the discussion of some sea level data vs VLM in Hearty et al. (2020), Paleoceanography and Paleoclimatology: https://doi.org/10.1029/2019PA003835

