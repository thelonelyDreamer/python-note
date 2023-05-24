### 1. 字符串方法
1.replace

2.trim




### 2. 字符串比较
```python
print('sd'<'sdf') # True
print('df'<'a') # False
```

### 3. 字符串编解码
```python
import os
import sys
print(os.getcwd())
print(sys.getdefaultencoding())
s='天涯共此时'
print(s.encode(encoding='GBK'))
print(s.encode(encoding='UTF_8'))

print('===解码===')
byte = s.encode(encoding='GBK')
print(byte.decode(encoding='GBK'))
byte=s.encode(encoding='utf-8')
print(byte.decode(encoding='utf-8'))

```

### 4. 字符串截取
```python
a = 'hello world!'
print(a[:5]) # hello
print(a[1:5:2]) # el
print(a[::-1]) # !dlrow olleh

b = 'test python'
print(b[-1:-7:-1]) # nohtyp

```

```python
my_str = "text ollhe world!"
result1 = my_str[::-1][7:12]
print(f'result1:{result1}')
result2= my_str[5:10][::-1]
result3=my_str.split(" ")[1][::-1]
```

