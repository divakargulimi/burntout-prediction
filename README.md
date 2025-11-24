🌟 **Employee Burnout Prediction – Project Overview**

Employee burnout is one of the most serious issues faced by modern organizations, often leading to reduced productivity, low job satisfaction, and increased attrition.
In this project, I built a machine learning system that predicts an employee’s burnout level based on multiple work-related and personal factors.
The goal of the project is to identify employees at risk early, so HR teams and managers can take meaningful action before burnout leads to performance drops or resignations.


🎯 **Project Objective**
To develop an accurate machine learning model that predicts employee burnout (Burn Rate) using HR, workload, and behavioral data.
This model helps organizations proactively prevent burnout, instead of reacting after it happens.

**Dataset Summary**
The dataset contains employee metadata such as:
Gender
Company Type
WFH Setup Available
Designation Level
Resource Allocation (workload)
Mental Fatigue Score
Date of Joining → Experience
The target variable is:
Burn Rate (0 to 1; higher = more burnout)

⚙️ **Approach & Workflow**
1. **Data Cleaning**
Removed missing values carefully
Converted categorical variables using One-Hot Encoding
Engineered a new feature: Experience_Years from Date of Joining
Handled scaling for numerical fields
2. **Model Training**
Trained multiple ML algorithms:
i.Linear Regression
--->Fast, interpretable
--->Surprisingly high accuracy on this dataset
ii.Random Forest Regressor
--->Handles non-linear patterns
--->More robust to noise
--->One of the best performers
iii.Gradient Boosting (optional)
--->Advanced boosting model
--->Slight improvement over Random Forest depending on data
3. **Evaluation Metrics**
Both Linear and Random Forest performed exceptionally well:
Model	MAE	RMSE	R²
Linear Regression	~0.046	~0.056	0.92
Random Forest	~0.047	~0.059	0.91
These metrics show that the model can explain 90%+ of burnout variations, with only 4–5% error.
5. **Final Output**
Generated a professional CSV file containing:
Employee ID
Actual Burn Rate
Predicted Burn Rate (Linear)
Predicted Burn Rate (Random Forest)
Predicted Burn Rate (Gradient Boosting)


🧠 **Key Insights from the Model**
Mental fatigue is the strongest indicator of burnout
Employees with high mental fatigue showed consistently high burn rates.
Workload imbalance leads to burnout
High resource allocation directly correlates with stress.
Designation level has a moderate impact
Mid-level employees show higher risk due to responsibility pressure.
WFH & company type have minor but noticeable effects
Depending on company culture and remote support tools.

Real-world Usage
This model can be integrated into HR operations to:
🔎 Detect High-Risk Employees Early
HR can receive an alert when predicted burnout exceeds a threshold (e.g., 0.65).
📉 Reduce Attrition
By identifying and supporting stressed employees early, organizations can prevent resignations.
🔄 Dynamic Workload Balancing
The model helps managers redistribute tasks to avoid overworking specific employees.

