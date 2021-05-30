# C++实现常用数据结构
记录使用C++实现常用数据结构的学习过程。

## 参考

[sky12345数据结构与算法系列]: https://www.cnblogs.com/skywang12345/p/3603935.html

## 目录

[TOC]

## 栈

栈是一种线性数据结构，有以下两种特点：

- 按照“后进先出”的顺序访问；
- 只能对栈顶元素进行操作。

栈的三种常用操作：

1. push：向栈顶增加元素；
2. pop：返回栈顶元素并删除该元素；
3. peek：返回栈顶元素，不删除。

### 1 栈的示意图

![img](https://images0.cnblogs.com/blog/497634/201402/231830345432345.jpg)

栈中的数据依次是 30→20→10。

### 2 出栈

![img](https://images0.cnblogs.com/blog/497634/201402/231830540262932.jpg)

**出栈前**：栈顶元素是30。此时，栈中的元素依次是 30→20→10。
**出栈后**：30出栈之后，栈顶元素变成20。此时，栈中的元素依次是 20→10。

### 3 入栈

![img](https://images0.cnblogs.com/blog/497634/201402/231831135784303.jpg)

**入栈前**：栈顶元素是20。此时，栈中的元素依次是 20→10。
**入栈后**：40入栈之后，栈顶元素变成40。此时，栈中的元素依次是 40→20→10。

### 4 C++实现

使用模板实现存储任意类型数据，参考文件MyStack.h。因为使用了模板，所以实现也放在头文件中，如果实现放在`.cpp`文件中，会报链接错误。

原因参考[C++模板的定义是否只能放在头文件中？](https://blog.csdn.net/imred/article/details/80261632)



## 双向循环链表
## 队列