# Paleo sea level utilities
This repository contains a variety of sea level calculation scripts, used in different papers published or in preparation.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4091380.svg)](https://doi.org/10.5281/zenodo.4091380)

## Folder "ESL_Calculations"
This folder contains a Jupyter notebook that calculates global mean sea level from RSL data (observation and ages) and estimates of Glacial Isostatic Adjustment (GIA) and vertical land motions (VLMs) for two sea-level indicators. Results are compared to a  reference value.

## Folder "GIA_Correction"
This folder contains a Jupyter notebook that implements a Monte-Carlo approach to subtract GIA and VLMs from a set of observed (and dated) sea-level index points, plotting the results as Kernel Density Estimate plots.

## Folder "Post_Ind_SL_plot"
A Jupyter notebook that downloads and plots post-industrial sea-level data from Frederikse et al., 2020 (https://doi.org/10.1038/s41586-020-2591-3).

## Folder "Sea_Level_Curves"
This folder contains two Jupyter notebooks. The first (SL_Curves) plots several sea-level curves spanning the past few million years and compares them to user-inserted observed RSL data. It also includes a function to make an interactive sea-level plot using the same curves. The second (SL_CO2_T) plots sea level, temperature and carbon dioxide curves for the past 700 ka on the same graph.

## Folder "Tide_Plotting"
This folder contains a Jupyter notebook that downloads and plots tide gauge data from the PSMSL website. The script allows plotting as many stations as needed.

## Folder "VLM Simple"
This folder contains a Jupyter notebook that calculates long-term vertical land motion (VLM) rates from an eustatic sea level (ESL) estimate for a given time period, the time interval (Time), GIA corrections for the same time period and observed Relative sea level (RSL) are required.

### Papers using the notebooks contained in these folders.
Version 1.3 of this repository was used to calculate values for the discussion of some sea level data vs VLM in Hearty et al. (2020), https://doi.org/10.1029/2019PA003835

Version 1.4 of this repository was used in the first version of Rovere et al (2020), https://eartharxiv.org/ycp6t/

Version 1.5 of this repository was used in the final version of Rovere et al (2020), https://eartharxiv.org/ycp6t/, then published as https://doi.org/10.1038/s43247-020-00067-6

Version 1.6 of this repository was used in various talks, to create an image for the dissemination book "Il mare che sale" by S. Carniel, and for the first version of a manuscript on Last Interglacial Sea level in Madagascar (Weil-Accardo et al., in prep.)

### License
This software is relased under the MIT license.

Copyright 2022 - Alessio Rovere

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

### Research funding acknowledgments
This script and associated data were created in the framework of the European Reasearch Council Starting Grant WARMCOASTS (Grant Agreement Number 802414), funded under the European Union's Horizon 2020 research and Innovation programme.