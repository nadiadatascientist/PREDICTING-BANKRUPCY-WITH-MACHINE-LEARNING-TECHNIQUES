📉 Predicting Bankruptcy with Machine Learning Techniques

This project is part of my master's thesis and applies machine learning techniques to predict corporate bankruptcy. It combines data preprocessing, model development, class imbalance treatment, and model interpretability using real-world financial indicators.



🎯 Objective

- Predict bankruptcy status of companies based on 96 financial indicators
- Evaluate the performance of various machine learning models
- Handle class imbalance using SMOTE
- Enhance interpretability through SHAP analysis



📊 Dataset

- **Source**: Public dataset (Kaggle, GitHub)
- **Companies**: 6,819 Taiwanese companies
- **Features**: 96 financial ratios and macroeconomic indicators
- **Target**: Binary classification — bankrupt (1) vs. non-bankrupt (0)
- **Imbalance**: 3.2% bankrupt / 96.8% non-bankrupt



⚙️ Methodology

 1. Data Cleaning & Preprocessing
- Removal of redundant features
- Median imputation for missing values
- Standardization and outlier analysis
- Multicollinearity reduction (threshold: 0.8)

2. Exploratory Data Analysis (EDA)
- Boxplots, distributions, class imbalance visualization
- Feature-target relationships

3. Class Imbalance Handling
- SMOTE (Synthetic Minority Oversampling Technique) applied on training set



🤖 Modeling Approaches

 ➤ Traditional ML Models
- Logistic Regression  
  - Accuracy: 86.8% | Recall: 76.47% | Precision: 18.84%
- Decision Tree  
  - Accuracy: 90.47% | Recall: 68.63% | Precision: 23.49%
- Random Forest
  - Accuracy: 94.57% | Recall: 54.90% | Precision: 35.44%
- XGBoost 
  - Accuracy: 96.19% | Recall: 52.94% | Precision: 49.09%
- LightGBM
  - Accuracy: 96.85% | Recall: 52.94% | Precision: 58.70%

 ➤ PCA-Based Models
- Lowered recall and precision significantly  
- PCA is not ideal for this dataset

 ➤ Neural Networks
- Accuracy: 89.30%
- Recall: 76.47%
- Precision: 22.54%
- F1 Score: 34.82%


🧠 Model Interpretability with SHAP

- SHAP was used to explain model predictions
- Key bankruptcy risk indicators:
  - High debt ratio
  - Low operating profit margin
  - Equity-to-liabilities structure


 ✅ Key Insights

- Neural networks offered the best balance between precision and recall
- SMOTE helped mitigate class imbalance effectively
- SHAP provided crucial insights for decision-making transparency



 📁 Project Files

- `bankruptcy_prediction.ipynb` — Main notebook
- `bankruptcy_data.csv` — Dataset (sample)
- `README.md` — This documentation file



👩‍💻 Author

**Nadia Anjouar**  
Master's Student in Data Science for Business  
Former Premium Banking Advisor with 17+ years experience  
🔗 [LinkedIn](https://www.linkedin.com/in/nadia-jbilou-1107215a)



📝 License

To be defined. No license applied at this stage.
