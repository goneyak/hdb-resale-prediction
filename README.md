# 🏙️ Singapore HDB Resale Price Prediction (Sep 2024 – Dec 2024)

This project predicts resale prices of HDB flats in Singapore using machine learning and statistical modeling. The analysis was performed using real-world data enriched with geolocation and lease information.

> 🔍 **Georgia Tech MGT 6203 — Data Analytics in Business** Course Project  
> 📆 Date Range: Sep 2024 – Dec 2024  
> 👩‍💻 Tools: R, caret, randomForest, dplyr, ggplot2, base plotting

---

## 📌 Project Highlights

- Modeled **housing resale ROI** using:
  - Flat type/model
  - Floor area
  - Lease info
  - Proximity to MRT
- Conducted **EDA, outlier detection, transformation**  
- Applied:
  - **Linear Regression** with cluster-specific models
  - **Random Forest Regression** achieving **R² up to 0.97**
- Visualized insights via residual plots, boxplots, scatterplots

---

## 🧠 Methods

### 🔹 Data Preprocessing
- Cleaned and standardized categorical features
- Converted lease data to months
- Converted "YYYY-MM" to date format

### 🔹 Clustering
- K-means clustering on `resale_price` and `distance to MRT`
- Determined optimal k with elbow method (`k = 4`)
- Performed **cluster-wise regression analysis**

### 🔹 Modeling
- Linear Regression per cluster
- Random Forest (ntree = 500, mtry = 4)
- Feature importance analysis

---

## 📈 Key Results

| Model Type        | R² Score  |
|-------------------|-----------|
| Linear Regression | ~0.63     |
| Random Forest     | **0.97**  |

- Most predictive features:  
  ✅ Town, Month, Floor Area, Distance to MRT  
  ❗ Less important: Flat Type, Remaining Lease

---

## 📁 Structure

```
HDB_Price_Prediction/
├── [MGT 6203] Final.pdf        # Full report with code, analysis, visuals
├── README.md                   # Project overview
```

---

## 📚 References

- Data Source: [Singapore HDB Resale Data (data.gov.sg)](https://data.gov.sg)
- Libraries: `randomForest`, `caret`, `e1071`, `Hmisc`, `dplyr`, `ggplot2`

---

## 📬 Author

**Goyeun Yun**  
Regulatory Affairs & Data Analytics | Georgia Tech OMS Analytics  
GitHub: [@goneyak](https://github.com/goneyak)
