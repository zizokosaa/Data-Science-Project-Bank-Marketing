# Data-Science-Project-Bank-Marketing

## Dataset Information:

**Title:** Bank Marketing

**Sources:** Created by Paulo Cortez (Univ. Minho) and Sérgio Moro (ISCTE-IUL) @ 2012,
            https://archive.ics.uci.edu/dataset/222/bank+marketing

**Past Usage:** The full dataset was described and analyzed in:

S. Moro, R. Laureano and P. Cortez. Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology. In P. Novais et al. (Eds.), Proceedings of the European Simulation and Modelling Conference - ESM'2011, pp. 117-121, Guimarães, Portugal, October, 2011. EUROSIS.

**Relevant Information:**

The data is related to direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact with the same client was required to determine if the product (bank term deposit) would be subscribed or not.

There are two datasets:
1. `bank-full.csv` with all examples, ordered by date (from May 2008 to November 2010).
2. `bank.csv` with 10% of the examples (4521), randomly selected from `bank-full.csv`. The smaller dataset is provided to test more computationally demanding machine learning algorithms (e.g., SVM).

The classification goal is to predict if the client will subscribe to a term deposit (variable y).

**Number of Instances:** 45211 for `bank-full.csv` (4521 for `bank.csv`)

**Number of Attributes:** 16 + output attribute

**Attribute Information:**

For more information, read [Moro et al., 2011].

Input variables:
1. age (numeric)
2. job: type of job (categorical)
3. marital: marital status (categorical)
4. education: education level (categorical)
5. default: has credit in default? (binary)
6. balance: average yearly balance, in euros (numeric)
7. housing: has housing loan? (binary)
8. loan: has personal loan? (binary)
9. contact: contact communication type (categorical)
10. day: last contact day of the month (numeric)
11. month: last contact month of the year (categorical)
12. duration: last contact duration, in seconds (numeric)
13. campaign: number of contacts performed during this campaign and for this client (numeric)
14. pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric)
15. previous: number of contacts performed before this campaign and for this client (numeric)
16. poutcome: outcome of the previous marketing campaign (categorical)


Output variable (desired target):

17. y: has the client subscribed to a term deposit? (binary)

**Missing Attribute Values:** None


Certainly! Here's how you can structure your workflow for a GitHub README:

---

## Workflow

1. **EDA (Exploratory Data Analysis)**
   - Conducted exploratory data analysis to understand the dataset and its characteristics.

2. **Data Preprocessing**
   - Performed necessary preprocessing steps such as handling missing values, and redundant features.

3. **Feature Encoding**
   - Encoded categorical columns using label encoding, except for the month column which was encoded using one-hot encoding due to its categorical nature.

4. **Feature Scaling**
   - Utilized Standardization for feature scaling to ensure consistency in feature magnitudes.

5. **Feature Imbalance Handling**
   - Addressed class imbalance in the target column by employing the SMOTE (Synthetic Minority Over-sampling Technique) method to balance class distribution.

6. **Data Modeling**
   - Utilized various machine learning models including KNN, RandomForest, Logistic Regression, and Naive Bayes for predictive modeling.

7. **Model Evaluation**
   - Evaluated model performance using appropriate metrics, with the RandomForest model achieving the highest accuracy of 93.5%.

8. **Feature Importance**
   - Determined feature importance using techniques such as RandomForest feature importances, revealing the top 3 features: Campaign, month, and balance.
