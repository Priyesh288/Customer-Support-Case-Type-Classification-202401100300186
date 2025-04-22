# 🧠 Support Case Classification using Random Forest

This project demonstrates how to build a machine learning classifier that predicts the type of a support case based on message length and response time. It uses a Random Forest model for classification and includes visualizations and an example for predicting new cases.

---

## 📂 Dataset

The dataset is expected to be a CSV file named `support_cases.csv` with the following columns:

- `message_length` – Length of the support message (in characters)
- `response_time` – Time taken to respond (in minutes)
- `case_type` – The category of the support case (target variable)

---

## ⚙️ How It Works

### 1. **Data Preparation**
- Load the dataset using `pandas`
- Select features (`message_length`, `response_time`) and the target (`case_type`)

### 2. **Model Training**
- Split data into training and test sets
- Train a `RandomForestClassifier`

### 3. **Evaluation**
- Compute accuracy and classification metrics
- Display confusion matrix
- Visualize case type distribution

### 4. **Prediction**
- Use `classify_case()` function to predict new, unseen cases

---

## 📈 Visualizations

- 📊 **Distribution of Case Types** – Helps understand class balance
- 🔲 **Confusion Matrix** – Measures model performance visually

---

## 🧪 Example Prediction

```python
classify_case(250, 20)  # Predicts case type based on message length and response time
