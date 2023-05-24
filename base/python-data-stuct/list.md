### 1. 简介


### 2. 操作

#### 2.1 创建



```
list1=[1,2,3,4]
list2=[1,2,5,6]

for i in list1:
    for j in list2:
        if i==j:
            list1.remove(j)
            list2.remove(j)

print(list1,list2)
```