# udacity_datascience_prj_01 - AirBnB data analysis
This project is the first project of the udacity nanodegree for datascience. 

It is an analysis of AirBnB dataset for Berlin and some statistical data about Berlin's population. The analysis was done in Jupyter Lab notebook. 
The repository contains the jupyter lab notebook. The datasets have to be downladed from the original sources.


# Installation of the environment


## with Anaconde - Reccomended way 
* conda create -n prj_env
* conda config --env --add channels conda-forge
* conda config --env --set channel_priority strict
* conda install python=3 geopandas
* conda install jupyterlab matplotlib seaborn scikit-learn scipy

(see also requirements.txt)


## References

|Resource                      | Reference                                                                                            | Description |
|----------------              |------------------------------------------------------------------------------------------------------|-------------|
|Data                          | http://insideairbnb.com/get-the-data.html / 12th of March 2021                                       | AirBnB data sets|
|Data Dcitionary               | https://docs.google.com/spreadsheets/d/1iWCNJcSutYqpULSQHlNyGInUvHg2BoUGoNRIGa6Szc4/edit?usp=sharing | AirBnB data dictionary describes the data set columns|
|Zip Code areas and Population | https://www.suche-postleitzahl.org/downloads                                                         | zip codes and their geolocation polygon together with population |
|mapping_neighboorhood_zip     | https://www.statistik-berlin-brandenburg.de/produkte/verzeichnisse/ZuordnungderBezirkezuPostleitzahlen.xls | mapping of berlin neighbourhoods on zip codes. **Note** The file under the link this is raw data that needs to be formatted to get the result of this file|


## The datasets
|File                          | Description                                                                                           |have to be downloaded|
|----------------              |-------------------------------------------------------------------------------------------------------|-----|
airbnb_calendar.csv            | price per day and listing                                                                             | yes |
airbnb_listings.csv            | Summary of AirBnB Listings (offers) in Berlin (see data dictionary for column desc )                  | yes |
airbnb_listings_dtl.csv        | Details of AirBnB Listings (offers) in Berlin                                                         | yes |
airbnb_neighbourhoods.csv      | neighboorhoods (district areas)                                                                       | yes |
airbnb_neighbourhoods.geojson  | geometry of the neighbourhood as polygon                                                              | yes |
mapping_neighbourhood_zip.csv  | zip code -> neighbourhood mapping / assigns each zip code a neighbourhood it belongs to               | **no** |
plz_einwohner.csv              | population per zip code area                                                                          | yes |
plz-gebiete.shp                | geometry (as polygon) for zip code areas                                                              | yes |
zuordnung_plz_ort.csv          | zip code to city (city area) assignment                                                               | yes |
zuordnung_plz_ort_landkreis.csv| zip code to city (city area) assignment                                                               | yes |


# Jupyter Notebook
The analysis is done in **airbnb_project_02.ipynb**