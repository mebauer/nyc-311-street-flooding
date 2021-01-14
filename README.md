# Analyzing NYC's 311 Street Flooding Complaints from 2010 to 2020  
Mark Bauer  

![cover photo](figures/cover-photo.png) 

# Table of Contents

   * [Executive Summary](#Executive-Summary)
   * [Introduction](#Introduction)
   * [Getting Started](#Getting-Started)
       * [Prerequisites](#Prerequisites)
           * [Data Science Tools: Anaconda](#Data-Science-Tools-Anaconda)
               * [Included Python Libraries](#Included-Python-Libraries)
               * [Additional Libraries](#Additional-Libraries)     
       * [Notebooks](#Notebooks)
       * [Data](#Data)     
   * [Resources](#Resources)
   * [Media](#Media)
   * [Further Reading](#Further-Reading)
   * [Say Hello!](#Say-Hello)

# Executive Summary

In progress...

# Introduction

I conducted an analysis of street flooding complaints with NYC Open Data's 311 data set. Specifically, I attempted to answer the following questions:

- What is the distribution of street flooding complaints by neighborhood, borough and citywide?
- How have street flooding complaints changed over time?
- Which streets experienced the most 311 street flooding complaints?
- Which days and weeks experienced the most street flooding complaints?
- What are the average and median response hours to 311 street flooding complaints?

I've also included case studies from the neighborhoods:

- Hammels, Arverne, and Edgemere, Queens  
- New Dorp - Midland Beach, Staten Island


# Getting Started

## Prerequisites

### Data Science Tools: Anaconda

Download and install [Anaconda](https://www.anaconda.com/products/individual) python distribution.

#### Included Python Libraries

- pandas
- matplotlib
- seaborn

#### Additional Libraries

I am using a Mac, but if you're using Windows, you may need to install these packages:

- geopandas

`conda install -c conda-forge geopandas`

- geoplot

`conda install -c conda-forge geoplot`

- fiona

`conda install -c conda-forge fiona`

- pywin32

`conda install -c anaconda pywin32`

- jupyter_contrib_nbextensions

`conda install -c conda-forge jupyter_contrib_nbextensions`

`jupyter contrib nbextension install --user`

- watermark

`conda install -c conda-forge watermark`

## Notebooks

| File Name | Description |
| :-------- | :---------- |
| [311-street-flooding-complaints.ipynb](analysis-nyc-311-street-flooding.ipynb) | Analysis of citywide street flooding complaints in the 311 data set. Analysis includes maps, timeseries, bar plots and other types of visualizations. |
| [assign-complaints-to-streets.ipynb](analysis-assign-complaints-to-streets.ipynb) | Analysis for assigning 311 street flooding complaints to streets. Also includes data visualizations about which streets have the most street flooding complaints, as well as case studies for Midland Beach, Staten Island and Arverne, Queens. |
| [data-wrangling-311-data.ipynb](/data-wrangling/data-wrangling-311-data.ipynb) | Data wrangling for exporting the 311 data using Socrata's API. Note: I signed up for an API key. |
| [data-wrangling-streets-data.ipynb](/data-wrangling/data-wrangling-streets-data.ipynb) | Data wrangling for clipping and extracting NYC streets. |

## Data 

| Data Set | Description |
| :-------- | :---------- |
| [311 Street Flooding Complaints](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data-raw/raw-street-flooding-data.csv) | Raw data for all 311 Service Requests from 2010 to present where descriptor == Street Flooding. |
| [Streets](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data-raw/raw-streets-clipped.json) | Raw data of the NYC Street Centerline (CSCL) data set where street centerline roadway type == Street. |
| [Neighborhood Tabulation Areas]() | Raw data for NYC Neighborhood Tabulation Areas (NTA). |
| [Boroughs]() | Raw data of NYC boroughs. |

Data dictionaries for the data sets above can be found in the [data-dictionaries](https://github.com/mebauer/nyc-311-street-flooding/tree/main/data-dictionaries) folder. 

# Resources

- [NYC Open Data](https://opendata.cityofnewyork.us/)

- [About NYC 311](https://portal.311.nyc.gov/about-nyc-311/)

- [311 Service Requests from 2010 to Present Webpage](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9)

- [Report Street Flooding to NYC 311](https://portal.311.nyc.gov/article/?kanumber=KA-02198)

# Media

- [NYC DOT Facebook post](https://www.facebook.com/NYCDOT/posts/if-you-see-ponding-or-flooding-on-any-nyc-street-or-highway-report-it-to-nyc-311/10156270397437887/) about NYC 311 Street Flooding.

- [NYC 311 Twitter post](https://twitter.com/nyc311/status/1067131135749165056) about NYC 311 Street Flooding.

# Further Reading

Inspiration for the project came from an article by [Localize.city](https://www.localize.city/) titled, "[Puddles or Small Ponds? Where New Yorkers Feel Most Deluged by Street Flooding](https://www.localize.city/blog/puddles-or-small-ponds-where-new-yorkers-feel-most-deluged-by-street-flooding/)."

# Say Hello!   

I can be reached at:  

[Twitter](https://twitter.com/markbauerwater)  
[LinkedIn](https://www.linkedin.com/in/markebauer/)