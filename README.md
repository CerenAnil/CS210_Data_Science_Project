# CS210_Data_Science_Project
## Airbnb New York Price Prediction
**INTRODUCTION**

This project is aiming to predict a price range for a house/room given the specific attributes using machine learning algorithms. A price prediction would be very useful to both hosts and guests who are using this service, because it would help hosts to avoid overpricing/underpricing the place and the guests to avoid paying much more than deserved to a place. The data used in this project is from between 2011-2018, it is explored and explained in detail in the Description of the Dataset (EDA) & Preprocessing part in detail. After the through exploration of the data missing values got handled in appropriate manners which are explained in the related fields. Also, in Preprocessing we created a new dataframe which has ranges for price instead of the exact price. We choose our range size as [x-20, x+20]. Lessening the complexity of the project and with that getting a faster response was important so, to see if dropping a specific attribute would or would not affect the overall accuracy of the project, a hypothesis testing was conducted. Attributes were chosen so the similarity of it to another attribute was significant. But results showed that no attributes should be dropped. As the last part of the project, we started to apply our chosen Machine Learning methods to our data. We used different dataframes for different methods and in total we used 2 different dataframes, one with normal price values and one with price ranges, and in total we used 5 different machine learning methods which are Random Forest Classifier, Linear Regression, Random Forest Regressor, MLP Classifier and Logistic Regression. We also used Grid Search and Cross Validation in Random Forest Regressor. Results were at first was not really good when we tried to predict exact price using Random Forest Classifier, Linear Regression, Random Forest Regressor. So, we had to change something to make it better. We decided to make our problem more like a classification problem and we changed our prices to price ranges after applying Random Forest Classifier, MLP Classifier and Logistic Regression we obtained much better results and the best we had was Random Forest Classifier.

**PROBLEM DESCRIPTION**

Main problem of this project is that can we predict a price range for a rental Airbnb place given its features like the location and qualifications (all features are explained in detail in Description of the Dataset). Of course, to solve this problem we need to answer some sub-questions. Most important of these questions is “What machine learning method we should use to get the best possible results?”. We are aiming to have the best accuracy. Another important question is the feature selection. We have 15 features in the raw data except our target variable price. In data preprocessing we dropped some features for different reasons, those reasons are explained in detail in the place where they are dropped. In addition, we conducted some hypothesis testing in some features we thought could be dropped without a problem. So, to sum it up our main question is “What is the price range of a given Airbnb rental depending on its features?”. And our hypothesis testing questions are “Is neighborhood group affecting the price of the rental?”, “Is longitude affecting the price of the rental?”, “Is latitude affecting the price of the rental?”
