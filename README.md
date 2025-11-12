💉 Vaccine Adverse Event Reporting System (VAERS) – Capstone Project

🧩 Problem Statement

Domain: Healthcare
Focus: Vaccine Adverse Event Reporting System (VAERS)

The project aims to identify potential adverse effects post-vaccination using real-world VAERS data. The task involves comprehensive data cleaning, transformation, and predictive modeling to classify and analyze the nature of adverse events.

🗂️ Data Preprocessing and Cleaning
 Data Merging & Deduplication

Merged multiple VAERS datasets.

Removed duplicate and redundant features.

 Missing Value Treatment

Imputed missing values in AGE_YRS using CAGE_YR.

Replaced invalid ONSET_DATE values (earlier than VAX_DATE) with corresponding VAX_DATE.

Estimated missing NUMDAYS values using VAX_DATE and ONSET_DATE.

Created new feature AGE_GROUP by bucketing AGE_YRS.

Feature Engineering

Generated meaningful derived variables to improve model performance.

📊 Exploratory Data Analysis
Univariate Analysis

Distribution analysis for key features such as age, vaccine type, and gender.

Bivariate Analysis

Correlation between target and predictor variables.

Identified relationships and trends influencing adverse events.

🧠 Natural Language Processing (NLP)

The ‘SYMPTOMS POST VACCINATION’ feature contained unstructured text data, which was processed for model compatibility.

Steps:

Text Cleaning: Removed punctuation, stop words, and converted to lowercase.

Lemmatization: Standardized words to their root forms.

Text Vectorization:

Implemented Bag of Words (BoW) model.

Built a Document-Term Matrix (DTM) for representation.

📈 Statistical Analysis

Performed statistical significance tests to identify relationships between independent and dependent variables:

Chi-Square Test of Independence

One-Way ANOVA

✅ All independent variables showed statistical significance with the target variable.

⚖️ Class Imbalance Treatment

Used resampling techniques to address imbalance in the dataset.

Compared model performance before and after sampling.

🔡 Encoding Techniques

Target Encoding for independent variables.

Ordinal Encoding for target variable.

🚫 Outlier Detection & Treatment

Identified and mitigated the impact of extreme data points to enhance model robustness.

🤖 Model Development & Evaluation
Base Models

Trained and compared multiple machine learning algorithms:

Model	ROC_AUC Score	Accuracy
Logistic Regression	Base reference	–
Random Forest Classifier	Highest	Best performance
AdaBoost Classifier	Moderate	–
Gradient Boost Classifier	Moderate	–
XGBoost Classifier	Moderate	–
🧩 Final Model Selection

Based on comparative analysis, Random Forest Classifier (default hyperparameters) demonstrated the best performance across both Accuracy and ROC_AUC metrics.

✅ Chosen as the Final Model

🚀 Deployment

The final model was deployed as a web application using:

Flask (Backend)

HTML (Frontend UI)

This deployment allows users to input vaccine-related data and predict potential adverse effects post-vaccination.

🛠️ Tech Stack

Languages: Python

Libraries: pandas, NumPy, scikit-learn, NLTK, Flask

Visualization: Matplotlib, Seaborn

Statistical Tests: SciPy

Deployment: Flask, HTML/CSS
