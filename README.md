# Roeland Portfolio
Portfolio of my current and finished projects in Data Science and Analytics


# Fun Side Projects

## [Project 1: Automated Padel Booking Script]
* Wrote python scripts that will automatically chose padel courts based upon prefered Location / Time / Court-type / Duration
* It knows the ideal booking time and will book the court if available automatically
* Currently it works for 3 of the main suppliers of padel courts in the area of Amsterdam.
  1. Peakz Padel (available nation wide)
  2. Frans Otten (Booking system widely used and code could be replicated easily to other places)
  3. Playtomic (App used worldwide)
 
## [Project 2: Digital Personal Assistent]
* Currently in development stage
* During my work I notice that I get many small tasks, that I cannot always do immediately on the spot and later on might forget...
* I wanna create a workflow that will store and creates to-do's automatically


# Machine Learning

## [Project 1: Predict Hotel Booking Cancellations](https://github.com/roelrrr/Predicting_Cancellations)
* We Built a predictive model that returns an expected net demand for hotel bookings
* The output can be adjusted towards the prefered timeframe in days or season.
* The dataset contains of 79,330 records and contains information about booking reservations from a Portuguese hotel chain

* One of the challenges to overcome was data leakage during the machine learning process since we are working with timeseries
* Our solution was to use a time series split method, which is a method to avoid future data predicting current data in the machine learning process.

* Since hotels are working with seasonality they asked us to incorporate overbooking problems into the model
* As performance metrics we used two different F scores, namely F0.5 (High season) and F1.5 (Low season).
* The F0.5 reduces false positives and therefor reduce possible overbookings. 
* The F1.5 reduces false negatives, because we wanted to have false negatives more "costly".
* After trying different machine learning techniques the XGBoost delivered the highest performance with F1.5 : 0.84 & F0.5 : 0.74

* For the deployement we have built an application where a potential hotel manager could import a dataset into the application and adjust the time frame and seasonality. After importing, it will do a feature importance analysis and you can chose which features to incorporate and which machine learning technique to use. As a result it will return the F score as measurement and a list with cancellation probability for each client. Lastly it will return an image of net demand (as shown below )for the timeframe asked at the beginning.
* Example of net demand visual:
![NET Demand Visual](https://github.com/roelrrr/Predicting_Cancellations/blob/main/Images/Net_demand_Visual.png)


* For the Project description click on the [link](https://github.com/roelrrr/Predicting_Cancellations#readme)

## [Project 2: Predicting Online Buying Behavior](https://github.com/roelrrr/Predicting_Online_Buying_Behavior)
* Build a predictive model that answer the question "Which customers are more likely to buy our products?"
* Use PCA to reduce dimensionality 
* Evaluation criteria: F1 score
* Testing the following ML models: Linear & Logistic Regression, Naïve Bayes, Instance based KNN-Classifier, Decision Tree, Neural Networks, AdaBoost, Gradient Boosting Classifier, Random Forest, Bagging Classifier, Stacking Classifier
* All our notebooks for the different modeling can be found [here](https://github.com/roelrrr/Predicting_Online_Buying_Behavior/tree/main/Scripts)
* Based upon F1 scores we checked which method had the best outcome
* We developed a model that was good for a 9th place of 56 groups in the [(Kaggle competition)](https://www.kaggle.com/c/techscape-ecommerce/leaderboard?tab=public)
* A full report about our modelling can be found [here](https://github.com/roelrrr/Predicting_Online_Buying_Behavior/blob/main/Description/Guidelines_Group_Project_Master_202122.pdf)

# MySQL DataBase 

## [Project 1: DBMS: Portuguese Restaurant Chain](https://github.com/roelrrr/DatabaseSystem-For-A-Burger-Restaurant-Chain) 
* Created a DBMS for a Burger Restaurant Chain to optimize workflow of orders
* Built Triggers for updating a log table with incoming orders 
* Built Views for creating receipt
* Using SQL to understand revenue performances of the different restaurants --> [Code](https://github.com/roelrrr/DatabaseSystem-For-A-Burger-Restaurant-Chain/tree/main/Scripts)
* [Project Description](https://github.com/roelrrr/DatabaseSystem-For-A-Burger-Restaurant-Chain/blob/main/Description/description.pdf)
* Built an ERD-Diagram
![ERD-Diagram](https://github.com/roelrrr/DatabaseSystem-For-A-Burger-Restaurant-Chain/blob/main/Analysis/ERD-Diagram.png)

# Data Mining

## [Project 1: Customer Segmentation:](https://github.com/roelrrr/Datamining---Wonderful-World-Of-Wines-Marketing-Strategies-)
* Performed two segmentations based upon value & engagement and buying behavior of customers
* Goal: Establish data-driven marketing strategies for the company Wonderful World of Wines (WWW)
* Dataset consisted of 10.000 records with 18 features, delivered by WWW
* Relative clean dataset, focus on the use of datamining techniques and providing marketing strategies
* Combined Hierarchical Clustering with Kmeans Clustering to reach to valuable outcomes
* Including a full written [report](https://github.com/roelrrr/Datamining---Wonderful-World-Of-Wines-Marketing-Strategies-/blob/main/Content/B01-WonderfulWinesoftheWorld.pdf) and [presentation](https://github.com/roelrrr/Datamining---Wonderful-World-Of-Wines-Marketing-Strategies-/blob/main/Content/Final_Presentation.pptx) with findings.
![Cluster 1 & 2](https://github.com/roelrrr/Datamining---Wonderful-World-Of-Wines-Marketing-Strategies-/blob/main/Analysis/Radargraph%20Cluster%201%20%26%202.png)

![Cluster 3](https://github.com/roelrrr/Datamining---Wonderful-World-Of-Wines-Marketing-Strategies-/blob/main/Analysis/RadarGraph%20Cluster%203.png)



