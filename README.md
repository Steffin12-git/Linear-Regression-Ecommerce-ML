# Linear Regression — E-Commerce Customer Spend Analysis

**Repository:** *Linear Regression Ecommerce*  
**Notebook:** `Linear Regression Ecommerce.ipynb`  

## 🎯 Objective
Predict **Yearly Amount Spent** by e-commerce customers using behavioral and membership features. Perform exploratory data analysis, fit a regression model, validate results, and provide business recommendations.

---

## 🔑 Key Results
- **Model performance (test set):**
  - R² = **0.981**
  - RMSE ≈ **10.19**
  - MAE ≈ **8.43**
- **Top drivers of spend:**
  - `Length of Membership` (strongest predictor)  
  - `Time on App`  
  - `Avg. Session Length`  
  - `Time on Website` → negligible impact  
- **Business implication:** Loyalty (membership) and mobile app engagement are the biggest levers to grow revenue.

---

## 📊 Exploratory Data Analysis
- Pairplot of all variables  
  ![Pairplot](images/Pair%20plot%20of%20all%20varuable.png)

- Strong linear trend between **Length of Membership** and **Yearly Amount Spent**  

---

## 🧑‍💻 Modeling
- **Algorithm:** Linear Regression (`scikit-learn`)  
- **Features used:**  
  `['Avg. Session Length', 'Time on App', 'Time on Website', 'Length of Membership']`  
- **Target:** `Yearly Amount Spent`  
- **Train/Test split:** 70/30, random_state=42  

### Evaluation
- Predicted vs Actual values:  
  ![Evaluation Plot](images/Evaluation%20of%20prediction%20model.png)

- Residual distribution:  
  ![Residuals](images/Resdiual%20count.png)

- Q-Q plot for residual normality:  
  ![Probability Plot](images/Probability%20plot.png)

---

## 📈 Business Insights
1. **Retention drives revenue** → Longer memberships strongly correlate with higher spend.  
2. **Mobile app is key** → App engagement is a bigger driver than website usage.  
3. **Optimize website funnel** → Direct web users toward app for higher conversions.  
4. **Target high-value users** → Use the model to segment and prioritize premium offers.  

---

## ⚠️ Limitations
- Dataset is small (500 rows) — may not generalize.  
- Coefficients show correlation, not causation.  
- Multicollinearity possible (website/app/session features).  

---

## ▶️ How to Run
1. Clone this repository.  
2. Ensure `Ecommerce.csv` and the notebook are in the root directory.  
3. Install dependencies:  

```bash
pip install pandas matplotlib seaborn scikit-learn scipy jupyter
````

4. Open and run `Linear Regression Ecommerce.ipynb`.

---

## 📂 Project Files

* `Linear Regression Ecommerce.ipynb` — full analysis notebook
* `Dataset/` — Dataset
* `images/` — visualizations for README
* `Ecommerce.csv` — dataset (500 rows)


---

## 💡Highlights

* Built and validated regression model to predict annual customer spend; achieved **R² = 0.981** and **RMSE ≈ \$10**.
* Delivered actionable insights: retention and app engagement as primary drivers of revenue.
* Tools: Python (pandas, scikit-learn, seaborn), EDA, regression modeling, and diagnostics.

