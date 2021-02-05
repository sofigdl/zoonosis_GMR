# Zoonosis in the Greater Mekong Region (GMR)
<p> **Author:** Sofia Garcia </p>
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

## Sources

1. Han, Barbara A., Andrew M. Kramer, and John M. Drake. “Global Patterns of Zoonotic Disease in Mammals.” Trends in Parasitology 32, no. 7 (July 2016): 565–77. https://doi.org/10.1016/j.pt.2016.04.007.
2. Hansen, M. C., P. V. Potapov, R. Moore, M. Hancher, S. A. Turubanova, A. Tyukavina, D. Thau, et al. “High-Resolution Global Maps of 21st-Century Forest Cover Change.” Science 342, no. 6160 (November 15, 2013): 850–53. https://doi.org/10.1126/science.1244693.
3. Steven J. Phillips, Miroslav Dudík, Robert E. Schapire. [Internet] Maxent software for modeling species niches and distributions (Version 3.4.1). Available from url: http://biodiversityinformatics.amnh.org/open_source/maxent/. Accessed on 2021-2-5.
4. Wegmann, M., Leutner, B., & Dech, S. (Eds.). (2016). Remote sensing and GIS for ecologists: Using open source software. Pelagic Publishing.
5. WorldPop, and Bondarenko, Maksym. “Individual Countries 1km UN Adjusted Population Density (2000-2020).” University of Southampton, 2020. https://doi.org/10.5258/SOTON/WP00675.

