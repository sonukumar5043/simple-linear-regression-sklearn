
# Simple Linear Regression using Scikit-Learn

## Project Overview

This project demonstrates **Simple Linear Regression** using **Python** and **Scikit-Learn** to predict **Height from Weight**.

The workflow includes:

- Data loading and preprocessing
- Data visualization
- Correlation analysis
- Train/Test split
- Feature scaling using StandardScaler
- Model training using Linear Regression
- Prediction and evaluation

---

## Dataset

Dataset: `height-weight.csv`

Features:

- **Weight** → Independent Variable (X)
- **Height** → Dependent Variable (y)

Example:

| Weight | Height |
|--------|--------|
|45|120|
|58|135|
|48|123|

---

## Libraries Used

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## Data Visualization

Scatter Plot used to visualize relationship between:

- Weight
- Height

Correlation Matrix:

```text
Weight ↔ Height = 0.931142
```

Strong positive correlation.

---

## Machine Learning Pipeline

### 1. Train Test Split

```python
train_test_split(test_size=0.25, random_state=42)
```

### 2. Feature Scaling

Used **StandardScaler**.

```python
scaler.fit_transform(X_train)
scaler.transform(X_test)
```

### 3. Model Training

```python
LinearRegression(n_jobs=-1)
```

Model trained using:

```python
regression.fit(X_train,y_train)
```

---

## Learned Equation

Linear Regression Equation:

```text
y = mx + b
```

Learned parameters:

```text
m (coefficient) = 17.2982057
b (intercept) = 156.47058823529412
```

---

## Predictions

Example predictions:

| Weight | Predicted Height |
|--------|------------------|
|50|132.92|
|105|190.56|

---

## Model Evaluation

Metrics used:

### Mean Squared Error (MSE)

```text
114.84069295228699
```

### Mean Absolute Error (MAE)

```text
9.66512588679501
```

### Root Mean Squared Error (RMSE)

```text
10.716374991212605
```

### Training Score (R²)

```text
0.9208287444697435
```

Model performance indicates a strong fit.

---

## Project Structure

```text
simple-linear-regression-sklearn/
│
├── height-weight.csv
├── simplelinearModel.ipynb
└── README.md
```

---

## Author

**Sonu Kumar**

B.Tech CSE | Python | Machine Learning | Scikit-Learn
