# Predicting Food Delivery Time – Hackathon by IMS Proschool
This a machine learning hackathon brought together by Analytics India Magazine and IMS Proschool in the MachineHack platform.

As the title reads this competition was about building a machine learning model to predict food delivery time of the orders places online. The data is taken from restuarnt spread across few cities across India. 

Link : https://www.machinehack.com/course/predicting-food-delivery-time-hackathon-by-ims-proschool/

I bagged the 3rd place in the Hackthon.

## Features available
* Restaurant: A unique ID that represents a restaurant.
* Location: The location of the restaurant.
* Cuisines: The cuisines offered by the restaurant.
* Average_Cost: The average cost for one person/order.
* Minimum_Order: The minimum order amount.
* Rating: Customer rating for the restaurant.
* Votes: The total number of customer votes for the restaurant.
* Reviews: The number of customer reviews for the restaurant.
* Delivery_Time: The order delivery time of the restaurant. (Target Classes) 

## Approach
Try as many new features as possible and ensemble models using different combination of features

## Feature Engineering
* Average reviews, rating, voting of each of the restaurant. 
* Extracting the city from the Location feature
* Convert the cusines features into OHE which creates one feature for each of the cuisine.

## Final Model
The final model that gave good accuracy was an Ensemble of 2 Random Forest models each of them taking few features that are not available in the other. The Ensemble was done by taking the mean of the predition probabilities of each of the classes from the 2 models
