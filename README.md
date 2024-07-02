### Predicting Breast Cancer Recurrence using Machine Learning

**Aaron Leung**

#### Executive summary

#### Rationale
Breast cancer is one of the most common cancers among women. Understanding the factors that contribute to its recurrence can significantly improve prognosis and survival rates. Furthermore, integrating predictive models into clincal practice allows healthcare providers to develop effective, targeted intervention in high risk patients.

#### Research Question
How can machine learning models be used to accurately predict the recurrence of breast cancer based on patient demographics, clinical and treatment-related features?

#### Data Sources
The dataset, sourced from UCI Machine Learning Repository, contains 9 attributes related to patient demographic, clinical characterisitcs and treatment as follows:
1. Class (Recurrence Event)
2. Age
3. Menopausal Stage
4. Tumor Size
5. Number of Lymph Nodes Involved
6. Presence of Extracapsular Extension
7. Degree of Malignancy
8. Breast (Left or Right)
9. Breat Quadrant
10. Irradiation

#### Methodology
Methods used comprise of the following:

_Data Exploration_
1. Get an Overview of the Dataset
2. Check for Missing Values
3. View Distribution of Each Feature
4. Visualize Data to Gain Insights to Data Distribution and Relationships

_Data Preprocessing_
1. Data Cleaning
2. Data Transformation (converting categorical features into numerical features)
3. Feature Scaling

_Exploration of Different Classifcation Models_
1. Logistic Regression
2. Decision Tree
3. K-Nearest Neighbors
4. Support Vector Machines
5. Neural Networks (maybe)

_Model Evaluation and Hyperparameter Tuning_
1. Access performance of models using metrics such as accuracy, precision, recall, f1-score
2. Perform hyperparameter tuning with GridSearchCV
   

#### Results
- Among the four models trained, Logistic Regression performed the best overall on the test set, displaying the high accuracy, recall and f1 score on the test set.
- In contrast, the other models exhibited noticeable drops across perfromance metrics from the training set to test set, even with GridSearchCV
- We were able to extract feature importance from the Logistic Regression and Decision Tree models, respectively. Interestingly, the top features differed significantly between the two models. For Logistic Regression, the top important features include, breast-quad?, menopauselt40, and irradiation. In contrast, for Decision Tree, the top features are the degree of malignancy, number of lymph nodes involved, age and tumor-size.

#### Next steps
- Improve performance of models by revisitng hyperparameter tuning and data preprocessing steps to enhance cross-validation score
- Identify additional visualizations to effectively present findings
- For future considerations, it would be benenficial to incorporate genetic information into dataset, as genetics can play a significant role. This includes factors such as genetic mutations and family history
#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
