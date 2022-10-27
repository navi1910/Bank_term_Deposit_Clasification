
# Term Deposit Outreach Client Classification
## Classifcation project
Classification is a supervised learning technique used to predict discrete traget variables using set of features/attributes.

## Project Objective
The aim of the project is to use client data to predict if the client will subscribe to term deposit or not.

## Methods
- Data Visualization
- Data Transformation - Encoding
- Heatmaps for correlation
- Feature Engineering
- Model Building
- Predictive Modelling
- Logistic Regression
- Decision Tree Classifier

## Technologies used
- Python
- Pandas
- matplotlib and seaborn
- sci-kit learn

## Project Description
Term deposits are a major source of income for a bank. A term deposit is a cash investment held at a financial institution. The bank has various outreach plans to sell term deposits to their
customers such as email marketing, advertisements, telephonic marketing
and digital marketing.

Telephonic marketing campaigns still remain one of the most effective way
to reach out to people. However, they require huge investment as large call centers are hired to actually execute these campaigns. Hence, it is crucial
to identify the customers most likely to convert beforehand so that they can
be specifically targeted via call. 

**Client personal data such as age of the client, their job type, their marital status, etc along with the call information such as the duration of the call, day and month of the call, etc is used to predict if the client will subscribe to term deposit or not.**



We use __Classification__ to predict the same.

## Procedure
- Import the required modules for Python.
- Import the training data as a Data Frame.
- Print the head of the data.
- The basic `info` is printed.
- The column names of attributes is also printed.
- `'ID'` column is dropped.
- `'subscribed'` is indentified as the Target Variable.
- Countplot of `'subscribed'` is plotted.
![barplot_subs](https://github.com/navi1910/Bank_term_Deposit_Classification/blob/master/barplot_subscribed.png 'barplot_subs')
- Stacked Barplot of `'Job'` vs Frequency is plotted such that it shows how many have subscribed or not. 
![stacked_bar](https://github.com/navi1910/Bank_term_Deposit_Classification/blob/master/job_stacked_subscribed.png 'stacked_bar')
- `LabelEncoder` from `sklearn.preprocessing` is used to convert all categorical variables to numeric variables.
- Heatmap is plotted to check the correlation among the variables.
![heatmap](https://github.com/navi1910/Bank_term_Deposit_Classification/blob/master/heatmap.png 'heatmap')
- Correlation Table is also created.

- Dependent and Independent Variables are separated.
- `train_test_split` from `sklearn.model_selection` is used to split the dependent and independent variables into Training and Validation sets.

## Model Building
### Logistic Regression
- `LogisticRegression` from `sklearn.linear_model` is initialized using `logi`.
- `X_train` and `y_train` are fit to `logi`.
- Prediction of `y_val` is done by applying `predict` on `X_val`.
- The model scores are calculated.

### Decision Tree Classifier
- `DecisionTreeClassifier` from `sklearn.tree` is initialized suing `dtc`.
- `X_train` and `y_train` are fit to `dtc`.
- Prediction of `y_val` is done by applying `predict` on `X_val`.
- The model scores are calculated.

## Model Testing
- Test data is imported as a Data Frame.
- Feature Engineering and Data Transformation is done on Testing data.
- `predict` is used to obtain predictions.
- csv file of predicted values is created as `'submission.csv'`.

## Model Results
- Logistic Regression
    - accuracy = 0.8829383886255924

- Decision Tree Regressor
    - accuracy = **0.8924170616113745**

#### Here Decision Tree Classifier (`dtc`) is slightly better than Logistic Regression model (`logi`).
- Some optional data exploration is done on test data to understand it better. 

## Contact
https://www.linkedin.com/in/naveen-a-902a671b3/

## Data Source
Internshala Data Science Course.
