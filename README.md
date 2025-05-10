# 🦠 COVID-19 Case Forecasting Using Machine Learning and LSTM

This project applies both traditional machine learning and deep learning techniques to forecast COVID-19 case surges globally. The primary objective is to support proactive public health planning by identifying early indicators of outbreak trends.

## 👩‍💻 Developed by
**Mehrvish Mirza** — Responsible for data preprocessing, exploratory data analysis (EDA), feature engineering, and model implementation.

## 📊 Project Overview
Leveraging the Kaggle COVID-19 Clean Complete dataset, this project builds a pipeline that transforms raw case data into predictive insights. It evaluates model performance using accuracy, recall, and F1 scores to determine their effectiveness in detecting case surges.

## 📁 Dataset Details
- **Source:** [Kaggle COVID-19 Clean Complete](https://www.kaggle.com/datasets/imdevskp/corona-virus-report)
- **Size:** ~49,000 records across 187 countries
- **Features:** Date, Region, Confirmed, Deaths, Recovered, Active, WHO Region

## 🧠 Techniques and Models
- **Preprocessing:** Label encoding, Min-Max scaling, and SMOTE for class balancing
- **EDA:** Statistical summaries, visualizations, and correlation analysis
- **Feature Engineering:** Lag variables, rolling averages, weekly percent changes
- **Models Implemented:**
  - Logistic Regression (baseline)
  - Random Forest
  - LSTM (two versions)
  - XGBoost

## 📈 Model Results Summary

| Model                | Accuracy | F1 Score (Surge / No Surge) |
|---------------------|----------|------------------------------|
| Logistic Regression | 0.788    | 0.65 / 0.85                  |
| Random Forest       | 1.000    | 1.00 / 1.00                  |
| LSTM (v1)           | 0.588    | 0.00 / 0.74                  |
| LSTM (v2)           | 0.901    | 0.87 / 0.92                  |
| XGBoost             | 0.999    | 0.99 / 0.99                  |

> The second LSTM and XGBoost models demonstrated strong predictive performance, highlighting their suitability for time-dependent data.

## 🗂 Repository Structure

```
covid-case-forecasting/
├── notebooks/
│   └── covid_case_trends.ipynb     # ML and LSTM forecasting workflow
├── requirements.txt                # Required Python libraries
└── README.md                       # Project documentation
```

## 🔗 Notebook Access
- [View in Google Colab](https://colab.research.google.com/drive/1j6goPviL65bVbJYrSNWuTSRgDwzLY5JC?usp=sharing)

## 🚀 Highlights
- Applied end-to-end forecasting pipeline using real-world time series data
- Compared traditional and deep learning approaches on public health use case
- Developed surge prediction models to support early intervention strategies

## 📄 License
Distributed under the MIT License.
