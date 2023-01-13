
# Title of Project

## Car Price Prediction

![1_ftnM93QhlS0A7I55QegbrA](https://user-images.githubusercontent.com/114376944/212347276-a3972028-72e7-4058-8a46-6d867f41e0a7.jpeg)

# Description
The cardheko data set is extracted out from cardheko website.
This dataset contains 8183 rows and 13 columns.
In this dataset lots of features are given like as fuel type, seller type, transmission, owner etc.
On the basis of these features we have to predict the selling price of car.

## Dataset
The data set is downloaded from kaggle.

To downlad the data set you can refer to this link:-

https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho


![car_dheko](https://user-images.githubusercontent.com/114376944/212347527-a2db0509-a160-4108-9854-1bfeecbc2ef9.PNG)


## Importance or Use case

India's automobile market is very big. Here lots of people wants to buy car in their budget.
New cars are costliers so due to this reason lots of people go for old cars

But People dont know how much money they have to spend to buy the car which has some specific features.

To solve this problem or to make easy for people to know about the selling price of car we have to cerate a model that predict the selling price of cars based on the features.

It means person will select the features and our model will predict the selling price based on these features. 
## Lab Environment
We have used Google colab to create this project

Link for google colab :-

https://colab.research.google.com/
## Task Done

### 1) Data collection
- First of all we have collected the data from kaggle 

### 2) EDA
### a) Data cleaning
- Data set contains some null values we handled these
- We have some columns like as mileage that contains values like '20 kmpl' and engine column contains like '1200 cc'.
So here we removed the text portion because we need only numerical value lik 20 from '20 kmpl'.
- Created car_age column column by substractinf current year from year of purchase.
- Created brand name columns that contains the brand name of cars that is extracted out from name column.
- Drop name, year, torque columns
### b) Statistical analysis
- Minimum selling price of cars is 29999 and maximum selling price is 10000000.
- Oldest car is 40 year old and latest car is 3 year old
- Top selling brand is maruti
- Car with Diesel fuel type is in most in demand
- Manual car are more in demand than automatic

#### c) Graphical analysis
-  Plot lots of graph to visualize the data set and find the pattern of data set

- Plot  bar graph, countplot,histogram, distplot, heatmap etc.
- Mean selling price of diesel cars is maximum with value of 791452.92
- Average mileage of CNG cars is maximum with value of 23.82
- Maximum car belongs to individual category
- Maximum car belongs to Firts_owner 
- Maximum number of cars belong to Maruti brand followed by Hyundai
- Diesel car which have automatic gear transmission are most expensive
- As the car is going to old the selling price is descresing.



 ### 3) Fetaure Engineering 
 - Fix the skewness by using log transformation
 - Encoding the categorical data using One Hot Encoder
 - Done Feature scaling using robust scaler


### 4) Spiting the data into training and testing 
- Split the data set into training and testing set
- 75% for training and 25% for testing


### 5) Model Building 
- Trained multiple models on training data set
- Compared the performance of models on the basis of cv_score or r2 score
- CV_regressor or R2_score of XGBRegressor are maximum that are  97.49%, or 93.8% respectively.
- So finalize this models as best performing models among used models
#### Done some prediction using XGBRegressor



## Future work

- We can also do hyperparameter tuning by using Grid Search CV or Random Search CV to find out best parameters
- We can also apply deep learning algorithm.
- After testing we will deploy the model
