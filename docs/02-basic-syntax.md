# 第 2 课：基本语法

!!! tip "提示"

    本页面旨在列出一些适合入门 Python 的基本语法，一些复杂的语法将在之后讲解。  
    部分内容来自 [菜鸟教程 Python3 基本语法](https://www.runoob.com/python3/python3-basic-syntax.html) 页面。

## print 输出
print 默认输出是换行的，如果要实现不换行需要在变量末尾加上 `end=""`：

```py
x="a"
y="b"

# 换行输出
print(x)
print(y)
 
print('---------')
# 不换行输出
print( x, end=" " )
print( y, end=" " )
print()
```
## 注释
Python 中单行注释以 `#` 开头，实例如下：

```py
# 这是一个注释
print ("hello world") # 另外一个注释
```

多行注释可以用多个 `#` 号，还有 `'''` 和 `"""`：

```py
# 这是一个注释
# 这也是一个注释

'''
注释 x3
注释 x4
'''

"""
注释 x5
注释 x6
"""

print ("这个不是注释")
```

执行代码后只会输出 `这个不是注释`。

## 行与缩进
Python 最具特色的就是使用缩进来表示代码块，不需要使用大括号 `{}` 。

缩进的空格数是可变的，但是同一个代码块的语句必须包含相同的缩进空格数。实例如下：

```py
if True:
    print ("Answer")
    print ("True")
else:
    print ("Answer")
  print ("False")    # 缩进不一致，会导致运行错误
```