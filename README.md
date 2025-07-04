# 🎬 IMDb Rating Prediction Using Machine Learning

## 📌 Overview

This project focuses on building machine learning models to predict IMDb ratings of top TV shows based on various attributes such as genre, year, certificate, duration, votes, and rank. The goal is to develop a reliable regression model using real-world data and explore how different features influence ratings.

---

## 📊 Objective

- Predict IMDb ratings using historical data from the IMDb Top 250 dataset.
- Perform data preprocessing, feature engineering, and visualization.
- Train and evaluate multiple regression models.
- Optimize the best model using hyperparameter tuning.
- Analyze feature importance and model performance.

---

## 🗂️ Dataset

- **Source**: IMDb Top 250 TV Shows Dataset
- **Features**:
  - `Title`: Name of the TV show
  - `Genre`: Categories (e.g., Drama, Comedy, War)
  - `Year`: Release year
  - `Certificate`: Age rating (e.g., PG-13, TV-MA)
  - `Duration`: Length of the show
  - `IMDb Votes`: Audience vote count
  - `Rank`: Position in IMDb Top 250
  - `Rating`: IMDb rating (target)

---

## 🛠️ Technologies Used

- **Language**: Python
- **Libraries**:
  - `pandas`, `numpy` – Data handling & numerical operations
  - `matplotlib`, `seaborn` – Data visualization
  - `scikit-learn` – Machine learning and preprocessing
  - `catboost` – Advanced gradient boosting for structured data

---

## 📈 Project Workflow

### 1. Data Preprocessing
- Handled missing values in `certificate` and `duration`.
- Converted `imdb_votes` to numeric.
- Created `duration_minutes` feature.
- Cleaned and formatted data types.

### 2. Exploratory Data Analysis (EDA)
- Correlation analysis between variables.
- Distribution plots for ratings and votes.
- Genre-based rating analysis.
- Scatter plots and heatmaps.

### 3. Feature Engineering
- One-hot encoding for `year_range` buckets.
- Multi-hot encoding for `genre`.
- Dropped non-predictive columns like `title`.

### 4. Model Training
Implemented and compared:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- CatBoost Regressor

### 5. Evaluation Metrics
- **MAE**: Mean Absolute Error
- **MSE**: Mean Squared Error
- **R² Score**: Coefficient of determination

### 6. Hyperparameter Tuning
- Grid Search & Random Search on tree-based models.
- Tuned parameters: `max_depth`, `n_estimators`, `learning_rate`.

---

## 🏁 Results & Insights

- **CatBoost Regressor** delivered the best performance:
  - **R² Score**: 0.84 on the test set
  - High accuracy and low residual error
- Key features influencing ratings:
  - `Rank`, `IMDb Votes`, `Year`, `Duration`, `Certificate`





