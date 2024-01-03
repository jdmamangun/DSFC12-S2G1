**Uncovering the Silent Epidemic: Insights into Stroke Risk Factors** 

Stroke stands as one of the leading global causes of mortality. While maintaining a healthy diet and adequate sleep are commonly advocated, our focus delves deeper.

With a thorough examination of patient demographics and comorbidities, we aim to determine key features that influence stroke prognosis.

The study involved training various models, including K-Neighbors, Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, AdaBoost, ExtraTrees, and XGBoost. Recognizing the highly imbalanced nature of the dataset, with only approximately 5% of observations indicating a stroke-positive case, resampling techniques were implemented. For oversampling, the methods considered were SMOTE, SMOTE-N, and ADASYN, while Tomek Links was applied for undersampling. The choice of evaluation metric stemmed from the emphasis on minimizing false negatives – ensuring that the model effectively identifies patients at risk of stroke. Consequently, the best-performing model with the highest recall was selected.

The ExtraTrees Classifier was identified as the optimal model, fine-tuned with max_depth = 3 and n_estimators = 200; trained and validated with ADASYN-resampled data. This configuration yielded a holdout recall score of 72.58%. Moreover, the beeswarm summary plot underscored the importance of age and glucose level as the primary features affecting model predictions. These findings collectively contribute to a robust understanding of stroke prediction, emphasizing the significance of specific variables in the model's decision-making process.
