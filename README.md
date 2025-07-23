# 🚢 Titanic Survival Prediction – Machine Learning Project

This project aims to predict the survival of passengers aboard the Titanic using supervised machine learning techniques. It demonstrates the full ML pipeline from data understanding to model deployment.

---

## 📂 Dataset Overview

The Titanic dataset contains information about passengers including their age, sex, class, fare, and survival status (`Survived` column). The objective is to predict whether a passenger survived the disaster based on these features.

---

## 🧠 Objectives

- Understand and explore the dataset.
- Handle missing values and clean the data.
- Engineer meaningful features.
- Encode categorical variables and scale numerical ones.
- Train classification models to predict survival.
- Evaluate models using accuracy and confusion matrices.
- Visualize survival patterns using demographic features.
- Save the trained model and reuse it for predictions.

---

## 📊 Data Exploration

- Displayed the first few rows to understand structure.
- Identified missing values in `Age`, `Cabin`, and `Embarked`.
- Used `df.info()` and `df.describe()` to understand data types and distributions.
- Checked if the dataset was imbalanced with respect to the target (`Survived`).

---

## 🧹 Data Cleaning & Preprocessing

- **Missing Values**:
  - Filled `Age` with median.
  - Filled `Embarked` with the mode.
  - Dropped `Cabin` due to excessive missing values.

- **Encoding Categorical Variables**:
  - `Sex`, `Embarked`, and `Pclass` were encoded using Label Encoding or One-Hot Encoding.

- **Feature Scaling**:
  - Used `StandardScaler` or `MinMaxScaler` for normalization.

---

## 🛠️ Feature Engineering

Analyzed features for their influence on survival:
- `Sex`: Females had higher survival rates.
- `Pclass`: First-class passengers were more likely to survive.
- `Age`: Children were prioritized during evacuation.
- `Fare`: Often correlated with better cabins or classes.

These insights helped shape the final feature set used for training.

---

## 🤖 Model Training & Evaluation

- Split the dataset using a **70/30 train-test split**.
- Trained a model using `RandomForestClassifier` or `LogisticRegression`.
- Evaluated using:
  - **Accuracy Score**
  - **Confusion Matrix**
  - **Classification Report**
- Extracted **feature importances** to identify top influencing variables.

---

## 📈 Visualizations

Created visual plots using Seaborn and Matplotlib:
- Survival by **Gender**
- Survival by **Passenger Class**
- Age distribution by **Survival Status**

These visuals helped uncover patterns and guided model intuition.

---

## 💾 Model Saving & Deployment

- Trained model saved using `joblib` or `pickle`.
- Can be reloaded and used for predictions on new data.

---

## ✅ Key Takeaways

- Importance of handling missing values correctly.
- Feature engineering greatly impacts model performance.
- Tree-based models provide interpretability through feature importances.
- Visualizations help build intuition and communicate insights.

---

## 📁 Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Jupyter Notebook
