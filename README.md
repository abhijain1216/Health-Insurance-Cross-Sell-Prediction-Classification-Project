# Health Insurance Cross Sell Prediction Classification Project

### *Project Summary*
In this project, our objective is to build a model that predicts whether a customer will be interested in Vehicle Insurance or not. This information is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue. Now, in order to predict whether the customer would be interested in vehicle insurance,we have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc. We have a dataset with approximately 38,000 observations and 12 features.

Steps that have been followed include Dataset loading, Data Cleaning, Data Wrangling, Handling of Outliers, and Missing Values ,Exploratory data analysis, and Feature Engineering etc.Through EDA,we have learned about different factors that affect a customer's response to vehicle insurance. Insights found from exploratory data analysis will be helpful in feature selection. For the treatment of outliers, the IQR (Interquartile Range) method was adopted because our data is positively skewed distributed.In the Feature Engineering part, for the encoding of categorical variables,we have used Label Encoding and One Hot Encoding.To check the normality of the data, a Q-Q plot was used, and the best transformation for the feature was determined by using the Q-Q plot. Log Transformation and Square Root Transformation were used for feature transformation. To detect multicollinearity,we have used a correlation matrix and performed VIF analysis, and with these techniques, multicollinearity from the data is effectively removed. For the evaluation of model metrics like recall,precision,f1-score and AUC ROC Score were calculated.From the point of view of the problem Recall is more important than precision because if recall is low and precision is high, then our model fails to capture all those customers who are actually interested in insurance, which is a loss to the company in terms of money. Whereas if recall is high and precision is low, we will be able to target those who are actually interested.We have also obtained the confusion matrix for a better understanding of model performance.For further improvement in the model and to find the best set of hyperparameters, we have performed hyperparameter tuning for each model, and the techniques utilised for this purpose are GridSearchCV and RandomizedSearchCV. To understand models better, a Model Explainability tool like SHAP has been used. Local as well as Global explainability have been explained using SHAP values.

For the current classification problem, we have used different algorithms like Logistic Regression,Decision Tree,Random Forest,Balanced Random Forest,XGBoost and K-Nearest Neighbours and implemented each algorithm successfully. The Balanced Random Forest algorithm is selected as the final prediction model because it gives the best results among all the algorithms.


### *Problem Statement*
Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.

For example, you may pay a premium of Rs. 5000 each year for a health insurance cover of Rs. 200,000/- so that if, God forbid, you fall ill and need to be hospitalised in that year, the insurance provider company will bear the cost of hospitalisation etc. for upto Rs. 200,000. Now if you are wondering how can company bear such high hospitalisation cost when it charges a premium of only Rs. 5000/-, that is where the concept of probabilities comes in picture. For example, like you, there may be 100 customers who would be paying a premium of Rs. 5000 every year, but only a few of them (say 2-3) would get hospitalised that year and not everyone. This way everyone shares the risk of everyone else.

Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

Now, in order to predict, whether the customer would be interested in Vehicle insurance, you have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.


### *Dataset Information*
* The dataset has information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.It has approximately 38,000 observations and 12 features.
* There are no null/missing values in the dataframe.
* There are no duplicate values in the dataframe, all rows are unique.

#### *Variable Description*
* **id :**	Unique ID for the customer
* **Gender	:** Gender of the customer
* **Age :**	Age of the customer
* **Driving_License :**	0 : Customer doesn't have Driving Licence, 1 : Customer already has Driving Licence
* **Region_Code :**	Unique code for the region of the customer
* **Previously_Insured	:** 1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance
* **Vehicle_Age :**	Age of the Vehicle
* **Vehicle_Damage	 :** 1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.
* **Annual_Premium	:** The amount customer needs to pay as premium in the year
* **PolicySalesChannel :**	Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.
* **Vintage :**	Number of Days, Customer has been associated with the company
* **Response :**	1 : Customer is interested, 0 : Customer is not interested


### *Project Work flow*

1. Importing Libraries

2. Loading the Dataset

3. Explore Dataset

4. Data Wrangling

5. Exploratory Data Analysis (EDA) 

6. Hypothesis Testing

7. Feature Engineering & Data Pre-processing

8. Machine Learning Model Implementation

9. Model Explainability

10. Future Work

11. Conclusions


### *Python Libraries Used*

* Numpy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* SciPy
* Shap
* Pylab
