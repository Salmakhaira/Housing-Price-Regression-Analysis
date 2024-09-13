# Housing Price Regression Analysis
Regression analysis of California housing data to predict median house values using decision tree, k-nearest neighbors, and linear regression models.

1. Linear Regression:
Mean Squared Error (MSE): 4728192458.218032
Training Score: Not explicitly shown.
Testing Score: Not displayed.
R2 Score: Not clearly visible from the output.

Conclusion:
The Linear Regression model produces a very high MSE, indicating that this model may not be suitable for the dataset used.
It is recommended to reassess the data preprocessing and check the linear relationship between variables.

2. K-Nearest Neighbors (KNN) Regression:
Mean Squared Error (MSE): 10726221040.76386 (higher than Linear Regression)
Training Score: 0.5924
Testing Score: 0.2136
R2 Score: -0.4161 (a negative R2 indicates poor model performance)

Conclusion:
KNN has a higher MSE than Linear Regression, and the negative R2 indicates very poor performance on the test data.
Further hyperparameter tuning such as adjusting the number of neighbors or better preprocessing may be needed.

3. Decision Tree Regression:
Mean Squared Error (MSE): 4833974491.953973 (lower than KNN but slightly higher than Linear Regression)
Training Score: 1.0 (indicating overfitting)
Testing Score: 0.6456
R2 Score: 0.6501 (fairly good compared to the other models)

Conclusion:
The Decision Tree model has the best R2 score among the three models and a relatively lower MSE compared to KNN.
However, there is clear overfitting, as shown by the perfect training score (1.0), meaning this model requires pruning or other techniques to prevent overfitting on the training data.

Overall Conclusion:
- Decision Tree Regression has the best performance among the three models in terms of R2 Score and MSE, although overfitting is a concern.
- KNN Regression performed the worst, with a negative R2 score and very high MSE, suggesting the model is not suitable for this data.
- Linear Regression had a lower MSE than KNN but is still relatively high, indicating issues with the linearity of the data.
  
It is recommended to further tune the models, especially Decision Tree, and consider trying other models like Random Forest or XGBoost to improve performance.
