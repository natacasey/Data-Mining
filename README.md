![Marvel Characters](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/marvel_image.jpg)
## Project Description

The focus of this project is data wrangling using data related to Marvel comic characters. Most of the data is categorical data of descriptive nature. 
The data came from three sources: a flat csv file from [kaggle](https://www.kaggle.com/fivethirtyeight/fivethirtyeight-comic-characters-dataset),
[ComicVine](https://comicvine.gamespot.com/api/documentation) API, and a website [marvel.com](https://www.marvel.com/characters).
After the three sources have been processed using pandas, regex, fuzzy matching, deduplication and other techniques, they were merged by character name and loaded into an SQLite database. 

## Development
Programming language - python 3.7. OS - Windows 10 Home. Library for scraping - Beautiful Soup. API - [ComicVine](https://comicvine.gamespot.com/api/)

Resulting dataframe:

![Dataframe](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/dataframe.PNG)


The data was anayzed with the help of visualizations created from the data loaded into SQLite.

![Word cloud](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/Word_cloud.PNG)

## Challenges of the project:

- The data on marvel.com is not arranged in one table which complicates the way the data is scraped. All of the URL-addresses with the information about Marvel characters from marvel.com sitemap need to be scraped. The rest of the data is obtained by looping through the URL-addresses and scraping the necessary information. 
- When pulling the data from the API only 100 observations are allowed per request. Filtering by the publisher can not be done when sending a request. Due to the pagination and lack of filtering by the publisher data pulling is time-consuming. 

## Future Use
The final dataset is cleaned and ready for further types of analysis, for example, classification analysis.  



