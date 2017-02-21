# How to install `requests`?

At 1st, Go to the Mac Terminal, type `pip install requests` and `return`.

Terminal replies:

```
Collecting requests
Using cached requests-2.13.0-py2.py3-none-any.whl
Installing collected packages: requests
Successfully installed requests-2.13.0
```

* Do not type `pip install requests` and `return` in IDLE. The good reason:

> pip is run from the command line, not the Python interpreter. It is a program that installs modules, so you can use them from Python. Once you have installed the module, then you can open the Python shell and do import selenium.

> The Python shell is not a command line, it is an interactive interpreter. You type Python code into it, not commands.

From: http://stackoverflow.com/questions/8548030/why-does-pip-install-inside-python-raise-a-syntaxerror

And next, type `import requests` in IDLE.

# How to install `numpy`?

In the Terminal, type `pip3 install numpy` and `return`

## A good example

* Data from DataCamp.

```
import numpy as np

height = [1.73, 1.68, 1.71, 1.89, 1.79]

height
$ [1.73, 1.68, 1.71, 1.89, 1.79]

weight = [65.4, 59.2, 63.6, 88.4, 68.7]
weight
$ [65.4, 59.2, 63.6, 88.4, 68.7]

np_height = np.array(height)

np_height
$ array([ 1.73,  1.68,  1.71,  1.89,  1.79])

np_weight = np.array(weight)

np_weight
$ array([ 65.4,  59.2,  63.6,  88.4,  68.7])

bmi = np_weight / np_height ** 2

bmi
$ array([ 21.85171573,  20.97505669,  21.75028214,  24.7473475 ,  21.44127836])
```

## Numpy Subseting

```
bmi > 23
$ array([False, False, False,  True, False], dtype=bool)

bmi[bmi > 23]
$ array([ 24.7473475])
```
## 2D Numpy Arrays
```
np_2d = np.array([[1.73, 1.68, 1.71, 1.89, 1.79],
                          [65.4, 59.2, 63.6, 88.4, 68.7]])
```

```
np_2d[0]
```
```
array([ 1.73,  1.68,  1.71,  1.89,  1.79])
```

```
np_2d[0][2]
```
or 
```
np_2d[0,2]
```

```
1.71
```

## Basic Statistics

```
np.mean(np_2d[0,:])
```
```
1.7600000000000002
```


