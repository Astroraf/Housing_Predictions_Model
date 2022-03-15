
# Kings County Housing Prediction 
<p align="center">
 <img width="800" height="500" src=https://media.istockphoto.com/photos/seattle-skyline-at-night-with-mt-rainier-in-the-distance-picture-id464852512?k=20&m=464852512&s=612x612&w=0&h=80x0r_rZbc8UOLlRd0xjWCpZZm5gJuNlFSyCqvWZvpY=
 </p>


# Overview:

With a such a monumental time occuring with one of the first pandemics to hit the modern times we have seen a lot of the US ecoonomy hit hard by this significant event. One sector that has not quite well is the housing market. According to Zillow, for the year 2020, 5.64 million homes were sold in 2020, with a 5.6% increase from 2019. People are moving away from cities and finally purchasing their forever homes because of the current situation. Thankfully, we have current technologies that enable us to predict housing locations based on square feet living, number of bedrooms to bathrooms, proximity to certain locations among others charactistics of the home.

This project aims at utlizing mutliple linear regression models to predict housing prices in the Kings County, Seatle WA area. The training data will be explored for any errors then use feature building, with the final model being built with SciKit learn python library. The data and scope of the project phase 2 was provided by Flatiron School for Data Science Immersive proogram.

# Repository Structure
    .
    ├── working_notebooks                  # project notebook with EDA/model implementation/Regression Models
    ├── images                             # project image/graph files
    ├── pickle                             # final regression models pickle
    └── README.md

# Business Problem:

Using a list of houses with all the same features to predict housing prices using contextual data from the Kings County, Seattle WA area. I am aiming to generate accurate predictions of the price of the housing that will aid real estate agents in the selling of the house to maximize profits that are interested in using this model. I will using a multiple linear regression model to create predictions based on the property data.

# Approach
1. Check for data completeness and integrity
2. Perform EDA with statistical analysis to determine statistically significant features
3. Visualize statistically significant features
4. Engineer new features based on statistical findings
5. Model Linear Regression models and evaluate each model for final implementation
6. Implement feature engineering and final model to the data set.

# Analysis
Upon basic analysis of the range of properties that we have we see a large a majority of the properties range below $100,000. This would make the most sense as most likely people are buying their first home.

<p align="center">
 <img width="500" height="400" src=images/PriceRange_Count.png
 </p>

Upon futher analysis of the houses that have renovations and houses that did not have renovations we saw a dramatic increase in price, as well as having a basement in the house. The basement did not increase the value as much as being newly renovated but still had some affect on the pricing of the house.

<p align="center">
 <img width="700" height="400" src=images/basement_renov.png
 </p>


Looking at the pricing for homes with more than 5 bathrooms greatly increased the value of the home, but also futher analysis concluded that a home with more than 15 bathrooms where outliers and most likely an improper input into the database.

<p align="center">
 <img width="500" height="400" src=images/AvgPriceBath.png
 </p>



Looking further into the quality grade of the house. We see exponential increase in the value of the house if the house was graded at higher level then a 6, in comparison to the average cost of a house being $540,800.

<p align="center">
 <img width="500" height="400" src=images/AvgPriceGrade.png
 </p>

#Modeling
Used Scitkit-learn package of 3 linear regression models were created.

* Simple Linear Regression Model
* Linear Regression with Recursive Feature Elimination/Selection
* Linear Regression with Recursive Feature Elimination/Selection with Cross Validation

# Summary
After completing King County Housing prices data analyzation, predictive models were then created. The most significant factors that affected the value of the price were coondition, grade, renovation, zip code, and waterfront. A baseline model was created with a simple LinearRegression model from statsmodel library. Once I had a basis for my model, I then applied Scikit-learn libraries to achieve a root mean squarred errors of $144,000 on the test data and $168,000 on the train data set. With a 17% difference without overfitting the model. The largest impact on the linear regression model was the dummy variables created via the zipcodes.

# Further work
To apply geopandas to the locations of the houses in comparison to downtown and other major landmarkets. Create a visualization of prices and locations of each house being sold.
