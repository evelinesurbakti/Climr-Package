# Climr Package
The package can be used to analyze and plot the latest global hemispheric climate data

## Data Set
http://data.giss.nasa.gov/gistemp/tabledata_v3/GLB.Ts+dSST.csv

http://data.giss.nasa.gov/gistemp/tabledata_v3/NH.Ts+dSST.csv

http://data.giss.nasa.gov/gistemp/tabledata_v3/SH.Ts+dSST.csv


## Required R Packages
library(devtools)
library(roxygen2)
library(knitr)
library(stats)
library(dplyr) 
library(magrittr)
library(ggplot2)
library(viridis) 
library(readr) 


## What's on?
- __load_clim__ to load the climate data.
- __fit.climr__ to fit the data into the regression model.
- __plot.climrfit__ to plot the predicted data and real data. 
- __gp_fit__ to fit the to fit the hyperparameters of the Gaussian process with the optimisation method.
- __plot.climr_gp_fit__ to plot the predicted data by Gaussian process and real data.


## Try it!

After install, check and build the package, you can __try it__ on your console:

data1 <- load_clim(“NH”)

data2 <- gp_fit(data1, “BFGS”)

plot(data2)


## Document format
This project is written in Rstudio 
We are using R version 4.0.2 and ggplot version 3.3.2
