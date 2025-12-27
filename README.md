# Building Energy Efficiency Analysis & Load Prediction

**Portfolio Project | Data Analysis & Machine Learning**

## Project Summary

This project analyzes how **building design choices** influence **heating and cooling energy demand** using the Energy Efficiency dataset.
I applied **exploratory data analysis, predictive modeling, and explainability techniques** to quantify the impact of geometry and glazing on energy consumption.

The focus is on:

* Translating **engineering features into data insights**
* Building **interpretable baseline models**
* Producing **actionable recommendations** relevant to real-world decision-making

---

## Problem Statement

Energy consumption in buildings is strongly affected by architectural design.
This project answers:

> *Which building features most strongly drive heating and cooling demand, and how well can we predict energy load from early-stage design parameters?*

---

## Dataset Overview

The dataset contains simulated residential building designs with varying geometry and glazing configurations.

**Key Inputs**

* Relative Compactness
* Wall Area, Roof Area, Surface Area
* Building Height & Orientation
* Glazing Area & Distribution

**Targets**

* Heating Load (kWh/m²)
* Cooling Load (kWh/m²)

---

## Analytical Approach

1. Data validation and preparation
2. Exploratory Data Analysis (EDA)
3. Feature–target relationship analysis
4. Linear Regression modeling (baseline)
5. Model evaluation and interpretation
6. Explainability using SHAP

---

## Key Results

| Target       | R² Score | RMSE  |
| ------------ | -------- | ----- |
| Heating Load | ~0.92    | ~2.91 |
| Cooling Load | ~0.89    | ~3.19 |

**Insight:**
A simple linear model explains most of the variability, indicating that building energy demand follows **strong, interpretable physical relationships**.

> ⚠️ Note: Metrics were initially computed on the training data to establish a baseline. For production or policy decisions, train/test split or cross-validation should be applied.

---

## Key Insights (What Matters)

* **Compact buildings** consistently reduce both heating and cooling demand
* **Wall area and glazing percentage** are major drivers of energy consumption
* **Heating load behaves more linearly** than cooling load
* **Excessive glazing significantly increases cooling demand**, especially when concentrated on solar-exposed façades

---

## Model Explainability

* Linear coefficients align with physical heat-transfer principles
* SHAP analysis confirms:

  * Relative compactness lowers energy demand
  * Glazing area and wall area increase energy load
* Results are **transparent, explainable, and stakeholder-friendly**

---

## 🛠 Tech Stack

* **Python**
* **Pandas, NumPy**
* **Matplotlib, Seaborn**
* **Scikit-learn**
* **SHAP**

---

## ▶️ How to Run the Project

```bash
git clone https://github.com/GogoHarry/building-energy-efficiency.git
cd building-energy-efficiency
pip install -r requirements.txt
jupyter notebook
```

Open:

```text
notebooks/energy_efficiency_analysis.ipynb
```

---

## 📁 Project Structure

```text
building-energy-efficiency/
│
├── data/
├── notebooks/
├── images/
├── requirements.txt
└── README.md
```

---

## Actionable Recommendations

* Prioritize **compact building forms** in early design
* Limit glazing percentage, especially on solar-exposed sides
* Use interpretable models to support **early-stage energy decisions**
* Apply more advanced models only after establishing a strong baseline

---

## Future Improvements

* Train/test split and cross-validation
* Non-linear models (Random Forest, XGBoost)
* Climate-specific weather integration
* Deployment as an energy estimation tool

---

## 👤 About Me

I’m a **Data Analyst / Data Scientist** with experience turning complex datasets into **clear insights and practical recommendations**.
This project demonstrates my ability to:

* Perform structured EDA
* Build interpretable ML models
* Communicate results in business and engineering terms

📫 **Contact:**

* LinkedIn: *[Your LinkedIn]*
* Email: *[gogoharrison66@gmail.com]*

---
