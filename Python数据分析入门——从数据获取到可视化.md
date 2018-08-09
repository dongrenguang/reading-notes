# Python数据分析入门——从数据获取到可视化
> 沈祥壮 著


## 第一章 准备

### 1. if \_\_name\_\_ == '\_\_main\_\_'
在当前程序被当做主程序被执行的时候，\_\_name\_\_自动被赋值为'\_\_main\_\_'；当它被作为模块被其他文件调用的时候，自动被赋值为模块所在的文件名。

### 2. 类属性、类方法、实例属性
``` python
class Person:
    // 类属性
    has_hair = True

    def __init__(self, name):
        // 实例属性
        self.name = name

    // 类方法
    def say(self, words):
        print(words)
```


## 第二章 数据的获取

### 1. robots.txt
用于声明对于爬虫的限制。而作为爬虫者，也理应遵循`robots.txt`中的规则。

### 2. requests 库
用于发送请求。

### 3. BeautifulSoup 库
用于解析网页并提取数据，常用方法：`find`、`find_all`。

### 4. UA伪装
``` python
import requests

url = 'https://****'
headers = {
    'User-Agent': ''
}
data = requests.get(url, headers=headers)
print(data.text)
```
也可以使用动态UA，例如：fake_useragent 库

### 5. try...except...else...finally
当 try 语句没有抛出异常时，执行 else 语句。

### 6. 编码检测
chardet 库。

### 7. r
避免转义。
``` python
s = r'hello\nworld'
print(s)
# 结果：hello\nworld
```

## 第三章 数据的存取与清洗


## 第四章 数据的分析及可视化


## 第五章 Python与生活