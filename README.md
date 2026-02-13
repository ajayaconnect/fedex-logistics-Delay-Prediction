# 📦 FedEx Logistics Shipment Delay Prediction

## 🚀 End-to-End Data Analytics + Machine Learning Project

This project analyzes real-world logistics shipment data and builds a **Machine Learning model to predict delivery delays before shipment dispatch**.

The project covers the complete lifecycle:
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Machine Learning Modeling
- Model Evaluation
- Deployment Ready Model

---

# 📌 Business Problem

Late deliveries in global logistics lead to:

- Customer dissatisfaction
- Contract penalties
- Increased operational costs
- Vendor performance issues

### 🎯 Goal
Build a predictive system that answers:

**Will a shipment be delayed or delivered on time?**

This allows operations teams to take **preventive action before shipment dispatch.**

---

# 📊 Dataset Overview

The dataset contains global shipment records including:

| Category | Features |
|---|---|
| Order Info | Project Code, Product Group, Quantity |
| Vendor Info | Vendor, Country, Manufacturing Site |
| Cost Metrics | Freight Cost, Pack Price, Insurance |
| Shipment Info | Shipment Mode, Weight |
| Timeline Info | PO Dates, PQ Dates |
| Target Variable | Delivery Status |

---

# 🔎 PART 1 — Exploratory Data Analysis (EDA)

## Data Quality Checks
- Missing value analysis
- Duplicate detection
- Outlier detection
- Data type validation

## Univariate Analysis
- Shipment Mode Distribution
- Product Group Distribution
- Vendor Frequency
- Country Distribution

## Bivariate & Multivariate Analysis
Key relationships explored:

- Weight vs Freight Cost
- Vendor vs Delivery Delay
- Country vs Delay
- Shipment Mode vs Cost
- Insurance vs Delay
- Product Groups vs Shipments

---

## 🔥 Key EDA Insights

- Heavy shipments have higher freight cost and delay risk
- Certain vendors consistently cause delays
- Some countries have significantly higher delay rates
- Air Charter shipments have highest freight cost
- High-value shipments require higher insurance
- Large orders increase procurement lead time

📌 **Conclusion:**  
Most delivery delays originate in **procurement and planning stages**, not transportation.

---

# ⚙️ PART 2 — Feature Engineering

### Data Cleaning
- Converted date columns to datetime
- Extracted Year / Month / Day
- Removed raw datetime columns
- Handled missing values using imputation
- Encoded categorical variables
- Removed data leakage features

---

# 🤖 PART 3 — Machine Learning Implementation

## 🎯 Target Variable
```
Delivery Status
0 → On Time  
1 → Delayed
```

---

## ML Pipeline

### Train Test Split
```
80% Training  
20% Testing
```

### Handle Imbalanced Dataset
Used **SMOTE** to balance delayed vs on-time shipments.

### Feature Scaling
Used **StandardScaler** on numeric features.

---

# 🧠 Models Trained

| Model | Purpose |
|---|---|
| Logistic Regression | Baseline model |
| Decision Tree | Non-linear relationships |
| Random Forest ⭐ | Final production model |

---

# 📊 Model Performance

| Model | Accuracy |
|---|---|
| Logistic Regression | 65% |
| Decision Tree | 87% |
| Random Forest | **94%** |

### Final Model → Random Forest

```
Accuracy  : 94%
Precision : 94%
Recall    : 94%
F1 Score  : 94%
```

Model generalizes well and avoids overfitting.

---

# 🔍 Feature Importance (Top Delay Drivers)

The model identified the strongest delay predictors:

1. Procurement timeline (PO & PQ dates)
2. Line item quantity & value
3. Vendor reliability
4. Country & manufacturing site
5. Unit & pack pricing
6. Shipment cost factors

📌 Delays originate in **procurement & supply planning stage**.

---

# 💼 Business Impact

This ML system can be used as a **Delay Risk Prediction Tool**.

### Before Shipping:
The company can:
- Predict delay probability
- Flag high-risk shipments
- Prioritize logistics resources
- Inform customers early
- Improve vendor selection

### Expected Benefits
- Reduced late deliveries
- Improved customer satisfaction
- Better vendor management
- Lower logistics cost
- Data-driven decision making

---

# 💾 Model Deployment

Saved model file:
```
fedex_delay_model.pkl
```

Ready for integration into:
- Web Apps
- Dashboards
- REST APIs
- Real-time logistics systems

---

# 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Analysis & ML |
| Pandas | Data Processing |
| NumPy | Numerical Computing |
| Matplotlib & Seaborn | Visualization |
| Scikit-Learn | Machine Learning |
| Imbalanced-Learn | SMOTE |
| Joblib | Model Saving |

---

# ▶️ How to Run Project

```bash
git clone https://github.com/yourusername/fedex-delay-prediction.git
cd fedex-delay-prediction
pip install -r requirements.txt
```

Run notebook:
```
FedEx_Logistics_Analysis.ipynb
```

---

# 🔮 Future Improvements

- Real-time tracking integration
- Weather & holiday data integration
- Deep learning models
- Deployment as REST API

---

# 🎉 Conclusion

This project demonstrates how **Data Analytics + Machine Learning**
can transform logistics operations from **reactive → proactive**.
