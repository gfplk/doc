# url编码解码

```python3
# 编码
from urllib import parse
s = 'DS1841N+T&R'
parse.quote(s) # 未对横线进行编码
parse.quote_plus(s) # 对横线进行编码

query = {
    'name': 'walker',
    'age': 99,
}
parse.urlencode(query)
```
