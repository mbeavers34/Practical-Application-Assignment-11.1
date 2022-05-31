# Practical-Application-Assignment-11.1
Practical Application Assignment 11.1: What drives the price of a car?
My initial plan is to:
#1 Remove every row from the data that contains an NaN.
The original data contains several thousand entrys, so removing bad data  will still allow for a large number of automobiles to be used for evaluation,
#2 Look for features (year, odometer reading, condition, etc.) that has a high corelation to price. I will look at the absolute value (abs) of the corelation becuase a high negative still has a high correlation, it just meanst that when the value of the feature is high the price tends to be lower.

#3 I will then test the features against smaller sets of data, for instance "F-150's" or "Camry's" only, to see if the same items are still highly correlated.

#4 I will them test on the type of vehicle, e.g. "sedan" or "truck"

Since I am assuming that the car dealer is interested in selling the most cars/trucks, I will select the models and type from the top 3 selling vehicles.
