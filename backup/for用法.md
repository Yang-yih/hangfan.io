`for` 循环是 Python 中最常用的循环之一，用于遍历序列（如列表、元组、字符串等）或其他可迭代对象。以下是一些常见的 `for` 循环用法示例：

### 1. 遍历列表
```python
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    print(number)
```
输出：
```
1
2
3
4
5
```

### 2. 遍历字符串
```python
message = "Hello"
for char in message:
    print(char)
```
输出：
```
H
e
l
l
o
```

### 3. 遍历元组
```python
fruits = ('apple', 'banana', 'cherry')
for fruit in fruits:
    print(fruit)
```
输出：
```
apple
banana
cherry
```

### 4. 使用 `range()` 函数
`range()` 函数生成一系列数字，常用于 `for` 循环中。
```python
for i in range(5):
    print(i)
```
输出：
```
0
1
2
3
4
```

### 5. 带有起始值和步长的 `range()`
```python
for i in range(2, 10, 2):
    print(i)
```
输出：
```
2
4
6
8
```

### 6. 遍历字典
可以遍历字典的键、值或键值对。
```python
person = {'name': 'Alice', 'age': 25, 'city': 'New York'}
# 遍历键
for key in person:
    print(key)
```
输出：
```
name
age
city
```

```python
# 遍历值
for value in person.values():
    print(value)
```
输出：
```
Alice
25
New York
```

```python
# 遍历键值对
for key, value in person.items():
    print(f"{key}: {value}")
```
输出：
```
name: Alice
age: 25
city: New York
```

### 7. 使用 `enumerate()`
`enumerate()` 函数在遍历序列时提供索引。
```python
colors = ['red', 'green', 'blue']
for index, color in enumerate(colors):
    print(f"Index {index} is {color}")
```
输出：
```
Index 0 is red
Index 1 is green
Index 2 is blue
```

### 8. 嵌套 `for` 循环
可以在一个 `for` 循环中嵌套另一个 `for` 循环。
```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
for row in matrix:
    for element in row:
        print(element, end=' ')
    print()
```
输出：
```
1 2 3 
4 5 6 
7 8 9 
```

### 9. 列表推导式
使用列表推导式可以在一行代码中完成对列表的遍历和处理。
```python
numbers = [1, 2, 3, 4, 5]
squares = [number ** 2 for number in numbers]
print(squares)
```
输出：
```
[1, 4, 9, 16, 25]
```

这些是 `for` 循环的一些常见用法。根据具体需求，可以选择适合的方法来遍历和处理数据。如果有更多问题或需要更详细的解释，请告诉我！