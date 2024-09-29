# Wine Classification with PCA and Logistic Regression

This project demonstrates the use of Principal Component Analysis (PCA) and Logistic Regression to classify wine samples into different categories using the `Wine.csv` dataset.

### Dataset:
The dataset contains 13 features of wines along with a target variable representing different wine classes. The features include:

- Alcohol
- Malic acid
- Ash
- Alcalinity of ash
- Magnesium
- Total phenols
- Flavanoids
- Nonflavanoid phenols
- Proanthocyanins
- Color intensity
- Hue
- OD280/OD315 of diluted wines
- Proline

The target variable represents three classes of wine.

## Implementation Steps

### 1. Data Preprocessing
- **Splitting the dataset**: The dataset is split into training and test sets.
- **Feature scaling**: Standardization of features is performed using `StandardScaler`.

### 2. Principal Component Analysis (PCA)
- PCA is applied to reduce the dimensionality of the dataset to 2 components.

### 3. Model Training
- A Logistic Regression model is trained using the training dataset.

### 4. Model Evaluation
- The model is evaluated using a confusion matrix and accuracy score.

## Output
<p align="center">
  <img src="https://github.com/user-attachments/assets/dfe87389-d4ef-4022-ad29-761326b40246" width="45%" />
  <img src="https://github.com/user-attachments/assets/83c5b530-2371-4589-9ab1-90a0aae859a9" width="45%" />
</p>
