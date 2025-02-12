# Blossom-Bank-Fraud_Detection
## AI and ML Models for Secure Digital Transactions at Blossom Bank

<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/Cover.png" alt="Displays" width="800" height="400"/> 

### 🥷🏿Executive Summary
With the rapid growth of online transactions, fraud detection has become critical for financial security. This report presents an in-depth analysis of online payment fraud detection using machine learning models. Through data exploration, feature engineering, and model evaluation, we identify patterns in fraudulent transactions and assess the effectiveness of various classification techniques. Our findings provide actionable insights for stakeholders to mitigate risks associated with fraudulent activities.

### 🥷🏿Dataset Overview

The dataset under scrutiny contains over 1 million records of online transactions, each characterized by several key attributes:

- **Step:** Represents a unit of time in the simulation.
- **Type:** The type of transaction (e.g., PAYMENT, TRANSFER, CASH_OUT).
- **Amount:** The transaction amount.
- **NameOrig:** The customer initiating the transaction.
- **OldbalanceOrg:** The initial balance before the transaction.
- **NewbalanceOrig:** The new balance after the transaction.
- **NameDest:** The recipient of the transaction.
- **OldbalanceDest:** The initial balance of the recipient before the transaction.
- **NewbalanceDest:** The new balance of the recipient after the transaction.
- **isFraud:** A binary indicator of whether the transaction is fraudulent.

<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/Summary.png" alt="Displays" width="500" height="300"/> 

### 🥷🏿Key Observations
- **Transaction Distribution:** Most transactions are within moderate amount ranges, with fewer extreme outliers.
- **Fraud Patterns:** Fraudulent transactions frequently involve CASH-OUT and TRANSFER types.
- **Correlation Analysis:** Fraud transactions are strongly associated with specific sender/receiver types and higher transaction amounts.
- **Time-Based Trends:** Fraud occurrences tend to spike at certain transaction steps.

### 🥷🏿Exploratory Data Analysis
**Univariate Analysis**
- **Transaction Types;** The dataset reveals a diverse array of transaction types, with the most common being CASH_OUT and PAYMENT, followed by CASH_IN, TRANSFER, and DEBIT. This distribution underscores the variety of financial activities captured in the dataset, each potentially susceptible to different forms of fraud.
- **Transaction Amounts;** A box plot of transaction amounts by type highlights significant variability. TRANSFER and CASH_OUT transactions exhibit higher median amounts compared to PAYMENT and CASH_IN. This suggests that larger transactions might be more prone to scrutiny and, potentially, fraud.

<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/Type.png" alt="Displays" width="500" height="300"/> 
<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/Amount.png" alt="Displays" width="500" height="300"/> 


**Bivariate Analysis**
- **Fraudulent Transactions by Type;** A critical aspect of fraud detection is understanding which transaction types are most susceptible to fraud. The dataset indicates that TRANSFER and CASH_OUT transactions are more likely to be flagged as fraudulent. This aligns with the intuition that these types of transactions, often involving large sums, are prime targets for fraudulent activities.

<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/Fraud.png" alt="Displays" width="500" height="300"/> 

**Correlation Analysis**

Exploring the correlation between transaction amounts and the likelihood of fraud reveals that higher amounts are more frequently associated with fraudulent activities. This correlation underscores the importance of monitoring large transactions for potential fraud.

<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/HeatMap.png" alt="Displays" width="600" height="300"/> 

**Patterns in Fraudulent Transactions** often exhibit distinct patterns, such as unusually high amounts, rapid succession of transactions, or discrepancies between the old and new balances of the involved accounts. By identifying these patterns, we can develop more effective fraud detection algorithms.


### 🥷🏿Enhancing Fraud Detection with Machine Learning
**Machine Learning Models**

Leveraging models like logistic regression, decision trees, and neural networks can significantly enhance fraud detection. These models, trained on historical data, predict the likelihood of fraud in new transactions, enabling proactive measures to prevent financial losses.

**Data Preprocessing**

To prepare the data, we performed feature engineering to create new attributes, converted categorical variables into numerical form, and applied normalization techniques to standardize the dataset.

### 🥷🏿Model Implementation and Evaluation
We implemented several models, including Decision Tree Classifier, Random Forest Classifier, SVM, XGBoost, and LightGBM. We assessed their performance using metrics such as accuracy, F1 score, ROC-AUC score, and confusion matrix. The confusion matrix revealed minimal false positives but indicated a need for further optimization to reduce false negatives.

**Model Building;** The dataset was split into training (80%) and testing (20%) sets, with a random state of 42 for reproducibility.

**First Model: Logistic Regression**; object was created, trained on the training subset, and used to predict the test subset.

**Model Evaluation and Results**
- **Logistic Regression:** AUC-ROC: 0.578, Accuracy: 0.999, F1 Score: 0.269, Precision: 0.972, Recall: 0.156
- **Random Forest Regressor:** R² Score: 0.778
- **Decision Tree Regressor:** R² Score: 0.678
- **Decision Tree Classifier:** AUC-ROC: 0.928, Accuracy: 0.999, F1 Score: 0.840

**More Experimental Models**
- **Random Forest Classifier:** Accuracy: 0.9998
- **SVM:** Accuracy: 0.9991
- **XGBoost:** Accuracy: 0.9998
- **LightGBM Classifier:** Accuracy: 0.9985

The confusion matrix revealed that while false positives were minimal, further optimization is needed to reduce false negatives and enhance fraud detection.

<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/Confusion%20matrix.png" alt="Displays" width="600" height="300"/> 

### 🥷🏿Key Recommendations
1. **Implement Ensemble Models** – Combining multiple models such as XGBoost and Random Forest can enhance fraud detection accuracy.
2. **Feature Engineering Enhancements** – Incorporating time-based transaction patterns and user behavior analytics can improve model predictions.
3.	**Real-Time Fraud Detection** – Deploying machine learning models in real-time transaction monitoring can help prevent fraud before completion.
4.	**Threshold Tuning for Alerts** – Optimizing classification thresholds can balance sensitivity and specificity in fraud alerts.
5.	**Ongoing Model Updates** – Continuous retraining with updated data ensures model effectiveness against evolving fraud techniques.

________________________________________
### 🥷🏿Conclusion
This analysis reveals critical insights into online payment fraud, highlighting the importance of understanding transaction patterns to develop robust detection mechanisms. By leveraging advanced machine learning techniques like XGBoost and LightGBM, we can significantly enhance fraud prevention and safeguard online payment systems. Collaboration among data scientists, financial institutions, and regulatory bodies is essential to create a secure digital financial ecosystem. This report underscores the power of data-driven decision-making in combating fraud, encouraging stakeholders to adopt a multi-faceted approach that integrates machine learning, feature engineering, and real-time monitoring. Ultimately, these efforts will protect financial systems, maintain customer trust, and ensure business continuity in an increasingly digital world. 🚀🚨🔐🔐
________________________________________

<br>

### *Kindly share your feedback and I am happy to Connect 🌟*

<img src="https://github.com/jamesehiabhi/Blossom-Bank-Fraud_Detection/blob/main/Displays/My%20Card1.jpg" alt="Displays" width="600" height="150"/>

