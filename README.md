# Assisting car buyers on cars.com in finding the best deals

For full presentation, click [here.](https://github.com/riwasabri/Regression-/blob/master/Regression%20-%20Presentation.pdf)

## **Abstract** 
The goal of this project is to build a linear regression model that would predict the price of used
cars in a 20 miles radius of the following ZIP Code: 11221 in New York. The model can be used
to understand what drives the price of a used or certified car by looking at features including but
not limited to: mileage,average mpg, accidents reported, model,make,year,engine
specifications,color,etc..

## **Design**
Features were created from scraped cars listings on Beautiful Soup. The goal being to use
these features to make predictions on used car prices in the radius defined above.
Baseline Model was created using numerical features: engine displacement,
year,make,model,mileage,convenience count, entertainment count, safety count. After that
additional feature engineering was performed on categorical and numerical variables to improve
R^2 and MSE scores.

## **Data**
Data was gathered from the website Cars.com using Beautiful Soup.
Initial Data Cleaning consisted of breaking down categorical and numerical variables into further
categories so they are interpretable, the examples listed below are non-exhaustive:
	
* Extracting Make,Year, Model from Name
* Counting the number of safety,convenience and entertainment features by cars
* Further breaking down categorical features to be relevant to the problem, for example
engine was broken down into valvetrain and engine displacement

## **Algorithm**
**Feature Engineering**:
	
* Adding Polynomial Relationship Year vs Price
* Dummy Variable Creation: Make, Model, Valvetrain Type
*  Interaction Variable : High Mileage x Luxury Cars
* Log Transformation of Target

**Models Used**:
OLS, Ridge,Lasso,Polynomial Regression

## **Tools**
	
* Web Scraping: Beautiful Soup
* Data Analysis and Cleaning: Pandas,Geopy
* Modeling: Scikit-learn,Statsmodel
* Data Visualization: Matplotlib,Seaborn
