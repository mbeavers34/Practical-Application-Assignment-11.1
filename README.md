# Practical-Application-Assignment-11.1
Practical Application Assignment 11.1: What drives the price of a car?
My initial plan is to:
#1 Remove every row from the data that contains an NaN.
The original data contains several thousand entrys, so removing bad data  will still allow for a large number of automobiles to be used for evaluation,
#2 Look for features (year, odometer reading, condition, etc.) that has a high corelation to price. I will look at the absolute value (abs) of the corelation becuase a high negative still has a high correlation, it just meanst that when the value of the feature is high the price tends to be lower.

#3 I will then test the features against smaller sets of data, for instance "F-150's" or "Camry's" only, to see if the same items are still highly correlated.

#4 I will them test on the type of vehicle, e.g. "sedan" or "truck"

Since I am assuming that the car dealer is interested in selling the most cars/trucks, I will select the models and type from the top 3 selling vehicles.

How the plan unfolded.
The data is messy. Lots of NaN's, and possible similar but different e.g. F-150 and F150. I did remove the large # of NaNs, but left the similarbut differet data alone. I also ended up running several types of regressions hoping to find something consistant, but was ultimatly dissapointed in being able to predict prices on the entire data set.  Price prediction by model or type were much better. 

The final analysis: 
There are only two factors in a used car that are consistent between the different makes and models of cars. These are Milage and odometer reading. 
Taking all makes and models into consideration, the factors that had the highest correlations with vehicle price were:
Odometer 	0.565981 - lower is better
Sedan 		0.315413 - Sedans tend to price more consistantly than other models        
Year 		0.290314 - newer is better
Diesel		0.272973
Gas 		0.267274 - electric vehicles prices are inconsistant
Pickup  	0.256121 - pickups tend to price more consistantly than other models 

The best selling used vehicles were from 2013 and had a transmission type of other
The top 5 best sellers were the F-150, Silverado, Corvette, Wrangler, and the Altima.
Automobiles in excellent, good, or like new shape sold for similar average prices.
The top 4 sellers were Sedan, SUV, Truck, and Pickup.
The top 4 makes were Chevy, Ford, Toyota, Nissan
White, Black and Silver were the highest selling, with White, Black, Red, and Yellow bringing the hiest prices 
When broken down by model, the top factors for price were:
F-150 -		year - odometer reading, condition 
Silverado - year, odometer, condition
Corvette – 	odometer, year, condition
Altima -	year, odometer, condition

When broken down by type, the top factors for price were:
Sedan - 	year, odometer,  all other factors were minor
SUV - 		year, odometer, gas (gas mas a minor consideration) 
Truck- 		year, odometer, diesel 0.407, gas 0.401, condition 0.33

Final recommendation:  White or Black, 2013 model or newer, low milage trucks or sedans that are made by Chevy, Ford, Toyota, Nissan, Jeep or Honda. These should typically be in excellent to good condition and do not have manual transmissions. (Tranmission type other had higer average prices than either auto or manual.) 

Note: Accurate price prediction must be done on a model to model basis and each model may have a particular set of features that make it more valuable in that context. For instance, diesel fueled may be a valuable feature in a truck but a negative feature for a sedan.
