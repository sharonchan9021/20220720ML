#
- 參考書:Hands-On Artificial Intelligence for Cybersecurity
- [Network Anomaly Detection with AI](https://subscription.packtpub.com/book/data/9781789804027/7)

# Botnet
- [【透視Emotet難以遏止的原因】全球最大Botnet起底，他們竟用敏捷開發來加速自我演化！(2021)](https://www.ithome.com.tw/news/143058)
- [ITHOME_BOTNET](https://www.ithome.com.tw/tags/botnet)

#

```
Network anomaly detection techniques
How to classify network attacks
Detecting botnet topology
Different machine learning (ML) algorithms for botnet detection
```

```python
import numpy as np
import pandas as pd

from sklearn.linear_model import *
from sklearn.tree import *
from sklearn.naive_bayes import *
from sklearn.neighbors import *
from sklearn.metrics import accuracy_score

from sklearn.model_selection import train_test_split

import matplotlib.pyplot as plt
%matplotlib inline

# Load the data.
dataset = pd.read_csv('../datasets/network-logs.csv')
samples = dataset.iloc[:, [1, 2]].values
targets = dataset['ANOMALY'].values
training_samples, testing_samples, training_targets, testing_targets = train_test_split(
         samples, targets, test_size=0.3, random_state=0)


# k-Nearest Neighbors model
knc = KNeighborsClassifier(n_neighbors=2)
knc.fit(training_samples,training_targets)
knc_prediction = knc.predict(testing_samples)
knc_accuracy = 100.0 * accuracy_score(testing_targets, knc_prediction)
print ("K-Nearest Neighbours accuracy: " + str(knc_accuracy))


# Decision tree model
dtc = DecisionTreeClassifier(random_state=0)
dtc.fit(training_samples,training_targets)
dtc_prediction = dtc.predict(testing_samples)
dtc_accuracy = 100.0 * accuracy_score(testing_targets, dtc_prediction)
print ("Decision Tree accuracy: " + str(dtc_accuracy))


# Gaussian Naive Bayes model
gnb = GaussianNB()
gnb.fit(training_samples,training_targets)
gnb_prediction = gnb.predict(testing_samples)
gnb_accuracy = 100.0 * accuracy_score(testing_targets, gnb_prediction)
print ("Gaussian Naive Bayes accuracy: " + str(gnb_accuracy))
```
