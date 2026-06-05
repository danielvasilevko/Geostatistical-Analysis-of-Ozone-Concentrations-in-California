# Geostatistical-Analysis-of-Ozone-Concentrations-in-California

This repository contains an R Markdown file and knitted PDF used for the 
demonstration of core geostatistical methods applied to EPA ozone monitoring 
data across California, along with the data used in the analysis.

# Repository Structure

* Project173.Rmd - R Markdown file featuring the full geostatistical analysis 
and visualization of ozone concentrations in California.
* Project173.pdf - A knitted PDF containing the full output of the analysis, 
including all plots, variogram fits, kriging predictions, and cross-validation 
results.
* Records.csv - EPA ozone monitoring data containing daily maximum 8-hour ozone 
concentrations from 142 stations across California.

# What Project173.Rmd Does

* Computes summary statistics and produces exploratory visualizations (histogram, ECDF, QQ plot, boxplot) of daily maximum 8-hour ozone concentrations on March 10, 2025.
* Creates an h-scatterplot to examine spatial dependence between nearby monitoring stations.
* Creates a bubble plot mapping raw ozone concentrations across California by station location.
* Fits classical and robust omnidirectional variograms using exponential, spherical, and Gaussian covariance models.
* Interpolates ozone concentrations across a 100x100 prediction grid using  inverse distance weighting (IDW), ordinary kriging, simple kriging, and universal kriging.
* Produces raster maps and contour plots of the kriging prediction surfaces overlaid on the California state boundary.
* Performs leave-one-out cross-validation across all variogram and kriging models, reporting mean error and mean squared error for model comparison.
