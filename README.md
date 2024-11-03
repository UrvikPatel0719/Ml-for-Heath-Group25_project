# Ml-for-Heath-Group25_project

## Project Title:
Sepsis Prediction with Digital Phenotypes and Time Series Analysis

## Student Names and Numbers:
-  **Student Name**: Urvik Harshadkumar Patel  
  **Student Number**: 1440623  
- **Student Name**: Jiahao MA  
  **Student Number**: 1516228
- **Student Name**: Yesheng Yao
  **Student Number**: 1108951

## Description of the Project:
This project focuses on predicting sepsis in ICU patients by creating digital phenotypes and conducting time series analysis using data from the MIMIC-IV database. The primary objective is to leverage patient characteristics, time-dependent physiological data, and machine learning models to predict sepsis 3 hours in advance based on different observation windows. This project is structured across three main files, each building upon the previous steps to create and evaluate predictive models.

### Key Objectives:
1. **Digital Phenotyping**: Generate digital phenotypes for sepsis patients using MIMIC-IV data, focusing on identifying and preprocessing relevant features.
2. **Model Development and Prediction**:
   - **5-Hour Window Model** (`final_project`): Train a model using a 5-hour observation window to predict sepsis 3 hours ahead.
   - **10-Hour Window Model** (`final_project_part_2`): Train a model using a 10-hour observation window for the same prediction target.
3. **Evaluation Metrics**: Assess the models using standard metrics such as confusion matrix, ROC AUC, classification report, and feature importance to understand model performance.

## Project Structure

### Digital-phenotype
This script provides information on creating digital phenotypes for sepsis prediction. It extracts and preprocesses patient data, identifying key sepsis-related characteristics as features for model training and analysis.

### final_project
This file includes data preprocessing and model training with a 5-hour observation window. The model predicts sepsis 3 hours ahead and is evaluated using:
- **Evaluation Metrics**: Confusion matrix, ROC AUC, classification report, and feature importance.
- **Training and Validation Information**: Tracks model accuracy and loss for both training and validation.

### final_project_part_2
This file mirrors `final_project`, with the primary difference being a 10-hour observation window for sepsis prediction. The same metrics and performance tracking are used here.

## Instructions to Set Up the Environment:

1. **Install Anaconda/Miniconda**:
   - Download and install Anaconda/Miniconda from the [official website](https://www.anaconda.com/download).

2. **Install Required Packages**:
   - Install packages listed in `requirements.txt` by running:
     ```bash
     pip install -r requirements.txt
     ```

## Dependencies:
The dependencies are specified in `requirements.txt` and include:
- numpy==1.23.5
- pandas==1.5.3
- matplotlib==3.6.2
- scikit-learn==1.1.3
- IPython==8.7.0
- tensorflow==2.10.0
- imblearn==0.9.0
- google-cloud-bigquery==3.4.2
- bigframes==0.1.6

## Resources Used:
- **MIMIC-IV Dataset**: This project uses the MIMIC-IV (Medical Information Mart for Intensive Care IV) dataset for data analysis and model training.  
  - Reference: Johnson AE, Pollard TJ, Shen L, et al. MIMIC-IV (version 3.1); 2021. Available at [https://physionet.org/content/mimiciv/3.1/](https://physionet.org/content/mimiciv/3.1/).  
  - Note: Further references for specific methods are provided in the project report.

- **Python Libraries**: This analysis utilizes libraries like NumPy, Pandas, Scikit-Learn, TensorFlow, and Matplotlib for data manipulation, visualization, and model training.

## Notebook Structure:
Each notebook is structured with Markdown and includes:
- Importing Libraries
- Data Preprocessing and Digital Phenotyping
- Model Training and Evaluation
- Prediction Window Analysis (5-hour and 10-hour)
- Summary and Conclusions

## Conclusion:
This project offers insights into sepsis prediction through time series analysis of ICU patient data. By creating digital phenotypes and developing predictive models, the project demonstrates the potential to improve sepsis prediction accuracy and supports data-driven decision-making in critical care.
