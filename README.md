- Data

Rows/Columns: 1,470 employees, ~35 variables.
Quality: No missing/duplicate values; categorical variables encoded (e.g., Attrition New, OverTime New, BusinessTravel New).
File: employee_attrition.csv


- Prepare

Encode target Attrition → Attrition New (No=0, Yes=1).
Recode OverTime (No/Yes) and BusinessTravel (Non-Travel/Rarely/Frequently).


- Analyze

Age vs. Attrition: Leavers trend younger (early 30s).
Years at Company: Highest risk in first ~3 years.
Monthly Income: Leavers skew to lower income bands.
OverTime: Markedly higher attrition for overtime workers.
Business Travel: Frequent travelers show the highest attrition rates.


- Models

Logistic Regression 
SVM 
Random Forest
Gradient Boosting
Decision Tree
XGBoost


- Results

Logistic Regression: ~0.76 accuracy; interpretable; decent recall on leavers.
SVM: ~0.81 accuracy; balanced precision/recall for leavers.
Random Forest: ~0.82 accuracy; better F1 for leavers; feature importances available.
Gradient Boosting: ~0.86 accuracy (highest); weaker recall on leavers.
Decision Tree: ~0.74 accuracy; simplest/most explainable; weakest F1 on leavers.
XGBoost: ~0.83 accuracy; balanced precision/recall; solid dashboard choice.
Across models, OverTime and BusinessTravel consistently emerge as top drivers.


- Act Concrete actions
  limit overtime / add comp time
  rotate/mitigate travel
  support early-tenure
  review lower-band compensation
  deploy a predictive dashboard with Logistic/DT for explainability.
