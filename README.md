# -Detecting-Credit-Card-Fraud
📌 Welcome to this notebook. The goal of this notebook is to demonstrate how to handle credit card fraud datasets for ML fraud detection. Credit card fraud datasets have several specifications that make them unique and require specialized handling.
#### Context:
This study focuses on the identification of fraud in credit card transactions.

The dataset used here contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
 
Credit card companies need to detect fraudulent transactions to prevent customers from being charged for unauthorized purchases. 

#### Content:
- **Dataset**: Transactions made by European cardholders in September 2013.
- **Duration**: Two days, with 492 frauds out of 284,807 transactions.
- **Class Imbalance**: Fraudulent transactions (positive class) account for 0.172% of all transactions.
- **Features**:
  - Numerical input variables resulting from PCA transformation.
  - 'Time': Seconds elapsed between each transaction and the first transaction.
  - 'Amount': Transaction amount, suitable for cost-sensitive learning.

- **Target**:
  - 'Class': Response variable, 1 for fraud, 0 otherwise.
  
#### Source:
- The dataset has been collected and analyzed by Worldline and the Machine Learning Group (MLG) of Université Libre de Bruxelles (ULB) as part of a research collaboration on big data mining and fraud detection.
- More details on the current and past projects related to fraud detection are available on the [MLG website](http://mlg.ulb.ac.be) and [ResearchGate](https://www.researchgate.net/project/Fraud-detection-5).

#### Recommendations:
- Due to class imbalance, accuracy should be measured using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful.
  
## 12. Conclusions 


1. **Effective Model Development:** Through meticulous data preprocessing, feature selection, and model optimization steps, we've developed a robust fraud detection model.
   
2. **Importance of Imbalance Handling:** Addressing the imbalance in the dataset was critical. Downsampling the majority class improved model performance by ensuring balanced representation of fraudulent and non-fraudulent transactions.

3. **Model Performance:** Our final model, FRAUDFIGHTER, achieved an impressive accuracy of 97% with minimal false negatives and false positives. This underscores its capability to accurately detect fraudulent transactions.

4. **Threshold Optimization:** Fine-tuning the threshold for probability predictions significantly enhanced the model's sensitivity in detecting fraudulent activities, reducing false negatives and improving overall accuracy.

5. **Ensemble Approach:** Leveraging an ensemble method with carefully selected algorithms (LabelSpreading, LabelPropagation, XGBClassifier) proved effective in boosting predictive performance and robustness.

6. **Real-world Application:** The methodologies and techniques applied here are crucial for real-world applications, where the cost of misclassifying fraudulent transactions can be substantial both financially and in terms of trust and customer satisfaction.

7. **Future Directions:** Further enhancements could involve exploring advanced feature engineering techniques, integrating additional data sources, or deploying the model in a real-time environment to continuously improve fraud detection capabilities.
