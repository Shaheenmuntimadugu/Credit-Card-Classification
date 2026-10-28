# Credit-Card-Classification

Goal: Predict if customer will default next month.

Tech Stack: Python (Random Forest) + Power BI

Dataset: Default of Credit Card Clients - 30,000 customers, 25 features
Default Rate: 22% (imbalanced - handled with stratified split)

Results:
- Model Accuracy: 81% (on 30% test data)
- Precision: 68% | Recall: 55% | ROC-AUC: 0.78
- Baseline (predict all No Default) = 78% → Model beats baseline

Key Insight:
- <50K credit limit group has 32% default rate (highest risk)
- 500K+ has 11% default rate (lowest risk)
- Age 25-35 + <50K limit = highest risk segment

Dashboard:
- 2 KPI cards: Total Customers, Default Rate
- Visual: Default Rate by Limit Group (bar chart)
- Filter: Education, Marriage, Age Group

Business Impact:
Bank can flag <50K customers for early follow-up, payment reminders, lower limit increase to reduce NPA by ~15%.

Tools: pandas, sklearn (RandomForestClassifier), Power BI
