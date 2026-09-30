# 🗂️ Tasks Overview — OIBSIP Data Science Track

**Intern:** Vinay Singh Chaudhary · **Track:** Data Science · **Minimum required:** 3 of 5 · **Completed:** 5 of 5

This page maps **every item of the official Task-Card feature checklist** to where it is implemented in my notebooks,
so evaluators can verify completeness quickly.

---

## Program workflow followed for each task

| Step | What I do | Where |
|:----:|-----------|-------|
| 1 · Review | Read the task card & feature checklist | this page |
| 2 · Build | Clean, commented Jupyter Notebook | `DataScience-TaskN-*/VinaySinghChaudhary_TaskN.ipynb` |
| 3 · Push | Commit to this single `OIBSIP` repo using `[Track]-[Task]-[Project]` folders | GitHub |
| 4 · Demo video | Screen recording with a 2-second title card (Name · Track · Task) | LinkedIn |
| 5 · LinkedIn post | Video + tag **Oasis Infobyte** + `#oasisinfobyte` | LinkedIn |
| 6 · Peer evaluation | Substantive comments on ≥ 2 fellow interns' demo videos | LinkedIn |
| 7 · Submit | Official Task Submission Form with this repo link | Form |

---

## 🌸 Task 1 — Iris Flower Classification
**Objective:** classify iris flowers into Setosa / Versicolor / Virginica from 4 measurements.

| Checklist item | Status | Notebook section |
|----------------|:------:|------------------|
| Load Iris with `sklearn.datasets.load_iris()` | ✅ | §2 |
| EDA: shape, dtypes, nulls, descriptive statistics | ✅ | §3 |
| Pairplot by species + box plots per feature | ✅ | §4 (+ correlation heatmap) |
| Feature-selection discussion | ✅ | §5 — correlation, ANOVA F-test, RF importance |
| 80/20 `train_test_split` | ✅ | §6 (stratified) |
| ≥ 2 classifiers | ✅ | §7 — LogReg, KNN, Decision Tree, Random Forest, SVM |
| Accuracy, confusion matrix, classification report | ✅ | §8 |
| Best model declared with justification | ✅ | §9 — KNN, 97.3 % CV accuracy |
| Clean, commented notebook | ✅ | whole notebook |

## 📉 Task 2 — Unemployment Analysis with Python
**Objective:** regional & temporal unemployment trends in India with focus on COVID-19.

| Checklist item | Status | Notebook section |
|----------------|:------:|------------------|
| Dataset downloaded (Kaggle "Unemployment in India") | ✅ | `data/` |
| Loading, shape, nulls, type conversion | ✅ | §2–3 (28 empty rows dropped, dates parsed) |
| Region-wise averages, month-wise trends | ✅ | §4–5 |
| Time-series line chart ≥ 3 states | ✅ | §6 — 5 major states |
| Bar chart: top 10 states | ✅ | §7 |
| Heatmap: unemployment vs employment vs participation | ✅ | §8 |
| Pre-COVID vs post-COVID comparison | ✅ | §9 — split at 25-Mar-2020 lockdown |
| Written observations between charts | ✅ | after every chart |
| Extra | ➕ | Rural vs Urban (§10), zone-wise 2020 recovery (§11) |

## 🚗 Task 3 — Car Price Prediction with Machine Learning
**Objective:** predict a used vehicle's selling price.

| Checklist item | Status | Notebook section |
|----------------|:------:|------------------|
| Dataset downloaded (Kaggle "Vehicle dataset from cardekho") | ✅ | `data/car_data.csv` |
| Cleaning: nulls, duplicates, inconsistent categories | ✅ | §3 |
| Feature engineering: car age, brand from name | ✅ | §4 (+ vehicle type) |
| EDA: price distribution, price vs fuel box plot, price vs age scatter | ✅ | §5 |
| Encoding (One-Hot) | ✅ | §6 |
| Correlation heatmap | ✅ | §7 |
| Train/test split | ✅ | §8 |
| ≥ 2 regression models | ✅ | §9 — Linear, Tree, RF, GB (+ retained-value versions) |
| MAE, RMSE, R² | ✅ | §9 |
| Feature-importance chart for best model | ✅ | §10 |

## 📧 Task 4 — Email Spam Detection with Machine Learning
**Objective:** NLP classifier separating spam from ham.

| Checklist item | Status | Notebook section |
|----------------|:------:|------------------|
| Dataset downloaded (SMS Spam Collection) | ✅ | `data/spam.csv` |
| Class distribution (counts & %) | ✅ | §3 |
| Preprocessing: lowercase, punctuation, stopwords, stemming | ✅ | §4 |
| TF-IDF + markdown explanation | ✅ | §5 |
| Train/test split | ✅ | §5 (stratified) |
| Multinomial NB + alternative | ✅ | §6 — NB, Logistic Regression, Linear SVM |
| Accuracy, precision, recall, F1, confusion matrix | ✅ | §6–7 |
| "Why is recall important?" discussion | ✅ | §8 (+ threshold tuning) |
| (Bonus) WordClouds | ✅ | §9 |

## 📈 Task 5 — Sales Prediction Using Python
**Objective:** predict sales from TV / Radio / Newspaper ad spend.

| Checklist item | Status | Notebook section |
|----------------|:------:|------------------|
| Dataset downloaded (Advertising.csv) | ✅ | `data/` |
| EDA: nulls, statistics, pairplot | ✅ | §3 |
| Scatter plots: Sales vs TV / Radio / Newspaper | ✅ | §4 |
| Correlation heatmap | ✅ | §5 |
| Train/test split | ✅ | §6 |
| Linear Regression baseline + ≥ 1 other model | ✅ | §7 — Polynomial (deg 2), Random Forest |
| MAE, RMSE, R² | ✅ | §7 |
| Residual plot for best model | ✅ | §8 |
| Which channel has the highest impact? | ✅ | §9 — coefficients + RF importance |

---

## 📊 Summary of results

| Task | Best approach | Result |
|------|---------------|--------|
| 1 | KNN (scaled) | 97.3 % CV accuracy · 93.3 % test accuracy |
| 2 | EDA | Unemployment +87 % after lockdown (9.5 % → 17.8 %) |
| 3 | Gradient Boosting on retained-value ratio | R² 0.97 · MAE ₹ 0.58 lakh |
| 4 | Linear SVM (class-weighted) | Accuracy 98.5 % · spam F1 0.94 |
| 5 | Polynomial Regression (deg 2) | R² 0.99 · RMSE 0.64 |

*Evaluation criteria addressed: code quality & structure · creativity & problem-solving · completeness & functionality · documentation clarity.*
