Food Delivery Order Cancellation Analytics

Overview
This project analyzes and predicts food delivery order cancellations using a cost-sensitive, explainable modeling approach. The goal is to align prediction decisions with real operational costs, prioritizing high-recall interventions over raw accuracy.

Problem
Order cancellations result in revenue loss, wasted delivery capacity, and a poor customer experience. Standard accuracy-optimized models fail to capture these business trade-offs, so this project reframes cancellation prediction as a cost-optimization problem.

Approach
	•	Performed EDA and statistical analysis to identify key cancellation drivers
	•	Built a regularized logistic regression model (~0.68 ROC-AUC)
	•	Tuned prediction thresholds using FP vs FN cost trade-offs, selecting a recall-optimized threshold (0.37)
	•	Applied feature importance and SHAP for full model interpretability

Key Drivers Identified
	•	Payment mode
	•	Customer tenure
	•	Store-level operational variability
	•	Delivery distance and fees
	•	Promised delivery time
	•	Weekday vs weekend effects

Business Impact
The framework enables:
	•	Risk-aware order routing and ETA adjustments
	•	Store performance monitoring and audits
	•	Targeted onboarding for new customers
	•	Pricing and distance-based intervention strategies

Tech Stack
Python, SQL, Pandas, Scikit-learn, SHAP
