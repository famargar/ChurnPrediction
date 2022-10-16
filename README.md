# ChurnPrediction

Create a synthetic dataset with fake customers signing up for a certain service and churning in a time period that depends on some generic number of days, 
then size and industry. (*SynthDataGen*).

The data appears as 

Dates,AccountID,Churn,accounts,startdate,size,industry,tenure,enddate,Tenure
2021-01-01 00:00:00,80304,Active,80304,2020-11-05 18:09:01,Small,Manufacturing,349,2021-10-20 18:09:01,56
2021-01-01 00:00:00,47675,Active,47675,2020-05-04 05:22:26,Large,Manufacturing,373,2021-05-12 05:22:26,241
2021-01-01 00:00:00,3021,Active,3021,2020-12-01 07:31:51,Small,Military,360,2021-11-26 07:31:51,30
2021-01-01 00:00:00,28499,Active,28499,2020-05-02 03:51:04,Small,PublicSector,365,2021-05-02 03:51:04,243
2021-01-01 00:00:00,77346,Active,77346,2020-04-12 23:23:53,Large,Manufacturing,353,2021-03-31 23:23:53,263

Then compute Churn as a flag that means the customer will churn in the next 30 days

Then predict churn in the next 30 days (*PredictChurn*). I am also validating the results agains a different time frame (*OutOfTimeValidation*)

Then predict lenghth of tenure (*PredictTenure*) and realise that using that as predictor for churn would give much worse results. 
I suspect this is due to the fact that tenure itself is a strong predictor.
