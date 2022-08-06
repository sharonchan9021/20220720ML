## 推薦書籍
- [matplotlib 2D 到 3D 資料視覺化王者歸來 (全彩印刷)洪錦魁](https://www.tenlong.com.tw/products/9789860776959?list_name=srh)
- [Matplotlib 3.0 Cookbook](https://www.packtpub.com/product/matplotlib-3-0-cookbook/9781789135718)
  - [GITHUB](https://github.com/PacktPublishing/Matplotlib-3.0-Cookbook) 

## 產生滿足機率分布的直方圖
```python
%matplotlib inline

import numpy as np
import matplotlib.pyplot as plt

# 生成 100000 組標準常態分配（平均值為 0，標準差為 1 的常態分配）隨機變數
normal_samples = np.random.normal(size = 100000) 

# 生成 100000 組介於 0 與 1 之間均勻分配隨機變數
uniform_samples = np.random.uniform(size = 100000) 

plt.hist(normal_samples)
plt.show()
plt.hist(uniform_samples)
plt.show()
```


## 多表並陳
