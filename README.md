# Customer-Retention-Prediction

This project aims to predict customer retention for a telecommunication company based on historical data. The data is sourced from Kaggle and can be found [here](https://www.kaggle.com/blastchar/telco-customer-churn). Using a deep learning model (Artificial Neural Network), I was able to achieve an accuracy of 80%.


## Overview
Customer churn is a critical problem for telecommunication companies. Retaining customers is far more cost-effective than acquiring new ones, which makes churn prediction essential for maintaining business profitability.

In this project, I use an Artificial Neural Network (ANN) to predict whether a customer will churn or not, based on various features such as contract type, payment method, monthly charges, and tenure.


## Data Preprocessing
Data cleaning and preprocessing steps include:
1. **Handling missing values**: Removed rows with missing values in the `TotalCharges` column.
2. **Data type conversion**: Converted categorical variables like `gender`, `Contract`, and `PaymentMethod` into numerical values using one-hot encoding.
3. **Feature Scaling**: Applied feature scaling to numeric features like `TotalCharges`,`MonthlyCharges` and `tenure` using MinMaxScaler.
4. **Train-test split**: Split the dataset into training and testing sets in an 80-20 ratio.

## Model
I used an Artificial Neural Network (ANN) for classification. The model was built using the `Keras` library in Python.

### Model Architecture:
- **Input Layer**: 26 features as input
- **Hidden Layers**: Two hidden layers with 32 neurons each, using ReLU activation.
- **Output Layer**: A single neuron with sigmoid activation to output a binary classification (Churn or Not Churn).

### How to Use
- Clone this repository:
    ```bash
    git clone https://github.com/DhruvKumar-Patel98/Customer-Retention-Prediction.git
    ```

 - Install the required dependencies:
     ```bash
     pip install tensorflow keras numpy pandas matplotlib scikit-learn seaborn
     ```
 - Open Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
 - Run Customer-Retention-Prediction.ipynb file


