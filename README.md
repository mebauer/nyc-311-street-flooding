# Analyzing NYC's 311 Street Flooding Complaints from 2010 to Present  
Mark Bauer  
[![YouTube Video Views](https://img.shields.io/youtube/views/ejgrO5-RatE?label=Watch%20Presentation&style=social)](https://www.youtube.com/watch?v=ejgrO5-RatE)

# About The Project
I conducted an analysis of Street Flooding Complaints with NYC Open Data's 311 dataset. 

![cover photo](figures/cover-photo.png)

# Getting Started

## Prerequisites

### Data Science Tools: Anaconda

Download and install [Anaconda](https://www.anaconda.com/products/individual) python distribution.

#### Included Python Libraries

- pandas
- matplotlib
- Seaborn

#### Additional Python Libraries

- Geopandas

`conda install -c conda-forge geopandas`

- geoplot

`conda install -c conda-forge geoplot`

- fiona

`conda install -c conda-forge fiona`

- pywin32

`conda install -c anaconda pywin32`

- jupyter_contrib_nbextensions`

`conda install -c conda-forge jupyter_contrib_nbextensions`

`jupyter contrib nbextension install --user`

- watermark

`conda install -c conda-forge watermark`

## Notebooks

| File Name | Description |
| :-------- | :---------- |
| [311-street-flooding-complaints.ipynb notebook](analysis-nyc-311-street-flooding.ipynb) | Analysis |
| [data-wrangling-311-data.ipynb notebook](/data-wrangling/data-wrangling-311-data.ipynb) | Data wrangling for exporting the 311 data using Socrata's API |
| [assign-complaints-to-streets.ipynb notebook](analysis-assign-complaints-to-streets.ipynb) | Data wrangling for assigning complaints to streets |
| [data-wrangling-streets-data.ipynb notebook](/data-wrangling/data-wrangling-streets-data.ipynb) | Data wrangling for clipping and extracting only NYC streets |

## Data 

| Dataset | Description |
| :-------- | :---------- |
| [311 Street Flooding Complaints](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data/311-flooding-data.csv) | |
| [Streets](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data/streets_clipped.json) | |
| [311 Data Dictionary](https://github.com/mebauer/nyc-311-street-flooding/blob/main/data/311_SR_Data_Dictionary_2018.xlsx) | |

# Further Reading

Inspiration for the project came from an article by [Localize.city](https://www.localize.city/) titled, ["Puddles or Small Ponds? Where New Yorkers Feel Most Deluged by Street Flooding."](https://www.localize.city/blog/puddles-or-small-ponds-where-new-yorkers-feel-most-deluged-by-street-flooding/) 

# Say Hello!   

I can be reached at:  

[Twitter](https://twitter.com/markbauerwater)  
[LinkedIn](https://www.linkedin.com/in/markebauer/)