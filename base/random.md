### 1. 骰子
```python
from random import randint


class Die:
    def __init__(self, num_side=6):
        self.num_side = num_side

    def roll(self):
        return randint(1, self.num_side)


die = Die()
result = [0,0,0,0,0,0,0]
for i in range(10000000):
    result[0] +=1
    result[die.roll()] +=1
for i in range(1,7):
    print(result[i]/result[0])
```