# Human Activity Recognition with smartphones using Machine Learning Models
This project seeks to identify human activities using smartphone sensor data. The data is gathered from 30 people who engaged in six different activities
while holding a smartphone equipped with inertial sensors.

## Dataset Description
- The Human Activity Recognition (HAR) dataset was created by recording 30 research participants conducting activities of daily living (ADL) while carrying
  a smartphone attached on their waist with inbuilt inertial sensors. The actions carried out were:
  - WALKING
  - WALKING_UPSTAIRS
  - WALKING_DOWNSTAIRS
  - SITTING
  - STANDING
  - LAYING

## Project Overview

### Methodology
**1. Data Preprocessing**
- Standardization of sensor data
  - Label encoding of activity labels
  - Application of sliding window technique to segment the data
**2. Feature Extraction**
  - Extracted features from accelerometer and gyroscope signals
  - Created 561-feature vectors for each window
**3. Models Trained**
  - Support Vector Machine (SVM)
  - Random Forest (RF)
  - K-Nearest Neighbors (KNN)
**4. Hyperparameter Tuning**
  - Grid Search was used for hyperparameter optimization of SVM, RF, and KNN models

## Conclusion
The project demonstrates the effectiveness of machine learning models in classifying human activities using smartphone sensor data. 
The SVM model achieved the highest accuracy, followed by Random Forest and KNN.

