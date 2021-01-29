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

![alt-text-1](images/dist_data.png "Distrubtion of Data") ![alt-text-2](images/theorvslin "Theortical vs Linear fit")

We can see that are data set is not normally distrubted and this is skewed to the right. We can correct this by cleaning up our data set,
and checking for outliers. As well we can see that our data fits a more exponential curve rather than a linear fit line. This will all be 
corrected for when we clean up our data, create new features and pick what features will produce the best model.

# Features

* id - unique ID for a house
* date - Date day house was sold
* price - Price is prediction target
* bedrooms - Number of bedrooms
* bathrooms - Number of bathrooms
* sqft_living - square footage of the home
* sqft_lot - square footage of the lot
* floors - Total floors (levels) in house
* waterfront - Whether house has a view to a waterfront
* view - Number of times house has been viewed
* condition - How good the condition is (overall)
* grade - overall grade given to the housing unit, based on King County grading system
* sqft_above - square footage of house (apart from basement)
* sqft_basement - square footage of the basement
* yr_built - Year when house was built
* yr_renovated - Year when house was renovated
* zipcode - zip code in which house is located
* lat - Latitude coordinate
* long - Longitude coordinate
* sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
* sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors

We first want to see how each feature is skewed and if any outliers exist.

<p align="center">
 <img width="1600" height="600" src=images/botpltfeat.png>
 </p>


 
