markdown
# 🌍 Explainable AI for Malaria Outbreak Prediction in Central Africa

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.123456789.svg)](https://doi.org/10.5281/zenodo.123456789)

> **ICICT 2026 Conference Submission**: "Explainable AI for Malaria Outbreak Prediction in Central African Healthcare Systems: A SHAP-based Interpretable Machine Learning Approach"

## 📖 Overview

This repository contains the complete implementation for our research on **Explainable Artificial Intelligence (XAI)** for malaria outbreak prediction in Central Africa. The project develops an interpretable machine learning framework to predict estimated malaria cases using demographic, climatic, and socio-economic indicators across four Central African countries.

## 🎯 Key Features

- **Temporal Validation**: Robust train-test split (2010-2020 training, 2021-2023 testing) simulating real-world deployment
- **Explainable AI**: Comprehensive SHAP analysis for model interpretability and actionable insights
- **Multi-Country Analysis**: Coverage of DRC, Congo, CAR, and Cameroon over 14 years (2010-2023)
- **Clinical Relevance**: Feature importance analysis tailored for healthcare decision-makers

## 🏆 Model Performance

| Metric | Score | Description |
|--------|-------|-------------|
| **Test R²** | 0.9989 | 99.89% variance explained |
| **Test RMSE** | 429,589.51 cases | Root Mean Squared Error |
| **Best Model** | Linear Regression | Selected for performance + interpretability |

## 🔍 SHAP Analysis Results

### Top 5 Feature Contributions
| Rank | Feature | Contribution | Category |
|------|---------|--------------|----------|
| 1 | **Total_Population** | **32.52%** | Demographic |
| 2 | **Estimated_Malaria_Deaths** | **24.26%** | Health Outcome |
| 3 | **Confirmed_Malaria_Cases** | **12.24%** | Health Outcome |
| 4 | Urban_Population_Percent_YoY_Change | 8.07% | Demographic Trend |
| 5 | Total_Population_YoY_Diff | 6.43% | Demographic Trend |

### Country-Specific Insights
| Country | Primary Driver | Secondary Driver | Tertiary Driver |
|---------|----------------|------------------|-----------------|
| **DRC** | Total_Population | Estimated_Malaria_Deaths | Confirmed_Malaria_Cases |
| **Cameroon** | Estimated_Malaria_Deaths | Basic_Water_Access_Percent | Rural_Population_Percent_YoY_Diff |
| **CAR** | Total_Population | Estimated_Malaria_Deaths | Urban_Population_Percent_YoY_Change |
| **Congo** | Total_Population | Estimated_Malaria_Deaths | Urban_Population_Percent_YoY_Change |

## 📁 Repository Structure
├── XAI_Malaria_Central_Africa.ipynb # Main analysis notebook
├── MASTER_Dataset.csv # Primary dataset
├── Visualizations/ # Generated figures
│ ├── SHAP_summary_plot.png
│ ├── country_specific_analysis.png
│ └── model_performance_comparison.png
├── Tables/ # Output tables
│ ├── model_comparison.csv
│ ├── feature_importance.csv
│ └── country_insights.csv
└── requirements.txt # Python dependencies

text

## 🚀 Installation & Usage

### Prerequisites
```bash
# Clone repository
git clone https://github.com/yourusername/malaria-xai-prediction.git
cd malaria-xai-prediction

# Install dependencies
pip install -r requirements.txt
Dependencies
bash
pandas>=1.4.0
numpy>=1.21.0
matplotlib>=3.5.0
seaborn>=0.11.0
scikit-learn>=1.0.0
shap>=0.40.0
jupyter>=1.0.0
Execution
Place MASTER_Dataset.csv in the root directory

Open and run XAI_Malaria_Central_Africa.ipynb sequentially

Generated outputs will be saved in Visualizations/ and Tables/ folders

📊 Methodology
Data Preprocessing: Handling missing values, feature engineering, temporal splitting

Model Selection: Comparison of Linear Regression, Random Forest, and Gradient Boosting

Temporal Validation: Strict time-based split to ensure realistic performance estimation

XAI Implementation: SHAP analysis for global and local interpretability

Country-Level Analysis: Regional insights for targeted interventions

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

👥 Contributors
# Alidor Mbaya


📧 Contact
For questions or collaborations, please open an issue or contact :alidor.mbayandjambe@unikin.ac.cd 
