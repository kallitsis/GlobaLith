[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13768666.svg)](https://doi.org/10.5281/zenodo.13768666)

# GlobaLith model

The GlobaLith model presents a global carbon footprint model for the lithium-ion battery industry. The code implements a life cycle assessment (LCA) model to predict the carbon footprint (CF) of lithium-ion batteries (LIBs) based on various chemistries commonly used in electric vehicles,including NMC111, NMC622, NMC811, NCA and LFP.The model follows LCA principles employing a cradle-to-gate system boundary, focusing on material and energy contributions to the CF. It incorporates data from multiple literature sources to calculate the material demand and carbon footprint for LIB production, and a Monte Carlo simulation is performed to quantify uncertainties in the CF estimations. The geographical scope 
is global, accounting for variations in the carbon intensity of electricity supply in key battery manufacturing locations worldwide. The output of the code includes the cradle-to-gate CF of LIB production under different scenarios and projections of greenhouse gas emissions on a global scale. The code has been used in the publication "Think global act local: The dependency of global lithium-ion battery emissions on production location and material sources" to estimate the carbon footprint of battery manufacturing from a global context. 
The full version of the publication is openly accessible here: https://www.sciencedirect.com/science/article/pii/S0959652624011739.

The modelling logic is as follows:
* [Material carbon footprint](Material_carbon_footprint) extracts the carbon footprint of key battery materials from a combination of literature sources, industry reports and LCA databases.
* [Battery carbon footprint](Battery_carbon_footprint.ipynb) performs a Monte Carlo simulation by combining material and energy contributions to the carbon footprint of battery manufacturing.
