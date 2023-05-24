
### 1 json 库
```python
import json
username=input("What is your name?")
filename='username.json'
with open(filename,'w') as f:
    json.dump(username,f)
with open(filename) as f:
username = json.load(f)
print(f'Welcome back, {username}!')
```
#### 1.1 dumps()
将Python对象编码成json字符串


#### 1.2 loads()
解码json数据，返回python对象


#### 1.3 dump()
将python对象编码成json数据并写入json文件中

#### 1.4 load()
从json文件中读取数据并解码为Python对象