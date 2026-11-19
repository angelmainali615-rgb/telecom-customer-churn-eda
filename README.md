# Telecom Customer Churn Analysis (EDA)

An end-to-end Exploratory Data Analysis (EDA) project examining customer behavior, service subscriptions, and billing patterns to identify key drivers of customer churn in the telecommunications industry.

## 📌 Project Objectives
- Clean and preprocess raw customer demographic, billing, and service data.
- Engineer custom behavioral features (`Tenuregroup`, `MonthlyChargeCategory`, `TotalServices`, and `SpendingCategory`).
- Analyze churn rates across contract types, tenure durations, payment methods, and internet/add-on services.
- Provide actionable, data-driven business recommendations to improve customer retention.

## 🛠️ Tools & Technologies
- **Language:** Python 3
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

## 📂 Dataset Overview
- **File:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`
- **Size:** 7,043 customer records across 21 original features (demographics, account information, subscribed services, and churn status).
- **Data Cleaning:** Converted `TotalCharges` from string/object to numeric (`float64`) and imputed `0` for 11 newly joined customers with `0` months of tenure.

## 📊 Key Analytical Insights
1. **Contract Commitment is the Strongest Churn Predictor:**
   - **Month-to-month** contracts have a **42.7%** churn rate.
   - **One-year** contracts drop to **11.3%** churn, while **Two-year** contracts have only a **2.8%** churn rate.
2. **Early-Stage Customer Vulnerability:**
   - Churned customers have a median tenure of just **10 months**, compared to **38 months** for retained customers.
3. **High Monthly Charges Drive Attrition:**
   - Churned users pay a higher median monthly bill (**$79.65**) than retained users (**$64.43**).
4. **Service & Add-On Stickiness:**
   - **Fiber optic** internet subscribers experience a **41.9%** churn rate (vs. **19.0%** for DSL).
   - Customers without **Tech Support** (**41.6%** churn) or **Online Security** (**41.8%** churn) leave at nearly triple the rate of those who have them (~15%).
   - Customers subscribed to **6 or 7 total services** show the highest loyalty (churn rates under **12%**).
5. **Payment Friction & Demographics:**
   - **Electronic check** users exhibit the highest churn by payment method (**45.3%** vs. ~15–17% for automatic bank transfers/credit cards).
   - Customers without partners churn at **33.0%** compared to **19.7%** for those with partners.

## 💡 Business Recommendations
- **Incentivize Long-Term Contracts:** Offer targeted discounts, loyalty perks, or rate locks to transition month-to-month customers onto 1-year or 2-year plans.
- **Strengthen First-Year Onboarding:** Launch proactive check-ins and support touchpoints during a customer's first 10–12 months to reduce early churn.
- **Bundle Sticky Add-Ons:** Include **Online Security** and **Tech Support** as discounted or free trial bundles with internet packages—especially for Fiber Optic users.
- **Promote Auto-Pay Migration:** Provide small billing credits to encourage Electronic Check users to switch to automatic credit card or bank transfer payments.

## 🚀 How to Run
1. Clone this repository or download the `.ipynb` file and dataset.
2. Ensure Python and the required libraries are installed:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Launch Jupyter Notebook and run all cells:
   ```bash
   jupyter notebook
   ```
