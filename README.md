# 📱 Mobile Price Classifier Using AWS SageMaker

This project demonstrates an end-to-end machine learning pipeline for classifying mobile phone prices using a Random Forest model, with training and deployment on **AWS SageMaker**.

---

## 📌 Problem Statement

Given features like battery power, RAM, screen size, etc., predict the **price range** of a mobile phone (0 to 3).

---

## 🚀 Features

- 📊 Data preprocessing and EDA in Jupyter Notebook
- 🔍 Feature engineering and selection
- 🧠 Model training using `RandomForestClassifier`
- 📈 Model evaluation using accuracy and classification metrics
- ☁️ Deployment-ready script compatible with **AWS SageMaker**
- 🧪 Includes test/train CSV datasets and configurable hyperparameters

---
---

## ⚙️ How to Run

### 🧪 Locally

1. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2. Run the script:
    ```bash
    python script.py --n_estimators 100 --random_state 0 \
        --model-dir ./model --train ./ --test ./ \
        --train_file train_v1.csv --test_file test_v1.csv
    ```

### ☁️ On AWS SageMaker

- Upload `script.py`, training/testing CSV files.
- Use SageMaker’s training job configuration.
- Output model will be saved as `model.joblib`.

---

## 🧪 Model Performance (Example)

- Accuracy: ~89%
- Class-wise precision & recall reported via `classification_report`.

---

## 🛠️ Tech Stack

- Python 3.x
- Scikit-learn
- Pandas, NumPy
- AWS SageMaker
- Joblib

---

## 📜 License

This project is for educational purposes. Free to use and adapt.

---

## ✍️ Author

**Swaraj SD**  
🔗 [GitHub Profile](https://github.com/SwarajSD)
