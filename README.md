# Video Game Sales Prediction

> A comprehensive machine learning solution for predicting global video game sales using regression models and data analytics.

## Overview

This project presents a complete machine learning model for predicting global video game sales. It analyzes 16,599 historical video game records and leverages platform, genre, publisher, and regional sales data to build highly accurate predictive models.

**🏆 Best Model:** Decision Tree Regressor — **99.45% Accuracy**

## Dataset

The dataset comprises 16,599 video game records with the following attributes:

| Feature | Description |
|---------|-------------|
| Platform | Gaming platform (Wii, NES, DS, PS2, etc.) |
| Genre | Game category (Action, Sports, RPG, etc.) |
| Publisher | Game publisher |
| Year | Release year |
| Regional Sales | NA_Sales, EU_Sales, JP_Sales, Other_Sales (in millions) |
| **Global_Sales** | Total worldwide sales (target variable) |

## Methodology

The project follows a structured machine learning pipeline:

1. **Data Loading & Exploration** — Load and analyze dataset characteristics
2. **Data Preprocessing** — Handle missing values and analyze distributions
3. **Exploratory Data Analysis** — Visualize patterns across genres and platforms
4. **Outlier Treatment** — Apply IQR detection and Winsorization techniques
5. **Feature Engineering** — One-hot encode categorical features, normalize data
6. **Model Development** — Train multiple regression algorithms
7. **Model Evaluation** — Compare performance using cross-validation

## Model Performance Results

| Model | Best Score | Best Parameters |
|-------|-----------|-----------------|
| Decision Tree Regressor | ⭐ **99.45%** | criterion: friedman_mse, splitter: best |
| Linear Regression | 98.62% | fit_intercept: True |
| Lasso Regression | -13.32% | alpha: 1, selection: random |

**Key Finding:** Decision Tree Regressor achieved the highest accuracy at 99.45%, significantly outperforming all other models.

## Technology Stack

- **Language:** Python 3
- **Data Processing:** pandas, numpy
- **Visualization:** matplotlib, seaborn
- **Machine Learning:** scikit-learn

## Getting Started

### Installation

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Execution

```bash
jupyter notebook "vgsales prediction.ipynb"
```

## Project Structure

```
vedio-games-sales-prediction/
├── vgsales prediction.ipynb    # Complete analysis and modeling notebook
├── vgsales.csv                 # Dataset (16,599 video game records)
└── README.md                   # Documentation
```

---

*Last Updated: January 2026*
