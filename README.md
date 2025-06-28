# 📊 Telco Churn Analytics

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/yourusername/telco-churn-analytics/HEAD)

Predict customer churn in telecom using machine learning. This project analyzes key churn drivers, visualizes insights, and builds actionable strategies to help marketing teams improve customer retention.

## 📌 Project Overview

In this project, we apply **Logistic Regression**, **Decision Tree**, and **Random Forest** models to predict churn in a telecom dataset. We focus on:

- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Model training and evaluation
- Cross-validation for stability
- Hyperparameter tuning
- Model interpretability (coefficients, odds ratios, logistics regression visualization)
- Insights for marketing strategies


---

## 📂 Project Structure

```telco-churn-analytics/
├── data/ # Dataset (e.g., telco.csv)
├── notebooks/ # Jupyter notebooks for EDA & modeling
├── src/ # (Optional) scripts for modular code
├── models/ # Saved trained models
├── outputs/ # Generated figures, reports
├── requirements.txt # Python dependencies
├── .gitignore # Ignored files/folders
├── LICENSE # License (MIT recommended)
└── README.md # This file

```
---

## 🚀 Quick Start

1️⃣ **Clone this repo**  
```bash
git clone https://github.com/yourusername/telco-churn-analytics.git
cd telco-churn-analytics
```

2️⃣ **Create virtual environment with uv**
```bash
uv venv venv
venv\Scripts\activate
```

3️⃣ **Install dependencies**
``` bash
uv pip install -r requirements.txt
```
4️⃣ ***Launch the notebook***
``` bash
jupyter notebook notebooks/01_telco_churn_analysis.ipynb
```
📈 Results Highlights
✅ Best Model: Tuned Logistic Regression
✅ Cross-validated ROC AUC: ~0.84
✅ Top churn drivers:

📉 Fiber optic internet → increases churn risk

📈 Longer tenure → reduces churn risk

📃 Contract type → two-year contracts significantly lower churn

🔎 Key Insights
- Top churn drivers:
InternetService_Fiber optic, MonthlyCharges, Contract_Two year, tenure

- Best model: Tuned Logistic Regression (balanced performance + interpretability)
- ** Insights for Marketing **
Customers with Fiber optic internet and month-to-month contracts are at higher churn risk.

Customers with two-year contracts or long tenure are less likely to churn.

Promote longer contracts and service bundles to improve retention.

💻 Technologies Used
Python (pandas, numpy, scikit-learn, seaborn, matplotlib)

Jupyter Notebook

uv (fast Python package management)

Git & GitHub

📝 License
This project is licensed under the MIT License. See LICENSE for details.

🙌 Acknowledgements
Dataset inspired by IBM Telco Customer Churn sample dataset.

Thanks to the open-source community for tools that make this work possible!

🤝 Contributing
Pull requests are welcome! If you’d like to add features, improve documentation, or extend the analysis:

Fork the repo

Create a new branch (git checkout -b feature/my-feature)

Commit your changes (git commit -m 'Add new feature')

Push to the branch (git push origin feature/my-feature)

Open a Pull Request

📬 Contact
Have questions? Feel free to open an issue or reach out via [your-email@example.com].
