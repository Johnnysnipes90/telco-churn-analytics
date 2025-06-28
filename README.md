# 📊 Telco Churn Analytics

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/yourusername/telco-churn-analytics/HEAD)

Predict customer churn in telecom using machine learning. This project analyzes key churn drivers, visualizes insights, and builds actionable strategies to help marketing teams improve customer retention.

---

## 📌 Project Overview

In this project, we apply **Logistic Regression**, **Decision Tree**, and **Random Forest** models to predict customer churn in a telecommunications dataset. The project covers:

✅ Data cleaning and preprocessing  
✅ Exploratory data analysis (EDA)  
✅ Model training and evaluation  
✅ Cross-validation for model stability  
✅ Hyperparameter tuning  
✅ Model interpretability (coefficients & odds ratios)  
✅ Actionable insights for marketing strategies

---

## 📂 Project Structure

```plaintext
telco-churn-analytics/
├── data/               # Dataset files (e.g., telco.csv)
├── notebooks/          # Jupyter notebooks for EDA & modeling
├── src/                # (Optional) modular scripts
├── models/             # Saved trained models
├── outputs/            # Generated figures and reports
├── requirements.txt    # Python dependencies
├── .gitignore          # Ignored files/folders
├── LICENSE             # License file
└── README.md           # This file
```

---

## 📄 Dataset Description

Below is a summary of the main features in the cleaned Telco churn dataset:

| Feature              | Type         | Description                                                |
|----------------------|--------------|------------------------------------------------------------|
| customerID           | Object (ID)  | Unique customer identifier (dropped before modeling).      |
| gender               | Categorical  | Customer gender (`Male`/`Female`).                         |
| SeniorCitizen        | Integer      | 1 if customer is a senior citizen, else 0.                 |
| Partner              | Categorical  | Whether the customer has a partner (`Yes`/`No`).           |
| Dependents           | Categorical  | Whether the customer has dependents (`Yes`/`No`).          |
| tenure               | Numeric      | Number of months the customer has stayed.                  |
| PhoneService         | Categorical  | Whether the customer has phone service.                    |
| MultipleLines        | Categorical  | Multiple phone lines (`Yes`, `No`, or `No phone service`). |
| InternetService      | Categorical  | Type of internet service (`DSL`, `Fiber optic`, `No`).     |
| OnlineSecurity       | Categorical  | Online security add-on (`Yes`, `No`, `No internet service`).|
| OnlineBackup         | Categorical  | Online backup add-on.                                      |
| DeviceProtection     | Categorical  | Device protection add-on.                                  |
| TechSupport          | Categorical  | Technical support add-on.                                  |
| StreamingTV          | Categorical  | Streaming TV add-on.                                       |
| StreamingMovies      | Categorical  | Streaming movies add-on.                                   |
| Contract             | Categorical  | Contract type (`Month-to-month`, `One year`, `Two year`).  |
| PaperlessBilling     | Categorical  | Whether the customer uses paperless billing.               |
| PaymentMethod        | Categorical  | Payment method (`Electronic check`, `Mailed check`, etc.). |
| MonthlyCharges       | Numeric      | Monthly billing amount in USD.                             |
| TotalCharges         | Numeric      | Total amount charged during tenure in USD.                 |
| Churn                | Binary       | Target variable: whether the customer churned (`Yes`/`No`).|

**Dataset size**: 7,032 rows × 20 features (after cleaning, with customerID dropped).

---

## 🚀 Quick Start

1️⃣ **Clone this repo**
```bash
git clone https://github.com/yourusername/telco-churn-analytics.git
cd telco-churn-analytics
```

2️⃣ **Create a virtual environment with [uv](https://github.com/astral-sh/uv)**
```bash
uv venv venv
# Activate on Windows
venv\Scripts\activate
# Or on macOS/Linux
source venv/bin/activate
```

3️⃣ **Install dependencies**
```bash
uv pip install -r requirements.txt
```

4️⃣ **Launch the notebook**
```bash
jupyter notebook notebooks/01_telco_churn_analysis.ipynb
```

---

## 📈 Results Highlights

✅ **Best Model:** Tuned Logistic Regression  
✅ **Cross-validated ROC AUC:** ~0.84  
✅ **Top churn drivers:**
- Fiber optic internet → significantly increases churn risk
- Longer tenure → reduces churn risk
- Contract type → two-year contracts greatly lower churn risk

---

## 🔎 Key Insights

- Customers with **Fiber optic internet** and **month-to-month contracts** are at the highest risk of churning.
- Customers on **two-year contracts** or with **long tenure** are far less likely to churn.
- Marketing strategies like promoting longer contracts or bundling services can improve retention.

---

## 💻 Technologies Used

- **Python**: pandas, numpy, scikit-learn, seaborn, matplotlib  
- **Jupyter Notebook**  
- **uv** (fast Python package management)  
- **Git & GitHub**

---

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

Dataset inspired by the IBM Telco Customer Churn sample dataset.

Special thanks to the open-source community for the amazing tools that made this project possible!

---

## 🤝 Contributing

Contributions are welcome! 🚀 If you’d like to add features, improve documentation, or extend the analysis:

1. Create a new branch
   ```bash
   git checkout -b feature/my-feature
   ```
2. Commit your changes
   ```bash
   git commit -m "Add new feature"
   ```
3. Push to the branch
   ```bash
   git push origin feature/my-feature
   ```
4. Open a Pull Request

---

## 📬 Contact

Questions or suggestions? Open an issue or reach out at [johnolalemi90@gmail.com](mailto:johnolalemi90@gmail.com).
