## Veteran_Prediction
Paralyzed Veterans of America (PVA) data has been used to get classifications of donor vs non-donors

Target_B which dictates a person to be donor or non-donor is first predicted (60-40 split) using 67 finalized variables (pre-processing using decision trees, linear models and other techniques)
using logistic regression which appeared to be the model with highest accuracy in prediction of donors vs non-donors

We then used incorporated Target_D (amount of donation from each person). Prediction for Target_D has been best (lowest RMSE) realized
by Gradient Boosting Machines over Logistic Regression and OLS estimator

Combined the confidence of response (probability) from Target_B model with Target_D model predictions to get the prediction of donation $ amount.
Whereas, we incorporated the cost of sending mails and expected donation amount to get to final values of donation
