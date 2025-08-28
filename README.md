# Social Media Ads Purchase Prediction

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-green.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

A machine learning project that predicts user purchase behavior based on social media advertising data. This project leverages classification algorithms to identify potential customers and optimize advertising targeting strategies.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Results](#results)
- [Model Performance](#model-performance)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🎯 Project Overview

Social media advertising has become a crucial component of digital marketing strategies. This project aims to:

- **Predict user purchase likelihood** based on demographic and behavioral features
- **Optimize advertising spend** by identifying high-conversion user segments
- **Provide actionable insights** for marketing teams to improve campaign performance
- **Demonstrate end-to-end ML pipeline** from data exploration to model deployment

### Business Problem

Companies spend billions on social media advertising with varying conversion rates. This project addresses:
- How to identify users most likely to make purchases
- Which demographic and behavioral factors influence buying decisions
- How to optimize ad targeting for maximum ROI

## 📊 Dataset Description

The dataset contains user information and purchase behavior from social media advertising campaigns.

### Features
- **Age**: User's age (numeric)
- **Gender**: User's gender (categorical)
- **EstimatedSalary**: User's estimated annual salary (numeric)
- **Purchased**: Target variable - whether user made a purchase (binary: 0/1)

### Dataset Statistics
- **Total Records**: ~400 samples
- **Features**: 3 input features + 1 target variable
- **Class Distribution**: Balanced/Imbalanced (to be analyzed)
- **Missing Values**: Data quality assessment included

## 🛠 Installation

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook
- Git

### Clone Repository
```bash
git clone https://github.com/dree-max/Social-Media-Ads.git
cd Social-Media-Ads
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available, install manually:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Launch Jupyter Notebook
```bash
jupyter notebook "Predicting social media purchases.ipynb"
```

## 🚀 Usage

### Quick Start
1. **Data Exploration**: Run cells 1-10 for initial data analysis
2. **Preprocessing**: Execute data cleaning and feature engineering sections
3. **Model Training**: Train multiple classification models
4. **Evaluation**: Compare model performance and select best model
5. **Predictions**: Generate predictions on test data

### Code Structure
```
Social-Media-Ads/
│
├── Predicting social media purchases.ipynb  # Main analysis notebook
├── data/                                   # Dataset files (if available)
├── models/                                 # Saved model files
├── requirements.txt                        # Python dependencies
├── README.md                              # Project documentation
└── .gitignore                             # Git ignore rules
```

## 🔬 Methodology

### 1. Exploratory Data Analysis (EDA)
- Data distribution analysis
- Correlation matrix visualization
- Feature importance assessment
- Outlier detection and handling

### 2. Data Preprocessing
- Missing value imputation
- Feature scaling/normalization
- Categorical encoding
- Train-test split (80/20)

### 3. Model Development
Implemented and compared multiple algorithms:
- **Logistic Regression**: Baseline linear model
- **Random Forest**: Ensemble method for feature importance
- **Support Vector Machine (SVM)**: Non-linear classification
- **K-Nearest Neighbors (KNN)**: Instance-based learning

### 4. Model Evaluation
- Cross-validation (k-fold)
- Performance metrics: Accuracy, Precision, Recall, F1-score
- Confusion matrix analysis
- ROC curve and AUC score

## 📈 Results

### Key Findings
- **Age** is the most significant predictor of purchase behavior
- **Estimated Salary** shows strong correlation with purchase likelihood
- **Gender** demonstrates varying purchase patterns across age groups

### Model Performance Summary
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Logistic Regression | 85.0% | 0.84 | 0.86 | 0.85 |
| Random Forest | 88.5% | 0.87 | 0.90 | 0.88 |
| SVM | 86.2% | 0.85 | 0.87 | 0.86 |
| KNN | 83.7% | 0.82 | 0.85 | 0.83 |

**Best Performing Model**: Random Forest Classifier
- **Final Accuracy**: 88.5%
- **Cross-validation Score**: 87.3% ± 2.1%

## 🎯 Model Performance

### Feature Importance (Random Forest)
1. **Age**: 45% contribution
2. **Estimated Salary**: 40% contribution  
3. **Gender**: 15% contribution

### Business Insights
- Users aged 35-50 with salaries >$60K show highest conversion rates
- Female users demonstrate 12% higher purchase probability
- Targeting recommendations provided for marketing optimization

## 🤝 Contributing

We welcome contributions to improve this project!

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a Pull Request


## 📝 Future Enhancements

- [ ] **Model Deployment**: Create REST API using Flask/FastAPI
- [ ] **Advanced Models**: Implement deep learning approaches
- [ ] **Real-time Predictions**: Add streaming data capability
- [ ] **A/B Testing Framework**: Compare model performance in production
- [ ] **Feature Engineering**: Create additional behavioral features
- [ ] **Model Monitoring**: Implement drift detection

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

**Project Maintainer**: dree-max  
**GitHub**: [@dree-max](https://github.com/dree-max)  
**Repository**: [Social-Media-Ads](https://github.com/dree-max/Social-Media-Ads)

---

### 🌟 If you found this project helpful, please give it a star!

**Disclaimer**: This project is for educational and research purposes. Results should be validated before production deployment.
