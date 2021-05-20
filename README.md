# Prediciting Car Prices With Machine Learning

![Picture](https://github.com/Caparisun/data_mid_bootcamp_project_regression/blob/master/Pictures/real-state-project.jpg)

# Contents:

- [Introduction](#Introduction-to-the-project-and-tools-used)
- [Deliverables](#Deliverables)
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


## Insights into the data

### Automobile Dataset: 
This data set consists of three types of entities: (a) the specification of an auto in terms of various characteristics, (b) its assigned insurance risk rating, (c) its normalized losses in use as compared to other cars.

INSERT IMAGES CORRELATION 

### Electric Vehicle Dataset:




The distribution of a few important variables to our model:
Even though some of our variables had large outliers, we decided to keep them the way they are. We made this decision based on our experience with real estate markets, where outliers and skewed data usually have a meaning to them, and we didn't want to artificially change the influence of these variables on our model. In a later iteration it turned out to increase accuracy of the model, when some data ins transformed and outliers get removed.

![Picture](https://github.com/Caparisun/data_mid_bootcamp_project_regression/blob/master/Pictures/ditribution.png)

The relationship of price and living space of a unit:
As expected, price and living space appear positively correlated.

![Picture](https://github.com/Caparisun/data_mid_bootcamp_project_regression/blob/master/Pictures/sqftprice.png)

We also used a correlation matrix to identify variables that mean the same things and decided to only move forward with one of those correlated variables.


## Summary of the initial findings

After the initial exploration, we evaluated variables for the model and decided on features used for the first iteration. Datasets have been explored and wrangled where we have selected the numricales variables that are higher related to car prices. 


## Model application

### Linear regression model 

R2 score of 0.884 and an RMSE of 3980.9320 for the Automobile Dataset

R2 score of 0.717 and an RMSE of 16562.6295 for the EV Dataset


![Picture](https://github.com/Caparisun/Linear_Regression_Project/blob/master/Pictures/linear.png)
***

The result achieved with the linear regression has been already positive.

If you want to get insights into the process please check the [notebook](https://github.com/Caparisun/Linear_Regression_Project/blob/master/Notebooks_and_data/6.Refinement.ipynb)


## Conclusion

We do believe that the model is quite sufficient, but can't be used solely to predict the actual sales price of a home without viewing the home in reality. This is due to the large RSME error in the model. Additionally, variables that have a high impact on real estate prices like the neighborhood, location, and urban development were not scored in the dataset and are therefore excluded from the model.

To increase the precision of the model, the variables that include mostly zero values have to be resampled and balanced. We also assume that binning more values into groups could increase accuracy. 
We could not identify a causal relationship between high prices and a single variable, it seems like to correlation of multiple values lead to higher prices.


## Insights using Tableau

I created a Tableau Public story that can be viewes [here](https://public.tableau.com/profile/federico.giuliani#!/vizhome/1987CarmarketsVSTodaysElectricVehicles/PowertrainEV?publish=yes)


You can view a preview of our Tableau story below:

<div class='tableauPlaceholder' id='viz1618994686440' style='position: relative'><noscript><a href='#'><img alt='Prediciting House Prices With Linear Regression - Data exploration and visualization ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Mi&#47;Mid_Project_Data&#47;StoryProject&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Mid_Project_Data&#47;StoryProject' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Mi&#47;Mid_Project_Data&#47;StoryProject&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='de' /><param name='filter' value='publish=yes' /></object></div>


***

## Conclusion
#### Insights delivered

- Don't use the model solely to make investment decisions, but rather for confirming a price range of an asset
- Invest with an anticyclical approach
- Maximize living space instead of bedrooms to increase price
- Bellevue is the most expensive area
- We were unable to identify a single variable the allows to predict higher prices  

Thank you for your time!
We hope that our insights provide detailed answers to the questions. If there are any further questions, please don't hesitate to reach out!

