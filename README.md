# ml_telecom_churn
Machine Learning Telecom Churn Model

In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business goal.

To reduce customer churn, telecom companies need to predict which customers are at high risk of churn.

In this project, you will analyse customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn and identify the main indicators of churn.

### <font color='blue'>Business Goals:</font>
1. Retaining high profitable customers is the number one business goal.
2. This project is based on the Indian and Southeast Asian market.
3. In the Indian and the southeast Asian market, approximately 80% of revenue comes from the top 20% customers (called high-value customers). Thus, if we can reduce churn of the high-value customers, we will be able to reduce significant revenue leakage.
4. The business objective is to predict the churn in the last (i.e. the ninth) month using the data (features) from the first three months. To do this task well, understanding the typical customer behaviour during churn will be helpful.

### <font color='blue'>Analysis Goals:</font>
1. Predict which customers are at high risk of churn
2. Build predictive models to identify customers at high risk of churn and identify the main indicators of churn.
3. Prepaid is the most common model in India and southeast Asia. Focus on prepaid customers.
3. Curn definition used-- "Usage-based churn: Customers who have not done any usage, either incoming or outgoing - in terms of calls, internet etc. over a period of time." In this project, we will use the usage-based definition to define churn.
4. In this project, you will define high-value customers based on a certain metric (mentioned later below) and predict churn only on high-value customers.
5. especially high-value customers go through  three phases of customer lifecycle: a. The ‘good’ phase, b. The ‘action’ phase, c. The ‘churn’ phase

### <font color='blue'>Approach:</font>
Build Telecom Curn Model using for given unbalanced data using various Machine Lerning approaches. the project involves:
1. Data Cleaning
2. Adding Derived Variable and Identifing churn variable
3. Exploratory Data Analysis (univariate & Bivariate). 
4. Treating categorical variable.
5. Perform SMOTE to address data imbalance
6. Dimentinality Reduction  and selecting good features using sklearn (scikit-learn)
	a. PCA (Pricipal Component Analsis), 
	b. LASSO
	c. RFE (Recursive Feature Elimination) 
7. Michine Learning Model using sklearn (scikit-learn)
	a. Linear Regression
	c. Decission Tree
	b. Random Forest
8. Model Accuracy comparision
	a. Confusion Matrix
	b. Model accuracy using 
	
### <font color='blue'>Results:</font>
1. Identified dominant features some of them are [arpu_6, arpu_7, arpu_8, onnet_mou_6, onnet_mou_7, onnet_mou_8, offnet_mou_6, roam_ic_mou_6]
2. Identified the model gives best accuracy: "LASSO with Random Forest"
3. Other models is in the range of 82% to 86% with features 47 to 72 with a moderate false-positives.