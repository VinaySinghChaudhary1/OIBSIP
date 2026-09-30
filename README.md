<div align="center">

# 📊 OIBSIP — Oasis Infobyte Data Science Internship

### Vinay Singh Chaudhary · Data Science Intern · Oct – Nov 2026

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-Data-150458?logo=pandas&logoColor=white)
![Tasks](https://img.shields.io/badge/Tasks%20completed-5%20%2F%205-2ea44f)
![License](https://img.shields.io/badge/License-MIT-blue)

*A single repository holding all my task submissions for the **AICTE Oasis Infobyte Internship Program (OIBSIP)** — Data Science track.*

[Projects](#-projects-at-a-glance) · [Results](#-key-results) · [Run locally](#-run-the-projects-locally) · [Structure](#-repository-structure) · [Connect](#-connect-with-me)

</div>

---

## 👋 About this internship

| | |
|---|---|
| **Organisation** | [Oasis Infobyte](https://www.oasisinfobyte.com) — AICTE-approved internship program |
| **Domain** | Data Science |
| **Offer ref.** | OIB/O2/IP1954 |
| **Duration** | 1 month · commencement **5 Oct 2026** · final submission **15 Nov 2026** |
| **Requirement** | at least 3 of 5 tasks — **all 5 completed** ✅ |

Each task follows the program's workflow: **Review → Build → Push to GitHub → Demo video → LinkedIn post → Peer evaluation → Submit**.

---

## 🚀 Projects at a glance

| # | Project | Type | Techniques | Folder |
|:-:|---------|------|------------|--------|
| 1 | 🌸 **Iris Flower Classification** | Multi-class classification | EDA, pairplot, ANOVA feature ranking, LogReg / KNN / Tree / RF / SVM, 5-fold CV | [`DataScience-Task1-IrisFlowerClassification`](DataScience-Task1-IrisFlowerClassification) |
| 2 | 📉 **Unemployment Analysis (India, COVID-19)** | EDA & time series | Cleaning, datetime handling, state/zone trends, correlation, pre- vs post-lockdown | [`DataScience-Task2-UnemploymentAnalysis`](DataScience-Task2-UnemploymentAnalysis) |
| 3 | 🚗 **Car Price Prediction** | Regression | Text cleaning, feature engineering (age, brand, vehicle type), one-hot encoding, retained-value modelling, Gradient Boosting | [`DataScience-Task3-CarPricePrediction`](DataScience-Task3-CarPricePrediction) |
| 4 | 📧 **Email / SMS Spam Detection** | NLP binary classification | Text preprocessing, stemming, TF-IDF (1–2 grams), Naive Bayes / LogReg / SVM, threshold tuning, WordClouds | [`DataScience-Task4-EmailSpamDetection`](DataScience-Task4-EmailSpamDetection) |
| 5 | 📈 **Sales Prediction (Advertising)** | Regression | Linear vs Polynomial vs Random Forest, residual analysis, standardised coefficients, what-if budgeting | [`DataScience-Task5-SalesPrediction`](DataScience-Task5-SalesPrediction) |

---

## 🏆 Key results

| Task | Best model | Headline metric | Key insight |
|------|-----------|-----------------|-------------|
| 1 · Iris | K-Nearest Neighbours | **97.3 %** 5-fold CV accuracy | Petal length & width carry ~87 % of the signal |
| 2 · Unemployment | — (EDA) | Avg unemployment **9.5 % → 17.8 %** after lockdown (+87 %) | Urban always higher; Puducherry, Tamil Nadu, Jharkhand, Bihar hit hardest |
| 3 · Car price | Gradient Boosting on retained-value ratio | **R² = 0.97**, MAE ≈ ₹ 0.58 lakh | Predicting *% of new price kept* beat predicting price directly (R² 0.70 → 0.97) |
| 4 · Spam | Linear SVM (class-weighted) | **98.5 %** accuracy, spam **F1 = 0.94** | Lowering NB threshold to 0.3 lifts spam recall to ≈ 96 % |
| 5 · Sales | Polynomial Regression (deg 2) | **R² = 0.99**, RMSE ≈ 0.64 | Radio = best return per $, TV = biggest total impact, Newspaper ≈ 0 |

> Every notebook is fully executed — outputs and charts are visible directly on GitHub. Charts are also saved as PNG in each task's `outputs/` folder.

---

## 🛠️ Tech stack

`Python 3.11+` · `pandas` · `NumPy` · `matplotlib` · `seaborn` · `scikit-learn` · `NLTK` · `WordCloud` · `Jupyter Notebook`

---

## 💻 Run the projects locally

```bash
# 1. Clone the repository
git clone https://github.com/VinaySinghChaudhary1/OIBSIP.git
cd OIBSIP

# 2. (Recommended) create a virtual environment
python -m venv .venv
.venv\Scripts\activate          # Windows
# source .venv/bin/activate     # macOS / Linux

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch Jupyter and open any task notebook
jupyter notebook
```

Inside Jupyter: open a task folder → open `VinaySinghChaudhary_TaskN.ipynb` → **Kernel ▸ Restart & Run All**.
All datasets are included in each task's `data/` folder (Task 1 loads Iris from scikit-learn), so no downloads are required.

---

## 📁 Repository structure

```
OIBSIP/
├── README.md                     ← you are here
├── TASKS_OVERVIEW.md             ← objectives, checklists & results of all 5 tasks in one place
├── requirements.txt
├── LICENSE
├── DataScience-Task1-IrisFlowerClassification/
│   ├── README.md
│   ├── VinaySinghChaudhary_Task1.ipynb
│   └── outputs/                  ← saved charts (PNG)
├── DataScience-Task2-UnemploymentAnalysis/
│   ├── README.md
│   ├── VinaySinghChaudhary_Task2.ipynb
│   ├── data/                     ← Unemployment_in_India.csv, Unemployment_Rate_upto_11_2020.csv
│   └── outputs/
├── DataScience-Task3-CarPricePrediction/      (same layout — data/car_data.csv)
├── DataScience-Task4-EmailSpamDetection/      (same layout — data/spam.csv)
└── DataScience-Task5-SalesPrediction/         (same layout — data/Advertising.csv)
```

Folder names follow the program's mandatory format `OIBSIP/[TrackName]-[Task]-[ProjectName]/`,
and notebooks follow the file-naming format `YourName_TaskNumber`.

---

## 🎥 Demo videos

| Task | LinkedIn demo post |
|------|--------------------|
| 1 · Iris Flower Classification | *link will be added after posting* |
| 2 · Unemployment Analysis | *link will be added after posting* |
| 3 · Car Price Prediction | *link will be added after posting* |
| 4 · Email Spam Detection | *link will be added after posting* |
| 5 · Sales Prediction | *link will be added after posting* |

---

## 📚 Datasets & credits

| Task | Dataset | Source |
|------|---------|--------|
| 1 | Iris | Built into scikit-learn (`load_iris`) — Fisher, 1936 |
| 2 | Unemployment in India | Kaggle — *"Unemployment in India"* (CMIE data) |
| 3 | Vehicle dataset from CarDekho | Kaggle — *"Vehicle dataset from cardekho"* (`car data.csv`) |
| 4 | SMS Spam Collection | UCI Machine Learning Repository / Kaggle |
| 5 | Advertising | *An Introduction to Statistical Learning* / Kaggle `Advertising.csv` |

Datasets are redistributed here only for reproducibility of this learning project; all rights belong to their original authors.

---

## 🙏 Acknowledgement

Thanks to **Oasis Infobyte** for this hands-on internship opportunity. #oasisinfobyte #oibsip

## 🤝 Connect with me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Vinay%20Singh%20Chaudhary-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vinay-singh-chaudhary/)
[![GitHub](https://img.shields.io/badge/GitHub-VinaySinghChaudhary1-181717?logo=github&logoColor=white)](https://github.com/VinaySinghChaudhary1)

<div align="center"><sub>⭐ If you find this repository useful, consider giving it a star!</sub></div>
