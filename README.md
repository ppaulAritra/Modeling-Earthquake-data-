# Modeling-Earthquake-Damage

Based on aspects of building location and construction, our goal is to predict the level of damage to buildings caused by the 2015 Gorkha earthquake in Nepal.The data mainly consists of information on the buildings' structure and their legal ownership. Each row in the dataset represents a specific building in the region that was hit by Gorkha earthquake.

## Richter's Predictor: Modeling Earthquake Damage
 How artificial intelligence and predictive analysis can help in faster damage recovery from earthquake


### Overview


### General Overview of the data

Data collected from DrivenData.org competition website


#### Data Source: https://www.drivendata.org/competitions/57/nepal-earthquake/

 Inhouse data was collected through surveys by the Central Bureau of Statistics that work under the National Planning Commission Secretariat of Nepal. It is rumoured that this survey is one of the largest post-disaster datasets ever collected, containing valuable information on earthquake impacts, household conditions, and socio-economic-demographic statistics


### Problem description
 Predict the ordinal variable damage_grade, which represents a level of damage to the building that was hit by the earthquake. There are 3 grades of the damage:

1 represents low damage
2 represents a medium amount of damage
3 represents almost complete destruction

### Features
The dataset mainly consists of information on the buildings' structure and their legal ownership. Each row in the dataset represents a specific building in the region that was hit by Gorkha earthquake.

There are 39 columns in this dataset, where the building_id column is a unique and random identifier. The remaining 38 features are described in the section below. Categorical variables have been obfuscated random lowercase ascii characters. The appearance of the same character in distinct columns does not imply the same original value.


### Our Target

We are predicting the level of damage from 1 to 3(Low,Medium,High). The level of damage is an ordinal variable meaning that ordering is important. 
This can be viewd as a classification or Regression Problem


### performance metrics

To measure the performance of our algorithms, we have used the F1 score which balances the precision and recall of a classifier

F1 - performance on a binary classifier

But since we have three possible labels we used a variant called the micro averaged F1 score.

In Python, we can easily calculate this loss using sklearn.metrics.f1_score with the keyword argument average='micro'





