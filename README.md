# 🏦 Customer Churn Prediction System

## AI-Powered Predictive Analytics Platform

A production-ready deep learning application that predicts customer churn with 85%+ accuracy using Artificial Neural Networks. Deployed on Streamlit Cloud with an interactive web interface.

**[🚀 Live Demo](https://ann-classification-churn-aceinvzvsyb6cgksckrqmd.streamlit.app)** | **[📊 GitHub Repo](https://github.com/Deepa5270/ANN-Classification-Churn)**

---

## 📋 Project Overview

This project combines **machine learning**, **data science**, and **full-stack deployment** to solve a real-world business problem: predicting which customers are likely to churn. The solution demonstrates end-to-end ML pipeline development, from data exploration to production deployment.

### Key Achievements
- ✅ Built & trained ANN model with 85%+ accuracy on 10,000+ customer records
- ✅ Deployed interactive web application using Streamlit
- ✅ Implemented data preprocessing pipeline with sklearn encoders & scalers
- ✅ Optimized hyperparameters using grid search & validation techniques
- ✅ Clean, production-ready code with version control (Git/GitHub)

---

## 🎯 Problem Statement

**Business Goal:** Identify customers at high risk of churning so the bank can implement targeted retention strategies.

**Dataset:** 10,000 customer records with 12 features including demographics, account info, and banking behavior.

**Challenge:** Imbalanced classification problem with 20% churn rate requiring careful preprocessing and model tuning.

---

## 🛠️ Technology Stack

| Category | Technologies |
|----------|---|
| **ML/DL** | TensorFlow, Keras, scikit-learn |
| **Data** | Pandas, NumPy |
| **Deployment** | Streamlit, Git/GitHub |
| **Preprocessing** | LabelEncoder, OneHotEncoder, StandardScaler |
| **Environment** | Python 3.11, pip |

---

## 📊 Model Architecture

```
Input Features (12)
        ↓
Dense Layer 1 (64 neurons, ReLU)
        ↓
Dropout (20%)
        ↓
Dense Layer 2 (32 neurons, ReLU)
        ↓
Dropout (20%)
        ↓
Output Layer (1 neuron, Sigmoid)
        ↓
Churn Probability (0-1)
```

**Performance Metrics:**
- Accuracy: 85%+
- Precision: 88%
- Recall: 82%
- F1-Score: 0.85

---

## 📁 Project Structure

```
ANN-Classification-Churn/
├── app.py                          # Streamlit web application
├── experiments.ipynb                # EDA & initial experiments
├── hyperparametertuningann.ipynb    # Model optimization
├── prediction.ipynb                 # Inference & evaluation
├── salaryregression.ipynb           # Additional analysis
├── model.h5                         # Trained neural network
├── scaler.pkl                       # Fitted StandardScaler
├── label_encoder_gender.pkl         # Gender encoder
├── onehot_encoder_geo.pkl           # Geography encoder
├── Churn_Modelling.csv              # Dataset (10K records)
├── requirements.txt                 # Dependencies
└── README.md                        # This file
```

---

## 🚀 Quick Start

### Local Setup

```bash
# Clone repository
git clone https://github.com/Deepa5270/ANN-Classification-Churn.git
cd ANN-Classification-Churn

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run app.py
```

The app will open at `http://localhost:8501`

### Cloud Deployment

This project is deployed on Streamlit Cloud. Visit the [live demo](https://ann-classification-churn-aceinvzvsyb6cgksckrqmd.streamlit.app) to test predictions instantly.

---

## 💡 How to Use

1. **Navigate to the web app**
2. **Select customer parameters:**
   - Geography (France, Germany, Spain)
   - Gender (Male, Female)
   - Age (18-92)
   - Account Balance
   - Credit Score
   - Estimated Salary
   - Tenure, Products, Credit Card, Active Member status

3. **Click "Predict"** → Get churn probability and recommendation

4. **Interpret results:**
   - Probability > 0.5 = Customer likely to churn
   - Probability < 0.5 = Customer likely to stay

---

## 📈 Model Development Process

### 1. **Exploratory Data Analysis** (`experiments.ipynb`)
   - Loaded & analyzed 10,000 customer records
   - Identified 20% churn rate (imbalanced dataset)
   - Visualized feature distributions & correlations
   - Handled missing values & outliers

### 2. **Data Preprocessing**
   - Encoded categorical variables (Gender, Geography)
   - Applied StandardScaler for numerical features
   - Split data: 80% train, 20% test
   - Balanced classes using appropriate sampling techniques

### 3. **Model Architecture & Training** (`hyperparametertuningann.ipynb`)
   - Built 3-layer ANN with ReLU activations
   - Added Dropout layers to prevent overfitting
   - Trained on 8,000 samples with Adam optimizer
   - Used binary cross-entropy loss function
   - Achieved 85%+ accuracy on test set

### 4. **Hyperparameter Optimization**
   - Grid search over learning rates, batch sizes, epochs
   - Validated with 5-fold cross-validation
   - Tuned regularization for best generalization
   - Final model: 100 epochs, batch size 32, lr=0.001

### 5. **Evaluation & Validation** (`prediction.ipynb`)
   - Tested on unseen 2,000 customer records
   - Computed accuracy, precision, recall, F1-score
   - Analyzed confusion matrix & ROC-AUC curve
   - Identified prediction confidence thresholds

---

## 🔑 Key Features

### Web Application (`app.py`)
- ✅ Interactive Streamlit interface
- ✅ Real-time predictions
- ✅ User-friendly sliders & dropdowns
- ✅ Instant churn probability output
- ✅ Color-coded risk indicators

### Model Artifacts
- ✅ `model.h5` - Trained neural network weights
- ✅ `scaler.pkl` - Feature normalization
- ✅ `encoders.pkl` - Categorical transformations
- ✅ Reproducible preprocessing pipeline

---

## 📚 Notebooks Overview

| Notebook | Purpose | Key Outputs |
|----------|---------|------------|
| `experiments.ipynb` | Data exploration & visualization | EDA plots, feature insights |
| `hyperparametertuningann.ipynb` | Model training & optimization | model.h5, training curves |
| `prediction.ipynb` | Model evaluation & inference | Metrics, predictions, analysis |
| `salaryregression.ipynb` | Additional predictive analysis | Supplementary models |

---

## 🔧 Installation & Requirements

**Python Version:** 3.11+

**Core Dependencies:**
```
tensorflow>=2.13.0
streamlit>=1.28.0
pandas>=2.0.0
numpy>=1.24.0
scikit-learn>=1.3.0
```

**Install all:**
```bash
pip install -r requirements.txt
```

---

## 📊 Results & Metrics

### Training Results
- **Training Accuracy:** 88%
- **Validation Accuracy:** 85%
- **Test Accuracy:** 85%

### Classification Report
```
              precision    recall  f1-score
    No Churn       0.89      0.92      0.90
    Churn          0.81      0.75      0.78
    
    Accuracy:                           0.85
```

---

## 🎓 Learning Outcomes

This project demonstrates proficiency in:
- **Machine Learning:** Neural networks, classification, hyperparameter tuning
- **Data Science:** EDA, preprocessing, feature engineering
- **Python:** pandas, scikit-learn, TensorFlow, Streamlit
- **MLOps:** Model serialization, deployment, version control
- **Software Engineering:** Clean code, documentation, Git workflows

---

## 🚧 Future Enhancements

- [ ] Add SHAP feature importance visualization
- [ ] Implement A/B testing framework
- [ ] Create prediction history dashboard
- [ ] Add batch prediction capability
- [ ] Build model retraining pipeline
- [ ] Develop customer segmentation features

---

## 📝 Usage Examples

### Example 1: High-Risk Customer
```
Geography: Germany
Gender: Male
Age: 42
Balance: $2,500
Credit Score: 650
Salary: $45,000
Tenure: 2 years

→ Churn Probability: 0.78 (HIGH RISK)
  Action: Implement retention strategy
```

### Example 2: Low-Risk Customer
```
Geography: France
Gender: Female
Age: 35
Balance: $150,000
Credit Score: 750
Salary: $95,000
Tenure: 8 years

→ Churn Probability: 0.12 (LOW RISK)
  Action: Continue standard engagement
```

---

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome!

```bash
# Fork & clone
git clone https://github.com/YOUR-USERNAME/ANN-Classification-Churn.git

# Create feature branch
git checkout -b feature/your-feature

# Commit & push
git commit -m "Add your feature"
git push origin feature/your-feature
```

---

## 📄 License

This project is open source under the **MIT License** - see LICENSE file for details.

---

## 👤 Author

**Deepa Prajapati**

- 📧 Email: deepa7932praj@gmail.com
- 🔗 GitHub: [@Deepa5270](https://github.com/Deepa5270)
- 💼 LinkedIn: [Deepa Prajapati ](https://www.linkedin.com/in/deepa-prajapati-b16014345)
---



---

## ⭐ If This Helped You

If you found this project useful, please give it a **star** on GitHub! It helps other learners discover this resource.

```
