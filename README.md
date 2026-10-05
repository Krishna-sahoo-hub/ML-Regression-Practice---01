# Machine Learning Regression Practice :- 01

A hands-on Machine Learning practice project covering three important regression techniques using Python and Scikit-learn.

This repository demonstrates data loading, exploratory analysis, visualization, train-test splitting, model training, prediction, model evaluation, and interpretation of regression models.

## 📌 Project Overview

This project contains three regression problems using different datasets:

1. **Simple Linear Regression** — Predict exam scores based on study hours.
2. **Multiple Linear Regression** — Predict car prices using multiple vehicle features.
3. **Gradient Boosting Regressor** — Predict laptop prices using hardware specifications.

The project is designed to understand how different regression algorithms can be applied to different types of prediction problems.

---

## 🎯 Objectives

* Understand the fundamentals of regression.
* Perform basic data exploration and visualization.
* Prepare independent and dependent variables.
* Split datasets into training and testing sets.
* Build and train regression models.
* Make predictions on unseen test data.
* Evaluate models using regression metrics.
* Visualize actual vs predicted values.
* Understand feature influence and feature importance.
* Compare linear and non-linear regression approaches.

---

## 🧠 Machine Learning Models

### 1. Simple Linear Regression

**Dataset:** `study_hours_exam_score.csv`

**Dataset shape:** `1000 × 2`

**Features:**

* `StudyHours` — Input feature
* `ExamScore` — Target variable

### Workflow

* Load the dataset using Pandas.
* Check dataset shape and missing values.
* Visualize the relationship between study hours and exam score.
* Separate `X` and `y`.
* Split the data into training and testing sets.
* Train a Simple Linear Regression model.
* Calculate the slope and intercept.
* Predict exam scores.
* Evaluate training and testing performance.
* Visualize actual values, predicted values, and the best-fit line.

---

### 2. Multiple Linear Regression

**Dataset:** `car_price_multiple.csv`

**Dataset shape:** `5000 × 4`

**Features:**

* `EngineSize_L`
* `Mileage_km`
* `CarAge_years`

**Target:**

* `Price_USD`

### Workflow

* Load and inspect the dataset.
* Use `.info()` and `.describe()` for data exploration.
* Check for missing and duplicate values.
* Separate independent and dependent variables.
* Perform an 80/20 train-test split.
* Train a Multiple Linear Regression model.
* Generate price predictions.
* Analyze model coefficients and intercept.
* Calculate training and testing scores.
* Evaluate the model using:

  * MAE
  * MSE
  * RMSE
  * R² Score
* Create an Actual vs Predicted price visualization.

---

### 3. Gradient Boosting Regressor

**Dataset:** `laptop_price_gbr.csv`

**Dataset shape:** `10000 × 6`

**Features:**

* `RAM_GB`
* `Storage_GB`
* `ScreenSize_inch`
* `Weight_kg`
* `BatteryLife_hrs`

**Target:**

* `Price_USD`

### Model Configuration

```python
GradientBoostingRegressor(
    n_estimators=100,
    learning_rate=0.1,
    max_depth=3
)
```

### Workflow

* Load and inspect the dataset.
* Check shape and data types.
* Check for missing values.
* Separate features and target.
* Perform an 80/20 train-test split.
* Use `random_state=42`.
* Train the Gradient Boosting Regressor.
* Generate laptop price predictions.
* Evaluate predictions using:

  * MAE
  * MSE
  * RMSE
  * R² Score
* Plot Actual vs Predicted prices.
* Extract and visualize feature importances.
* Understand the advantage of Gradient Boosting for non-linear relationships.

---

## 📊 Evaluation Metrics

The project uses common regression evaluation metrics.

| Metric       | Description                                                      |
| ------------ | ---------------------------------------------------------------- |
| **MAE**      | Mean Absolute Error                                              |
| **MSE**      | Mean Squared Error                                               |
| **RMSE**     | Root Mean Squared Error                                          |
| **R² Score** | Measures how well the model explains the variation in the target |

### R² Score

An R² score closer to **1** generally indicates better explanatory performance on the evaluated data.

---

## 📈 Visualizations

The notebook includes visualizations such as:

* Study Hours vs Exam Score
* Regression best-fit line
* Actual vs Predicted Car Prices
* Actual vs Predicted Laptop Prices
* Feature Importance for Gradient Boosting

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**
* **Jupyter Notebook**

---

## 📁 Repository Structure

```text
ML-Regression-Practice/
│
├── ML_Practice_Regression.ipynb
│
├── study_hours_exam_score.csv
├── car_price_multiple.csv
├── laptop_price_gbr.csv
│
├── requirements.txt
│
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/ML-Regression-Practice.git
```

Move into the project directory:

```bash
cd ML-Regression-Practice
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

Or install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
ML_Practice_Regression.ipynb
```

Run the notebook cells sequentially.

Make sure the CSV datasets are located in the same directory as the notebook, or update the dataset paths accordingly.

---

## 💡 Key Learning Outcomes

Through this project, I practiced:

* Regression fundamentals
* Data preprocessing
* Exploratory data analysis
* Data visualization
* Train-test splitting
* Model training
* Prediction
* Regression evaluation metrics
* Model coefficients
* Feature importance
* Linear vs non-linear regression

The project also demonstrates that **Gradient Boosting can capture non-linear relationships and feature interactions**, while linear regression models relationships using a linear combination of features.

> **Note:** The Multiple Linear Regression and Gradient Boosting sections use different datasets, so their R² scores should not be treated as a direct model-vs-model benchmark. A fair comparison requires evaluating both models on the same dataset.

---

## 🚀 Future Improvements

* Add more regression algorithms such as:

  * Decision Tree Regressor
  * Random Forest Regressor
  * Random Forest
  * XGBoost
* Perform hyperparameter tuning.
* Add cross-validation.
* Compare multiple models on the same dataset.
* Improve data preprocessing and feature engineering.
* Create a model comparison table.
* Deploy a selected regression model as a web application.

---

## 👨‍💻 Author

**Krishna Sahoo**

B.Tech Computer Science Engineering Student
Aspiring Data Analyst / Data Science Enthusiast

---

## ⭐ If You Find This Project Useful

If you find this repository useful for learning Machine Learning and Regression, consider giving it a ⭐ on GitHub.
