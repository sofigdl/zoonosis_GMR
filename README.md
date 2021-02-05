# Zoonosis in the Greater Mekong Region (GMR)
**Author:** Sofia Garcia
This repository contains the R code for a presece-only maxent model to map possible zoonosis outbreaks in the GMR

## Functionality
It allows to build spatial model sing georeferenced presence-data (vector .shp) and a raster with predictors (.tiff).
Using this code, you could:
* Create background points for the presence data
* Extract data from the enviroment (predictors) into a data frame
* Analyse collinearity between variables
* Model using [Maxent](https://biodiversityinformatics.amnh.org/open_source/maxent/) (Maximum Entropy) algorithm
* Plot the variable importance and the response curves
* Generate a raster with the spatial prediction
* Perform cross validation

**Notes**
The code is to analyse population density, zoonotic host richness and tree cover, but could be replace/compliment by other variables.

You can read the dismo/maxent [documentation](https://cran.r-project.org/web/packages/dismo/dismo.pdf) for more information.
## Prerequesites

It requires the packages
- raster
- RStoolbox
- rgdal
- e1071
- randomForest
- dismo
- rms
- mgcv
- car
- rJava
