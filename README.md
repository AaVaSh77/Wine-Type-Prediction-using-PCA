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

## Code Explanation

### Data Preprocessing

```python
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler

# Load dataset
dataset = pd.read_csv('Wine.csv')
X = dataset.iloc[:, :-1].values
y = dataset.iloc[:, -1].values

# Split dataset
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 0)

# Feature scaling
sc = StandardScaler()
X_train = sc.fit_transform(X_train)
X_test = sc.transform(X_test)
