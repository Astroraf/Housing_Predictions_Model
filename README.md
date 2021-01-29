# Housing_Predictions_Model
This project is for Phase 2 at Flatiron School. We just several independent variables from the Kings County housing market in Seattle, Washington to predict what attributes have the greatest impact on selling a house.  

## Precting Housing Prices for Seattle, Washington
Our company was hired to use model predictions to predict our housing prices in the Seatle, WA area. 
In order to make the best possible predictions for the housing market of Seattle, WA, our company 
takes in numerous amounts of paramters that are independent of the price of the house to create the 
best model prediction to inform future buyers. 

<p align="center">
 <img width="1600" height="600" src=images/SeattleWA.jpg>
 </p>

# Overview:

- Explore the data with a train set data that involves our target
- Create visualizations to better understand the interaction of the features we given and decide which are highly correlated
- Clean our data set for any discrepencies
- Create new features that we believe will influence our predictions to the highest possible degree
- Create Polynomial features and dummy variables to see there influence on our model predictions
- Create a split of our target and the variables that we have created to see how well our model performs
- Perfecm model test that select the best features that influence our model predictions
- Perform hypothesis test on several features to make sure that our features influence the price in the way we think they do
- Grab the best features and perform it on our hold data set to see 

# Eploration:

We explore the data set with visualizations of how our variables effect price; if any extreme outliers in are data sets, 
we can correct for these. We first start with see how are data is distrubuted, overlaying a dsitrubuted scale, and check for linearity. 

<p float="left">
  <img src="images/dist_data.png" width="100" />
  <img src="images/theorvslin" width="100" /> 
</p>
 
 Distribution of our data  |  Linear fit to actual data
:-------------------------:|:-------------------------:
![](src=images/dist_data.png)  |  ![](src=images/theorvslin.png)
