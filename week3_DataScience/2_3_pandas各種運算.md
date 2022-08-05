## 2_pandas資料匯入與資料清理(Data cleaning)
- [經典:Python 資料分析, 2/e](https://www.tenlong.com.tw/products/9789864769254)
  - [GITHUB](https://github.com/wesm/pydata-book) 
  - [中譯](https://github.com/LearnXu/pydata-notebook/tree/master/)
  - 第八章 資料處理：連接、合併和重塑
  - 第十章 資料聚合和分組
- [Pandas 資料分析實戰：使用 Python 進行高效能資料處理及分析 (Learning pandas : High-performance data manipulation and analysis in Python, 2/e) Michael Heydt ](https://www.tenlong.com.tw/products/9789864343898)
  - [GITHUB](https://github.com/PacktPublishing/Learning-Pandas-Second-Edition) 
  - Chapter 11：結合、關聯以及重塑資料
    - 11.1 設定pandas
    - 11.2 串連幾個物件的資料
    - 11.3 合併與連結資料
    - 11.4 資料值與索引的樞紐操作
    - 11.5 堆疊與解堆疊
    - 11.6 堆疊資料帶來的效能好處
  - Chapter 12：資料聚合
    - 12.1 設定pandas
    - 12.2 拆開、套用、結合（SAC）模式
    - 12.3 範例資料
    - 12.4 拆開資料
    - 12.5 套用聚合函數、轉換以及過濾
    - 12.6 轉換分組資料
    - 12.7 過濾分組資料
# Combining and Merging Datasets（合併資料集）
- join：連接
- combine：合併
- reshape：整形
- merge：歸併
- concatenate：串聯
- pivot：旋轉
- stack：堆疊

## concatenate：串聯
```python
df1 = pd.DataFrame(np.arange(9).reshape(3, 3), columns=['a', 'b', 'c'])
df2 = pd.DataFrame(np.arange(9, 18).reshape(3, 3),  columns=['a', 'b', 'c'])
pd.concat([df1, df2])
```
```python
df3 = pd.DataFrame(np.arange(9).reshape(3, 3), columns=['a', 'b', 'c'])
df4 = pd.DataFrame(np.arange(9, 18).reshape(3, 3), columns=['a', 'c', 'd'])
pd.concat([df3, df4])
```
## merge (資料庫風格的DataFrame Joins)
```python
import numpy as np
import pandas as pd

import datetime
from datetime import datetime, date


customers = {'CustomerID': [10, 11],
             'Name': ['Mike', 'Marcia'],
             'Address': ['Address for Mike',
                         'Address for Marcia']}
customers = pd.DataFrame(customers)

orders = {'CustomerID': [10, 11, 10],
          'OrderDate': [date(2014, 12, 1),
                        date(2014, 12, 1),
                        date(2014, 12, 1)]}
orders = pd.DataFrame(orders)

customers.merge(orders)
```

## Pivoting 運算
```
!wget https://raw.githubusercontent.com/PacktPublishing/Learning-Pandas-Second-Edition/master/data/accel.csv

sensor_readings = pd.read_csv("./accel.csv")
sensor_readings[sensor_readings['axis'] == 'X']
sensor_readings.pivot(index='interval', columns='axis', values='reading')
```
