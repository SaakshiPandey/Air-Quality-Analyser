# Air Quality Analyser  
## Machine Learning Project using the UCI Air Quality Dataset

This project analyses air quality data from the UCI Air Quality Dataset to model, classify, and cluster pollution patterns. It incorporates regression, classification, clustering, and ensemble learning techniques, along with comprehensive performance evaluations.

---

## 1. Project Overview

The objective of this project is to build predictive and analytical models capable of estimating air pollutant levels, identifying pollution categories, and uncovering hidden patterns in environmental data.

### Workflow Includes:
- Preprocessing UCI Air Quality Dataset  
- Regression modelling for pollutant concentration prediction  
- Classification modelling for air quality categorisation  
- Clustering analyses to detect inherent data groupings  
- Model evaluation using performance and confusion metrics  

---

## 2. Dataset

**Source:** UCI Machine Learning Repository – Air Quality Data Set  

The dataset contains hourly averaged responses of gas sensors deployed in an indoor environment, providing concentrations of CO, NMHC, NOx, O3, temperature, relative humidity, and absolute humidity.

### Key Features:
- CO(GT), NMHC(GT), NOx(GT), O3(GT)  
- Temperature  
- Relative Humidity  
- Absolute Humidity  
- Date & Time (parsed appropriately)

### Preprocessing Performed:
- Missing value handling  
- Outlier detection and removal  
- Data type correction  
- Normalisation / standardisation  
- Feature engineering (if applicable)  
- Train-test split  

---

## 3. Modelling Techniques

### 3.1 Linear Regression
Used to predict continuous pollutant levels such as CO(GT) or O3(GT). Focuses on capturing linear relationships between environmental features and pollutant concentrations.

### 3.2 Multiple Linear Regression
Extends simple linear regression by incorporating multiple predictors simultaneously to improve pollutant concentration estimation.

### 3.3 Logistic Regression
Used to classify air quality into categories (e.g., Good, Moderate, Poor) based on pollutant thresholds or AQI-like labels.

### 3.4 Support Vector Machine (SVM)
Implemented for classification with kernel-based decision boundaries to separate pollution level classes more effectively.

### 3.5 Random Forest
An ensemble model trained for both regression and classification tasks, providing robustness against noise and nonlinear relationships.

### 3.6 K-Means Clustering
Unsupervised algorithm to group observations based on similarity in sensor readings and meteorological conditions.

### 3.7 K-Medoids Clustering
A more robust clustering technique using medoids instead of centroids, reducing sensitivity to outliers.

---

## 4. Evaluation Metrics

### 4.1 Regression Metrics  
Used for Linear Regression, Multiple Linear Regression, and Random Forest Regression:
- Mean Absolute Error (MAE)  
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

### 4.2 Classification Metrics  
Used for Logistic Regression, SVM, and Random Forest Classification:
- Accuracy  
- Precision  
- Recall  
- F1 Score  

### 4.3 Confusion Matrix  
A confusion matrix was generated for each classification algorithm to visualise class-wise prediction performance.

### 4.4 Clustering Evaluation:
- Within-Cluster Sum of Squares (WCSS) for K-Means  
- Silhouette Score  
- Cluster visualisations in 2D/3D using PCA  

---

## 5. Results Summary

### Regression Findings:
- Multiple Linear Regression and Random Forest generally outperformed simple Linear Regression.  
- Random Forest provided the lowest error rates and best R² score due to its ability to capture nonlinear patterns.  

### Classification Findings:
- SVM and Random Forest produced higher accuracy and better F1 scores than Logistic Regression.  
- Logistic Regression served as a good baseline model.  

### Clustering Findings:
- K-Means produced clearer cluster separation but was sensitive to outliers.  
- K-Medoids offered more stable clusters when noisy data was present.  

---

## 6. Technologies Used
- Python  
- NumPy, Pandas, SciPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## Conclusion

This project demonstrates the application of both supervised and unsupervised machine learning approaches to air quality analysis. By leveraging multiple models and evaluation techniques, it provides insights into pollutant prediction, air quality classification, and data-driven grouping of environmental conditions.

The modular structure allows easy extension into real-time air quality monitoring, IoT integration, or deployment as an analytics service.
