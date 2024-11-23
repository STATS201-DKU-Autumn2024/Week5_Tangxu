# Advancing Predictive Maintenance for Vehicle Systems Using Multimodal and Real-Time Data

## Overview
The purpose of this code folder is to provide a comprehensive implementation of predictive maintenance analysis using machine learning techniques. It focuses on analyzing and modeling multimodal datasets, including the NASA Turbofan Engine Degradation Data and the MetroPT dataset. The tasks performed include:

1. **Data Preprocessing**: Loading, cleaning, normalizing, and preparing data for predictive modeling.
2. **Exploratory Data Analysis (EDA)**: Analyzing key data trends and visualizing sensor readings, failure patterns, and operational conditions.
3. **Machine Learning Models**: Training and evaluating models such as Random Forest and Support Vector Machine (SVM) to predict Remaining Useful Life (RUL) and component failures.
4. **Model Interpretability**: Using SHAP analysis to understand feature importance and model decision-making.
5. **Visualization**: Generating insightful plots to support data-driven decision-making and maintenance strategies.

## Files Included

### [**`Advancing_Predictive_Maintenance.ipynb`**](https://colab.research.google.com/drive/1jFpqHdT2FzVdd1g5KstMsEbXj-PRv9R0)
This Jupyter Notebook contains the complete workflow for predictive maintenance analysis and modeling. It is divided into the following key sections:

1. **Data Loading and Preprocessing**:
   - Loads the MetroPT and NASA Turbofan Engine Degradation datasets.
   - Performs data cleaning, normalization, and feature extraction for machine learning models.

2. **Exploratory Data Analysis (EDA)**:
   - Summarizes the datasets with descriptive statistics.
   - Visualizes key trends, such as sensor measurements, time-series patterns, and failure rates.

3. **Predictive Modeling**:
   - Implements machine learning models, including:
     - Random Forest
     - Temporal Convolutional Networks (TCNs)
   - Evaluates models on Remaining Useful Life (RUL) predictions using performance metrics such as RMSE and MAE.

4. **Model Explainability**:
   - Uses SHAP (SHapley Additive exPlanations) to interpret model predictions.
   - Generates SHAP summary plots and dependence plots to analyze feature importance and interactions.

5. **Visualization**:
   - Includes visualizations for both time-series data trends and SHAP analysis.
   - Provides insights into how sensor data and operational settings impact maintenance predictions.

This notebook serves as a complete implementation of the predictive maintenance project, from data exploration to advanced modeling and explainability.

## Prerequisites

The environment requirements for running this project can be accessed from the main page: [Environment Requirements](https://github.com/STATS201-DKU-Autumn2024/Week5_Tangxu/tree/main).

Ensure all dependencies listed in the repository are installed before running the notebook.

## Usage Instructions

The primary code for this analysis is contained in the Jupyter Notebook file **Advancing_Predictive_Maintenance.ipynb**. This notebook can be executed in Google Colab, providing an interactive environment where students and researchers can modify parameters and observe real-time results of the predictive maintenance models.

### Download the Dataset

1. Download the **NASA Turbofan Engine Degradation Simulation Data** from the NASA data repository, respectively.
2. Upload the downloaded data files to your Google Colab environment for easy access.

### Running the Notebook

1. Open the **Advancing_Predictive_Maintenance.ipynb** file directly in Google Colab by selecting "Open in Colab" above or by uploading it to your Colab environment.
2. Ensure that all required libraries (e.g., `pandas`, `numpy`, `matplotlib`, `scikit-learn`) are installed within the Colab environment.
3. Execute each cell in the notebook to perform data analysis, visualization, and model training for predictive maintenance.

## Expected Outputs

### Visualizations
- **SHAP Analysis**:
  - **SHAP Dependence Plot**: Provides insights into the relationship between `sensor_measurement_2` and its SHAP values. The plot highlights how the feature impacts the model's predictions, with `sensor_measurement_8` used as a color-coded interaction variable.
    - Observations:
      - A strong negative correlation between `sensor_measurement_2` and its SHAP values indicates that lower values of this feature lead to higher importance in predicting Remaining Useful Life (RUL).
      - Interaction with `sensor_measurement_8` reveals additional patterns, with higher values amplifying the effect of `sensor_measurement_2`.
    - ![SHAP Dependence Plot](https://github.com/STATS201-DKU-Autumn2024/Week5_Tangxu/blob/main/Code/SHAP.png)
  - **SHAP Summary Plot**: Highlights the overall feature importance across all features in the model.

- **Time-Series Trends**:
  - Visualizes trends in `sensor_measurement_2` and `sensor_measurement_3` for specific units in the NASA dataset.
    - Observations:
      - Both sensor measurements exhibit increasing trends as the unit progresses through operational cycles.
      - High variability in the sensor measurements emphasizes the importance of capturing these patterns for accurate predictive maintenance.
    - ![Time-Series Analysis](https://github.com/STATS201-DKU-Autumn2024/Week5_Tangxu/blob/main/Code/Time-Series%20Analysis.png)

- **Statistical Insights**:
  - Correlation heatmaps uncover relationships between sensor measurements and Remaining Useful Life (RUL).
  

### Performance Metrics
- **Model Evaluation**:
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
  - Precision and Recall for model predictions
- **Comparison of Approaches**:
  - Performance comparison between single-modality and multimodal data approaches.


### Explanatory Insights
- Insights into how operational settings and sensor readings influence RUL predictions.
- Feature importance rankings derived from SHAP analysis to identify critical factors for maintenance strategies.

These outputs collectively enable data-driven predictive maintenance decisions and provide actionable insights for real-world applications.


## Dataset

This project utilizes two primary datasets to explore and model predictive maintenance:

1. **MetroPT Dataset**: This dataset provides detailed logs on maintenance activities, operational metrics, and failure events from Lisbon’s metro system. It includes key variables that track the conditions and degradation of metro components over time, offering a robust foundation for predictive maintenance modeling in public transportation.

2. **NASA Turbofan Engine Degradation Simulation Data**: This dataset contains real-time sensor readings from simulated turbofan engines under different operational conditions. It captures degradation patterns across high-stress engine components, allowing for real-time analysis and prediction of component failure.

### Data Dictionary
A comprehensive data dictionary describing all relevant variables in each dataset can be found in the [Data](https://github.com/STATS201-DKU-Autumn2024/Week5_Tangxu/tree/main/Data) section of this repository. The data dictionary includes detailed descriptions, data types, and units for each variable, facilitating better understanding and usage of the datasets within the predictive maintenance context.
