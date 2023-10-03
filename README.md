==========================================================================
# Bike-sharing-assignment
==========================================================================
#### Built a linear regression model for the prediction of demand for shared bikes.
==========================================================================
**You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.** 

==========================================================================
## General Information
==========================================================================

	- This case study is based on Predictive Analytics and Linear Regression(Machine Learning). Multiple linear regression is performed on the dataset.
	- It also consists of a separate PDF file that has answers to all the subjective questions that were given to us as part of the assignment.
	- I have done this case study assignment as part of the Executive PG Diploma program of UpGrad in collaboration with IIIT Bangalore. 
	- Language used: Python for Data Science. Tools Used - MS Excel

==========================================================================
## Business objective
==========================================================================

>The objective is to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

==========================================================================
## Project Statement
==========================================================================

> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short-term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


==========================================================================
## Data Set
==========================================================================

> day.csv has the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from https://usoas.usmission.gov/holiday-calendar/ & https://www.commerce.gov/hr/employees/leave/holidays)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered


==========================================================================
## Methods Usedology
==========================================================================

* Reading and Understanding the Data
* Exploratory Data Analysis
* Data Visualization
* Data Preparation for Linear Regression
* Data Modelling with Train & Test Set
* Data Evaluation

==========================================================================
## Technologies Used
==========================================================================

	- Python -version 3.11.3
	- Pandas - version 1.5.3
	- NumPy - version 1.23.5
	- Seaborn - version 0.12.2
	- MatplotLib - version 3.4.3
	- Plotly - version 5.7.0
	- statsmodels - version 0.12.2
	- sklearn - version 0.24.2
	- scipy - version 1.7.1
	- Jupyter Notebook - Version 6.5.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of the library used in this project -->


==========================================================================
## Problem Statement
==========================================================================

>A US bike-sharing provider BoomBikes a Mobility Services firm has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

>Essentially the company wants :
	- To understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19, by creating a linear model.
	- To identify the variables affecting their revenues i.e. Which variables are significant in predicting the demand for shared bikes.
	- To know the accuracy of the model, i.e. How well those variables describe the bike demands

>They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


==========================================================================
## Problem Solving Methodology
==========================================================================

* Data Understanding-
> Understanding and working with the data dictionaries and getting good knowledge of all the columns and their domain-specific uses.
* Data Visualization-
> Perform EDA to understand various variables.
> Check the correlation between the variables.
* Data Preparation for Linear Regression-
> Create dummy variables for all the categorical features.
> Divide the data to train and test the Set.
> Perform Scaling.
> Divide data into dependent & Independent variables.
* Data Modelling & Evaluation-
> Create a Linear Regression model using a mixed approach (RFE & VIF/p-value).
> Check the various assumptions.
> Check the Adjusted R-Square for both train and test data.
> Report the final model.


==========================================================================
## Motivation
==========================================================================
>Several bike/scooter ride-sharing facilities have started up lately, especially in metropolitan cities like San Francisco, New York, Chicago, and Los Angeles, and one of the most important problems from a business point of view is to predict the bike demand on any particular day. While having excess bikes results in wastage of resources (both with respect to bike maintenance and the land/bike stand required for parking and security), having fewer bikes leads to revenue loss (ranging from a short-term loss due to missing out on immediate customers to potential longer-term loss due to loss in future customer base), Thus, having an estimate on the demands would enable efficient functioning of these companies.

==========================================================================
## Important Points to remember while solving the Assignment :
==========================================================================

	- The commands are syntactically correct.
	- The output of the code is correct in terms of the question and format.
	- The data frame has been thoroughly inspected using the taught commands.
	- In the case of dataframes, the results contain the same rows and columns as expected
	- Regarding plots, making appropriate charts with the mentioned libraries and getting the right trends. Writing clear and concise inferences for the charts wherever asked.
	- The code is concise. Wherever appropriate, built-in functions are used instead of making the code longer (if-else statements, for loops,loc/iloc ).
	- If new variables are created, the names are descriptive and unambiguous. Following the variable/dataframe names mentioned in the question wherever it is provided.
	- Charts are neatly formatted including proper chart sizes, annotations(if required) and labeling.
	- Mention the inferences for each of the graphs after thoroughly inspecting them.

==========================================================================
## Conclusions
==========================================================================
>We explored several types of information that influence bike rental count. Hence, it can be clearly concluded that the Significant variables to predict the demand for shared bikes are:

	- Holiday & Sunday: We see 2 rental patterns across the day in bike rentals count - first for a Working Day where the rental count is high at peak office hours (8am and 5pm) and the second for a Non-working day where the rental count is more or less uniform across the day with a peak at around noon.
	- temp (Temperature): People generally prefer to bike at moderate to high temperatures.
	- hum (Humidity): With increasing humidity, we see a decrease in the number of bike rentals count.
	- windspeed
	- Season
	- months(January, July, September, November, December) should be considered by the company as they have a higher demand as compared to other months.
	- Year (2019): The year 2019 had a higher count of users as compared to the year 2018. Based on previous data it is expected to have a boom in the number of users once the situation comes back to normal, compared to 2019.
	- weathersit( Light Snow, Mist + Cloudy): As one would expect, we see the highest number of bike rentals on a clear day and the lowest on a snowy or rainy day

==========================================================================
## Acknowledgements
==========================================================================
>This project was inspired by UpGrad IITB Programme as a case study for the Machine Learning and Artificial Intelligence course.


==========================================================================
## Contributors
==========================================================================
- [Debasish Deaty]
 - Email: ddeaty@gmail.com 
- (https://github.com/ddeaty/)

==========================================================================
