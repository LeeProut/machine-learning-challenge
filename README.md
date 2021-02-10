# Exoplanet Exploration with Machine Learning

### Applying machine learning models to NASA data from the Kepler mission to determine classification of exoplanets. 

#### NASA data sourced from [Kaggle](https://www.kaggle.com/nasa/kepler-exoplanet-search-results). 

#### Data cleaning: 
- dropped null columns and rows
- formatted the orginal FALSE POSITIVE value to FALSE_POSITIVE 

#### Selected features: 
- began each model by including all features
- after running models, selected for features with the largest impact on results, as determined by fitting the model

#### Tune the model's parameters
- used GridSearch to tune params and train the model

#### Models used: 
- Random Forest Classifier
- Deep Learning

#### Packages used: 
- pandas
- sklearn
- joblib
- keras

#### Model Performance: 
- Random Forest Classifier 
    - the first Random Forest Classifier scored 1.0 on training data and 0.89 on testing data
    - after using feature_importances_ to tune the features, the training data scored 1.0 and the testing data scored .90
    - GridSearch on the second model had a best score of .89 and test accuracy of .89
    - precision was highest for the FALSE_POSITIVE classification, with a score of 0.98, and overall accuracy of classification had a weighed average of .90

- Deep Learning
    - adding layers to the deep learning model did not improve accuracy with this data
    - the first layer model's Normal Neural Network Accuracy was 0.89
    - adding a layer for the deep model resulted in a Normal Neural Network Accuracy of 0.88

    
