## 推薦書籍
- [非監督式學習｜使用 Python Ankur A. Patel 著 盧建成 譯](https://www.tenlong.com.tw/products/9789865024062?list_name=srh)
  - [Hands-On Unsupervised Learning Using Python(2019)O'Reilly](https://www.oreilly.com/library/view/hands-on-unsupervised-learning/9781492035633/)
  - [GITHUB](https://github.com/aapatel09/handson-unsupervised-learning)
  - 推薦章節
- [Hands-On Unsupervised Learning with Python(2019) Giuseppe Bonaccorso](https://www.packtpub.com/product/hands-on-unsupervised-learning-with-python/9781789348279)
  - [簡體中譯本: Python 無監督學習(2020)](https://www.tenlong.com.tw/products/9787115540720?list_name=srh)
  - [GITHUB(舊版)](https://github.com/packtpublishing/hands-on-unsupervised-learning-with-python)  
  - 推薦章節: 第 2章　聚類基礎知識
    - 2.3　K-means　
    - 2.4　威斯康星州乳腺癌數據集分析　Breast Cancer Wisconsin dataset
    - 2.5　評估指標
      - 2.5.1　最小化慣性
      - 2.5.2　輪廓分數Silhouette score
      - 2.5.3　完整性分數Completeness score
        - from sklearn.metrics import completeness_score
      - 2.5.4　同質性分數Homogeneity score
        - from sklearn.metrics import homogeneity_score 
      - 2.5.5　調整後的相互信息分數Adjusted Mutual Information (AMI) score
        - from sklearn.metrics import adjusted_mutual_info_score 
        - V-measure
          - from sklearn.metrics import v_measure_score 
      - 2.5.6　調整後的蘭德分數Adjusted Rand score 
        - from sklearn.metrics import adjusted_rand_score
      - 2.5.7　列聯矩陣Contingency matrix
        - from sklearn.metrics.cluster import contingency_matrix


# TOPICS
- [Anomaly detection](https://subscription.packtpub.com/book/data/9781789348279/6/ch06lvl1sec51/probability-density-functions)
  - [Anomaly detection with the KDD Cup 99 dataset](https://subscription.packtpub.com/book/data/9781789348279/6/ch06lvl1sec51/probability-density-functions) 
    - 參考資料:Hands-On Unsupervised Learning with Python(2019)Giuseppe Bonaccorso CHAPTER 6.
  - credit card fraud
  - Breast Cancer Wisconsin dataset


# Unsupervised Learning 
- CLUSTERING
  - Hard clustering VS SOFT clustering 
  - Distance functions
    - Euclidean distance
    - Manhattan (or city block) distance
    - Minkowski distances 
  - BASIC Clustering
    - K-means
    - K-means++
    - K-Nearest Neighbors (KNN)
    - Vector Quantization (VQ)
  - Advanced Clustering
    - Spectral clustering
    - Mean shift
    - DBSCAN
    - K-medoids
    - Online clustering
  - Hierarchical Clustering
    - Cluster hierarchies
    - Agglomerative clustering
  - Soft clustering
    - Fuzzy c-means
    - Gaussian Mixture Models
- PCA(Principle Component Analysis)
- SOM(Self-organizing maps)
- GAN(Generative Adversarial Networks)

# [Unsupervised learning@@scikit-learn 1.1.2](https://scikit-learn.org/stable/unsupervised_learning.html)
```
2.1. Gaussian mixture models
2.2. Manifold learning
2.3. Clustering
2.4. Biclustering
2.5. Decomposing signals in components (matrix factorization problems)
     2.5.1. Principal component analysis (PCA)
     2.5.2. Kernel Principal Component Analysis (kPCA)
     2.5.3. Truncated singular value decomposition and latent semantic analysis
     2.5.4. Dictionary Learning
     2.5.5. Factor Analysis
     2.5.6. Independent component analysis (ICA)
     2.5.7. Non-negative matrix factorization (NMF or NNMF)
     2.5.8. Latent Dirichlet Allocation (LDA)
2.6. Covariance estimation
2.7. Novelty and Outlier Detection
2.8. Density Estimation

2.9. Neural network models (unsupervised)
     2.9.1. Restricted Boltzmann machines
     SEE chapter 10　推薦系統使用受限波爾茲曼機
```
