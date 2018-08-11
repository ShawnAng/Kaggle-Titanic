# Kaggle-Titanic
This repo contains codes used in a Kaggle competition, _Titanic: Machine Learning from Disaster_.
## Predict by EXCEL
A simple method, comparing the probability of some features, is used in prediction by excel.

I got 0.78468 in this way. Command is below:
```
PClass -> Sex -> Sibsp -> Parch
B2 -> D2 -> F2 -> G2
IF(B2=1,IF(OR(D2="female",AND(D2="male",F2=0,G2=2),AND(D2="male",F2=2,G2=0)),1,0),IF(B2=2,IF(OR(D2="female",AND(D2="male",F2=0,G2=2),AND(D2="male",F2=1,G2=1),AND(D2="male",F2=2,G2=1)),1,0),IF(OR(AND(D2="female",F2=0,G2<4),AND(D2="female",F2=1,OR(G2<2,G2=5)),AND(D2="female",F2=2,G2=0),AND(D2="male",F2=0,G2>0)),1,0)))
```
## Predict by 
