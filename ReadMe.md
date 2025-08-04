# 🧠 Mental Health Prediction Based on Survey Responses

This project predicts whether an individual might experience mental health issues at work, based on responses from a publicly available mental health survey. We built a classification model using a Random Forest Classifier, achieving a test accuracy of over 85%.

---

## 📊 Dataset Overview

- Source: Open mental health in tech industry survey
- Target: `treatment` (whether the individual has sought treatment for mental health)

### 🧾 Features include:
- Age, Gender, Country, State
- Family history of mental illness
- Remote work, company size, benefits
- Attitude towards mental health at workplace
- Work interference, supervisor support, etc.

---

## ⚙️ ML Pipeline

1. **Data Cleaning**
   - Filled missing values using `.fillna()` (mean for numerical, "unknown" for categorical)
   - Dropped excessive NaNs initially (consider using `SimpleImputer` instead to avoid data loss)

2. **Encoding**
   - Categorical columns were label encoded using `LabelEncoder()`

3. **Standardization**
   - StandardScaler used to normalize feature distributions

4. **Model**
   - `RandomForestClassifier` from `sklearn.ensemble`
   - Trained on 90% of data, tested on 10%

---

## 🧠 Model Performance

| Metric           | Training Set | Testing Set |
|------------------|--------------|-------------|
| Accuracy_score   | ~88%         | ~84%        |
|  F1_score        | ~88.4%       | ~85%        |


## ⚙️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mental-health-predictor.git


2. Navigate into the project directory
   ```bash
   cd mental-health-predictor

3. Install dependencies:
   ```bash
   pip install -r requirements.txt

4. Launch the Jupyter Notebook:
    ```bash
    jupyter notebook

## ✍️ Author

**Tanya Chauhan** 
