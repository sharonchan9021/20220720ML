# 參考資料
- [NumPy Tutorial](https://www.w3schools.com/python/numpy/default.asp)


##


## NumPy ufuncs
- [NumPy ufuncs](https://www.w3schools.com/python/numpy/numpy_ufunc.asp)
  - ufuncs stands for "Universal Functions" and they are NumPy functions that operates on the ndarray object.
  - ufuncs are used to implement vectorization in NumPy which is way faster than iterating over elements.
  - They also provide broadcasting and additional methods like reduce, accumulate etc. that are very helpful for computation.
- [Rounding Decimals](https://www.w3schools.com/python/numpy/numpy_ufunc_rounding_decimals.asp)
  - There are primarily five ways of rounding off decimals in NumPy:
    - truncation
    - fix
    - rounding
    - floor
    - ceil
```python

import numpy as np

arr1 = np.trunc([-3.1666, 3.6667])
arr2 = np.fix([-3.1666, 3.6667])
arr3 = np.around(3.1666, 2)
arr4 = np.floor([-3.1666, 3.6667])
arr5 = np.ceil([-3.1666, 3.6667])

print(arr1)
```
