# SWYNEX Final Data Science Project
## Titanic Survival Prediction

### 1. Project Overview

This project focuses on analyzing the Titanic passenger dataset and using machine learning to predict whether a passenger survived the Titanic disaster.

The project brings together the major stages of a data science workflow, including data preparation, exploratory data analysis (EDA), feature engineering, model training, evaluation, and interpretation of results.

It was completed as part of the Data Science Internship at SWYNEX Technologies.

### 2. Relationship with Previous Internship Tasks

This final project builds upon the work completed in the previous three internship tasks:

- **Task 1 – Data Cleaning:** Detailed data inspection, missing-value treatment, duplicate checking, and data preparation.
- **Task 2 – Exploratory Data Analysis (EDA):** Detailed analysis of survival patterns using statistical summaries, visualizations, and correlation analysis.
- **Task 3 – Modeling and Evaluation:** Logistic Regression model training, evaluation using classification metrics, and confusion matrix analysis.

**Task 4 consolidates these stages** into a unified project, presenting the problem statement, key analytical findings, modeling workflow, evaluation approach, limitations, and conclusions in one documented notebook.

The previous tasks contain the detailed work for their respective stages, while this final project provides an integrated overview of the complete data science workflow.

### 3. Project Objectives

- Understand the Titanic passenger dataset.
- Examine data quality and prepare the dataset for analysis.
- Explore survival patterns across different passenger characteristics.
- Identify relationships between numerical features.
- Prepare relevant features for machine learning.
- Train a Logistic Regression classification model.
- Evaluate model performance using suitable classification metrics.
- Document findings, limitations, and possible improvements.

### 4. Technologies Used

- **Python** – Programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Machine learning and model evaluation
- **Jupyter Notebook** – Interactive development and documentation

### 5. Dataset Description

The project uses the Titanic passenger dataset, which contains information about passengers, including:

- Passenger class (`Pclass`)
- Gender (`Sex`)
- Age (`Age`)
- Number of siblings and spouses aboard (`SibSp`)
- Number of parents and children aboard (`Parch`)
- Ticket fare (`Fare`)
- Port of embarkation (`Embarked`)
- Survival status (`Survived`)

The notebook uses `cleaned_titanic.csv`, prepared during the earlier data-cleaning task.

The target variable is `Survived`, where:
- `0` represents a passenger who did not survive.
- `1` represents a passenger who survived.

### 6. Project Workflow

#### A. Data Inspection and Preparation
- Load the cleaned Titanic dataset.
- Examine dataset dimensions, column names, data types, and missing values.
- Use the prepared dataset from Task 1.

#### B. Exploratory Data Analysis
- Analyze the overall survival distribution.
- Compare survival rates by gender and passenger class.
- Examine age distributions among survivors and non-survivors.
- Investigate survival rates by family size and embarkation port.
- Use a correlation heatmap to examine numerical relationships.

#### C. Feature Engineering and Preparation
- Create a `FamilySize` feature for EDA.
- Select relevant predictors for the model.
- Encode categorical features using one-hot encoding.
- Separate the input features from the target variable.
- Divide the data into training and testing sets using stratified sampling.

#### D. Model Training
- Use Logistic Regression as the baseline classification algorithm.
- Train the model on the training dataset.
- Generate survival predictions for the testing dataset.

#### E. Model Evaluation
Evaluate the model using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

#### F. Findings and Conclusion
- Summarize important survival patterns.
- Interpret the model's evaluation results.
- Discuss the limitations of the analysis.
- Identify possible future improvements.

### 7. Key Findings

The exploratory analysis investigates the following patterns:

- **Gender:** Female passengers had a substantially higher observed survival rate than male passengers.
- **Passenger class:** First-class passengers had a higher observed survival rate than passengers in second and third class.
- **Age:** Comparing age distributions helps identify potential differences between survivors and non-survivors.
- **Family size:** Survival rates varied across different family sizes.
- **Port of embarkation:** Observed survival rates differed across embarkation ports.

These are patterns observed in the dataset and do not establish that any individual characteristic directly caused a passenger to survive.

### 8. Model Evaluation

Logistic Regression was selected as a baseline model for binary classification.

Its performance is evaluated using accuracy, precision, recall, F1-score, and a confusion matrix. Together, these measures help assess overall predictive performance and identify different types of classification errors.

The actual metric values and confusion matrix are available in the output of `final_data_science_project.ipynb`.

### 9. Limitations

- The dataset represents a single historical event.
- Missing values in the original dataset required imputation.
- Logistic Regression may not capture complex relationships between passenger characteristics.
- Only a selected set of passenger features was used for prediction.
- Some family-size groups contain relatively few passengers, which can make their survival rates less reliable.
- The observed relationships are associations and should not be interpreted as proof of causation.
- Model performance on this dataset does not guarantee similar performance on other datasets.

### 10. Future Improvements

- Compare Logistic Regression with Decision Tree and Random Forest models.
- Apply cross-validation and hyperparameter tuning.
- Investigate additional features, including ticket and cabin information.
- Evaluate performance across different passenger groups.
- Explore alternative feature engineering approaches.
- Improve the model through systematic experimentation.

### 11. How to Run the Project

1. Clone or download this repository.
2. Ensure that `cleaned_titanic.csv` and `final_data_science_project.ipynb` are in the same folder.
3. Install the required Python libraries.
4. Open the notebook using Jupyter Notebook or JupyterLab.
5. Run the cells from top to bottom.

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 12. Repository Structure

```text
SWYNEX-Final-Data-Science-Project/
├── cleaned_titanic.csv
├── final_data_science_project.ipynb
└── README.md
```

### 13. Internship Information

**Program:** Data Science Internship  
**Organization:** SWYNEX Technologies  
**Project:** Titanic Survival Prediction – Final Data Science Project  
**Task:** Task 4 – End-to-End Data Science Case Study

This project demonstrates practical experience with data analysis, visualization, feature preparation, baseline machine learning, model evaluation, and technical documentation.