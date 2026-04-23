# Business Performance & Predictive Revenue Analysis

## 📊 Project Overview
This analysis investigates the relationship between marketing investments, promotional strategies, and daily revenue performance. By applying advanced statistical methods and machine learning, this project identifies the specific drivers of revenue growth and provides a highly accurate model for future financial forecasting.

## 📈 Key Metrics at a Glance
Based on the analysis of 200 data points:
* **Average Daily Revenue:** ₹11,730.12
* **Customer Satisfaction Score:** **4.25/5.00**, indicating that approximately 85% of customers are highly satisfied with the service
* **Marketing Efficiency:** The average marketing spend is ₹1,328.22 with a standard deviation of ₹169.17, showing consistent and reasonable investment levels

## 🔍 Statistical Deep-Dive

### 1. Data Distribution & The "M" Shape
Visual analysis through histograms revealed an **"M" shaped (bimodal) distribution** in both revenue and spend.
* **Non-Normality:** Formal Shapiro-Wilk tests returned p-values of **0.000**, confirming the data does not follow a standard bell curve
* **The Driver:** This bimodality is not a flaw but a feature—it proves the business operates in two distinct performance "modes" driven by different promotion strategies

### 2. Hypothesis Testing: The Power of Aggressive Discounts
A **Mann-Whitney U Test** was used to compare the "Standard" vs. "Aggressive_Discount" strategies.
* **Result:** P-value ≈ **4.98e-33**
* **Impact:** The result is statistically overwhelming. The Aggressive Discount strategy is not just better by chance; it is a legitimate and powerful driver of significantly higher revenue
* **Revenue Benchmarks:**
    * **Standard Strategy Average:** ₹10,323.15
    * **Aggressive Discount Average:** ₹13,840.59

### 3. Near-Perfect Correlation
There is a nearly perfect **Spearman Correlation of 0.999** between Marketing Spend and Daily Revenue. This indicates an extremely strong and predictable relationship between investment and return.

## 🤖 Predictive Modeling (Multiple Linear Regression)
A multiple linear regression model was developed to forecast daily revenue based on spend and strategy.

* **Model Performance (R²):** **99.74%**
    * This means the model explains 99.74% of revenue variance, with only 0.26% attributed to random noise
* **The Revenue Formula:**
    * **Return on Investment (ROI):** For every **₹1 spent** on marketing, revenue increases by **₹9.42**
    * **Strategic Boost:** Simply switching from a Standard to an **Aggressive Discount** strategy adds a baseline boost of **₹529.61** to the day's revenue

## 💡 Business Recommendations
1. **Prioritize Aggressive Discounts:** Since the confidence intervals for the two strategies do not overlap, Aggressive Discounts are mathematically guaranteed to outperform standard operations in the current environment
2. **Scale Marketing Spend:** With a 9.4x return, the business should consider increasing marketing budgets within the proven range to drive aggressive revenue growth

---

## 📊 Model Summary

| Metric | Value |
|--------|-------|
| R² Score | 99.74% |
| ROI per ₹1 Spent | ₹9.42 |
| Strategy Impact | +₹529.61 (Aggressive vs Standard) |
| Data Points Analyzed | 200 |
| Average Daily Revenue | ₹11,730.12 |
| Customer Satisfaction | 4.25/5.00 (85%) |

---

## 🎯 Next Steps
To further optimize business performance:
- Test additional promotional strategies
- Expand the model to include seasonal factors
- Monitor long-term sustainability of aggressive discount approach
- Conduct A/B testing to validate model predictions in real-time

---

### ❓ Customization Options
To enhance this README further, consider adding:
1. **Project Name:** Specify the business or project name
2. **Code Snippets:** Include key Python blocks (Mann-Whitney test, regression analysis)
3. **Visuals:** Add plots showing Revenue vs Spend scatter plots
4. **Target Audience:** Adjust tone for technical portfolio or business presentation

---

## 📁 Project Structure

```
├── 📄 business_data.csv
├── 📄 hypothesis_test_result.txt
├── 📄 requirements.txt
├── 📝 README.md
├── 📕 statistical_analysis_report.pdf
├── 📓 statistical_analysis.ipynb
└── 📕 week7_notes.pdf
```