# PG227_AIML_Project

Overview of the project


Problem Domain

• Domain: Healthcare / Preventive Diagnostics
• Real-world Context:
Cardiovascular diseases (CVD) are the leading cause of death globally, accounting
for 17.9 million deaths each year (WHO, 2023).
Early detection of high-risk individuals allows doctors to intervene earlier, reducing
mortality and healthcare costs.


Project Goal

• To clean, preprocess, and analyze patient health data.
• To build a processed dataset ready for machine learning models that can predict
cardiovascular disease risk.
• To identify key risk factors (age, BMI, blood pressure, cholesterol, etc.) through
EDA.


Preprocessing Techniques Applied

Each group member handled one preprocessing step:
Missing Values & Data Quality Check → Verified dataset completeness and
cleaned anomalies.
Outlier Detection & Removal → Removed unrealistic height, weight, and blood
pressure values.
Encoding Categorical Variables → Converted gender, cholesterol, and glucose into
meaningful numeric/encoded values.
Normalization / Scaling → Standardized numerical features for consistency.
Class Imbalance Handling → Used SMOTE to balance disease vs no-disease
samples.
Feature Engineering → Created new features (BMI, age in years) and selected
important predictors.


Exploratory Data Analysis (EDA)

• Correlation Heatmap: Showed relationships between numerical features.
• Histogram (Age): Most patients were aged 40–60.
• Boxplot (BMI vs Cardio): Patients with cardiovascular disease had higher BMI.


Expected Impact

• Helps prioritize high-risk patients for advanced screening.
• Supports resource allocation in hospitals.
• Provides insights into preventive healthcare measures.


Dataset Details

• Source: Cardiovascular Disease dataset (cardio_train.csv)
• Link-https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset
• Size: ~70,000 patient records
• Features: Includes demographic (age, gender, height, weight), lifestyle indicators
(smoking, alcohol, activity), and medical attributes (blood pressure, cholesterol,
glucose).
• Target Variable: cardio → (0 = No cardiovascular disease, 1 = Cardiovascular
disease)


Group member roles

IT24103251 - Sandeepani K.A.D.A – Handling missing values
IT24103325 - Weerasekara S.W.P .N – Outlier detection & removal
IT24103379- Bulugahapitiya M.U.S.S –Encoding categorical variable
IT24103238 - Sedara Ransiluni G.K – Scaling numeric features
IT24103185- Hewavasan P .H.C – Class imbalance checking
IT24103222 - Thishanujan K – Feature Engineering


How to run code?


To run the code for this project, we ensured that Python 3.x is
installed along with the required libraries such as pandas, numpy,
matplotlib, seaborn, scikit-learn, and imbalanced-learn. The dataset
file, named cardio_train.csv, should be placed inside
the data/raw/ folder, as this is the path specified in the code. The
dataset can be read into the program using the pandas library with the
command pd.read_csv("data/raw/cardio_train.csv",
sep=";"), where the separator is explicitly defined because the
dataset uses a semicolon delimiter. Each group member has
developed their own preprocessing notebook located in
the notebooks/ directory, and these can be opened and executed
step by step using Jupyter Notebook. After running the individual
notebooks, the integrated pipeline notebook
named PG227_pipeline.ipynb should be executed to combine
all preprocessing techniques, generate the exploratory data analysis
visualizations, and produce the final cleaned dataset. The processed
dataset will then be automatically saved in
the results/outputs/ folder as processed_cardio_dataset.csv,
which can be used for further model training or analysis.
