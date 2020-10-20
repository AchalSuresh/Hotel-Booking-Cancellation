
# Prediciton of Hotel booking Cancellation

The objective of this project is to use techniques taught in class to study the data patterns or to predict factors behind cancellation of hotel bookings. Refer to the Appendix for the reference and description of the data set.

# Dataset


The data was retrieved from Kaggle https://www.kaggle.com/jessemostipak/hotel-booking-demand and illustrated the records from 4 hotels in Portugal from 2015-2017. The data set contains roughly 119390 instances which is a good amount of volume that can be split into training and test data for model generation

# Process

* Data Exploration: Conducting a deep exploratory analysis for the data
* Methodologies: The alogrithms being used to test the hypothesis
* COnclusions: The final findings from the analysis

# Data Exploration

Through our initial analysis, we saw that there are a large number of null values in the columns Agent and Company had a large number of columns. Also, columns such as reservation status have values similar to our target variable ‘is_canceled’.   We also had to convert a number of columns such as hotels, meals, etc to factors for our analysis.
We have also created two new columns stay nights total = weekend nights + weekday nights and stay total cost =  stay nights total * cost per night (adr).


More detailed exploration data is present in the Project_Report.pdf file

# Methodologies
* Logistic Regression
* Decision Tree
* Random Forest
* Naive Bayes

# Results:

We can see from the results that random forest achieves the highest auc, therefore, providing most useful information for us. We can see that lead time, deposit type, adr, previous cancellations, and stay cost total are highly influential in determining if a customer will cancel the reservation this time. The model shows us tendencies of customers so that hotels can make reasonable arrangements to avoid risks. 
Accuracy of the model is still a problem. Even though random forest is our best model so far, it still only achieves 83% accuracy. On a large scale, the hotel  will turn 17% of its business chance away. Since random forest is an ensemble method, we can incorporate more weak learners to enhance the performance of the classifier and achieve better performance.




