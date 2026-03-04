# BME6938 Spring Project 1 - Chronic Kidney Disease Prediction
**Group 7**

## 📋 Project Overview

This project implements machine learning models to predict chronic kidney disease (CKD) progression based on patient metrics. The goal is to develop a reliable predictive model that can assist in early detection and intervention.

### Dataset
- **Source**: [Chronic Kidney Disease Dataset (OpenML #42972)](https://www.openml.org/d/42972)
- **Task**: Binary classification for disease risk prediction
- **Features**: Patient health metrics including laboratory tests and clinical measurements

## 🎯 Objectives

1. Load and explore the CKD dataset
2. Perform comprehensive exploratory data analysis (EDA)
3. Implement robust data preprocessing pipeline
4. Train and evaluate multiple machine learning models
5. Compare model performance using clinical metrics
6. Recommend best model for deployment

## 🤖 Model Implemented

This project implements and evaluates:

**Multi-Layer Perceptron (MLP) Neural Network**
- Two hidden layers (100 and 50 neurons)
- ReLU activation function
- Adam optimizer with adaptive learning rate
- Early stopping to prevent overfitting
- L2 regularization for weight constraints

## 📊 Evaluation Metrics

Each model is evaluated using clinically relevant metrics:

- **Accuracy**: Overall prediction correctness
- **Precision**: Reliability of positive predictions
- **Recall/Sensitivity**: Ability to catch all at-risk patients
- **F1-Score**: Harmonic mean of precision and recall
- **ROC-AUC**: Model's discriminative ability
- **Confusion Matrix**: Breakdown of predictions
- **Cross-Validation**: 5-fold stratified CV for reliability

## 📁 Project Structure

```
BME6938-Spring-Project1-G7/
├── Project1_code.ipynb      # Main Jupyter notebook with complete analysis
├── README.md                 # This file
└── requirements.txt          # Python dependencies (to be created)
```

## 🚀 Getting Started

### Prerequisites

```bash
# Required Python packages
numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost
lightgbm (optional)
scipy
```

### Installation

```bash
# Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn xgboost scipy

# Optional: Install LightGBM
pip install lightgbm
```

### Running the Analysis

1. Open `Project1_code.ipynb` in Jupyter Notebook/Lab or VS Code
2. Run all cells sequentially
3. The notebook will:
   - Load data from OpenML
   - Perform EDA
   - Preprocess data
   - Train all models
   - Generate comprehensive evaluation reports
   - Display comparison visualizations

## 📈 Notebook Structure

The notebook is organized into the following sections:

1. **Setup and Library Imports**
2. **Data Loading and Initial Inspection**
3. **Exploratory Data Analysis (EDA)**
   - Correlation analysis
   - Feature distributions
   - Outlier detection
4. **Data Preprocessing**
   - Missing value imputation
   - Categorical encoding
   - Train-test split
   - Feature scaling
5. **Model Evaluation Framework**
   - Comprehensive evaluation functions with detailed comments
   - Cross-validation utilities with explanations
6. **Model Training and Evaluation**
   - Multi-Layer Perceptron implementation
   - Detailed line-by-line comments explaining each parameter
   - Architecture rationale and clinical considerations
7. **Model Results and Analysis**
   - Performance metrics with clinical interpretation
   - Cross-validation results with stability analysis
   - Visualization of all metrics
   - ROC curve analysis with optimal threshold identification
8. **Conclusions and Clinical Recommendations**
   - Performance summary and interpretation
   - Clinical deployment recommendations
   - Limitations and considerations
   - Future work and enhancements

## 🏥 Clinical Relevance

**Why This Matters:**

Chronic kidney disease affects millions worldwide. Early prediction enables:
- Preventive interventions
- Optimized treatment planning
- Reduced healthcare costs
- Improved patient outcomes

**Model Selection Criteria:**

For CKD prediction, we prioritize:
1. **High Recall**: Catching all at-risk patients is critical
2. **Balanced F1-Score**: Maintaining good overall performance
3. **ROC-AUC**: Strong discriminative ability

## 📝 Key Features

- ✅ Complete end-to-end ML pipeline
- ✅ Comprehensive EDA with visualizations
- ✅ Robust preprocessing with proper train-test split
- ✅ Multi-Layer Perceptron Neural Network implementation
- ✅ **Extensively commented code** - every line/section explained
- ✅ All required evaluation metrics with clinical interpretation
- ✅ Cross-validation for reliability with stability analysis
- ✅ Publication-ready visualizations
- ✅ Detailed clinical interpretation of results
- ✅ Architecture rationale and parameter explanations

## 🔬 Results

Results will be generated when you run the notebook. The notebook includes:
- Detailed performance metrics for MLP Neural Network
- Confusion matrix with detailed breakdown
- ROC curve with optimal threshold identification
- Feature importance analysis
- Cross-validation scores with confidence intervals
- Comprehensive clinical interpretation of all metrics
- Stability analysis across CV folds

## 👥 Team

**Group 7** - BME6938 Spring 2026

## 📚 References

- OpenML Dataset: https://www.openml.org/d/42972
- Scikit-learn Documentation: https://scikit-learn.org/
- XGBoost Documentation: https://xgboost.readthedocs.io/

## 📄 License

This project is for educational purposes as part of BME6938 coursework.

---

**Last Updated**: March 4, 2026
