# machineLearning

## Mean, Median, Mode
1. Mean - The average value
2. Median - The mid point value
3. Mode - The most common value

### Mean
```python
# Mean --> The average of the data
# (99+86+87+111+86+103+87+94+78+77+85+86) / 13 = 89.77
# 13 is the number of elements

import numpy

speed = [99, 86, 87, 88, 111, 86,103,87,94,78,77,85,86]

meanOfData= numpy.mean(speed)

print(meanOfData)
```
```
89.76923076923077
```


### Median
```python
import numpy

speed = [99, 86, 87, 88, 111, 86,103,87,94,78,77,85,86]

mediunOfData = numpy.median(speed)
print(mediunOfData)
```
```
87.0
```

### Mode
```python
from scipy import stats

speed = [99, 86, 87, 88, 111, 86,103,87,94,78,77,85,86]

modeOfData = stats.mode(speed)
print(modeOfData)
print(modeOfData.mode) # What is the element which occurs the most
print(modeOfData.count) # how many time it occurs
```
```
ModeResult(mode=np.int64(86), count=np.int64(3))
86
3
```