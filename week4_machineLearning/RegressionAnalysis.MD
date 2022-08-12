# Regression Analysis迴歸分析

# 推薦書籍
- [Python Machine Learning: Machine Learning and Deep Learning with Python, scikit-learn, and TensorFlow, 3/e](https://www.packtpub.com/product/python-machine-learning-third-edition/9781789955750)
  - [github](https://github.com/rasbt/python-machine-learning-book-3rd-edition) 
  - [Python 機器學習 (上), 3/e](https://www.tenlong.com.tw/products/9789864345182?list_name=srh)
    - 推薦章節
      - 第10章：以迴歸分析預測連續目標變數

探索房屋數據集
使用RANSAC找出強固的迴歸模型
評估線性迴歸模型的效能
使用正規化方法做迴歸
將線性迴歸模型轉成曲線－多項式迴歸
使用隨機森林處理非線性關係
## DATASET:  房價預測問題
- Boston House Prices
  - Harrison, D. and Rubinfeld, D.L. `Hedonic prices and the demand for clean air', J. Environ. Economics & Management, vol.5, 81-102, 1978. 
  - http://lib.stat.cmu.edu/datasets/boston
  - https://www.kaggle.com/datasets/vikrishnan/boston-house-prices
  - [sklearn.datasets.load_boston](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_boston.html)
- California housing dataset
- [UC Irvine Machine Learning Repository(有612個資料集)](https://archive-beta.ics.uci.edu/)
```
CRIM: Per capita crime rate by town
ZN: Proportion of residential land zoned for lots over 25,000 sq. ft.
INDUS: Proportion of non-retail business acres per town
CHAS: Charles River dummy variable (= 1 if tract bounds river and 0 otherwise)
NOX: Nitric oxide concentration (parts per 10 million)
RM: Average number of rooms per dwelling
AGE: Proportion of owner-occupied units built prior to 1940
DIS: Weighted distances to five Boston employment centers
RAD: Index of accessibility to radial highways
TAX: Full-value property tax rate per $10,000
PTRATIO: Pupil-teacher ratio by town
B: 1000(Bk – 0.63)2, where Bk is the proportion of [people of African American descent] by town
LSTAT: Percentage of lower status of the population
MEDV: Median value of owner-occupied homes in $1000s
```

## 分析
- [What impacts Boston Housing Prices](https://medium.com/li-ting-liao-tiffany/python-%E5%BF%AB%E9%80%9F%E8%B3%87%E6%96%99%E5%88%86%E6%9E%90-boston-housing%E6%B3%A2%E5%A3%AB%E9%A0%93%E6%88%BF%E5%83%B9-9c535fb7ceb7)
