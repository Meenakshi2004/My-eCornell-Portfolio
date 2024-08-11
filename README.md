<h1> Exploring Demographic Bias in Income Prediction: An Analysis of US and Non-US Native Groups </h1>
<h2> Project Objective</h2>
<p> 
  This project utilizes the 1994 Census dataset to predict income levels based on demographic attributes. The primary focus is on analyzing how different demographic groups, specifically US-native versus non-US-native individuals, are represented within the data. The project involves data cleaning and feature engineering to prepare the dataset for modeling. 
  I built several machine learning models to predict income levels and evaluate their performance through accuracy and AUC-ROC scores. 
  The analysis reveals general trends in demographic representation and provides a foundation for future work, which could include a deeper examination of potential biases and fairness assessments in the model's predictions.
  <br> </p>
<em> *The 1994 Census dataset includes various demographic attributes such as age, work class, education level, marital status, occupation, and native country. The dataset contains a mix of categorical and numerical features, with a total of 32,561 records.* </em>

<h2> Data preparation and Findings </h2>
<p> 
Initial data exploration involved examining the distribution of demographic features and identifying potential imbalances. Notable observations included the over-representation of White individuals and the varied representation of different nationalities. The 'native-country' feature was transformed into a binary variable, merely distinguishing between US-natives and non-US-natives. This transformation facilitated a clearer analysis of the impact of native status on income levels.
The analysis revealed several insights: <br>
</p>

<ul>
  <li> Demographic Disparities: The education level was found to be slightly higher among US-natives compared to non-US-natives. However, this finding was nuanced by the higher variability in education levels among non-US-natives, suggesting that the educational background varies more widely within this group.</li>
  <li> Correlation Analysis: A weak positive correlation was observed between education level and US-native status, suggesting that US-natives generally have slightly higher 
    educational attainment compared to non-US-natives. The median education level for US-natives was also higher than that for non-US-natives. 
    However, this observation can be misleading, as the non-native population includes diverse groups with varying educational levels. For instance, 
    Asian-Pacific Islanders exhibit higher average education levels, indicating that the general statement about US-natives being more educated might
    oversimplify the complexity of the data. This could potentially lead to discrepancies in the model's perception and inadvertently introduce biases. 
  </li>
</ul>

<h2> ML Modelling & Analysis: </h2>
<p> 
  The following Machine Learning Models - Logistic Regression, Random Forest, Gradient Boosting, K-Nearest Neighbors, and Decision Trees - were trained and evaluated. 
  The Gradient Boosting model emerged as the best performer, achieving the highest accuracy and AUC-ROC scores. To ensure the prevention of significant overfitting, I 
  practiced agile model development by increasing the model complexity in separate iterations. It turns out that Gradient Boosting was still the most effective in 
  distinguishing between income levels based on the given features.
</p>

<h2> Future Work: </h2>
<p> 
  Further exploration is needed to improve model fairness. Given the scope of this project, potential disparities were addressed, but in the next iterations, 
  additional data pre-processing such as oversampling or undersampling techniques, could be considered to balance the dataset. Further analyzing and mitigating biases in specific demographic groups will enhance the 
  model's accuracy and fairness in predicting income levels.
</p>
