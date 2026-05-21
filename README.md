# 🏏 Cricket Match Outcome Prediction using Machine Learning

## 📌 Project Overview
This project applies **Machine Learning techniques** to analyze cricket ODI match data from the **Cricsheet dataset** and predict match outcomes using ball-by-ball and match-level features.

We explore:
- Data extraction from YAML files
- Feature engineering on cricket statistics
- Exploratory Data Analysis (EDA)
- Machine learning model training
- Model comparison (Logistic Regression, Random Forest, XGBoost)

---

## 📂 Dataset
- Source: Cricsheet ODI Dataset
- Format: YAML files (ball-by-ball data)
- Converted into structured CSV for analysis

---

## ⚙️ Workflow

### 1. Data Processing
- Parsed YAML match files
- Extracted:
  - Runs, extras, wickets
  - Match info (teams, venue, toss, winner)
- Converted into structured DataFrame

### 2. Feature Engineering
- Run rate
- Required run rate
- Balls left / runs left
- Toss impact
- Venue-based statistics
- Team performance metrics

### 3. Exploratory Data Analysis (EDA)
- Correlation heatmaps
- Run distribution per inning
- Toss impact on winning probability
- Venue scoring trends

### 4. Machine Learning Models
We trained and compared:

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### 5. Evaluation Metrics
- Accuracy
- Log Loss
- ROC-AUC
- Precision-Recall Curve
- Confusion Matrix
- Sensitivity & Specificity

---

## 🏆 Results Summary

| Model              | Accuracy | AUC   | Log Loss |
|-------------------|----------|-------|----------|
| Logistic Regression | ~XX%     | ~XX   | ~XX      |
| Random Forest       | ~XX%     | ~XX   | ~XX      |
| XGBoost             | ~XX%     | ~XX   | ~XX      |

👉 XGBoost performed best overall in most experiments.

---

## 📊 Visualizations
- Correlation Heatmap
- ROC Curves Comparison
- Precision-Recall Curve
- Feature Importance (Random Forest)
- Team performance analysis

---

## 🧰 Tech Stack
- Python 🐍
- Pandas / NumPy
- Scikit-learn
- XGBoost
- Matplotlib / Seaborn
- YAML parsing

---

## 🚀 How to Run

### 1. Clone repository
```bash
git clone https://github.com/your-username/cricket-ml-analysis.git
cd cricket-ml-analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run notebooks
Open Jupyter / Colab and run notebooks in order:

```
01 → 02 → 03 → 04 → 05
```

---

## 📦 Requirements
```
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
pyyaml
```

---

## 📈 Future Improvements
- Deep learning (LSTM for innings prediction)
- Live match win probability API
- Player-level performance modeling
- IPL dataset extension
- Real-time dashboard (Streamlit)

---

## 👩‍💻 Author
**Hamna Mushtaq**

---

## ⭐ If you like this project
Give it a ⭐ on GitHub!
