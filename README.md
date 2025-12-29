# Customer Credit Risk & Default Prediction Analysis

## 📌 Project Overview
This project develops a data-driven framework to identify high-risk bank customers and predict potential loan defaults. Using a dataset of 10,000 customers, I performed end-to-end data science tasks, including cleaning, exploratory analysis, and building a calibrated Logistic Regression model. The goal is to reduce financial risk while maintaining a positive experience for safe borrowers.

## 📊 Business Questions Answered
1. **Identify High-Risk Drivers**: Which customer attributes (e.g., Loan-to-Income ratio) correlate most strongly with default?
2. **Actionable Risk Tiers**: How can customers be segmented into risk buckets (High to Very Low) for automated decisioning?
3. **Loss Mitigation**: How much financial loss can be prevented by using a predictive model vs. random chance?
4. **Model Strategy**: How can we calibrate the model's decision threshold to prioritize bank safety?

## 💡 Key Findings & Insights
* **Primary Risk Driver**: The **Loan-to-Income ratio** was identified as the leading indicator of default risk.
* **Safety Buffers**: High **account balances** and **credit scores** act as the strongest "insurance" against default.
* **Model Sensitivity**: By shifting the decision threshold to **0.4**, the model successfully catches **76% of actual defaults**.
* **Financial Impact**: Implementing this "Safety-First" model mitigates approximately **$1.41 Million** in potential losses for this customer segment.

## 🛠️ Technical Implementation
* **Data Cleaning**: Handled missing values in employment length and ensured signal integrity for 9,800 records.
* **Feature Engineering**: Created business-critical ratios including `loan_to_income_ratio` and `balance_to_loan_ratio`.
* **Modeling**: Utilized `Scikit-Learn` to build a **Logistic Regression** model with balanced class weights to handle the rare occurrence of defaults.
* **Evaluation**: Achieved a baseline **ROC AUC of 0.69**.
* **Calibration**: Conducted threshold analysis to prioritize **Recall (0.76)** over Precision, ensuring maximum preservation of the bank's principal capital.

## 📂 Project Structure
* `banking_python_portfolio.ipynb`: The complete Jupyter Notebook containing the Python code, visualizations, and modeling logic.
* `banking_credit_risk_dataset.csv`: The raw customer data used for the analysis.

## 🎯 Strategic Recommendations
1. **Calibrated Approval Logic**: The bank should adopt a 0.4 probability threshold for automated flags to prevent 3 out of every 4 defaults.
2. **Income-to-Debt Capping**: Stricter limits should be enforced for borrowers with high Loan-to-Income ratios.
3. **Liquidity Incentives**: Marketing should prioritize applicants with higher existing account balances as they represent lower risk profiles.

---
*Project Completed as part of a Data Analytics Portfolio.*
