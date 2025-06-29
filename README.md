# 🛒 E-commerce Return Rate Reduction Analysis

## 📌 Objective
To analyze product return behavior and reduce return rates by:
- Understanding return patterns by category and supplier
- Predicting high-risk return products using machine learning
- Visualizing insights through an interactive Power BI dashboard

---

## 🧰 Tools Used
- **Python (Google Colab)**: Data cleaning, feature engineering, model training
- **Scikit-learn**: Random Forest Classifier
- **Pandas / Seaborn / Matplotlib**: Data manipulation & visualization
- **Power BI**: Dashboard creation and data visualization

---

## 🧠 Tasks Performed

### ✅ Google Colab (Python)
1. **Data Cleaning**  
   - Loaded `Ecommerce_Product_Sales.csv`  
   - Checked for missing values and duplicates  
   - Standardized column names

2. **Return Rate Analysis**  
   - Analyzed average return rate by `Category` and `Seller_Name`  
   - Created bar plots using Seaborn

3. **Feature Engineering**  
   - Created features like `Name_Length`  
   - One-hot encoded categorical features

4. **Modeling**  
   - Used Random Forest classifier to predict high return risk  
   - Achieved ~54% accuracy  
   - Predicted `High_Return` and `Return_Probability`

5. **Result Export**  
   - Exported full test results to `high_risk_products.csv` including predicted labels and probabilities

---

### ✅ Power BI
1. **Imported `high_risk_products.csv`**
2. **Created the following visuals:**
   - Pie Chart: Predicted Return split (0 vs 1)
   - Bar Chart: Avg Return Probability by Seller
   - Table: Product-level predictions
   - Card: Total count of high-risk predicted products
   - Slicer: Single slicer using field parameters (`Predicted`, `Actual`, `Return_Probability`)

3. **Used dynamic filters** via slicers for better drill-through analysis

---

## 📦 Deliverables
- `e_commerce_return_rate_reduction_analysis.py`: Python codebase
- `high_risk_products.csv`: Full prediction results
- `Ecommerce_Return_Analysis_Final_Report.pdf`: 2-page summary report
- Power BI Dashboard: Interactive visual report based on predictions

---

## ✅ Outcome
The project identifies products with a high risk of return using machine learning and enables easy filtering, visualization, and decision-making using Power BI.

---

### 💡 Final Notes:

* Dataset includes all predictions (0 and 1), allowing meaningful visuals.
* Single slicer through field parameter keeps the layout minimal.
* This dashboard supports strategic decision-making on high-return suppliers or product segments.
