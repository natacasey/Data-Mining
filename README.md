# Wrangling_Marvel_Data_with_Python

![Marvel Characters](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/Marvel.jpg)
## Project Description

The focus of this project is data wrangling using data related to Marvel comic characters. Most of the data is categorical data of descriptive nature. 
The data came from three sources: a flat csv file (downloaded from [kaggle](https://www.kaggle.com/fivethirtyeight/fivethirtyeight-comic-characters-dataset),
API ([ComicVine](https://comicvine.gamespot.com/api/documentation) API), and a website ([marvel.com](https://www.marvel.com/characters)).
After the three sources have been processed using pandas, regex, fuzzy matching, deduplication and other techniques, they were merged by character name and loaded into an SQLite database. 

Resulting dataframe:

![Dataframe](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/final_df.PNG)


The data was anayzed with the help of visualizations created from the data loaded into SQLite.
![Pie Chart](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/pie_chart.PNG)


Word cloud was used to display the most popular Universes taht Marvel characters come from.

![Word cloud](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/Word_cloud.PNG)

## Challenges of the project:

- The data on marvel.com is not arranged in one table which complicated the way the data was scraped. All of the URL-addresses with the information about Marvel characters from marvel.com sitemap needed to be scraped. The rest of the data was obtained by looping through the URL-addresses and scraping the necessary information. 
- When pulling the data from the API I had to work with pagination (only 100 observations were allowed per request).  Filtering by publisher couldn't be done when sending a request. I had to pull the information about comic characters from all publishers which resulted in a big number of records. Due to the pagination data pulling took a long time to complete the request. 

## Use
The final dataset is cleaned and ready for further types analysis, for example, classification analysis.  



