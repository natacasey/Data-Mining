# Wrangling_Marvel_Data_with_Python

![Marvel Characters](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/Marvel.jpg)
## Project Description

The focus of this project is data wrangling using data related to Marvel comic characters. Most of the data is categorical data of descriptive nature. 
The data came from three sources: a flat csv file (downloaded from [kaggle](https://www.kaggle.com/fivethirtyeight/fivethirtyeight-comic-characters-dataset),
API ([ComicVine](https://comicvine.gamespot.com/api/documentation) API), and a website ([marvel.com](https://www.marvel.com/characters includes)).
After the three sources have been processed using regex, fuzzy matching, deduplication and etc., they were merged and loaded into an SQLite database. 

Resulting dataframe:
![Dataframe](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/final_df.PNG)


The data was anayzed with the help of visualizations created from the data loaded into SQLite.
![Pie Chart](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/pie_chart.PNG)


World cloud was used to represent the distribution of the Universes the Marvel characters come from.

![Word cloud](https://github.com/natacasey/Wrangling_Marvel_Data_with_Python/blob/master/_assets/Word_cloud.PNG)



