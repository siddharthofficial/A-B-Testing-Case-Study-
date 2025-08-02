# 📊 A/B Testing Case Study – Banner Click Analysis

This project is a **hands-on A/B test** designed to evaluate whether **Product A's banner** results in a significantly higher **Click-Through Rate (CTR)** compared to **Product B's banner**. 

---

## 📁 Dataset Overview

- **File**: `clicks.csv`
- **Size**: 10,000 rows × 2 columns  
- **Columns**:
  - `product`: Banner type shown to a user (`a` or `b`)
  - `banner_clicked`: User click response (1 = Clicked, 0 = Not Clicked)

---

## 🎯 Business Objective

To determine whether the **CTR of Product A's banner** is significantly higher than Product B’s, based on actual user interaction data.

---

## 🧠 Analytical Approach

A **2-sample Z-test for proportions** was used to compare the CTRs. The following values were computed from the data:

| Metric                             | Value              |
|-----------------------------------|--------------------|
| Click-Through Rate (CTR A)        | **13%**            |
| Click-Through Rate (CTR B)        | **11%**            |
| Absolute Difference in CTRs       | **2%**             |
| Standard Error (SE)               | **0.0065**         |
| Z-Test Statistic                  | **2.039**          |
| Z-critical (α = 0.05, two-tailed) | **±1.96**          |
| P-value                           | **0.041**          |
| Confidence Interval (95%)         | **[0.001, 0.026]** |
| Minimum Detectable Effect (MDE)   | **10%**            |
| Significance Level (α)            | **5%**             |

---

## 📈 Results

- ✅ **Statistical Significance**:  
  Since `Z = 2.039 > 1.96` and `P = 0.041 < 0.05`, we **reject the null hypothesis**. Product A’s banner shows a **statistically significant improvement** in CTR over Product B.

- ❌ **Practical Significance**:  
  The observed lift is **only 2%**, which is **less than the predefined MDE of 10%**. Therefore, the result is **not practically significant** from a business impact perspective.

---

## 💡 Business Insights

- Product A’s banner outperforms Product B in CTR based on user data.
- The gain, however, is **too small** to make a meaningful business difference or justify a full-scale implementation.

---

## ✅ Recommendations

**Stick with ad A**: Even though there might be a small improvement, it’s not practically large enough to confidently switch campaigns or invest further in Ad B.


---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- SciPy (Z-test implementation)
- Matplotlib 

---


## ✍️ Author

Siddharth Jain  
Connect with me on [LinkedIn](https://www.linkedin.com](https://www.linkedin.com/in/siddharth-jain-979a35253/)

