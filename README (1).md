# Machine-Learning-Project
Exploratory Data Analysis (EDA) 
                            on Customer Churn Dataset

 Introduction :-
This report presents the findings from an exploratory data analysis (EDA) conducted on a Customer Churn dataset. The primary objective of this analysis is to understand the characteristics of the data, identify significant patterns, and prepare the data for further predictive modeling. The dataset comprises various features related to customer behavior, demographics, and service usage, which are crucial for predicting customer churn.

 Data Loading and Preprocessing :-

Data Loading:-

The dataset was loaded using Pandas, a powerful data manipulation library in Python. This step involves reading the dataset from a CSV file and storing it in a DataFrame for easy manipulation and analysis.

 Initial Exploration:-

Initial exploration involved checking the structure of the dataset, including the number of entries, column names, and data types. We also examined the dataset for any missing values. This step is crucial for understanding the basic properties of the data and identifying any immediate data quality issues.

 


Renaming Columns:-
To improve readability and ease of analysis, the column names were renamed. The original column names contained spaces and were not very descriptive. Renaming them to more intuitive names helps streamline the analysis process.

 Data Visualization:-

Target Variable Distribution:-
The distribution of the target variable, 'Churn', was visualized using a count plot. This helps in understanding the balance of the classes in the dataset. An imbalanced dataset can significantly affect the performance of machine learning models.

Age Group Analysis:-
The distribution of customers across different age groups was examined. Additionally, the churn rates within each age group were visualized to identify any patterns or trends related to age and customer churn.

 Charge Amount Distribution:-
The distribution of the 'charge_amount' feature was analyzed to understand the spending behavior of customers. This can provide insights into whether higher or lower spending customers are more likely to churn.

 Pie Chart for Age Distribution:-
A pie chart was created to visualize the proportion of customers in different age categories. This helps in understanding the demographic composition of the customer base.



 Categorical Feature Exploration:-
The unique values and frequency counts for key categorical features, such as 'complains', 'charge_amount', 'tariff_plan', 'status', 'age', and 'Churn', were examined. This provides insights into the distribution and variability of these features.

 Correlation Analysis:-
A heatmap of the correlation matrix was created to visualize the relationships between numerical features. This helps in identifying potential multicollinearity issues and understanding how different features are related to each other and to the target variable, 'Churn'.

Outlier Analysis:-
Outliers in continuous features were identified using the Interquartile Range (IQR) method. Box plots were used to visualize the distribution of these features and highlight any outliers. Handling outliers is essential for ensuring the robustness of machine learning models.

 Outlier Handling:-
Outliers were replaced with the mean value of the respective feature. This step ensures that extreme values do not adversely affect the model training process.

 Data Preparation for Modeling:-

Train-Test Split:-
The dataset was split into training and testing sets. This is a critical step for evaluating the performance of machine learning models. By training the models on one subset of the data and testing them on another, we can get an unbiased estimate of their performance.

Machine Learning Models:-

Several machine learning models were trained and evaluated:

1. Decision Tree Classifier: A simple and interpretable model that splits the data based on feature values.
2. Random Forest Classifier: An ensemble model that improves the accuracy and robustness by combining multiple decision trees.
3. Support Vector Machine (SVM): A model that finds the optimal hyperplane for classification.
4. Logistic Regression: A linear model that estimates the probability of a binary outcome.

Each model's accuracy and classification report were evaluated to determine their effectiveness in predicting customer churn.

 Conclusion:-
The exploratory data analysis provided valuable insights into the Customer Churn dataset. Key patterns and relationships were identified, and the data was prepared for predictive modeling. The analysis highlighted the importance of feature engineering, handling imbalanced classes, and dealing with outliers. The next steps involve fine-tuning the machine learning models, feature selection, and further validation to improve prediction accuracy.
