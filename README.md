# Investigating most popular movies on Netflix
This project is part of [Data Scientist with Python](https://app.datacamp.com/learn/career-tracks/data-scientist-with-python?version=5) Career path on [Datacamp](https://app.datacamp.com/learn)

## Files:
* [Investigating-Netflix-Movies-and-Guest-Stars-in-The-Office-Guided.ipynb](https://github.com/Nour-Ibrahim-1290/EDA-Analysis-Netflix-Movies/blob/main/Investigating%20Netflix%20Movies%20and%20Guest%20Stars%20in%20The%20Office-Guided.ipynb): a [Jupyter Notebook](https://jupyter.org/) of the EDA Analysis of Netflix Movies dataset.
* [netflix_data.csv](https://github.com/Nour-Ibrahim-1290/EDA-Analysis-Netflix-Movies/blob/main/netflix_data.csv): dataset on the Netflix movies.

## Explatory Data Analysis steps:
At first; A Firend suggested a list of average movie durations along the years from 2011 to 2020, using that suggestions:
1. years from 2011 to 2020, the average movie durations are 103, 101, 99, 100, 100, 95, 95, 96, 93, and 90, respectively in a [dictionary](https://docs.python.org/3/c-api/dict.html).
2. create a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html?highlight=dataframe#pandas.DataFrame) out of this [dictionary](https://docs.python.org/3/c-api/dict.html).
3. inspecting the relation between year and durations.

![LineChart](https://github.com/Nour-Ibrahim-1290/EDA-Analysis-Netflix-Movies/blob/main/Netflix-Movies-Years-Duration-LineChart.PNG)

Afterwards; reading the netflix_data.csv into a Pandas DataFrame
1. exploaring the data, It contains observations about (type, title, director,	cast,	country,	date_added,	release_year,	duration, and much more!)
2. Filtring the data to contain only Movies, then substting the DataFrame to contain obvservations of (title, country, genre, release_year,	and duration) only.
3. Plotting a [ScatterPlot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html) of the relationship between release_year and duration; we see that while newer movies are overrepresented on the platform, 
   many short movies have been released in the past two decades. 

![ScatterPlot](https://github.com/Nour-Ibrahim-1290/EDA-Analysis-Netflix-Movies/blob/main/Netflix-Movies-Years-Duration-ScatterPlot.PNG)

4. digging deeper on Short movies by filtring the data to Movies of duration less than 60 minutes.
5. seeing a trend in the genre of short movies where alot of them are "Children", "Stand-Up", or "Documentaries", 
   I decided to plot the result with color coded [ScatterPlot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html) based on Genre.
6. Creating colors [list](https://docs.python.org/3/tutorial/datastructures.html) that has has different value for each of these genres and black fro everything else.
7. Plotting the results, while intergrating colors [list](https://docs.python.org/3/tutorial/datastructures.html) in the scatter function, I get..

![colored-ScatterPlot](https://github.com/Nour-Ibrahim-1290/EDA-Analysis-Netflix-Movies/blob/main/Netflix-Movies-Years-Duration-Colored-ScatterPlot.PNG)

## Using these Python Libraries:
* [Pandas](https://pandas.pydata.org/docs/)
* [Matplotlib.pyplot](https://matplotlib.org/stable/users/index.html)
