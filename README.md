# 📊 ERP Implementation Duration Prediction

## 🎯 Objective  
Develop a neural network-based regression model to predict the duration (in days) of ERP implementation projects based on various input features. The goal is to improve prediction accuracy by applying feature engineering techniques and optimizing model architecture.

## 🛠️ Tools & Technologies  
- Python 3.x  
- TensorFlow / Keras (Deep Learning)  
- scikit-learn (Feature Engineering & Dimensionality Reduction)  
- NumPy & pandas (Data Manipulation)  
- Jupyter Notebook / Google Colab (Development Environment)  

## 📂 Dataset Overview  
- **Samples:** 800 project instances  
- **Features:** 171 initial variables describing project characteristics and parameters  
- **Target:** Duration of ERP implementation (continuous variable in days)  

## 🔍 Data Preprocessing & Feature Engineering  
- Original dataset normalized and cleaned for model input  
- Polynomial feature expansion increased feature count drastically (171 → 14,877)  
- Principal Component Analysis (PCA) applied to reduce dimensions to 100 components, retaining key variance  
- These steps aimed to capture nonlinear relations and reduce noise  

## 🧠 Model Development & Evaluation  
- Baseline neural network model with moderate layers achieved a test Mean Absolute Error (MAE) of ~4.31 days  
- Enhanced model incorporating PCA and increased neurons resulted in higher MAE (~16.5 days), indicating potential overfitting or information loss  
- Early stopping callback was used to mitigate overfitting during training  
- Model predictions compared against true project durations showed varying levels of accuracy  

## 📈 Insights & Interpretation  
- Baseline architecture demonstrated strong predictive capabilities on the original feature set  
- Aggressive feature expansion and PCA dimensionality reduction did not improve outcomes, highlighting the balance required between model complexity and generalization  
- Regularization and further hyperparameter tuning are necessary to enhance robustness  
- Future work may include feature importance analysis and domain-specific feature engineering  

## 📝 Summary  
This project presents a systematic approach to predicting ERP implementation durations using neural networks. While initial models performed well, more complex feature transformations did not translate into better accuracy, underscoring challenges in model tuning and data representation. The baseline model serves as a solid foundation for future experimentation and improvements.

---
