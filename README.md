# Investigate-and-analyze-IMBD-dataset
Learning Objectives

- Know all the steps involved in a typical data analysis process
- Be comfortable posing questions that can be answered with a given dataset and then answering those questions
- Know how to investigate problems in a dataset and wrangle the data into a format you can use
- Have experience communicating the results of your analysis
- Be able to use vectorized operations in NumPy and pandas to speed up your data analysis code
- Be familiar with pandas' Series and DataFrame objects, which let you access your data more conveniently
- Know how to use Matplotlib to produce plots showing your findings

Investigated important features from IMBD movie dataset and performed inferential statistics to relate the findings using python libraries like Numpy, Pandas and used Matplotlib to produce plots showing my findings.


The data contains information that are provided from The Movie Database (TMDb). It collects 5000+ movies basic move information and movie matrices, including user ratings, popularity and revenue data. These metrics can be seen as how successful these movies are. The movie basic information contained like cast, director, keywords, runtime, genres, etc. 

The primary goal of the project is to go through the general data analysis process — using basic data analysis technique with NumPy, pandas, and Matplotlib. It contains four parts:
1. AskingQuestions
2. Data Wrangling
3. Exploratory Data Analysis
4. Drawing Conclusion

Requirements:
This project requires Python 3 and the following Python libraries installed:

- Python 3.6.5
- NumPy
- Pandas
- Matplotlib
- Seaborn 

Data cleaning: In the data cleaning process I found that many values were null values in various columns. Hence I droppped null values in cast, genres and director.
The major problem with the data set was of 'zero' values in the dataset  in the revenue and budget column. And more than 50% of the films had 'zero' value in their columns. Which is realyy impossible in reality as there can be no films that had zero budget and revenue too zero. To my surprise that it was in large numbers. Hence I decided to to retain these rows and replace zero values with null values, to keep the integrity of the data.
The same case exists in column 'runtime' , but the zero values in that column very few so I dropped them.

Overall the data was clean and had only one duplicate row and it was dropped. The number of movies in the datset were enough to the analysis and will help us to understand the trend of the movies over the years and its co relation with other variables in better way.

Drawback in the dataset:
 It will be more informative if the actual cost of thee film was also included in the dataset because budget minus revenue is not the accurate way tto calculate the profit made by the movies.
The zero values in the revenue and budget were in excess and hence making calualtions related to these columns would not be a good idea.

#*Insights*:

Budget:- We usually think more is the budget more is the popularity as viewers are more keen to such movies which are expensive due to its expenses spent on technicl effects and locations of shoots or extra vagant expenses to give a best view experience. By the scatter plot I notice that the theres no much co relation between the budget of the movies and its popularity, that is more the budget more is its popularity is not true. There are movies whose budget were more than the other maximum movies but they were not popular.

Popularity:-  I was more curious to know if the popularity of the films, does it increase or decrease over the year with advent of technology and other means of entertainment in our day to day like like plays, game stations and tourism or amusemment parks etc. Through scatter plot I could understand the popularity of films have increased over the years and i think that can be due to innovation in film making of social media in the recent years.

Runtime:-  The question that I explored was that if the runtime is more how is its popularity? 
 The ansWer to it was very much obvious that more runtime, more is the popularity as people prefer a film more engaging with better story and entertain them for atleast 2 hours.


 Directors:- We usually think that directors who make maximum movies must be most popular but this was challenged by the graph that suggested that, client Eastwood made more popular movies than Woody Allen, Though Woody Allen made more movies than Clint Eastwood.
With more other forms of entertainement and inflation, I was curious to know do film makers make more movies or has it decreased over the years, As the years passed we see there was a rise in the number of movies released each year, but a recent drop near 2013-2015.

Ofcourse, I wanted to know the most popular movie in the dataset and Jurassic world was the most popular movie till date and it is not surprisisng to know that as it was indeed block buster movie.
    
It was certainly a great experience to analyze this dataset through various statistical graphs to clear pre concieved notions and know more about the dataset.
