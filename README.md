# Optimizing-app-offers-with-Starbucks

## Project Overview <br>
Promotional offers are a great way for Starbucks to attract customers' attention and motivate them to buy. 
In this project, a simulated dataset, that mimics 17,000 customers' behavior on the Starbucks reward mobile app, was used. This dataset is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of product. As a simplification, there are no explicit products to track, and only the amounts of each transaction or offers of users are recorded. In this simulation, once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. 


## Problem Statement<br>
Offers are used effectively to increase sales, but they need to be used correctly and viewed as a selling expense. Determining what to offer, how to offer, and who to offer is the key. Since there is no harm to the profit by sending the informational offer, I will focus on optimizing the BOGO and discount offers. For the profit, the BOGO and discount offers will not be sent to those, who will buy without offers and who will not buy even with offers.
In this project, I will combine the transaction, demographic and offer data to segment the users, according to the purchasing and the offer received histories. Three groups of users (buy with offer, buy without offer, never buy even with offer) will be identified. Then I will build machine learning models for the users, who will purchase with offers, to predict how they respond to the BOGO or the discount offer.
To achieve the goal, firstly, I will use pandas to preprocess three datasets about offer, demographic, and transaction data respectively, and then merge them into a comprehensive dataset. After getting the comprehensive dataset, a summary of transactions for all users will be created, including the total consumption amount, the response rate for each offer, and processed demographic data. Then three groups will be identified based on this summary of transaction. Lastly, Random Forest models will be built to predict whether the users, who buy with offer, will respond to the BOGO and discount offers or not.

