# Data Science Heart_Failure_Prediction_Dataset

## Analyzing Dataset to Predict Cardiovascular Disease 

Rodrigo Arguello-Serrano

Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worldwide. People with cardiovascular disease or with risk factors require early detection need early detection where a machine learning model can very useful.

## Data Source: 

[Data](https://raw.githubusercontent.com/pylabview/Heart-Failure-Prediction-Project-2-/main/heart.csv)

For this dataset, there were 8523 rows, 10 columns, and one Target feature.

## Data Dictionary
![Dict](https://raw.githubusercontent.com/pylabview/Heart-Failure-Prediction-Project-2-/main/Dictionary.png)
## To prepare this data, the data was cleaned, and the following processes were performed:

### Exploratory Data Analysis
```
- Dataframe datatypes of each variable.
- Removing duplicates.
- Identify missing values.
- Define strategy to address missing values.
- Confirm that there are no missing values after addressing them.
- Find and fix any inconsistent categories of data.
```


> The data set is pretty clean, no duplicate values or inconsistencies


 ### Explanatory Data Analysis

    - To visualize the data for explantory purposes, four bargraphs were chosen.
    - The bargraphs were chosen to show how the categories compare to each other. 



## Explanatory Visuals

![ByGender](https://raw.githubusercontent.com/pylabview/Heart-Failure-Prediction-Project-2-/main/By_Gender.png)

>Number of Males is significantly higher than Females

![ByChestPain](https://raw.githubusercontent.com/pylabview/Heart-Failure-Prediction-Project-2-/main/ByChestPain.png)


>The patients with Asymptomatic chest pain are the majority, and the Typical Angina has the lowest samples

![CorrelationFeatures](https://raw.githubusercontent.com/pylabview/Heart-Failure-Prediction-Project-2-/main/CorrelationHeatMap.png)

>There no strong or moderate correlation between features and target

 ### Machine Learning Using the Following Models:

    - KNN Baseline Model
    - KNN Tuned Model
    - Random Forest Tuned Model
    - KNN with PCA Model


​    

## Models Evaluated & Results

![Scores](https://raw.githubusercontent.com/pylabview/Heart-Failure-Prediction-Project-2-/main/Scores.png)


> Hyper-parameters used for tuning:
  - Logistic Regression Model: Decision Threshold
  - KNN Model: n_neighbors. For PCA, the 95% of the variance is the best value, by increasing or decreasing this parameters, the scores display underperformance.
  - Random Forrest:n_estimators


## Recommendations

>The model suggested for production is Random Forest, it has some bias with low variance. I am selecting Accuracy as the dataset is well balanced (55% for class diseases, and 45% for normal), it works well with binary classification, and all models show high accuracy. 



