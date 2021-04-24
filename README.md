# An Introduction to Python with Google Colab
### GEOS 212: Water in the West
### Spring 2021

This repository contains some Jupyter notebooks that were developed in Google Colab in order to provide sophomore-level students an early introduction to scientific programming with Python. The class, Water in the West, is a Geoscience class that introduces them to the water sciences. Introductory workshops, adopting the the Software Carpentry style of narrated live coding, occurred over two 75 minute class sessions in April 2021 via zoom. 

## Contents
The repository contains three notebooks that are of interest to the students:

1. A notebook that goes through a workflow of downloading USGS discharge data based on a site ID number for five water years, creates a labelled a plot, creates a vector of water years for subsequent analysis, and creates a Pandas dataframe with the data and saves it to a PKL file [GEOS212_SP2021_IntroToHydroPython.ipynb](./GEOS212_SP2021_IntroToHydroPython.ipynb)
2. A notebook that repeats most of the workflow from the above notebook, but was done in class in a narrated live coding fashion [MyFirstNotebook.ipynb](./MyFirstNotebook.ipynb)
3. __In progress:__ A notebook that takes the saved PKL file and performs some basic hydrologic statistical analysis on the time series

## Depdendencies
These notebooks are built on the following dependencies:

* Nwis: Used to download streamflow time series data from National Water Information System (Nwis). Nwis is a library developed in support of the Community Surface Dynamics Modeling System (CSDMS) [see Nwis repo](https://github.com/gantian127/nwis). Note: Nwis installs XArray for data storage.
* Numpy: Used to extract data from data objects returned by Nwis and provide novice students with more transparency on how statistics are computed
* Pandas: Used to group data to compute statistics on a water year basis
* Matplotlib: Used to create plots
