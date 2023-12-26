# Analyzing NYC's 311 Street Flooding Complaints from 2010 to 2020  
Author: Mark Bauer  

![cover photo](figures/cover-photo.png)   
![daily-and-weekly-counts](figures/daily-and-weekly-counts.png)  
![count-street-segment](figures/count-street-segment.png)  
![midland-beach](figures/midland-beach.png)  
![arverne](figures/arverne.png)

# Table of Contents

   * [Introduction](#Introduction)
   * [Prerequisites](#Prerequisites)
   * [Analysis Notebooks](#Analysis-Notebooks)
   * [Data](#Data) 
   * [Output Data](#Output-Data) 
   * [Data Wrangling Notebooks](#Data-Wrangling-Notebooks)
   * [Open Source Applications Used in Project](#Open-Source-Applications-Used-in-Project)
   * [Resources](#Resources)
   * [Media](#Media)
   * [Further Reading](#Further-Reading)
   * [Say Hello!](#Say-Hello)

# Introduction

Flooding poses a serious threat to coastal cities all around the world, and New York City is no exception. Hurricane Sandy in 2012 devastated the area, with many communities still suffering from its effects or unable to fully recover.  What can citizen science data tell us about where flooding occurs and how it is changing over time? Additionally, how can this data potentially play a role in how New York City prepares and ultimately mitigates flooding in the future?  

In this project, I explored NYC's 311 street flooding complaints data. Specifically, I attempted to answer the following questions:
1. The distribution of street flooding complaints throughout the five boroughs  
2. How street flooding complaints are changing over time  
3. Analyzing street flooding complaints by street  
3. Case studies from Midland Beach, Staten Island and Arverne, Queens  

[![YouTube Video Views](https://img.shields.io/youtube/views/ejgrO5-RatE?label=Watch%20Presentation&style=social)](https://www.youtube.com/watch?v=ejgrO5-RatE)

# Prerequisites

- Basics of Python or other  programming languages (R, SQL, etc.)
- Knowledge of Data Analysis
- Basics of Jupyter Notebooks

This project recommends beginner-level proficiency with Python and is focused on applying Python to data analysis.

# Analysis Notebooks

You can view these notebooks through your browser by clicking *View* under the *Static Webpage* column.  

| File Name | Description | Static Webpage |
| :-------- | :---------- | :------------- |
| [analysis-mapping.ipynb](https://github.com/mebauer/nyc-311-street-flooding/blob/main/analysis-mapping.ipynb) | Analyzing street flooding complaints by location. | [View](https://nbviewer.jupyter.org/github/mebauer/nyc-311-street-flooding/blob/main/analysis-mapping.ipynb) |
| [analysis-timeseries.ipynb](https://github.com/mebauer/nyc-311-street-flooding/blob/main/analysis-timeseries.ipynb) | Analyzing street flooding complaints through time. | [View](https://nbviewer.jupyter.org/github/mebauer/nyc-311-street-flooding/blob/main/analysis-timeseries.ipynb) |
| [analysis-streets.ipynb](https://github.com/mebauer/nyc-311-street-flooding/blob/main/analysis-streets.ipynb) | Analyzing street flooding complaints by street. | [View](https://nbviewer.org/github/mebauer/nyc-311-street-flooding/blob/main/analysis-streets.ipynb) |
| [analysis-streets-case-studies.ipynb](https://github.com/mebauer/nyc-311-street-flooding/blob/main/analysis-streets-case-studies.ipynb) | Analyzing street flooding complaints by street and case studies from Midland Beach, Staten Island and Arverne, Queens. | [View](https://nbviewer.jupyter.org/github/mebauer/nyc-311-street-flooding/blob/main/analysis-streets-case-studies.ipynb) |


# Data 

| Dataset | Description |
| :-------- | :---------- |
| [311 Street Flooding Complaints](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9) | All 311 Service Requests from 2010 to present. |
| [Streets](https://data.cityofnewyork.us/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b) | The NYC Street Centerline (CSCL) is a road-bed representation of New York City streets containing address ranges and other information such as traffic directions, road types, segment types. |
| [Neighborhood Tabulation Areas](https://data.cityofnewyork.us/City-Government/Neighborhood-Tabulation-Areas-NTA-/cpf4-rkhq) | GIS data: Boundaries of Neighborhood Tabulation Areas as created by the NYC Department of City Planning using whole census tracts from the 2010 Census as building blocks. These aggregations of census tracts are subsets of New York City's 55 Public Use Microdata Areas (PUMAs). |
| [Boroughs]() | GIS data of NYC boroughs. |

Data dictionaries for the datasets above can be found in the [data](https://github.com/mebauer/nyc-311-street-flooding/tree/main/data) folder. 
 

# Data Wrangling Notebooks

You can view these notebooks through your browser by clicking *View* under the *Static Webpage* column. 

| File Name | Description | Static Webpage |
| :-------- | :---------- | :------------- |
| [wrangling-street-flooding-query.ipynb](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data-wrangling/wrangling-street-flooding-query.ipynb) | Querying 311 street flooding complaints records from NYC Open Data using the Python library sodapy. | [View](https://nbviewer.jupyter.org/github/mebauer/nyc-311-street-flooding/blob/main/data-wrangling/wrangling-street-flooding-query.ipynb) |
| [wrangling-streets-geom.ipynb](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data-wrangling/wrangling-streets-geom.ipynb) | Cleaning the streets dataset. | [View](https://nbviewer.jupyter.org/github/mebauer/nyc-311-street-flooding/blob/main/data-wrangling/wrangling-streets-geom.ipynb) |
| [wrangling-data-inspection.ipynb](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data-wrangling/wrangling-data-inspection.ipynb) | Inspecting data before analysis. | [View](https://nbviewer.jupyter.org/github/mebauer/nyc-311-street-flooding/blob/main/data-wrangling/wrangling-data-inspection.ipynb) |

# Open Source Applications Used in Project

- [Anaconda](https://www.anaconda.com/): A distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment.  
- [Project Jupyter](https://jupyter.org/index.html): Project Jupyter is a non-profit, open-source project, born out of the IPython Project in 2014 as it evolved to support interactive data science and scientific computing across all programming languages.  
- [Jupyter Notebook](https://jupyter.org/try): The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.  
- [nbviewer](https://nbviewer.jupyter.org/): A web application that lets you enter the URL of a Jupyter Notebook file, renders that notebook as a static HTML web page, and gives you a stable link to that page which you can share with others.  
- [Binder](https://mybinder.org/): The Binder Project is an open community that makes it possible to create sharable, interactive, reproducible environments.

# Resources

- [NYC Open Data](https://opendata.cityofnewyork.us/): Open Data is free public data published by New York City agencies and other partners.  

- [About NYC 311](https://portal.311.nyc.gov/about-nyc-311/): NYC311’s mission is to provide the public with quick, easy access to all New York City government services and information while offering the best customer service. We help Agencies improve service delivery by allowing them to focus on their core missions and manage their workload efficiently. We also provide insight to improve City government through accurate, consistent measurement and analysis of service delivery.  

- [311 Service Requests from 2010 to Present Webpage](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9): 311 dataset on NYC Open Data.  

- [Report Street Flooding to NYC 311](https://portal.311.nyc.gov/article/?kanumber=KA-02198): The 311 portal to report flooding or ponding on a street.

You can run an interactive example on MyBinder through your browser - no installation required: click here [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mebauer/nyc-311-street-flooding/HEAD?filepath=mybinder-example%2Fmybinder_example.ipynb).

# Media

- [NYC DOT Facebook post](https://www.facebook.com/NYCDOT/posts/if-you-see-ponding-or-flooding-on-any-nyc-street-or-highway-report-it-to-nyc-311/10156270397437887/) about NYC 311 Street Flooding.

![nyc_dot_post](images/nyc_dot_post.png) 

- [NYC 311 Twitter post](https://twitter.com/nyc311/status/1067131135749165056) about NYC 311 Street Flooding.

![nyc311_post](images/nyc311_post.png) 

# Further Reading

Inspiration for the project came from an article by [Localize.city](https://www.localize.city/) titled, "[Puddles or Small Ponds? Where New Yorkers Feel Most Deluged by Street Flooding](https://www.localize.city/blog/puddles-or-small-ponds-where-new-yorkers-feel-most-deluged-by-street-flooding/)."

### Say Hello!
Contact information:  
Twitter: [markbauerwater](https://twitter.com/markbauerwater)  
LinkedIn: [markebauer](https://www.linkedin.com/in/markebauer/)  
GitHub: [mebauer](https://github.com/mebauer)

Keywords: *Street Flooding Complaints, Street Flooding, Flooding, Flood, NYC 311, 311, NYC Open Data*