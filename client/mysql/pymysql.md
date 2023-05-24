```python
from pymysql import Connection

conn = Connection(
    host="localhost",
    port=3306,
    user="root",
    password="password"
)

print(conn.get_server_info())

cursor = conn.cursor()
conn.select_db("test")
cursor.execute("select 1;")
tuple = cursor.fetchall()

for t in tuple:
    for i in t:
        print(i)
    pass
cursor.close()
conn.close()
```