### 列表的创建、访问、修改、删除、遍历

#### 创建列表

可以使用方括号 `[]` 创建列表，列表可以包含不同类型的元素：

```python
lst = [1, 2, 3, "apple", "banana"]
```

#### 访问列表元素

通过索引访问列表中的元素，索引从 0 开始：

```python
print(lst[0])  # 输出：1
print(lst[3])  # 输出：apple
```

#### 修改列表元素

可以直接通过索引修改列表中的元素：

```python
lst[1] = "orange"
print(lst)  # 输出：[1, 'orange', 3, 'apple', 'banana']
```

#### 删除列表元素

可以使用 `del` 语句或 `remove()` 方法删除列表中的元素：

```python
del lst[2]
print(lst)  # 输出：[1, 'orange', 'apple', 'banana']

lst.remove("orange")
print(lst)  # 输出：[1, 'apple', 'banana']
```

#### 遍历列表

可以使用 `for` 循环遍历列表：

```python
for item in lst:
    print(item)
```

### 二维列表的创建、访问、修改、遍历

#### 创建二维列表

二维列表是列表的列表：

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

#### 访问二维列表元素

可以使用两个索引访问二维列表中的元素：

```python
print(matrix[0][1])  # 输出：2
```

#### 修改二维列表元素

可以直接通过索引修改二维列表中的元素：

```python
matrix[1][1] = 50
print(matrix)  # 输出：[[1, 2, 3], [4, 50, 6], [7, 8, 9]]
```

#### 遍历二维列表

可以使用嵌套的 `for` 循环遍历二维列表：

```python
for row in matrix:
    for item in row:
        print(item, end=" ")
    print()
```

### 循环嵌套分支

在循环中嵌套分支语句用于实现更复杂的逻辑：

```python
for i in range(5):
    if i % 2 == 0:
        print(f"{i} is even")
    else:
        print(f"{i} is odd")
```

### 双层嵌套循环

双层嵌套循环用于遍历二维列表或实现其他双重循环逻辑：

```python
for i in range(3):
    for j in range(3):
        print(f"i = {i}, j = {j}")
```

这可以用于遍历二维列表：

```python
for i in range(len(matrix)):
    for j in range(len(matrix[i])):
        print(matrix[i][j], end=" ")
    print()
```

以上是 Python 中列表和二维列表的创建、访问、修改、删除、遍历，以及循环嵌套分支和双层嵌套循环的基本用法。