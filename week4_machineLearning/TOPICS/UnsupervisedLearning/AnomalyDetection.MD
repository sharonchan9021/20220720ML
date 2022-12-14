# AnomalyDetection
- Anomaly
  - balanced datasets VS unbalanced datasets
  - Histograms
  - Kernel density estimation (KDE)
    - Gaussian kernel
    - Epanechnikov kernel
    - Exponential kernel
    - Uniform (or Tophat) kernel
  - Estimating the density
- Anomaly detection | Outlier detection
  - [REVIEW:Anomaly Detection: A Survey (2009)](https://www.researchgate.net/publication/220565847_Anomaly_Detection_A_Survey)
  - TOPICS:
    - Anomaly detection with the KDD Cup 99 dataset
- Algorithms
  - One-class support vector machines
    - [原始論文:Estimating the Support of a High-Dimensional Distribution(2001)](https://dl.acm.org/doi/10.1162/089976601750264965)
    - from sklearn.svm import OneClassSVM
  - Isolation Forests(強大的演算法) 2008
    - [WIKI說明](https://en.wikipedia.org/wiki/Isolation_forest) 
    - [sklearn.ensemble.IsolationForest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.IsolationForest.html)
      - from sklearn.ensemble import IsolationForest
    - 後續發展
      - SCiForest(2010) [正式論文](https://link.springer.com/chapter/10.1007/978-3-642-15883-4_18#Bib1)
      - Extended Isolation Forest (EIF)  2018 [arxiv](https://arxiv.org/abs/1811.02141) [正式論文](https://ieeexplore.ieee.org/document/8888179)

## 程式範例說明
- 參考資料:Hands-On Unsupervised Learning with Python(2019)Giuseppe Bonaccorso CHAPTER 6.
