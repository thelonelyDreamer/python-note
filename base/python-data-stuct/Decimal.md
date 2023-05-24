### 
``` python
from decimal import Decimal


def test():
    a = 1.1
    b = 2.2
    print(a + b)

def test1():
    print(Decimal(1.1) + Decimal(2.2))

test1() # 3.300000000000000266453525910
```