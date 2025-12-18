# 📋 Project Charter: Spaceship Titanic Rescue Prediction

## 1. Business Objective
**Problem:** The Spaceship Titanic has collided with a spacetime anomaly, transporting half of the passengers to an alternate dimension. Rescue efforts are hampered by the inability to locate lost passengers.
**Solution:** Build a predictive model to identify which passengers were likely transported.
**Impact:** Optimize rescue operations by prioritizing search areas or identifying passenger profiles most at risk, ultimately assisting in the recovery of missing persons.

## 2. Stakeholders
- **Rescue Operations Command:** Primary users who will use predictions to allocate search resources.
- **Scientific Investigation Team:** Interested in understanding *why* certain passengers were taken (feature importance).
- **Passenger Families:** Beneficiaries of improved rescue efficiency.

## 3. Success Metrics
### Business Metrics
- **Rescue Efficiency:** Increase in successfully located passengers per search unit (conceptual).
- **Resource Optimization:** Reduction in wasted search time in sectors with low transport probability.

### Technical Metrics
- **Accuracy:** Must exceed the Majority Class Baseline (approx. 50-54% depending on dataset balance).
- **F1-Score:** Primary metric to balance Precision (don't search empty space) and Recall (don't leave anyone behind). Target > 0.80.

## 4. Timeline (4-Week Sprint)
- **Week 1: Foundations:** Data Quality Assessment, Question-Driven EDA, Baseline Model.
- **Week 2: Engineering:** Feature Engineering (Cabin decoding, spending behaviors), Model Selection.
- **Week 3: Refinement:** Hyperparameter Tuning, Cross-Validation, Error Analysis.
- **Week 4: Delivery:** Final Documentation, Business Impact Analysis, Visual Assets.

## 5. Assumptions & Risks
- **Risk:** "Cabin" feature has high cardinality and missing values; improper handling could lead to data leakage or poor generalization.
- **Risk:** Potential overlap between "VIP" status and spending features causing multicollinearity.
- **Assumption:** The training data is representative of the remaining missing passenger population.
