# Insights into Airbnb Data for the city of Munich, Germany
This project is part of my udacity Data Science Nanodegree Program and has been performed in April 2020. Beside several data analysis approaches it contains a price prediction model.

## Table of Contents

- [Required libraries](#libraries)
- [Motivation for the project](#motivation)
- [Repo Files Description](#files)
- [Results](#results)
- [Sources](#sources)

## Required libraries<a name="libraries"></a>

The project has been realized in Python 3 within the Jupyter Notebook included in this repository.
It requires the following Python libraries: 
- Numpy
- Pandas
- matplotlib 
- Seaborn
- Scikit-Learn
- datetime
- PIL & requests for some helping functions

## Motivation for the project<a name="motivation"></a>

This analysis and the [accompanying blog post](https://medium.com/@frank.merwerth/the-airbnb-business-in-munich-by-the-numbers-619cb812537b) was been created as part of my udacity Data Science Nanodegree program. 
I have chosen the Airbnb dataset for Munich as I live here for almost 20 years.

The analysis will focus on the following questions:

- How much do people charge to rent their homes ? How does this differs between the different city districts and throughout the year ?
- How did the demand develop over time ? Can we already see the impact of the COVID-19 pandemic in the figures ?
- Which are the most important features to predict room / apartment prices ?

## Repo Files Description<a name="files"></a>

`Munich_Airbnb_Data_Analysis.ipynb`:  
This Jupyter Notebook contains all the code and analysis on the above mentioned questions.

The data folder contains the datasets used for the analysis:

`calendar.csv.gz`:  
zipped calendar.csv - contains pricing information for each listed property for a specific day in the upcoming 12 months (4,087,646 datasets)

`listings.csv.gz`:  
zipped listings.csv - listings of rentals with 106 datapoints each like number of persons to accommodate, room type, average pricing information incl. cleaning fee and security deposit, geographical location, and detailed description of the property, the amenities etc.(11,199 datasets)

`reviews.csv.gz`:  
contains reviews.csv - data on reviews between October 2010 and March 2020 (175,413 datasets)

Please note that you have to unzip these files first before running the notebook in case you download or clone the repository.

## Results <a name="results"></a>

The results are doumented in more detail in a [medium blog post](https://medium.com/@frank.merwerth/the-airbnb-business-in-munich-by-the-numbers-619cb812537b).

The key takeaways include:
- Average pricing is at 113 EUR / night but highly fluctuates both between city districts and throughout the season. Ludwigsvorstadt / Isarvorstadt and Altstadt-Lehel are the most expensive districts while the Oktoberfest time is clearly not the right time for bargain hunters.
- The impressive success of Airbnb in recent years is clearly visible in the Munich figures. So is the impact of the COVID-19 pandemic as March 2020 has been the first month ever with a year-on-year drop in reviews and thus bookings
- A prediction model suggests that number of people to accommodate, the number of bedrooms, and the amount that is charged for extra people have the highest influence on the pricing.

## Sources <a name="sources"></a>

The data has been retrieved from the [Inside Airbnb website](http://insideairbnb.com/get-the-data.html) by March 19, 2020. 
