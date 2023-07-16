# Multiple_Linear_Regression_Bike-Sharing_Assignment
> This assignment is a programming assignment wherein you have to build a multiple linear regression model for the prediction of demand for shared bikes.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. 
The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan 
to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
- A model the demand for shared bikes with the available independent variables. It will be used by the management to understand
 how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand
 levels and meet the customer's expectations. 
Further, the model will be a good way for management to understand the demand dynamics of a new market
- 
- 
Dataset characteristics
=========================================	
day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
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
	

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- The best fitted line that we found was 
cnt = 0.5465 + 0.2382 * yr + 0.0371 * workingday - 0.2633 * hum - 0.2071 * windspeed - 0.1583 * season_spring + 0.0361
 * season_winter + 0.0350 * mnth_sept + 0.1858 * temperature_category_mild + 0.1419 * temperature_category_hot - 0.0332 * 
weathersit_moderate + 0.0436 * weekday_saturday
- Demand for shared bikes has been increasing over time (positive coefficient for 'yr'). Expect higher bike rental counts in the future
- Weekdays show higher demand for shared bikes compared to weekends or holidays ('workingday' variable). Target commuters and promote bike rentals for daily commuting purposes
- Unfavorable weather conditions, such as high humidity and wind speed, negatively impact bike rental counts. Consider weather-related promotions and alternative transportation options on such days.
- Winter season shows higher bike rental counts compared to spring ('season_spring' and 'season_winter' variables). Plan marketing campaigns and seasonal offers to capitalize on increased winter demand.
- September shows higher bike rentals. Run targeted promotional campaigns during this month
- Moderate and hot temperatures drive higher bike rental counts ('temperature_category_mild' and 'temperature_category_hot' variables). Market bike rentals as a convenient mode of transportation during these temperature ranges.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- pandas 1.0.1
- Python 3.9

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->




## Contact
Created by [@Nshank22] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
