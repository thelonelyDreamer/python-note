1. 生成器的定义

#### 1.1 无限制的
```python
def fibenacci():
    back1,back2=0,1
    while True:
        yield back1
        back1,back2=back2,back1+back2

f=fibenacci()
print(next(f)) # 0
print(next(f)) # 1
print(next(f)) # 1

```
#### 1.2 有限制的
```python
def test():
    i = 1
    while i < 2:
        yield i ** 2
        i += 1
o=test()
print(next(o)) # 1
print(next(o)) # 4
print(next(o)) # StopIteration
```
### 1.2 生成器方法
```
# 1. next() 生成一个值， 无法生成则抛出StopIteration

# 2. send() 发送给生成器一个值，赋值给 yield语句 返回值

# 3. throw() 与send()方法相同，只是给yield语句返回一个异常
# 4. stop 停止生成，再次生成会抛出StopIteration
```