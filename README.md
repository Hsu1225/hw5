# hw5

## Titanic: Machine Learning from Disaster

Start here! Predict survival on the Titanic and get familiar with Machine Learning basics

[Kaggle Titanic](https://www.kaggle.com/c/titanic)

## Training

1. perform *n*-fold crossvalidation on the training data and use three-way split to select the best prediction model
2. then apply the model on the test data 
3. report the accuracy of training procedure (averaeg accuracy of training, validation, testing in *n*-fold crossvalidation)  => there should be three lines for each part in total

```R
Rscript hw5_studentID.R --fold n --train Titanic_Data/train.csv --test Titanic_Data/test.csv --output performance.csv
```

## Testing

* Submit your prediction into Kaggle system under display name: [yourname]_DS@NCCU
* Make a snapshot of your score on Leaderboard

![titanicLeaderBoard](titanic.png)

## Score

* 6 testing parameters from fold 5 to fold 10

```R
Rscript hw5_9999.R --fold 5 --train Titanic_Data/train.csv --test Titanic_Data/test.csv --output performance1.csv
...
Rscript hw5_9999.R --fold 10 --train Titanic_Data/train.csv --test Titanic_Data/test.csv --output performance6.csv
```
Each testing parameters get 15 points
Penalty: without training, calibration, testing answer (-5 points of each answer)

## Bonus
* Round number to two decimal places: 2 points
* Performance Bonus: average testing performance
  * 0.90 ~ 0.95: 4 points
  * 0.85 ~ 0.90: 3 points
  * 0.80 ~ 0.85: 2 points
  * 0.75 ~ 0.80: 1 points
* Average testing performance is closed to the score of Kaggle (<= 0.05): 4 points
