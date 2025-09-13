# Heart Disease Prediction Project

This project aims to predict the presence of heart disease in individuals using a logistic regression model based on a dataset containing various health parameters.

## Dataset

The dataset used in this project is the Heart Disease Dataset from Kaggle. It contains the following attributes:

*   **age**: Age in years
*   **sex**: Sex (1 = male; 0 = female)
*   **cp**: Chest pain type (4 values: 0, 1, 2, 3)
*   **trestbps**: Resting blood pressure (in mm Hg on admission to the hospital)
*   **chol**: Serum cholestoral in mg/dl
*   **fbs**: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
*   **restecg**: Resting electrocardiographic results (values 0, 1, 2)
*   **thalach**: Maximum heart rate achieved
*   **exang**: Exercise induced angina (1 = yes; 0 = no)
*   **oldpeak**: ST depression induced by exercise relative to rest
*   **slope**: The slope of the peak exercise ST segment
*   **ca**: Number of major vessels (0-3) colored by flourosopy
*   **thal**: Thalassemia (0 = normal; 1 = fixed defect; 2 = reversable defect)
*   **target**: Diagnosis of heart disease (1 = presence; 0 = absence)

The original dataset can be found [here](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset).

## Project Structure

The project is organized as a Jupyter Notebook, performing the following steps:

1.  **Importing Dependencies**: Necessary libraries such as pandas, numpy, and scikit-learn are imported.
2.  **Data Collection and Processing**: The heart disease dataset is loaded into a pandas DataFrame.
    *   Basic data exploration is performed (checking head, tail, shape, info, and missing values).
    *   Statistical measures of the data are calculated.
    *   The distribution of the target variable is examined.
3.  **Splitting Features and Target**: The dataset is split into features (X) and the target variable (Y).
4.  **Splitting Data into Training and Test Sets**: The data is further split into training and testing sets to evaluate the model's performance. A test size of 20% is used, with stratification based on the target variable.
5.  **Model Training**: A Logistic Regression model is initialized and trained using the training data.
    *   A `ConvergenceWarning` might appear during training, suggesting that increasing the number of iterations (`max_iter`) or scaling the data could improve convergence.
6.  **Model Evaluation**: The trained model is evaluated on both the training and test datasets to calculate the accuracy scores.
7.  **Building a Predictive System**: A system is built to take new input data and predict whether a person has heart disease based on the trained model.

## Getting Started

### Prerequisites

*   Python 3.6+
*   Jupyter Notebook or Google Colab
*   Required Python packages (listed in the code cells):
    *   pandas
    *   numpy
    *   scikit-learn

### Installation

1.  Clone the repository (if applicable) or download the notebook file.
2.  Install the required packages:
