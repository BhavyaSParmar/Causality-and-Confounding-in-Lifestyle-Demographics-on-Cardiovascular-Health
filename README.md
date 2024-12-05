# Causality-and-Confounding-in-Lifestyle-Demographics-on-Cardiovascular-Health
###
This project is a comprehensive exploration of cardiovascular health, leveraging causal inference techniques and machine learning models to understand the intricate relationships between clinical, demographic, and lifestyle factors and their impacts on heart disease outcomes.
###
Project Overview
The aim of the study is to:

Identify key predictors of heart disease using data-driven approaches.
Understand the role of confounding variables such as age, gender, and chest pain type that may distort causal relationships.
Develop robust predictive models to support precision medicine and public health strategies.
Key Highlights
1. Data Preprocessing
Handled missing data by normalizing and standardizing numerical variables.
Categorical variables, such as gender and chest pain type, were encoded to make them suitable for analysis.
Conducted a thorough cleaning process to ensure high-quality data for modeling.
2. Exploratory Data Analysis (EDA)
Conducted correlation and pairwise analyses to understand the relationships between features.
Used visualizations like heatmaps and scatter plots to identify trends and patterns in the data.
Analyzed categorical variables against the target (presence or absence of heart disease) to highlight significant associations.
3. Causal Inference
Applied propensity score matching to control for confounding variables like age and chest pain type. This technique ensured that comparisons between groups (with and without heart disease) were fair and unbiased.
Created matched datasets using Nearest Neighbors, allowing for clearer causal insights.
Conducted sensitivity analysis to confirm the robustness of the findings.
4. Machine Learning Modeling
Trained a Random Forest Classifier to predict the presence of heart disease, achieving:
85% accuracy with the full feature set.
Improved 87% accuracy using a refined subset of features.
Extracted feature importance scores, identifying:
Number of major vessels (ca) as the most significant predictor.
Other important predictors like maximum heart rate (thalach) and ST depression (oldpeak).
5. Feature Selection
Simplified the model by focusing on clinically relevant features, improving its performance and interpretability.
Demonstrated how reducing noise in the data can enhance predictive power and generalization.
6. Key Insights
Lifestyle and Clinical Predictors: Maximum heart rate, chest pain type, and ST depression were strongly associated with heart disease risk.
Demographic Confounders: Age and gender showed a strong influence on outcomes and were controlled using causal inference techniques.
Model Performance: The Random Forest model demonstrated high precision and recall for both classes, making it a robust tool for cardiovascular risk prediction.
Technologies and Tools
Programming Language: Python
Libraries Used: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
Machine Learning Models: Random Forest Classifier
Causal Inference Methods: Propensity Score Matching, Nearest Neighbors Matching
Visualization: Heatmaps, Pairwise Plots, Feature Importance Graphs
Conclusion
This project highlights the critical role of data-driven methodologies in understanding cardiovascular health. By combining causal inference and machine learning, it provides actionable insights into the factors influencing heart disease and demonstrates how addressing confounders can improve predictive accuracy. The findings underscore the importance of precision in data analysis for developing effective interventions and public health policies.
