<div align="center">

# 🏏 Cricket Match Outcome Prediction

### 🤖 Machine Learning • Cricket Analytics • Predictive Modeling

**Predicting ODI match outcomes using ball-by-ball data, feature engineering, and machine learning.**

<br>

<img src="https://img.shields.io/badge/🏏_CRICKET-ANALYTICS-16A34A?style=for-the-badge" />
<img src="https://img.shields.io/badge/🤖_MACHINE-LEARNING-8B5CF6?style=for-the-badge" />
<img src="https://img.shields.io/badge/🐍_PYTHON-DATA%20SCIENCE-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/📊_PREDICTION-ODI%20MATCHES-F59E0B?style=for-the-badge" />

<br><br>

> **From every ball to the final result. 🏏**
>
> A machine learning pipeline that transforms raw cricket match data into meaningful features and outcome predictions.

</div>

---

# 🏏 What is This Project?

**Cricket Match Outcome Prediction** is a machine learning project built around **ODI cricket data from Cricsheet**.

The project takes detailed **ball-by-ball match data**, transforms it into structured information, engineers meaningful cricket features, performs exploratory analysis, and trains multiple classification models to predict match outcomes.

### The pipeline:

```text
🏏 Raw Cricket Data
        ↓
📄 YAML Match Files
        ↓
🧹 Data Processing
        ↓
🔧 Feature Engineering
        ↓
📊 Exploratory Data Analysis
        ↓
🤖 Machine Learning
        ↓
📈 Model Evaluation
        ↓
🏆 Match Outcome Prediction
```

---

# 🎯 Project Objectives

The main objective is to explore whether information available during and around an ODI match can be transformed into useful predictive features.

### 🔍 We investigate:

* How match statistics influence outcomes
* Whether toss information contributes to prediction
* How run rate affects winning probability
* How venue characteristics influence matches
* How different machine learning models perform
* Which features contribute most to predictions

---

# 📂 Dataset

### 🏏 Cricsheet ODI Dataset

The project uses **Cricsheet ODI match data** containing detailed ball-by-ball information.

| Data          | Description                       |
| ------------- | --------------------------------- |
| 📄 Format     | YAML                              |
| 🏏 Match Type | ODI                               |
| 🎯 Target     | Match Outcome                     |
| ⚾ Granularity | Ball-by-ball                      |
| 🔄 Processing | YAML → Structured DataFrame / CSV |

### Extracted Information

* Teams
* Venue
* Toss
* Match winner
* Runs
* Extras
* Wickets
* Innings information
* Ball-by-ball events

---

# ⚙️ Data Science Workflow

## 1️⃣ Data Processing

Raw YAML files are parsed and transformed into structured data.

```text
YAML Files
   │
   ├── Match Information
   ├── Teams
   ├── Toss
   ├── Venue
   ├── Innings
   ├── Runs
   ├── Extras
   └── Wickets
          │
          ▼
   📊 Structured Dataset
```

---

## 2️⃣ Feature Engineering

Raw cricket events are transformed into predictive features.

### 🏏 Match Features

* Team information
* Toss decision
* Toss winner
* Venue
* Match context

### 📈 Performance Features

* Run rate
* Required run rate
* Runs remaining
* Balls remaining
* Wickets remaining
* Team performance metrics

### 🎯 Engineered Features

```text
Runs
 ├── Current Score
 ├── Runs Required
 └── Run Rate

Overs
 ├── Balls Bowled
 ├── Balls Remaining
 └── Required Run Rate

Wickets
 ├── Wickets Lost
 └── Wickets Remaining

Match Context
 ├── Toss
 ├── Venue
 └── Team Performance
```

---

# 📊 Exploratory Data Analysis

Before training the models, the dataset is explored to understand patterns within ODI cricket.

### 🔎 Analysis Includes

📌 Correlation Analysis
📌 Run Distribution
📌 Toss Impact
📌 Venue Scoring Trends
📌 Team Performance
📌 Feature Relationships

### 📈 Example Questions

> 🏏 Does winning the toss increase the probability of winning?

> 📊 How does run rate change throughout an innings?

> 🏟️ Which venues tend to produce higher scores?

> 🎯 Which features are most strongly associated with match outcomes?

---

# 🤖 Machine Learning Models

Three classification models are trained and compared.

<table>
<tr>
<td align="center">

### 📊 Logistic Regression

A baseline classification model used to establish a simple predictive benchmark.

</td>

<td align="center">

### 🌲 Random Forest

An ensemble model capable of capturing nonlinear relationships between cricket features.

</td>

<td align="center">

### ⚡ XGBoost

A powerful gradient-boosting model used for high-performance classification.

</td>
</tr>
</table>

---

# 🧠 Model Pipeline

```text
              📊 FEATURES
                  │
                  ▼
          ┌───────────────┐
          │ Train / Test  │
          │    Split      │
          └───────┬───────┘
                  │
       ┌──────────┼──────────┐
       ▼          ▼          ▼
   📊 Logistic  🌲 Random   ⚡ XGBoost
    Regression   Forest
       │          │          │
       └──────────┼──────────┘
                  ▼
          📈 Evaluation
                  │
       ┌──────────┼──────────┐
       ▼          ▼          ▼
    Accuracy     AUC      Log Loss
```

---

# 📏 Evaluation Metrics

The models are evaluated using multiple metrics rather than relying only on accuracy.

| Metric                  | What it tells us                                |
| ----------------------- | ----------------------------------------------- |
| 🎯 **Accuracy**         | Overall percentage of correct predictions       |
| 📈 **ROC-AUC**          | Model's ability to distinguish between outcomes |
| 📉 **Log Loss**         | Quality of predicted probabilities              |
| 🔎 **Precision**        | Accuracy of positive predictions                |
| 🧲 **Recall**           | Ability to identify positive outcomes           |
| 🧮 **Confusion Matrix** | Breakdown of correct and incorrect predictions  |
| ⚖️ **Sensitivity**      | True positive detection                         |
| 🛡️ **Specificity**     | True negative detection                         |

---

# 🏆 Model Comparison

> 📌 **Note:** Replace the placeholder values below with the actual results from the experiments before publishing.

| Model                  | Accuracy | ROC-AUC | Log Loss |
| ---------------------- | :------: | :-----: | :------: |
| 📊 Logistic Regression |   `XX%`  |   `XX`  |   `XX`   |
| 🌲 Random Forest       |   `XX%`  |   `XX`  |   `XX`   |
| ⚡ XGBoost              |   `XX%`  |   `XX`  |   `XX`   |

### 🥇 Best Performing Model

**XGBoost** performed best overall across most experiments.

The final comparison is based on the evaluation metrics calculated from the test data.

---

# 📊 Visualizations

The project includes several visual analyses to understand both the dataset and model behavior.

### 🔥 Correlation Heatmap

Shows relationships between numerical cricket features.

### 📈 ROC Curve Comparison

Compares the classification performance of different models.

### 🎯 Precision-Recall Curve

Evaluates the trade-off between precision and recall.

### 🌲 Feature Importance

Highlights the features contributing most strongly to Random Forest predictions.

### 🏏 Team Performance Analysis

Explores team-level patterns and historical performance.

---

# 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python" />

</div>

| Category                | Technologies                    |
| ----------------------- | ------------------------------- |
| 🐍 **Language**         | Python                          |
| 📊 **Data Processing**  | Pandas, NumPy                   |
| 🤖 **Machine Learning** | Scikit-learn, XGBoost           |
| 📈 **Visualization**    | Matplotlib, Seaborn             |
| 📄 **Data Parsing**     | PyYAML                          |
| 📓 **Environment**      | Jupyter Notebook / Google Colab |

---

# 📁 Project Workflow

```text
cricket-ml-analysis/
│
├── 📓 notebooks/
│   ├── 01_data_extraction
│   ├── 02_data_processing
│   ├── 03_feature_engineering
│   ├── 04_eda
│   └── 05_model_training
│
├── 📊 data/
│   ├── raw/
│   └── processed/
│
├── 📈 visualizations/
│
├── 📄 requirements.txt
│
└── 📘 README.md
```

---

# 🚀 Getting Started

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/cricket-ml-analysis.git

cd cricket-ml-analysis
```

## 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

## 3️⃣ Launch the Notebooks

Open the project using **Jupyter Notebook** or **Google Colab**.

Run the notebooks in order:

```text
01 → 02 → 03 → 04 → 05
```

---

# 📦 Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
pyyaml
```

Install everything with:

```bash
pip install -r requirements.txt
```

---

# 🔬 End-to-End ML Pipeline

```text
        🏏 CRICSHEET
             │
             ▼
       📄 YAML FILES
             │
             ▼
      🧹 DATA CLEANING
             │
             ▼
    🔧 FEATURE ENGINEERING
             │
             ▼
          📊 EDA
             │
             ▼
      ✂️ TRAIN / TEST
             │
       ┌─────┼─────┐
       ▼     ▼     ▼
      📊    🌲    ⚡
      LR     RF   XGB
       │     │     │
       └─────┼─────┘
             ▼
       📏 EVALUATION
             │
             ▼
       🏆 PREDICTION
```

---

# 💡 Key Learning Outcomes

This project provided hands-on experience with:

### 🧹 Data Engineering

Parsing raw YAML files and transforming unstructured match information into analysis-ready datasets.

### 🔧 Feature Engineering

Turning cricket concepts such as run rate, required runs, wickets, and balls remaining into machine learning features.

### 📊 Exploratory Analysis

Using statistical visualization to identify patterns within ODI matches.

### 🤖 Machine Learning

Training multiple classification algorithms and comparing their performance.

### 📏 Model Evaluation

Understanding why accuracy alone isn't enough when evaluating predictive models.

### 🏏 Domain-Based Modeling

Applying machine learning concepts to a real-world sports analytics problem.

---

# 📊 Project at a Glance

<table>
<tr>
<td align="center">

🏏<br> <b>ODI DATA</b>

</td>
<td align="center">

📄<br> <b>YAML PARSING</b>

</td>
<td align="center">

🔧<br> <b>FEATURE ENGINEERING</b>

</td>
<td align="center">

🤖<br> <b>ML MODELS</b>

</td>
<td align="center">

📈<br> <b>EVALUATION</b>

</td>
</tr>
</table>

---

# 🔗 Google Colab

<div align="center">

### 📓 Explore the Analysis

<a href="https://colab.research.google.com/drive/1T2z8jzClo432C76Hd9X6rnh6Zg4owlnS?usp=sharing">

<img src="https://img.shields.io/badge/🚀_OPEN_IN-GOOGLE_COLAB-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />

</a>

</div>

---

# 👩‍💻 Author

<div align="center">

### **Hamna Mushtaq**

🏏 Sports Analytics · 🤖 Machine Learning · 🐍 Python · 📊 Data Science

</div>

---

<div align="center">

# 🏏 From Ball-by-Ball Data to Match Predictions

**Turning cricket data into machine learning insights. 🤖📊**

<br>

⭐ **If you found this project interesting, consider starring the repository!**

</div>
