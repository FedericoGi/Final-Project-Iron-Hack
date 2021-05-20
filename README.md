# Prediciting Car Prices With Machine Learning

![Picture](https://github.com/FedericoGi/Final-Project-Iron-Hack/blob/main/3.%20Pictures/EV-vs-Gasoline.jpg)

# Contents:

- [Introduction](#Introduction-to-the-project-and-tools-used)
- [Method and approach](#Method-and-approach)
- [Initial insights](#Insights-into-the-data)
- [Models and evaluation](#Model-application)
- [Tableau](#Insights-using-Tableau)
- [Conclusion](#Last-words)
***


## Introduction to the project and tools used

The automotive industry is changing really fast. With this in mind I decided to elaborate an overview of the major trends and an in-depth analysis of the United States car market during the late 80's to be compared to today's EV - electric vehicle - market. 

I'll analyze customer trends, prices, number of cars sold, and much more in order to evidence the main difference between the growing market of electric cars and the 1987 US car market. I did build machine learning models that would help us to predict the prices for both markets based on our two dataset. 

Both set of data have been extracted from the website www.kaggle.com. 

Additionally, I wanted to explore some relationships within the data using visualizations to make these relationships easy to consume for the stakeholders and decision-makers. I used Tableau to achieve this goal. After our analysis was completed, I'll deliver our insights in a 5-minute presentation, focussing on the business implications of our results. 

I hope you will enjoy the ride!


## Method and approach

It was important to keep a flexible structure and an agile approach, to be able to handle bugs and errors that occurred during the process, thus I used the tool Trello in order to track the tasks and progress. 
I used Python for the prediction of prices, data wrangling amd cleaning.

## Insights into the data

### Automobile Dataset: 
This data set consists of three types of entities: (a) the specification of an auto in terms of various characteristics.
Below you can find the correlation among the variables of the dataset.


![Picture](https://github.com/FedericoGi/Final-Project-Iron-Hack/blob/main/3.%20Pictures/Screenshot%202021-05-17%20at%2021.21.38.png)


### Electric Vehicle Dataset:
When looking for simple datasets on EVs, there don't seem to be any. Also, given the growth in this market, this is something many would be curious about. Hence, the reason for creating this dataset.
Below you can find the correlation among the variables of the dataset.

![Picture](https://github.com/FedericoGi/Final-Project-Iron-Hack/blob/main/3.%20Pictures/Screenshot%202021-05-17%20at%2021.22.10.png)



## Model application

### Linear regression model 

R2 score of 0.884 and an RMSE of 3980.9320 for the Automobile Dataset. The features that has been taken into consideration are width, curb weight, engine size, and horsepower. 

R2 score of 0.717 and an RMSE of 16562.6295 for the EV Dataset. The features that has been taken into consideration are topspeed, range of kilometers, and efficiency (or the amount of energy the vehicle neeed to cover 1 km).


Actual prices VS Predicted prices in 1987 market. 

![Picture](https://github.com/FedericoGi/Final-Project-Iron-Hack/blob/main/3.%20Pictures/Automobile%20Actual%20vs%20predicted.png)

Actual prices VS Predicted prices in EV market. 

![Picture](https://github.com/FedericoGi/Final-Project-Iron-Hack/blob/main/3.%20Pictures/EV%20actual%20vs%20predicted.png)

***

The result achieved with the linear regression has been already positive.

## Insights using Tableau

I created a Tableau Public story that can be view [here](https://public.tableau.com/profile/federico.giuliani#!/vizhome/1987CarmarketsVSTodaysElectricVehicles/PowertrainEV?publish=yes)
Within the tableau folder you can find more charts and visual [here]

## Conclusion

The linear regression model I have used gave me reliable outcome as confirmed with the R2 score calculation. Thus I can use the selected features of a car in order to predict prices. 
The powertrain structure changed over decades. Today car manufacturers are building more All-Wheel drive than the late 80's when Rear wheel and Front wheel drive were more common on vehicles. 
Car buyers in the late 80's were paying more for a vehicle that had more horsepower which means larger size of engines and higher gasoline consumption and less efficiency. The price of electric vehicles will depend mainly on the range of kilometers and the efficiency. 
There are some brands of car that have their strong presence both in 1987 and today's market. Among them we can find Audi, Volkswagen, BMW, Porsche, Volvo. 
Finally, the body type of cars changed during the years with an increase in production for SUV (Sport Utility Vehicle) and body style like hatchback that maintain their shares in this category. 

For the future we could expect a predominancy of SUV vehicle with 4 wheels drive and their value/price will be very likely depending from factors like the autonomy with one charge and their efficiency. 

Thank you very much! 


***


