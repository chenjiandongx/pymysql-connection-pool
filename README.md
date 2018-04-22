# pymysql 连接池

使用 queue 为 pymysql 提供一个连接池，减少多次创建实例的开销

### 用法

``` python
pool = ConnectionPool(
    # maxsize=100, maxsize 非必须，用于指定最大连接数
    host="localhost",
    port=3306,
    user="test_user",
    passwd="test_passwd",
    db="test_db"
)
pool.execute("select * from test")
```

### LICENSE

MIT [©chenjiandongx](https://github.com/chenjiandongx)
