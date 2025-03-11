# Colorectal Cancer Dataset Analysis

## Repository Name
`colorectal-cancer-analysis`

## What is this Repository Doing?
This repository is focused on analyzing the **Colorectal Cancer Dataset** using **Machine Learning** models. The project explores various risk factors, survival rates, and patient characteristics through **data visualization, statistical analysis, and predictive modeling**. It evaluates different models like **Logistic Regression, Random Forest, and XGBoost** for survival prediction based on clinical and demographic features.

## Task Overview
The goal of this project is to:
1. **Preprocess** the colorectal cancer dataset from Kaggle.
2. **Explore and visualize** patient demographics, risk factors, and survival rates.
3. **Train Machine Learning models** to predict **5-year survival rates**.
4. **Evaluate models** based on accuracy, precision, recall, F1-score, and ROC AUC.
5. **Compare results** to determine the best-performing model for predicting survival outcomes.

## Repository Structure
```
colorectal-cancer-analysis/
│── data/                    # Dataset (not included in GitHub, Kaggle link reference)
│── notebooks/               # Jupyter notebooks
│   ├── comprehensive-colorectal-cancer-dataset-analysis.ipynb
│── results/                 # Results & images
│   ├── images/              # Visualizations
│   ├── result.txt           # Model performance results
│── src/                     # Scripts for preprocessing, training, evaluation
│   ├── preprocess.py
│   ├── train.py
│   ├── evaluate.py
│── images/                  # Folder containing uploaded images
│── README.md                # Project overview
│── requirements.txt         # Python dependencies
│── .gitignore               # Ignore unnecessary files (dataset, temp files)
```

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Codennmu/colorectal-cancer-analysis.git
   cd colorectal-cancer-analysis
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the Dataset**
   - The dataset is available on Kaggle: [Colorectal Cancer Dataset](https://www.kaggle.com/)
   - Place the dataset inside the `data/` directory.

4. **Run the Jupyter Notebook**
   ```bash
   jupyter notebook notebooks/comprehensive-colorectal-cancer-dataset-analysis.ipynb
   ```

---

## **Visualizations**
Here are some key visualizations used in the analysis:

- **Country-wise Distribution**  
  ![Country-wise Distribution](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/countrywise.png)

- **Cancer Stage Distribution**  
  ![Cancer Stage Distribution](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/cancerstage.png)

- **Correlation Matrix of Features**  
  ![Correlation Matrix](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/correlation.png)

- **5-Year Survival Rate**  
  ![5-Year Survival Rate](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/5_years.png)

- **Treatment Types by Cancer Stage**  
  ![Treatment Types by Cancer Stage](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/treatment_types_by_cancer_stage.png)

- **ROC Curve Comparison of Models**  
  ![ROC Curve Comparison](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/roc_curve_comparison.png)

- **Healthcare Costs by Treatment Type**  
  ![Healthcare Costs by Treatment Type](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/healthcare_costs_by_treatment_type.png)

- **Healthcare Costs vs. Survival Rate by Country**  
  ![Healthcare Costs vs. Survival Rate](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/healthcare_costs_vs_survival_by_country.png)

- **Actual vs. Predicted Healthcare Costs**  
  ![Actual vs. Predicted Healthcare Costs](https://raw.githubusercontent.com/Codennmu/colorectal-cancer-analysis/main/Images/actual_vs_predicted_healthcare_costs.png)

---

## **Notebook Overview**
The Jupyter Notebook `comprehensive-colorectal-cancer-dataset-analysis.ipynb` performs the following tasks:
1. **Loads and preprocesses** the colorectal cancer dataset, handling missing values and encoding categorical variables.
2. **Explores the dataset** through summary statistics and visualizations.
3. **Performs feature engineering** to enhance model performance.
4. **Trains multiple machine learning models** (Logistic Regression, Random Forest, and XGBoost) to predict 5-year survival.
5. **Evaluates model performance** using accuracy, precision, recall, F1-score, and ROC AUC.
6. **Analyzes healthcare costs** across treatment types and cancer stages.
7. **Predicts healthcare costs** using regression models and compares the predicted values against actual values.

---

## **Model Performance Summary**
```
                     accuracy  precision    recall  f1_score   roc_auc  
XGBoost              0.589672   0.603478  0.929014  0.731670  0.509297   
Logistic Regression  0.602179   0.602179  1.000000  0.751700  0.498788   
Random Forest        0.588090   0.602272  0.930352  0.731197  0.498167   

                     training_time  
XGBoost                   3.684197  
Logistic Regression       1.833410  
Random Forest            49.542443  
```

---

## **Contribution**
Feel free to fork the repo and contribute to improving the analysis!

## **License**
This project is open-source under the MIT License.
