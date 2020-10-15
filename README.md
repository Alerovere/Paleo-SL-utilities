# Paleo sea level utilities
This repository contains a variety of sea level calculation utilities related to paleo sea level changes, used in different papers published or in preparation.

## Folder "VLM Simple"

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
This script compares published sea-level curves with sea-level observations.
At present, the following sea level curves are available:

### de Boer et al., 2014
*de Boer, B., et al. (2014) Persistent 400,000-year variability of Antarctic ice volume and the carbon cycle is revealed throughout the Plio-Pleistocene. Nature Communications 5, 2999.*

Retrieved from the original publication.

### Stap et al., 2017
*Stap, L. B., Van De Wal, R. S., De Boer, B., Bintanja, R., & Lourens, L. J. (2017). The influence of ice sheets on temperature during the past 38 million years inferred from a one-dimensional ice sheet-climate model. Climate of the Past, 13(9), 1243-1257.*

Retrieved from the original publication.

### Rohling et al., 2014
*Rohling, E. J., Gavin L. Foster, K. M. Grant, Gianluca Marino, A. P. Roberts, Mark E. Tamisiea, and Frances Williams. "Sea-level and deep-sea-temperature variability over the past 5.3 million years." Nature 508, no. 7497 (2014): 477-482*

Retrieved from the personal website of EElco Rohling, "data in Figure 2" of Rohling et al., 2014.
 
### de Boer et al., 2010
*de Boer, B., Van de Wal, R. S. W., Bintanja, R., Lourens, L. J. & Tuenter, E. Cenozoic global ice-volume and temperature simulations with 1-D ice-sheet models forced by benthic d18O records. Ann. Glaciol. 51, 23–33 (2010).*

Retrieved from the personal website of EElco Rohling, "data in Figure 2" of Rohling et al., 2014.

### Sosdian and Rosenthal, 2009
*Sosdian, S. & Rosenthal, Y. Deep-sea temperature and ice volume changes across the Pliocene-Pleistocene climate transitions. Science 325, 306–310 (2009).*

Retrieved from the personal website of EElco Rohling, "data in Figure 2" of Rohling et al., 2014.

### Elderfield et al., 2012
*Elderfield, H. et al.Evolution of ocean temperature and ice volume through the MidPleistocene Climate Transition. Science 337, 704–709 (2012).*

Retrieved from the personal website of EElco Rohling, "data in Figure 2" of Rohling et al., 2014.

### Miller et al., 2012 / Naish et al., 2009
*Miller, K. G. et al. High tide of the warm Pliocene: implications of global sea level for Antarctic deglaciation. Geology 40, 407–410 (2012).*

*Naish, T. et al. Obliquity-paced Pliocene West Antarctic ice sheet oscillations. Nature 458, 322–328 (2009).*

Retrieved from the personal website of EElco Rohling, "data in Figure 2" of Rohling et al., 2014.

### Stap et al., 2016
*Stap, L.B., de Boer, B., Ziegler, M., Bintanja, R., Lourens, L.J. and van de Wal, R.S., 2016. CO2 over the past 5 million years: Continuous simulation and new δ11B-based proxy data. Earth and Planetary Science Letters, 439, pp.1-10.*

Retrieved from the original publication.

### Grant et al., 2014
*Grant, K.M., Rohling, E.J., Ramsey, C.B., Cheng, H., Edwards, R.L., Florindo, F., Heslop, D., Marra, F., Roberts, A.P., Tamisiea, M.E. and Williams, F., 2014. Sea-level variability over five glacial cycles. Nature communications, 5(1), pp.1-9.*

Retrieved from the original publication.

### Lisiecki and Raymo, 2005
*Lisiecki, L.E. and Raymo, M.E., 2005. A Pliocene‐Pleistocene stack of 57 globally distributed benthic δ18O records. Paleoceanography, 20(1).*

As used in *Rovere A., Pappalardo M, Richiano S., Aguirre M., Sandstrom M.R., Hearty P.J., Austermann J., Castellanos I., Raymo M.E. An Early Pliocene relative sea level record from Patagonia (Argentina). EarthArXIV - https://doi.org/10.31223/osf.io/ycp6t*

### Miller et al., 2020
*Miller, K.G., Browning, J.V., Schmelz, W.J., Kopp, R.E., Mountain, G.S. and Wright, J.D., 2020. Cenozoic sea-level and cryospheric evolution from deep-sea geochemical and continental margin records. Science advances, 6(20), p.eaaz1346.*

Retrieved from PANGAEA: https://doi.pangaea.de/10.1594/PANGAEA.923126

## Papers using the scripts contained in these folders.
Version 1.3 of this repository was used to calculate values for the discussion of some sea level data vs VLM in Hearty et al. (2020), https://doi.org/10.1029/2019PA003835

Version 1.4 of this repository was used in the first version of Rovere et al (2020), https://eartharxiv.org/ycp6t/

Version 1.5 of this repository was used in the final version of Rovere et al (2020), https://eartharxiv.org/ycp6t/
