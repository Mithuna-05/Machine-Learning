## Objective
To explore public datasets from the UCI Machine Learning Repository and Kaggle, identify the appropriate machine learning tasks, and apply a complete machine learning workflow including loading, EDA, preprocessing, feature selection, model training, and evaluation.

## Datasets and ML Task Type
| Dataset                              | ML Task Type       | Model Type         |
|-------------------------------------|--------------------|--------------------|
| Loan Amount Prediction              | Supervised         | Regression         |
| Handwritten Character Recognition   | Supervised         | Classification     |
| Email Spam Classification (Spambase)| Supervised         | Classification     |
| MNIST Digit Classification          | Supervised         | Classification     |
| Diabetes Prediction (PIMA/sklearn)  | Supervised         | Classification     |
| Iris Dataset                        | Supervised         | Classification     |

##  ML Workflow Steps Followed

### 1. Loading the Dataset
- Datasets loaded from `sklearn.datasets`, UCI (via `ucimlrepo`), or Google Drive (CSV).

### 2. Exploratory Data Analysis (EDA)
- Summary statistics using `df.describe()`, `df.info()`.
- Visualizations: Histograms, Countplots, Heatmaps, Scatterplots, Boxplots using Seaborn/Matplotlib.

### 3. Data Preprocessing
- Handled missing values using `dropna()` or `fillna()`.
- Encoded categorical variables using `get_dummies()` or `LabelEncoder`.
- Normalized features using `StandardScaler` or `MinMaxScaler`.

### 4. Feature Selection
- Applied techniques like `SelectKBest`, `Chi-Square Test`, or correlation heatmaps.

### 5.  Data Splitting
- Used `train_test_split()` to split data into training and testing sets (80-20 or 75-25).

### 6. Model Training & Evaluation
- Used models like `LinearRegression`, `LogisticRegression`, `RandomForestClassifier`, and `GaussianNB`.
- Evaluated performance using:
  - **Classification**: Accuracy, Precision, Recall, F1-score, Confusion Matrix, ROC Curve
  - **Regression**: Mean Squared Error (MSE), R² Score
- Visualized model results with confusion matrices, feature importance plots, and ROC curves.

## Libraries Used
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn  
- ucimlrepo (for UCI datasets)
