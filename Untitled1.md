```python
x=1
```


```python
x = 2 
```


```python
print("Hello,world!")
```

    Hello,world!
    


```python
s = '12\\34'
```


```python
print
```

    12\34
    


```python
from datetime import datetime, date, time
```


```python
dt = datetime(2020,7,17,17,57,36)
```


```python
dt.year

```




    2020




```python
dt.day

```




    17




```python
dt.hour
```




    17




```python
dt.month
```




    7




```python
dt.date()
```




    datetime.date(2020, 7, 17)




```python
dt.time()
```




    datetime.time(17, 57, 36)




```python
dt.strftime('%m/%d/%Y %H:%M')
```




    '07/17/2020 17:57'




```python
dt2= datetime(2020,6,17,17,57)
```


```python
delta = dt- dt2
```


```python
delta
```




    datetime.timedelta(days=30, seconds=36)




```python
seq = [(1,2,3),(4,5,6),(7,8,9)]
```


```python
for a,b,c in seq:
    print('a={0},b={1},c={2}'.format(a,b,c))
```

    a=1,b=2,c=3
    a=4,b=5,c=6
    a=7,b=8,c=9
    


```python
for a,b, in seq:
    print('a={1},b={2}'.format(a,b))
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-19-8ed76e3e9154> in <module>
    ----> 1 for a,b, in seq:
          2     print('a={1},b={2}'.format(a,b))
    

    ValueError: too many values to unpack (expected 2)



```python
for a,b in seq:
    print('a={1},b={2}'.format(a,b))
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-20-f8aca65a3794> in <module>
    ----> 1 for a,b in seq:
          2     print('a={1},b={2}'.format(a,b))
    

    ValueError: too many values to unpack (expected 2)



```python
seq=[1,5,9,6,4,3,5]
seq.insert(1,100)
print(seq)
```

    [1, 100, 5, 9, 6, 4, 3, 5]
    


```python
seq=[1,5,9,6,4,3,5]
seq.insert(-1,888)
print(seq)
```

    [1, 5, 9, 6, 4, 3, 888, 5]
    


```python
seq=[1,5,9,6,4,3,5]
seq.insert(5,100)
print(seq)
```

    [1, 5, 9, 6, 4, 100, 3, 5]
    


```python
numbers = list(range(1,6))
print(numbers)
```

    [1, 2, 3, 4, 5]
    


```python
numbers = list(range(1,101))
print(numbers)
```

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100]
    


```python
even_numbers = list(range(2,101,2))
print(numbers)
```

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100]
    


```python
even_numbers = list(range(2,101,2))
print(even_numbers)
```

    [2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 96, 98, 100]
    


```python
odd_numbers = list(range(1,100,2))
print(odd_numbers)
```

    [1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25, 27, 29, 31, 33, 35, 37, 39, 41, 43, 45, 47, 49, 51, 53, 55, 57, 59, 61, 63, 65, 67, 69, 71, 73, 75, 77, 79, 81, 83, 85, 87, 89, 91, 93, 95, 97, 99]
    


```python
min(odd_numbers)
```




    1




```python
sum(odd_numbers)
```




    2500




```python
max(odd_numbers)
```




    99




```python
squares = [value**2 for value in range(1,101)]
print(squares)
```

    [1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169, 196, 225, 256, 289, 324, 361, 400, 441, 484, 529, 576, 625, 676, 729, 784, 841, 900, 961, 1024, 1089, 1156, 1225, 1296, 1369, 1444, 1521, 1600, 1681, 1764, 1849, 1936, 2025, 2116, 2209, 2304, 2401, 2500, 2601, 2704, 2809, 2916, 3025, 3136, 3249, 3364, 3481, 3600, 3721, 3844, 3969, 4096, 4225, 4356, 4489, 4624, 4761, 4900, 5041, 5184, 5329, 5476, 5625, 5776, 5929, 6084, 6241, 6400, 6561, 6724, 6889, 7056, 7225, 7396, 7569, 7744, 7921, 8100, 8281, 8464, 8649, 8836, 9025, 9216, 9409, 9604, 9801, 10000]
    

python编程从入门到实践 习题4-3


```python
for value in range(1,21):
    print(value)
```

    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    11
    12
    13
    14
    15
    16
    17
    18
    19
    20
    


```python
numbers = list(range(1,1000001))
print(sum(numbers))
```

    500000500000
    


```python
2**3
```




    8




```python
4**3
```




    64




```python
2**3
```




    8




```python
3**3
```




    27



列表解析


```python
new_value = [value**3 for value in range(1,11)]
print(new_value)

```

    [1, 8, 27, 64, 125, 216, 343, 512, 729, 1000]
    


```python

```
