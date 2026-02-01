# Human Activity Recognition with Smartphones

This project focuses on predicting and classifying human actions based on sensor data obtained from wearable devices. By leveraging machine learning models, the system accurately categorizes physical activities using data from a smartphone's inbuilt accelerometer and gyroscope.

## Project Overview
Human Activity Recognition (HAR) is a significant field with applications in healthcare, sports, and human-computer interaction. This study investigates the classification of activities using sensor data from 30 subjects. The goal is to provide a scalable strategy for monitoring actions such as health tracking and context-aware services in wearable computing settings.

## Project Files
- `Human Activity Recognition.ipynb`: Jupyter notebook containing the complete data analysis, model training, and evaluation code.
- `HumanActivityRecognitionProjectReport.pdf`: Detailed project report covering the methodology, data visualization, and comparative results.

## Dataset Description
The study utilizes the Human Activity Recognition database built from recordings of 30 participants performing Activities of Daily Living (ADL).
- **Sensor Data**: Triaxial linear acceleration and triaxial angular velocity sampled at a constant rate of 50Hz.
- **Activities**: Walking, Walking Upstairs, Walking Downstairs, Sitting, Standing, and Laying.
- **Data Features**: Each record consists of a 561-feature vector with variables from both temporal and frequency domains.

## Technical Implementation

### Data Preprocessing
To ensure successful model training, the raw sensor data underwent a multi-step pipeline:
- **Noise Filtering**: Applied to sensor signals to smooth out artifacts while preserving underlying activity patterns.
- **Standardization**: Converted data to a mean of zero and a standard deviation of one to ensure all input characteristics have a comparable scale.
- **Segmentation**: Divided continuous sensor data into fixed-width sliding windows of 2.56 seconds with a 50% overlap.
- **Label Encoding**: Categorical activity labels were converted into numerical values for model processing.

### Models Evaluated
The research compared different machine learning architectures to identify the most effective classification technique. Hyperparameters for each algorithm were optimized using **GridSearchCV** to ensure peak performance.

| Model Category | Algorithms Used | Optimization Strategy |
| :--- | :--- | :--- |
| **Supervised Learning** | Support Vector Machine (SVM) | GridSearchCV |
| **Ensemble Learning** | Random Forest Classifier | GridSearchCV |
| **Instance-based Learning** | K-Nearest Neighbors (KNN) | GridSearchCV |

## Performance Results
The models were evaluated based on Accuracy, Precision, Recall, and F1-score. Hyperparameter tuning through **GridSearchCV** provided a measurable increase in performance across models.

### Key Findings
- **Top Performer**: The Support Vector Machine (SVM) achieved the best results with an accuracy of 96.01% after tuning.
- **Ensemble Success**: Random Forest demonstrated high robustness with an accuracy of 93.25%.
- **Tuning Impact**: Optimization significantly improved the K-Nearest Neighbor model accuracy from 87.62% to 90.35%.

## Future Work
- Exploring deep learning architectures like LSTMs or CNNs to further improve temporal feature extraction.
- Incorporating more diverse datasets with broader age groups and different wearable placements.
- Developing a real-time activity monitoring application for mobile platforms.
