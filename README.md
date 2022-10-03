# Data-analysis  

## Adult data 
- [Adult Data](https://archive.ics.uci.edu/ml/datasets/Adult)를 사용하여 'Earnings-Raw'열의 값이 >50 k 또는 <=50k인지를 예측하는 모델을 만듦
- Onehotencoding, correlation coefficient, GridSearch 사용
- f1 score : 0.9


## Basketball - Home team
- 2015-2016 시즌의 NBA 경기 기록 데이터를 사용하여 홈팀의 승패를 예측하는 모델을 만듦
- 데이터의 형태


|Row Name|Description|
|--|--|
|Date|경기 날짜|
| Visitor Team|원정팀|
|Home Team|홈팀|
|HomePts|홈팀 득점|
|Attend.|관중수|

- DecisionTreeClassifier 사용(max_depth = 15, random_state = 42)
- f1 score : 0.89

## CIFAR-10 Data set classification - trained model
- 테스트 성능이 최대가 되는 CIFAR-10 Data set image classification model을 만듦
- 사전 훈련된 구현 model인 VGG의 learning rate, batch size를 바꾸어가며 test
- Maximum Accuracy : 88.54%


## STL-10 Data set classification - non trained model
- 테스트 성능이 최대가 되는 STL-10 Data set image classification model을 만듦
- 사전 훈련된 구현 model을 사용하지 않고 model을 직접 구현
- Alexnet을 직접 구현하고 거기에 padding을 추가하거나 Conv2d, Maxpool, ReLU층을 추가하거나 batch size을 바꾸어가며 test
- Maximum Accuracy : 58.1125%
