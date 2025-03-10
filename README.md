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
│   │   ├── distribution_country.png
│   │   ├── distribution_gender.png
│   │   ├── distribution_cancer_stage.png
│   │   ├── survival_5_years.png
│   │   ├── treatment_types_cancer_stage.png
│   │   ├── correlation_matrix.png
│   │   ├── roc_curve_comparison.png
│   │   ├── healthcare_costs_treatment.png
│   │   ├── actual_vs_predicted_healthcare.png
│   │   ├── healthcare_costs_vs_survival.png
│   ├── result.txt           # Model performance results
│── src/                     # Scripts for preprocessing, training, evaluation
│   ├── preprocess.py
│   ├── train.py
│   ├── evaluate.py
│── README.md                # Project overview
│── requirements.txt         # Python dependencies
│── .gitignore               # Ignore unnecessary files (dataset, temp files)
```

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your_username/colorectal-cancer-analysis.git
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

## Visualizations
Here are some key visualizations used in the analysis:
- **Country-wise Distribution** (`![1](https://github.com/user-attachments/assets/013db61e-dd90-4fe3-a765-cd08e7dcc94d)
`): Displays the distribution of cases across different countries.
- **Cancer Stage Distribution** (`![5](https://github.com/user-attachments/assets/af878778-b9d0-424d-8c00-88c14839a690)
`): Illustrates the number of patients in different cancer stages (Localized, Regional, Metastatic).
- **5-Year Survival Rate** (`![2](https://github.com/user-attachments/assets/9fed381a-d19c-46b6-b50d-126adaba3b03)
`): Represents the proportion of patients who survived for 5 years versus those who did not.
- **Treatment Types by Cancer Stage** (`![15](https://github.com/user-attachments/assets/563c7b0f-9ef7-46be-8c2b-d0ee6cb7ded1)
`): A stacked bar plot showing the treatment preferences for each cancer stage.
- **Correlation Matrix of Features** (`![14](https://github.com/user-attachments/assets/390d5d0d-e9d8-4ae1-8d72-abdda6b22864)
`): A heatmap depicting the correlation between numerical features in the dataset.
- **ROC Curve Comparison of Models** (`![roc curve comaprison](https://github.com/user-attachments/assets/6d7c295b-cc56-4d80-ab63-fd233f6eee62)
`): A Receiver Operating Characteristic (ROC) curve comparing the performance of Logistic Regression, Random Forest, and XGBoost models.
- **Healthcare Costs by Treatment Type** (`![13](https://github.com/user-attachments/assets/192d0afa-cbf1-4c80-bc0c-e9d5c20fb8da)
)
`): A boxplot showing the distribution of healthcare costs for different treatment types and cancer stages.
- **Actual vs. Predicted Healthcare Costs** (`![16](https://github.com/user-attachments/assets/dc908aa2-b8b9-48b9-b5d5-32eec3870162)
`): A scatter plot visualizing the predicted versus actual healthcare costs.
- **Healthcare Costs vs. Survival Rate by Country** (`![17](https://github.com/user-attachments/assets/a12a172f-d368-442d-bfc6-27b390c95d1e)
`): A bubble chart comparing healthcare costs and survival rates for different countries.

## Notebook Overview
The Jupyter Notebook `comprehensive-colorectal-cancer-dataset-analysis.ipynb` performs the following tasks:
1. **Loads and preprocesses** the colorectal cancer dataset, handling missing values and encoding categorical variables.
2. **Explores the dataset** through summary statistics and visualizations.
3. **Performs feature engineering** to enhance model performance.
4. **Trains multiple machine learning models** (Logistic Regression, Random Forest, and XGBoost) to predict 5-year survival.
5. **Evaluates model performance** using accuracy, precision, recall, F1-score, and ROC AUC.
6. **Analyzes healthcare costs** across treatment types and cancer stages.
7. **Predicts healthcare costs** using regression models and compares the predicted values against actual values.

## Model Performance Summary
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

## Contribution
Feel free to fork the repo and contribute to improving the analysis!

## License
This project is open-source under the MIT License.
