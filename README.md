# Predictive Maintenance (ML + Power BI)

##  Overview
This project analyzes machine sensor data and predicts equipment failures using machine learning and Power BI.

##  Goal
Detect failures early and support maintenance decisions.

## Dataset
- ~10,000 records
- Target: failure (0 = normal, 1 = failure)
- Strong class imbalance (~3%)

##  Machine Learning
Models used:
- Logistic Regression
- Random Forest

### Key Metrics:
- Accuracy: ~0.98
- Recall (failure): ~0.57
- ROC-AUC: ~0.90

 Recall is prioritized to avoid missing failures.

## 📈 Power BI Dashboard

The dashboard includes:

### 1. Overview
- Failure rate (%)
- Average torque and temperature
- Failure distribution

### 2. Analysis
- Average torque by failure
- Average speed by failure

### 3. Interactive Filtering
- Machine type (L / M / H)

### 4. Relationship Analysis
- Speed vs Torque (scatter plot)

## 🔍 Key Insights
- Higher torque increases failure probability
- Lower speed is associated with failures
- Temperature also contributes to risk
- Class imbalance affects model performance

##  Files
- `predictive_maintenance_ml.ipynb` — ML analysis
- `predictive_maintenance_dashboard.pbix` — Power BI dashboard

##  Conclusion
Random Forest provides better balance between precision and recall.

The dashboard enables:
- failure monitoring
- root cause analysis
- proactive maintenance decisions

##  Future Improvements
- Handle imbalance (SMOTE)
- Hyperparameter tuning
- Deployment (API / real-time monitoring)
