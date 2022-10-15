# ChurnPrediction

Create a synthetic dataset with fake customers signing up for a certain service and churning in a time period that depends on some generic number of days, 
then size and industry. (*SynthDataGen*).

Then compute Churn as a flag that means the customer will churn in the next 30 days

Then predict churn in the next 30 days (*PredictChurn*). I am also validating the results agains a different time frame (*OutOfTimeValidation*)

Then predict lenghth of tenure (*PredictTenure*) and realise that using that as predictor for churn would give much worse results. 
I suspect this is due to the fact that tenure itself is a strong predictor.
