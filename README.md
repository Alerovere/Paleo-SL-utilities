# Paleo sea level utilities
This repository contains a variety of sea level calculation utilities related to paleo sea level changes, used in different papaers published or in preparation.

## Folder "VLM Simple"
This folder contains a simple Jupyter notebook that calculates long-term vertical land motion (VLM) rates from three inputs:

1. An eustatic sea level (ESL) estimate for a given time period (interval, with max-min)
2. The time interval (Time) (interval, max-min)
3. GIA corrections for the same time period (mean and standard deviation)
4. Observed Relative sea level (RSL) for the same period (mean and standard deviation)

With these three inputs, the script calculates long-term uplift rates with the following rationale:

1. The ESL estimate and Time are sampled randomly, with no assumptions on its probability distribution
2. GIA and RSL are sampled as normally distributed
3. The calculation of the rate is iterated 1.000.000 times with the formula (RSL − GIA − ESL)/Time

A histogram plot is then drawn, together with percentile bounds
This script was used to calculate values for the discussion of some sea level data vs VLM in Hearty et al. (submitted), Paleoceanography and Paleoclimatology.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Alerovere/Paleo-SL-utilities.git/master?urlpath=https%3A%2F%2Fgithub.com%2FAlerovere%2FPaleo-SL-utilities%2Fblob%2Fmaster%2FVLM_Simple%2FSea%2520level%2520calculations.ipynb)
