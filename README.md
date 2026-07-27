# 🧬 Antimicrobial Resistance Prediction using Machine Learning

A complete machine learning pipeline for predicting **Antimicrobial Resistance (AMR)** from bacterial genome metadata using the BV-BRC dataset. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and comparison of multiple classification algorithms.

---

## 📌 Project Overview

Antimicrobial Resistance (AMR) is one of the biggest global healthcare challenges. This project applies supervised machine learning techniques to classify bacterial samples as resistant or non-resistant based on genome metadata.

The notebook demonstrates an end-to-end machine learning workflow including:

- Data loading
- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Feature Encoding
- Train-Test Split
- Model Training
- Model Evaluation
- Performance Comparison

---

## 📂 Project Structure

```
.
├── notebook.ipynb
├── requirements.txt
├── README.md
├── .gitignore
└── data/
    └── BVBRC_genome_amr.csv   (Not included)
```

---

## 📊 Dataset

This project uses the **BV-BRC Genome AMR Dataset**.

The dataset is **not included** in this repository due to its large size.

After obtaining the dataset, place the ZIP file inside the `data/` folder.

```
data/
└── BVBRC_genome_amr.zip
```

The notebook reads the dataset directly from the ZIP file using Pandas, so there is no need to extract it manually.

Example:

```python
import pandas as pd

df = pd.read_csv("data/BVBRC_genome_amr.zip", compression="zip", low_memory=False)
```

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Google Colab

---

## 🚀 Machine Learning Pipeline

### 1. Data Loading

- Import dataset
- Inspect data types
- Understand dataset dimensions

### 2. Exploratory Data Analysis

- Missing value analysis
- Resistant phenotype distribution
- Feature visualization
- Class imbalance inspection

### 3. Data Cleaning

- Remove missing target values
- Handle invalid records
- Prepare clean dataset

### 4. Feature Engineering

Examples include:

- Genus extraction
- Metadata processing
- Categorical feature preparation

### 5. Data Preprocessing

- Label Encoding
- One-Hot Encoding
- Feature selection

### 6. Model Training

Models implemented:

- XGBoost Classifier
- Random Forest Classifier

### 7. Model Evaluation

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

---

## ▶️ How to Run

### Clone the repository

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Place the dataset

Create a folder named:

```
data/
```

Copy

```
BVBRC_genome_amr.csv
```

into that folder.

### Open the notebook

Run the notebook using:

- Jupyter Notebook
- Jupyter Lab
- Google Colab

---

## 📈 Results

The project compares the performance of:

- XGBoost
- Random Forest

using multiple evaluation metrics to determine the most effective classifier for AMR prediction.

---

## 📌 Future Improvements

- Hyperparameter tuning
- Cross-validation
- Additional feature engineering
- Explainable AI (SHAP/LIME)
- Model deployment using Flask or FastAPI
- Deep learning approaches

---

## 📄 License

This project is for educational and research purposes.

---

## 👩‍💻 Author

**Ayesha Akram**

BS Computer Science

Machine Learning & AI Enthusiast
