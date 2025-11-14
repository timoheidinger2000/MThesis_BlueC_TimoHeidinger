# README: Blue Carbon Modelling Script
[Code_BlueC_TimoHeidinger_GitHub.ipynb]

as part of the Master Thesis "Mapping Blue Carbon and Ecosystem Perceptions in The Gambia: A Socio-Ecological Approach in the Niumi UNESCO Biosphere Reserve"

by Timo Heidinger (2025)

This script develops an end-to-end machine learning and remote sensing pipeline to model and map blue carbon stocks in the Niumi UNESCO Biosphere Reserve using 
Sentinel-1 and Sentinel-2 imagery combined with field plot data. By integrating multi-sensor feature extraction, SHCE-based feature selection, and Random Forest modeling, 
the workflow produces high-resolution biomass and blue carbon maps that support ecosystem monitoring and conservation planning.

## Overview

The workflow includes:
* Loading protected area boundaries and Global Mangrove Watch mangrove extent
* Preprocessing Sentinel-2 imagery (cloud masking, resampling, vegetation indices)
* Processing Sentinel-1 imagery (VV/VH, GLCM textures, SAR transforms)
* Combining S1 and S2 into a multi-band feature stack
* Integrating field plot data from Google Sheets
* Applying SHCE feature selection (Boruta, JMIM, RFE, MDA)
* Selecting predictors using an AIC curve
* Training and tuning a Random Forest model
* Predicting biomass carbon across the study area
* Computing and exporting blue carbon and CO₂-equivalent rasters

## Outputs

* Sentinel 1 and 2 Composites
* RGB image
* SHCE feature ranking table
* Selected predictors from AIC
* Trained Random Forest model
* Biomass carbon and blue carbon GeoTIFFs
* Evaluation metrics and cross-validation results

## Requirements
see libraries in Code_BlueC_TimoHeidinger_GitHub.ipynb

## Additional:

* Google Earth Engine account
* Google Drive access

## Author
Timo Heidinger (2025)

## Citation
Heidinger, T. (2025). MThesis_BlueC_TimoHeidinger. GitHub. URL

