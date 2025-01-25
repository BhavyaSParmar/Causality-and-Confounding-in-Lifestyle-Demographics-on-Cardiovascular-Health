# **Causality and Confounding in Lifestyle and Demographics on Cardiovascular Health**

This repository explores the intricate relationships between clinical, demographic, and lifestyle factors and their influence on cardiovascular health. Using **causal inference techniques** and **machine learning models**, the project aims to derive actionable insights to support precision medicine and public health strategies.

---

## **Project Objectives**
- Identify key determinants of cardiovascular health using **data-driven approaches**.
- Address the effects of confounding variables (e.g., age, gender, chest pain type) to ensure unbiased causal relationships.
- Develop robust machine learning models for predicting cardiovascular outcomes.

---

## **Project Workflow**

### 1. **Data Preprocessing**
- Handled missing data using imputation and normalized numerical variables to ensure uniformity.
- Encoded categorical features (e.g., gender, chest pain type) with techniques like **one-hot encoding**.
- Cleaned and validated datasets to minimize noise and inconsistencies.

### 2. **Exploratory Data Analysis (EDA)**
- Performed **pairwise correlation** and dependency analysis to identify feature relationships.
- Visualized trends and patterns with **heatmaps**, **scatter plots**, and **distribution plots**.
- Conducted hypothesis testing on categorical variables to determine their significance relative to heart disease outcomes.

### 3. **Causal Inference**
- Applied **propensity score matching (PSM)** to control for confounders such as age and chest pain type.
- Used **Nearest Neighbors Matching** to create balanced datasets for robust causal analysis.
- Performed sensitivity analysis to validate the stability of causal inferences under various assumptions.

### 4. **Machine Learning Modeling**
- Built and trained a **Random Forest Classifier** to predict heart disease presence:
  - Achieved **85% accuracy** with the full feature set.
  - Improved to **87% accuracy** using feature-optimized subsets.
- Extracted feature importance metrics, identifying:
  - **Number of major vessels (ca)** as the most significant predictor.
  - Other key predictors: **maximum heart rate (thalach)** and **ST depression (oldpeak)**.

### 5. **Feature Selection**
- Streamlined the model by focusing on clinically relevant features to improve interpretability.
- Applied **Recursive Feature Elimination (RFE)** to reduce dimensionality and enhance model performance.

---

## **Key Insights**
### **1. Lifestyle and Clinical Predictors**
- Strong associations were found between **maximum heart rate**, **chest pain type**, and **ST depression** with cardiovascular health.

### **2. Demographic Confounders**
- Variables such as **age** and **gender** significantly influenced outcomes and were controlled using causal inference techniques.

### **3. Model Performance**
- The **Random Forest Classifier** demonstrated high precision, recall, and overall robustness, making it an effective tool for cardiovascular risk prediction.

---

## **Technologies and Tools**
- **Programming Language:** Python
- **Libraries:**
  - **Data Processing:** Pandas, NumPy
  - **Visualization:** Matplotlib, Seaborn
  - **Machine Learning:** Scikit-learn
- **Techniques:**
  - **Machine Learning:** Random Forest Classifier
  - **Causal Inference:** Propensity Score Matching, Nearest Neighbors Matching
  - **Feature Engineering:** Recursive Feature Elimination (RFE)
- **Visualizations:** Heatmaps, Pairwise Plots, Feature Importance Graphs

---

## **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/causality-cardiovascular-health.git
## **Install required libraries**
2.pip install -r requirements.txt
## **Run the preprocessing and analysis scripts**
3.python preprocess_data.py
python analyze_data.py
python train_model.py

---

## *Directory Structure**
├── data
│   ├── raw_data.csv            # Raw dataset
│   ├── cleaned_data.csv        # Preprocessed dataset
├── notebooks
│   ├── EDA.ipynb               # Exploratory Data Analysis
│   ├── causal_analysis.ipynb   # Causal Inference Workflow
│   ├── modeling.ipynb          # Model Training and Evaluation
├── src
│   ├── preprocess_data.py      # Data cleaning and preprocessing
│   ├── analyze_data.py         # EDA and visualization
│   ├── train_model.py          # Model training and evaluation
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation

## **Results**
- The model achieved **87% accuracy** after feature selection, highlighting significant predictors such as:
  - **Number of major vessels (ca)**
  - **Maximum heart rate (thalach)**
  - **ST depression (oldpeak)**
- Addressing confounders like **age** and **gender** significantly enhanced the robustness of causal insights and minimized biases.

---

## **Contributing**
Contributions are welcome! If you would like to improve the project or add new features, please:
1. Fork the repository.
2. Create a new branch for your feature or improvement.
3. Submit a pull request, providing a clear description of your changes.

---

## **License**
This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

---

## **Acknowledgments**
- Special thanks to the creators of the datasets used in this analysis.
- Gratitude to the open-source community for developing the libraries and tools that made this project possible.
