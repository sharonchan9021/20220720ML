## 推薦書籍
- [matplotlib 2D 到 3D 資料視覺化王者歸來 (全彩印刷)洪錦魁](https://www.tenlong.com.tw/products/9789860776959?list_name=srh)
- [Matplotlib 3.0 Cookbook](https://www.packtpub.com/product/matplotlib-3-0-cookbook/9781789135718)
  - [GITHUB](https://github.com/PacktPublishing/Matplotlib-3.0-Cookbook) 
- [Matplotlib 3.5.2 documentation](https://matplotlib.org/stable/users/getting_started/)

## Elements of a Figure
- [解說圖形組成](https://github.com/PacktPublishing/Matplotlib-3.0-Cookbook/blob/master/Chapter01/Chapter%201%20-%20Anatomy%20of%20Matplotlib.ipynb)

## 官方範例
```python
import numpy as np
import matplotlib.pyplot as plt

x = np.arange(0, 5, 0.1)
y = np.sin(x)
fig, ax = plt.subplots()
ax.plot(x, y)
```
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


## 多表並陳(subplot、subplots)
- 程式範例 [建立多個子圖表 ( subplot、subplots )](https://steam.oxxostudio.tw/category/python/example/matplotlib-subplot.html)

- [subplot(row, column, index)](https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.subplot.html)
```python
import matplotlib.pyplot as plt
x = [1,2,3,4,5]
y = [5,4,3,2,1]
fig = plt.figure()
plt.subplot(221)
plt.plot(x)
plt.subplot(224)
plt.plot(y)
plt.show()
```
- [matplotlib.pyplot.subplots](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html#matplotlib.pyplot.subplots)
```python
import matplotlib.pyplot as plt
x = [1,2,3,4,5]
y = [5,4,3,2,1]
fig, ax = plt.subplots(2,2)
ax[0][0].plot(x)
ax[1][1].plot(y)
plt.show()
```
